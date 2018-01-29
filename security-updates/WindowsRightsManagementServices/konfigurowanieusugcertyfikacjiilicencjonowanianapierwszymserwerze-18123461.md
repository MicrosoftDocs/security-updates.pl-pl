---
TOCTitle: Konfigurowanie usług certyfikacji i licencjonowania na pierwszym serwerze
Title: Konfigurowanie usług certyfikacji i licencjonowania na pierwszym serwerze
ms:assetid: 'cce29a2f-984f-48ed-9187-0eb68286ec5b'
ms:contentKeyID: 18123461
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747756(v=WS.10)'
---

Konfigurowanie usług certyfikacji i licencjonowania na pierwszym serwerze
=========================================================================

Aby skonfigurować program RMS w lesie, należy najpierw zainstalować i zastrzec jeden serwer. Pierwszy rozmieszczony serwer jest serwerem głównej certyfikacji. Ten serwer zapewnia obsługę certyfikacji i licencjonowania i może być używany jako jedyny serwer w konfiguracji z pojedynczym serwerem lub jako serwer początkowy dla klastra głównej certyfikacji.

Role, uprawnienia oraz prawa wymagane do instalacji i zastrzegania dodatkowych serwerów programu RMS
----------------------------------------------------------------------------------------------------

Aby zainstalować program RMS, należy zalogować się za pomocą konta posiadającego uprawnienia administratora lokalnego. Ponadto należy zalogować się do domeny za pomocą ważnego konta domeny, aby usługa Active Directory mogła uwierzytelnić program RMS. Jeśli program RMS jest rozmieszczany w środowisku, w którym infrastruktura usługi Active Directory używa trybu macierzystego systemu Windows 2000, program RMS może nie mieć możliwości odczytania atrybutu memberOf obiektów usługi Active Directory, gdy usługa próbuje rozszerzyć członkostwo grupy. Aby program RMS mógł odczytywać atrybut memberOf, konto usługi programu RMS musi być kontem domeny, które należy do grupy dostępu zgodnej z systemami wcześniejszymi niż Windows 2000, znajdującej się w danym lesie. Jeśli rozmieszczono grupy z ukrytym członkostwem, należy także skonfigurować konto usług programu RMS z uprawnieniami umożliwiającymi mu odczyt ukrytego członkostwa.

> [!note]  
> Jako konta usługi programu RMS nie można użyć konta, za pomocą którego instalowano program RMS. 

Proces instalacji i zastrzegania dla serwera początkowego
---------------------------------------------------------

Rozmieszczanie serwera programu RMS składa się z dwóch etapów. Najpierw należy zainstalować oprogramowanie serwera RMS oraz wszystkie programy pomocnicze, tj. Internetowe usługi informacyjne (IIS), usługę kolejkowania wiadomości i ASP.NET. Aby uzyskać więcej informacji dotyczących instalacji, zobacz „Instalowanie programu RMS z dodatkiem Service Pack 1” w części „Obsługa serwerów programu RMS” w tym zestawie dokumentacji.

> [!note]  
> Program RMS można również zainstalować z wiersza polecenia. Aby uzyskać więcej informacji, zobacz „Instalacja programu RMS z wiersza polecenia” w części „Obsługa serwerów programu RMS” w tym zestawie dokumentacji. 

Po zainstalowaniu programu RMS na serwerze należy zastrzec go do użytku tylko w jednej witrynie sieci Web znajdującej się na serwerze. Podczas zastrzegania tej witryny sieci Web wiele ustawień witryny jest modyfikowanych oraz dodawane są katalogi wirtualne. Aby uzyskać więcej informacji dotyczących tych zmian, zobacz „Obsługa Internetowych usług informacyjnych w programie RMS” w części „Informacje techniczne dotyczące programu RMS” w tym zestawie dokumentacji.

Można użyć domyślnej witryny sieci Web usług IIS lub można utworzyć nową witrynę sieci Web. Aby zastrzec program RMS w witrynie innej niż domyślna witryna sieci Web, należy utworzyć witrynę sieci Web przed rozpoczęciem procesu zastrzegania. Jeśli domyślna witryna sieci Web jest używana do innych celów, należy utworzyć nową witrynę dla programu RMS, tak aby konfiguracja domyślna została zachowana dla domyślnej witryny sieci Web.

Po kliknięciu polecenia **Administracja programem Windows RMS** w menu **Start** zostanie wyświetlona strona **Administracja globalna**. Na tej stronie można rozpocząć proces zastrzegania witryny sieci Web. Aby zastrzec pierwszy serwer RMS, należy wprowadzić następujące informacje:

-   Określ nazwy bazy danych konfiguracji, która będzie używana z bazami danych konfiguracji, rejestrowania oraz usług katalogowych programu RMS.
    Jeśli wystąpienie programu SQL Server ma nazwę inną niż nazwa lokalnego serwera, należy skonfigurować je jako zdalne wystąpienie programu SQL Server, nawet jeśli jest zainstalowane na tym samym serwerze.
    Podczas zastrzegania aktualnie zalogowany użytkownik musi mieć uprawnienia do tworzenia baz danych na serwerze bazy danych.
