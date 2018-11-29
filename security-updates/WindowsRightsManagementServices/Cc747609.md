---
TOCTitle: Zabezpieczenia podczas normalnych operacji w programie RMS
Title: Zabezpieczenia podczas normalnych operacji w programie RMS
ms:assetid: '98f3d584-6320-4aa1-9959-7133cfdb6df7'
ms:contentKeyID: 18123358
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747609(v=WS.10)'
---

Zabezpieczenia podczas normalnych operacji w programie RMS
==========================================================

Po zainstalowaniu i zastrzeżeniu programu RMS usługi sieci Web tego programu działają jako aplikacje usług IIS, uzyskując dostęp do różnych zasobów systemowych, które wymagają uwierzytelniania i autoryzacji. Wszystkie zasoby systemowe wymagają uwierzytelniania i nie można ich skonfigurować w inny sposób. W dalszej części tej strony opisano projekt uwierzytelniania w programie RMS.

Usługi sieci Web programu RMS działają w kontekście puli aplikacji usług IIS. Każda pula aplikacji usług IIS ma unikatową tożsamość odpowiadającą kontu użytkownika domeny, kontu użytkownika lokalnego, lokalnemu kontu Usługa sieciowa lub lokalnemu kontu System lokalny. Każde z tych kont ma inny stopień uwierzytelniania w systemie. Podczas zastrzegania programu RMS można wybrać, czy usługi sieci Web programu RMS będą działać jako konto System lokalny, czy jako konto użytkownika domeny. To konto następnie stanie się tożsamością puli aplikacji programu RMS. Pula aplikacji witryny sieci Web Administracja globalna nosi nazwę „DRMS Application Pool”. Pula aplikacji zastrzeżonej witryny sieci Web nosi nazwę „\_DRMSAppPool1”. Usługa rejestrowania programu RMS działa jako osobna usługa systemu Windows na tym samym koncie, które określono dla tożsamości puli aplikacji programu RMS.

Zasoby, do których dostęp muszą uzyskać usługi sieci Web programu RMS, obejmują różne pliki i foldery systemowe, bazy danych i procedury przechowywane na serwerze bazy danych, rejestr lokalny, usługę Active Directory, pamięć podręczną zestawu, pamięć i inne procesy działające w systemie. Usługa rejestrowania programu RMS wymaga również dostępu do kolejki rejestrowania w systemie lokalnym. Każdy z tych zasobów ma własne listy DACL definiujące, kto może uzyskiwać dostęp do zasobu oraz co może z nim zrobić. 

Aby uprościć przypisywanie uprawnień i zarządzanie kontami usług, wszystkie wymagane uprawnienia są przypisywane do lokalnej grupy RMS Service Group, którą program RMS tworzy podczas zastrzegania. Ponieważ konto usługi programu RMS jest członkiem tej grupy, otrzymuje wszystkie uprawnienia do niej przypisane.

Poniższa lista zawiera podsumowanie uprawnień udzielanych grupie RMS Service Group:

-   Uprawnienie do odczytu w głównych katalogach wirtualnych
-   Uprawnienie do zapisu w katalogu pamięci podręcznej zestawu
-   Uprawnienie do zapisu w systemowym katalogu tymczasowym
-   Uprawnienie do zapisu w kolejce rejestrowania
-   Uprawnienie do odczytu w usłudze Active Directory

Jeśli używanym serwerem bazy danych jest program Microsoft SQL Server 2000, należy mieć na uwadze, że używa on nieco innej metody przypisywania uprawnień niż system Windows Server 2003. Zastrzeżenie programu RMS powoduje utworzenie nazwy logowania dla konta usługi programu RMS na serwerze programu SQL Server. Jeśli wybrano zastrzeżenie programu RMS przy użyciu konta System lokalny, tworzona jest nazwa logowania serwera programu SQL Server w formacie *DOMENA\\nazwa\_komputera*, gdzie *DOMENA* jest nazwą domeny usługi Active Directory, do której należy komputer, a *nazwa\_komputera* jest nazwą serwera. Tworzona jest rola serwera programu SQL Server o nazwie rms\_service, której przypisywane są wszystkie niezbędne uprawnienia. Do tej grupy jest dodawana nazwa logowania konta usługi programu RMS. Kontu usługi programu RMS nie są jawnie udzielane żadne uprawnienia.

Ponadto program SQL Server przypisuje każdej bazie danych właściciela bazy danych (DBO). Prawo własności bazy danych jest podczas zastrzegania przypisywane w poniższy sposób:

-   Rola DBO dla bazy danych konfiguracji jest przyznawana kontu domeny, za pomocą którego zastrzeżono program RMS.
-   Rola DBO dla baz danych usług katalogowych i rejestrowania jest przyznawana kontu usługi programu RMS.

Podczas projektowania programu RMS, kierując się potrzebą zapewnienia właściwych zabezpieczeń, bardzo uważnie wybrano uprawnienia dotyczące wszystkich zasobów tworzonych przez program RMS. Nie powinny pojawić się powody, dla których należałoby modyfikować uprawnienia do dowolnych zasobów przypisywane podczas zastrzegania. Jeśli po zastrzeżeniu konieczna jest zmiana konta użytkownika lub hasła konta usługi, można to zrobić z poziomu strony sieci Web Administracja globalna programu RMS. Aby uzyskać więcej informacji, zobacz „Zmienianie konta usługi programu RMS” w części „Obsługa serwerów programu RMS” w tym zestawie dokumentacji.
