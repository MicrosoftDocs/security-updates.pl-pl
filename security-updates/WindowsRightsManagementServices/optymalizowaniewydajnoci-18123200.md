---
TOCTitle: Optymalizowanie wydajności
Title: Optymalizowanie wydajności
ms:assetid: '24dc9ca4-652b-41a6-9a99-95fdeca9120b'
ms:contentKeyID: 18123200
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720220(v=WS.10)'
---

Optymalizowanie wydajności
==========================

W tematach zawartych w tej części podano informacje dotyczące optymalizowania wydajności rozmieszczenia programu RMS.

Optymalizowanie wydajności usług katalogowych
---------------------------------------------

W programie RMS można monitorować dołączone do niego liczniki wydajności usług katalogowych. W razie potrzeby można zoptymalizować wydajność przez modyfikację ustawień rejestru, od których zależą atrybuty pamięci podręcznej usługi Active Directory.

Od ustawień rejestru zależą następujące atrybuty pamięci podręcznej usługi Active Directory:

-   Maksymalna liczba podmiotów przechowywanych w pamięci podręcznej
-   Okres ważności informacji na temat podmiotów przechowywanych w pamięci podręcznej
-   Maksymalna liczba grup przechowywanych w pamięci podręcznej
-   Okres ważności informacji na temat grup przechowywanych w pamięci podręcznej
-   Maksymalna liczba wpisów członkostwa w grupach
-   Okres ważności informacji na temat członkostwa w grupach przechowywanych w pamięci podręcznej

Ogólnie można powiedzieć, że im dłuższy jest okres ważności informacji przechowywanych w pamięci podręcznej lub im więcej wpisów znajduje się w tej pamięci, tym szybciej program RMS odpowiada na żądania wymagające uzyskania informacji z usług katalogowych. Jeśli te informacje są przechowywane w pamięci podręcznej usługi Active Directory, nie jest wymagane błądzenie do usługi Active Directory w celu wyszukania informacji. Dzięki temu czas odpowiedzi na żądanie jest krótszy.

Należy jednak pamiętać, że do przechowywania większej ilości informacji w pamięci podręcznej usługi Active Directory wymaganych jest więcej zasobów pamięci systemowej. Ponadto przy konfigurowaniu ustawień rejestru należy zwrócić uwagę na fakt, że im dłuższy okres ważności określony dla elementu, tym większe prawdopodobieństwo, że niektóre wyniki zwracane z pamięci podręcznej usługi Active Directory będą nieprawidłowe. Może się tak zdarzyć w przypadku, gdy w usłudze Active Directory nastąpi zmiana informacji, ale nie zostanie ona odzwierciedlona w pamięci podręcznej tej usługi. Jeśli w usłudze Active Directory zachodzą częste zmiany, warto zastosować krótszy okres ważności informacji przechowywanych w pamięci podręcznej, odpowiedni dla częstotliwości zmian.