-   Określ konto, które będzie używane jako konto usługi programu RMS. W przypadku konfiguracji lokalnej można użyć konta System lokalny, chociaż nie jest to zalecane ze względu na problemy z zabezpieczeniami występujące w przypadku uruchamiania usługi z uprawnieniami konta System lokalny.
    W przypadku instalacji obejmującej serwer zdalny programu SQL Server lub więcej niż jeden serwer programu RMS należy określić konto domeny. Używane konto domeny musi mieć uprawnienia wyszukiwania w usłudze Active Directory. Konto zostanie użyte do utworzenia puli aplikacji usług IIS, w której działa konsola administracyjna. Jeśli istniejąca baza danych nie jest uaktualniana ani używana, konto usługi programu RMS wymaga uprawnień do tworzenia bazy danych. Jeśli używane są istniejące bazy danych, konto musi mieć uprawnienia do odczytu i zapisu dla każdej bazy danych programu RMS.
-   Określ adres URL dostępu do tej witryny sieci Web. Domyślną wartością jest nazwa zastrzeganej witryny (na przykład Domyślna witryna sieci Web, jeśli zastrzegany jest serwer w domyślnej instalacji usług IIS). Można określić niestandardowy adres URL umożliwiający dostęp do innej witryny sieci Web, na przykład aby obsługiwać adres URL równoważenia obciążenia lub obsługiwać dostęp z sieci intranet i Internet. Należy sprawdzić, czy niestandardowy adres URL działa oraz dodać nazwę witryny do usługi DNS, aby strony **Administracja globalna** i **Zastrzeganie** mogły odszukać wirtualne katalogi główne. Jeśli ten adres URL jest przeznaczony dla instalacji obsługującej dostęp z Internetu, należy sprawdzić, czy nowy adres URL jest dostępny z Internetu i z sieci korporacyjnej.
-   Wybierz mechanizm używany do ochrony klucza prywatnego instalacji głównej używanego do rejestrowania. Domyślnym ustawieniem jest korzystanie z szyfrowania programowego i przechowywanie zaszyfrowanego klucza prywatnego w bazie danych konfiguracji programu RMS. W przypadku korzystania z konfiguracji domyślnej należy podać silne hasło do szyfrowania wartości w bazie danych.
    Jednak jeśli w komputerze dostępny jest zainstalowany i skonfigurowany sprzętowy moduł zabezpieczeń, można wybrać dostawcę usług kryptograficznych (CSP) do współpracy ze sprzętowym modułem zabezpieczeń w celu przechowywania kluczy prywatnych w urządzeniu, takim jak karta inteligentna. Program RMS wymaga dostawcy pełnego RSA i tylko tacy dostawcy są dostępni na liście CSP. Do ochrony klucza prywatnego RMS zdecydowanie zaleca się korzystanie ze sprzętowego modułu zabezpieczeń.
    W przypadku korzystania z opcji programowego dostawcy CSP do zabezpieczenia klucza prywatnego RMS za pomocą hasła, należy zabezpieczyć hasło i umieścić w bezpiecznym archiwum do wykorzystania w przyszłości. Należy również zachować kopię zapasową bazy danych konfiguracji z hasłem. Dzięki temu będzie możliwe przywrócenie programu RMS, jeśli baza danych programu SQL Server zostanie uszkodzona. W przypadku zmiany hasła należy wykonać nową kopię zapasową bazy danych konfiguracji, która przechowuje klucz prywatny zabezpieczony tym hasłem, a następnie umieścić hasło i kopię w bezpiecznym archiwum. Aby uzyskać więcej informacji dotyczących tworzenia kopii zapasowej bazy danych konfiguracji i przywracania danych z tej kopii, zobacz „Tworzenie kopii zapasowych systemu i jego przywracanie dla programu RMS” w części „Planowanie rozmieszczenia programu RMS” w tym zestawie dokumentacji.
-   Określ nazwę, która ma być używana w certyfikacie licencjodawcy serwera. Domyślnie jest to nazwa serwera.
-   Jeśli to konieczne, określ serwer proxy (w tym adres i port) używany do dostępu do Internetu.
-   Określ adres e-mail używany przez innych administratorów programu RMS do kontaktowania się z administratorem w przypadku problemów z podrejestrowywaniem serwera licencji. Po zastrzeżeniu głównej instalacji można zmienić adres.
-   Wybierz metodę odwołania certyfikatu licencjodawcy serwera w celu określenia, kto, oprócz usługi rejestrowania firmy Microsoft, może odwołać certyfikat licencjodawcy serwera dla instalacji głównej. Aby używać odwołania innej firmy, należy podać ścieżkę i nazwę pliku zawierającego klucz publiczny dla jednostki innej firmy.

