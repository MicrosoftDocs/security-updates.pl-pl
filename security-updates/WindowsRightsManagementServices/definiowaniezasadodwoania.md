---
TOCTitle: Definiowanie zasad odwołania
Title: Definiowanie zasad odwołania
ms:assetid: 'e2fffe9f-def7-439b-a8aa-43f8a065813d'
ms:contentKeyID: 18123490
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747782(v=WS.10)'
---

Definiowanie zasad odwołania
============================

Definiowanie organizacyjnych zasad odwołania wymaga szczegółowego planowania i rozwagi, ponieważ mimo że implemenacja odwołania zapewnia większe bezpieczeństwo chronionej zawartości, może też wpłynąć na możliwość korzystania z tej zawartości przez użytkowników. Zasady odwołania przeznaczone dla rozmieszczenia programu RMS można określić z poziomu administracyjnej witryny sieci Web.

Odwołanie przez niezależny podmiot
----------------------------------

Ponieważ wystawcą certyfikatu licencjodawcy serwera dla serwera głównej certyfikacji w rozmieszczeniu programu RMS jest usługa rejestrowania firmy Microsoft, właśnie firma Microsoft może odwołać certyfikat licencjodawcy serwera. Jednak firma Microsoft odwoła certyfikat licencjodawcy serwera tylko w sytuacji, gdy będzie to wymagane nakazem sądowym.

Poza usługą rejestrowania firmy Microsoft można także określić niezależny podmiot, który będzie odwołał certyfikat licencjodawcy serwera odpowiadający serwerowi programu RMS. Tym niezależnym podmiotem może być jednostka zewnętrzna lub para kluczy publiczny-prywatny wygenerowana przez administratora w imieniu organizacji. Klucza prywatnego tak określonego niezależnego podmiotu można użyć do podpisania listy odwołania, która spowoduje odwołanie certyfikatu licencjodawcy serwera. Niezależny podmiot określa się przy użyciu jego klucza publicznego podczas zastrzegania programu RMS. Ponadto szablony zasad praw dostępu związane z serwerem można tak skonfigurować, aby pozwalały niezależnym podmiotom na odwołanie zawartości, manifestów aplikacji, licencji i certyfikatów wystawionych przez instalację programu RMS. Aby uzyskać więcej informacji, zobacz „[Tworzenie i modyfikowanie szablonów zasad praw dostępu](https://technet.microsoft.com/6014176f-ef71-4d29-b3e3-da129c18563d)” w dalszej części tego tematu.

> [!Important]  
> Jeśli zostanie podjęta decyzja o wygenerowaniu własnej pary kluczy służącej do odwołania certyfikatu licencjodawcy serwera dla serwera głównej certyfikacji, należy zadbać o przechowywanie jej w bezpiecznym miejscu. 

Odwołanie certyfikatu licencjodawcy serwera jest ważną decyzją, ponieważ powoduje unieważnienie wszystkich certyfikatów i licencji wystawionych przez daną instalację programu RMS. Aby uzyskać więcej informacji dotyczących odwoływania certyfikatów licencjodawcy serwera, zobacz „[Odwołanie certyfikatów licencjodawcy serwera](https://technet.microsoft.com/8020861d-d196-4431-8282-044675ef5616)” w dalszej części tego tematu.

Uwagi na temat obowiązywania list odwołania
-------------------------------------------

Jeśli dla pewnego elementu chronionej zawartości wymagane jest odwołanie, to spełnienie określonego warunku powoduje zastosowanie i wejście w życie wszystkich list odwołania zarejestrowanych na komputerach klienckich. Dlatego przy implementowaniu odwołania należy zachować rozwagę, ponieważ czynność ta powoduje zarejestrowanie na komputerach klienckich list odwołania, których zakres obowiązywania może się okazać szerszy od spodziewanego. Aby uzyskać więcej informacji dotyczących konfigurowania tej opcji, zobacz „[Tworzenie i modyfikowanie szablonów zasad praw dostępu](https://technet.microsoft.com/6014176f-ef71-4d29-b3e3-da129c18563d)” w dalszej części tego tematu.

Równowaga między zabezpieczeniami i użytecznością
-------------------------------------------------

Kiedy w szablonie zasad praw dostępu określa się zasady odwołania, należy zachować właściwą równowagę między potrzebą lepszego zabezpieczenia dokumentów a możliwością napotkania przez użytkowników na problemy przy użytkowaniu zawartości, tak jak to opisano w poniższym przykładzie.

Konfigurując listę odwołania w szablonie zasad praw dostępu, określono także interwał odświeżania tej listy. Aby korzystać z zawartości opublikowanej przy użyciu tego szablonu zasad praw dostępu, użytkownik musi mieć na swoim komputerze listę odwołania, przy czym lista ta nie może być starsza niż określony interwał odświeżania. Na przykład jeśli interwał odświeżania wynosi 10, stosować można listę odwołania utworzoną najdalej 10 dni temu. Jeśli na komputerze klienckim nie ma listy odwołania lub jeśli data utworzenia listy jest wcześniejsza niż wynika to z interwału odświeżania, aplikacja obsługująca technologię RMS pobiera najnowszą listę odwołania z lokalizacji określonej w licencji użytkowania. Jednak użytkownik, który nie jest podłączony do sieci, nie będzie w stanie uzyskać aktualnej listy odwołania, a zatem nie będzie mógł korzystać z zawartości.

Problem ten można załagodzić przez zastosowanie się do następujących wskazówek:  

-   Określając interwał odświeżania listy odwołania, należy zachować ostrożność, podejmując przy tym kroki w celu zapewnienia użytkownikom stałej dostępności aktualnej listy odwołania.
-   Listy odwołania należy przechowywać pod adresami URL, które są dostępne zarówno z sieci firmowej, jak i spoza niej.
-   Należy używać programu Systems Management Server (SMS) firmy Microsoft® lub podobnego mechanizmu w celu rozprowadzania zaktualizowanych kopii list odwołania do wszystkich komputerów klienckich z określoną częstotliwością, na przykład co noc.
-   Odwołania należy wymagać tylko przy najbardziej wrażliwych typach dokumentów.