Liczniki wydajności usług katalogowych opisano w części „[Program RMS: Liczniki wydajności usług katalogowych](https://technet.microsoft.com/37afea1d-f320-4040-96d8-57c0b45e6d46)” w dalszej części tego tematu. Aby uzyskać instrukcje dotyczące korzystania z nich, zobacz „[Korzystanie z liczników wydajności](https://technet.microsoft.com/096c3b17-c082-46c4-939c-4373af0c9dec)” we wcześniejszej części tego tematu. Należy monitorować liczniki pozwalające porównać „trafienia” z „chybieniami”. Program RMS musi dla każdego chybienia przeprowadzić wyszukiwanie w usłudze Active Directory.

Aby uzyskać szczegółowe informacje dotyczące ustawień rejestru i instrukcje dotyczące ich modyfikowania, zobacz „[Modyfikowanie ustawień pamięci podręcznej usługi Active Directory](https://technet.microsoft.com/8789a7a5-2065-4fae-9104-e0a70f1f2fb6)” w dalszej części tego tematu.

Optymalizowanie ustawień puli połączeń usługi Active Directory
--------------------------------------------------------------

W celu zwiększenia wydajności systemu można dodawać i modyfikować klucze rejestru, od których zależą ustawienia puli połączeń LDAP (Lightweight Directory Access Protocol) usługi Active Directory. Konfigurowanie kluczy rejestru opisano w części „[Modyfikowanie ustawień rejestru dotyczących puli połączeń](https://technet.microsoft.com/c61d91db-a1ad-4ca5-a492-015da629afbc)” w dalszej części tego tematu.

Program RMS zaprojektowano pod kątem optymalnego korzystania z połączeń LDAP. Ustanawia on jedno połączenie dla każdego wykazu globalnego usługi Active Directory, przy czym każde połączenie może obsługiwać wiele wątków. W celu zapewnienia niezawodności program utrzymuje pulę połączeń służących do obsługi żądań. Aby nie dopuścić do poważnego obciążania pojedynczego wykazu globalnego, program RMS za pomocą specjalnego algorytmu rozdziela żądania poprzez równoważenie obciążenia wykazów globalnych z listy wykazów objętych kwerendą. Ponadto automatycznie obsługuje on błędy LDAP i w razie potrzeby przekierowuje żądania do innego wykazu globalnego.

Program RMS tworzy listę wykazów globalnych, w których należy przeprowadzić kwerendę, za pomocą algorytmu wykrywania topologii. Można określić minimalną i maksymalną liczbę wykazów globalnych, którą algorytm wykrywania topologii musi zlokalizować przed uruchomieniem usług programu RMS. Wykrywanie topologii najpierw wykrywa wykazy globalne znajdujące się w bieżącej lokacji. Następnie, jeśli wymagane są dodatkowe wykazy globalne, wyszukuje je w innych lokacjach. Można także określić maksymalną liczbę połączeń, które mogą stać się niedostępne zanim program RMS przestanie akceptować żądania. Jeśli jeden lub więcej wykazów globalnych z listy kwerend stanie się w późniejszym czasie niedostępnych, algorytm wykrywania topologii rozpocznie wyszukiwanie zastępczych wykazów globalnych w celu dodania ich do listy.

Innym rozwiązaniem jest samodzielne stworzenie listy wykazów globalnych, z których ma korzystać program RMS. W takim przypadku algorytm wykrywania topologii nie wyszukuje wykazów globalnych, które można by dodać do listy kwerend.

Można także skonfigurować ustawienia, które określają, w jaki sposób w programie RMS równoważone jest obciążenie poszczególnych wykazów globalnych. Można określić, jak ważne względem siebie mają być poniższe ustawienia, kiedy podejmowana jest decyzja o wysłaniu konkretnego żądania do konkretnego wykazu globalnego:

-   **Działanie okrężne (WtRoundRobin)**. Ten parametr określa względną ważność równoważenia obciążenia, w którym używane są reguły logiczne działania okrężnego. Domyślne ustawienie tej wagi wynosi 1, co oznacza, że jest to najmniej ważne z ustawień, które serwer powinien uwzględnić przy wybieraniu wykazu globalnego.
-   **Liczba wątków podczas połączenia (WtThreadCount)**. Ten parametr określa względną ważność liczby wątków przydzielonych do połączenia. Domyślne ustawienie tej wagi wynosi 100, co oznacza, że przy wybieraniu połączenia mała liczba wątków w wykazie globalnym jest 100 razy ważniejsza niż równoważenie obciążenia przy użyciu reguł logicznych działania okrężnego.
-   **Wolne połączenie (WtSlow)**. Ten parametr określa względną ważność połączenia o niedużej szybkości. Domyślne ustawienie tej wagi wynosi 1 000, co oznacza, że przy wybieraniu połączenia z wykazem globalnym duża szybkość połączenia jest 10 razy ważniejsza od małej liczby wątków.