Po wybraniu opcji rejestrowania w trybie online i kliknięciu przycisku **Wyślij** na stronie **Zastrzeganie** (po skonfigurowaniu wszystkich odpowiednich opcji) program RMS wygeneruje parę kluczy i wyśle klucz publiczny do usługi rejestrowania firmy Microsoft. (W przypadku wyświetlenia komunikatów o błędach nie należy zamykać strony, na której wyświetlono te komunikaty. Po rozwiązaniu problemów należy użyć polecenia `IISReset` w wierszu poleceń, aby zatrzymać i ponownie uruchomić usługi IIS. Następnie należy powrócić do poprzedniego ekranu, ponownie wpisać informacje na ekranie zastrzegania i ponownie kliknąć przycisk **Wyślij**. Usługa rejestracji firmy Microsoft utworzy certyfikat licencjodawcy serwera i w ciągu kilku minut zwróci go do bazy danych konfiguracji. Ponieważ jest to pierwszy serwer w domenie, w której zainstalowano program RMS, ten krok jest procesem rejestracji serwera głównej certyfikacji.

Jeśli wybrano opcję rejestracji w trybie offline, serwer rejestruje się ręcznie za pomocą usługi rejestracji firmy Microsoft przed zakończeniem zastrzegania. Proces rejestrowania musi zostać zakończony, aby można było korzystać z serwera. Aby uzyskać więcej informacji, zobacz „Ręczne rejestrowanie serwera głównej certyfikacji” w części „Obsługa serwerów programu RMS” w tym zestawie dokumentacji.

Po zakończeniu zastrzegania i rejestrowania serwera łącza na stronie **Administracja globalna** zostaną zmienione. Łącze **Zastrzeż program RMS w tej witrynie sieci Web** zmieni się na łącze **Administruj programem RMS w tej witrynie sieci Web**, łącze **Dodaj ten serwer do klastra** zostanie zastąpione łączem **Zmień konto usługi programu RMS**, a ponadto na stronie zostanie dodane łącze **Usuń program RMS z tej witryny sieci Web**.

Ten serwer początkowy ustanawia główną instalację programu RMS. Główna instalacja może składać się z jednego serwera lub klastra. Po zakończeniu instalowania i zastrzegania serwera początkowego można skonfigurować dodatkowe serwery w celu dostarczenia nadmiarowości lub obsługi równoważenia obciążenia dla usług certyfikacji i licencjonowania.

Po zakończeniu konfiguracji należy zarejestrować punkt połączenia usługi klastra głównej certyfikacji w usłudze Active Directory, aby umożliwić klientom obsługującym technologię RMS wykrywanie usługi. Aby uzyskać więcej informacji, zobacz „Rejestrowanie punktu połączenia usługi” w części „Obsługa serwerów programu RMS” w tym zestawie dokumentacji. Jeśli punkt połączenia usługi nie zostanie zarejestrowany, nie będzie można używać klienta programu RMS z systemem RMS.

> [!Important]  
> Należy dokończyć instalację i zastrzeganie programu RMS na pierwszym serwerze przed rozpoczęciem instalacji programu na innych serwerach. Program RMS obsługuje ochronę zawartości grup usługi Active Directory, których członkostwo obejmuje wiele lasów. Jeśli organizacja nie ma wielu lasów lub grup obejmujących wiele lasów, można zoptymalizować wydajność procesu wystawiania licencji użytkowania na serwerze programu RMS poprzez modyfikację zasad klastra **MaxCrossForestCalls** w bazie danych konfiguracji programu RMS. Zasada ta określa maksymalną liczbę przekroczeń granic lasu przez członkostwo w grupie. Domyślną wartością jest 10. Aby zmienić tę wartość na 0, należy wprowadzić następujące polecenie w języku SQL:`update DRMS_ClusterPolicies set PolicyData=0 where PolicyName='MaxCrossForestCalls'` 

W poniższych tematach szczegółowo omówiono czynności wymagane do wykonania zadań dostępnych na stronie Administracja globalna programu RMS:

-   Aby uzyskać informacje dotyczące korzystania z kreatora instalacji w celu zainstalowania serwera początkowego, zobacz „Instalowanie programu RMS z dodatkiem Service Pack 1” w sekcji „Obsługa serwerów programu RMS” w tym zestawie dokumentacji.
-   Aby uzyskać informacje dotyczące zastrzegania serwera początkowego, zobacz „Zastrzeganie pierwszego serwera głównej certyfikacji” w sekcji „Obsługa serwerów programu RMS” w tym zestawie dokumentacji.
-   Aby uzyskać informacje dotyczące dodawania serwerów do głównej instalacji w celu utworzenia klastra, zobacz [Dodawanie serwerów do obsługi certyfikacji i licencjonowania](https://technet.microsoft.com/089ceb62-2a96-444f-ab42-1d5deaabd0c3) w dalszej części tego tematu.
