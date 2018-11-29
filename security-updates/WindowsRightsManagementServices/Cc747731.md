---
TOCTitle: Planowanie infrastruktury serwera bazy danych
Title: Planowanie infrastruktury serwera bazy danych
ms:assetid: 'b12354bd-3143-4d1f-b5aa-450c4550653c'
ms:contentKeyID: 18123436
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747731(v=WS.10)'
---

Planowanie infrastruktury serwera bazy danych
=============================================

Ponieważ program RMS do obsługi operacji korzysta z baz danych i przechowywanych procedur, do jego zastosowania w danej organizacji wymagana jest infrastruktura bazy danych. Serwer bazy danych może znajdować się na tym samym serwerze, co program RMS, lub na innym serwerze. Jeśli infrastruktura użytkownika nie obejmuje serwera bazy danych, który obsługiwałby program RMS, jako serwera bazy danych, za pomocą którego można sprawdzić program RMS, można użyć programu Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) w wersji A.

Zaleca się używanie programu Microsoft SQL Server Desktop Engine do obsługi baz danych programu RMS tylko w środowiskach testowych, ponieważ nie są w nim dostępne narzędzia niezbędne do pełnej obsługi bazy danych w całym przedsiębiorstwie. Ponadto ponieważ program MSDE nie obsługuje sieci zdalnej, należy zainstalować go na tym samym serwerze, co program RMS. Nie można także dodawać nowych serwerów RMS do klastra programu RMS. Zasady użytkowania programu Microsoft SQL Server Desktop Engine zabraniają używania narzędzi klienckich programu SQL Server do pracy z bazami danych programu Microsoft SQL Server Desktop Engine. Dlatego nie można tworzyć kopii zapasowych bazy danych konfiguracji programu RMS i przywracać z nich danych, przeglądać informacji dotyczących logowania ani bezpośrednio modyfikować danych przechowywanych w bazie danych konfiguracji.

Jeśli planowane jest umieszczenie baz danych na innym serwerze niż serwer z instalacją programu RMS, obsługę baz danych należy realizować za pomocą produktu serwerowego ze wszystkimi niezbędnymi funkcjami obsługi baz danych, np. programu SQL Server. Należy dostarczyć konto usługi programu RMS z odpowiednimi uprawnieniami do odczytu, zapisu i tworzenia znajdujących się na serwerze baz danych, które służą do obsługi programu RMS.

Mimo że program RMS opracowano i przetestowano z wykorzystaniem serwerów baz danych z programem SQL Server 2000 i MSDE, a firma Microsoft nie popiera korzystania z programu RMS wraz z dostawcą baz danych innym niż program SQL Server 2000 lub MSDE, program RMS można używać na innych serwerach baz danych, które korzystają z interfejsu ADO.NET udostępnianego przez platformę Microsoft .NET Framework. Dlatego też inni producenci baz danych mogą opracować zgodne programy baz danych przeznaczone dla programu RMS. Użytkownik może korzystać z dowolnego dostawcy baz danych wraz z programem RMS pod warunkiem, że odpowiadający mu serwer bazy danych spełnia następujące kryteria:

-   Serwer bazy danych musi być zgodny z technologią Transact-SQL, ponieważ ta technologia jest używana przez skrypty inicjalizacyjne oraz procedury przechowywania programu RMS.
-   Serwer baz danych musi obsługiwać rozszerzenia unikatowe dla programu Microsoft SQL Server.

Dostawca bazy danych musi także:

-   Odpowiadać na wywołania metod obszaru nazw System.Data.SqlClient platformy .NET Framework.
-   Udostępniać odpowiednią funkcjonalność obszaru nazw System.Data.SqlClient.
-   Korzystać ze zintegrowanego uwierzytelniania systemu Windows, a nie uwierzytelniania SQL.

W przypadku korzystania z programu RMS w dowolnych innych konfiguracjach należy skontaktować się z odpowiednim producentem bazy danych lub dostawcą rozwiązań, którego produkt został użyty w niestandardowym wdrożeniu.

> [!Caution]  
> Wszystkie bazy danych programu RMS są tworzone przy domyślnie włączonej opcji Pełne przywracanie, ale nie tworzy się zadań tworzenia kopii zapasowej dziennika transakcji. Może to spowodować zapełnienie dysku twardego serwera i awarię serwera bazy danych. Dla bazy danych DRMS\_configuration zaleca się używanie opcji Pełne przywracanie. Dla innych baz danych DRMS można skonfigurować inny model przywracania, odpowiedni dla danej organizacji. 

W tej części omówiono następujące zagadnienia:

-   [Szacowanie rozbudowy bazy danych](https://technet.microsoft.com/87652cc2-b886-4797-8d40-356669768089)
-   [Konserwacja bazy danych usług katalogowych](https://technet.microsoft.com/911a62f2-c1d6-4091-99b0-b53211be27a7)
-   [Konserwacja bazy danych rejestrowania](https://technet.microsoft.com/de55058b-0d1a-4997-8a45-e14678ddd13f)
