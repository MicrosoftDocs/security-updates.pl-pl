---
TOCTitle: Pamięć podręczna usługi Active Directory programu RMS
Title: Pamięć podręczna usługi Active Directory programu RMS
ms:assetid: 'c721a2eb-2fe9-4346-b426-3cc169b97265'
ms:contentKeyID: 18123413
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747662(v=WS.10)'
---

Pamięć podręczna usługi Active Directory programu RMS
=====================================================

Każdy serwer lub klaster głównej certyfikacji programu RMS oraz serwer licencji ma lokalną pamięć podręczną usługi Active Directory, która zawiera wyniki kwerend dotyczących członkostwa w grupach wykazu globalnego usługi Active Directory. Oprócz pamięci podręcznej na każdym serwerze istnieje także współużytkowana pamięć podręczna dla każdego klastra, która jest przechowywana w bazie danych usług katalogowych. Te pamięci podręczne mają za zadanie ograniczyć liczbę kwerend wysyłanych do wykazu globalnego oraz skrócić czas odpowiedzi na żądania licencji.

Gdy użytkownik żąda licencji użytkowania, odpowiadający serwer musi sprawdzić, czy użytkownikowi udzielono odpowiednich praw dostępu w licencji publikacji. W najprostszym przypadku użytkownik, który zażąda licencji, jest jawnie wymieniony w licencji publikacji. Jednak w wielu sytuacjach autor udziela praw dostępu grupie, a nie pojedynczym użytkownikom.

Jeśli w licencji publikacji nie wymieniono jawnie nazwy użytkownika żądającego licencji, ale udzielono praw dostępu grupie, serwer musi sprawdzić przynależność użytkownika do danej grupy, aby określić, czy użytkownik jest członkiem grupy, której udzielono praw dostępu. W tym celu serwer wysyła kwerendę LDAP do wykazu globalnego.

Serwery programu RMS przechowują wyniki wszystkich kwerend dotyczących członkostwa w grupach zarówno w lokalnej pamięci podręcznej usługi Active Directory, jak i w bazie danych usług katalogowych klastra. Serwery mogą następnie uzyskać informacje o przynależności do grup z tych pamięci podręcznych, co zmniejsza liczbę kwerend, które są wysyłane do wykazu globalnego. Domyślnie kwerenda jest wysyłana do najbliższego serwera, jednak można skonfigurować klucz rejestru GC, tak aby wskazywał serwery wykazu globalnego. Aby uzyskać więcej informacji o tym ustawieniu, zobacz „Modyfikowanie ustawień rejestru dotyczących puli połączeń” w części „Obsługa serwerów programu RMS” w tym zestawie dokumentacji.

W celu określenia przynależności użytkownika do grup serwer najpierw sprawdza w swojej pamięci podręcznej, czy informacje o przynależności do grup są tam przechowywane. Jeśli tak nie jest, serwer sprawdza bazę danych usług katalogowych dla klastra. Jeśli informacje o przynależności do grup są przechowywane w tej bazie danych, serwer następnie wysyła kwerendę do wykazu globalnego.

Dla użytkowników i grup następujące atrybuty usługi Active Directory są przechowywane w pamięci podręcznej:

-   mail
-   ProxyAddresses (tylko adres e-mail SMTP)
-   objectSID
-   sidHistory
-   memberOf (identyfikatory GUID grup, których członkiem jest dany użytkownik lub grupa)

Wpisy w pamięci podręcznej usługi Active Directory są oznaczane sygnaturą czasową. Ustawienia rejestru określają okres ważności wpisów w pamięci podręcznej oraz całkowitą liczbę wpisów, jaka może być przechowywana w pamięci podręcznej. Te ustawienia mogą mieć wpływ na wydajność serwerów. Aby uzyskać więcej informacji, zobacz „Modyfikowanie ustawień pamięci podręcznej usługi Active Directory” w części „Obsługa serwerów programu RMS” w tym zestawie dokumentacji.
