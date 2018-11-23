---
TOCTitle: 'Informacje o wersji programu Windows Server Update Services 3.0'
Title: 'Informacje o wersji programu Windows Server Update Services 3.0'
ms:assetid: '94d1385f-4872-4c29-8822-3a4ec5e45ae4'
ms:contentKeyID: 18136670
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc708491(v=WS.10)'
---

Informacje o wersji programu Windows Server Update Services 3.0
===============================================================

W tych informacjach o wersji opisano znane problemy związane z programem Microsoft® Windows® Server Update Services (WSUS) 3.0. W pliku znajdują się także zalecenia i wymagania dotyczące instalowania tej aplikacji. Informacje podzielone zostały na następujące sekcje:

-   Wymagania systemowe do instalacji serwera WSUS 3.0
-   Wymagania konfiguracyjne do instalacji serwera WSUS 3.0
-   Wymagania systemowe do instalacji konsoli zdalnej WSUS 3.0
-   Wymagania konfiguracyjne dla konsol zdalnych WSUS 3.0
-   Wymagania systemowe do instalacji klienta
-   Wymagania programowe do instalacji serwera WSUS 3.0
-   Wymagania dotyczące minimalnej ilości wolnego miejsca na dysku dla instalacji serwera WSUS 3.0
-   Wymagania dotyczące uaktualnienia WSUS 3.0
-   Parametry wiersza polecenia Instalatora
-   Problemy dotyczące instalacji i uaktualniania
-   Znane problemy
-   Program WSUS 3.0 w systemie Windows Server® 2008
-   Program WSUS 3.0 w systemie Windows Small Business Server 2003

> [!note]  
> Kopia tego dokumentu w wersji do pobrania jest dostępna w witrynie [Microsoft Download Center](http://go.microsoft.com/fwlink/?linkid=71220) ([http://go.microsoft.com/fwlink/?LinkId=71220](http://go.microsoft.com/fwlink/?linkid=71220)). 

Ważna kwestia dotycząca konfiguracji: Konieczne jest zastąpienie hasła serwera proxy w kreatorze konfiguracji
-------------------------------------------------------------------------------------------------------------

W przypadku korzystania z serwera proxy, który wymaga uwierzytelnienia przy użyciu nazwy użytkownika lub hasła, serwer WSUS może nie być w stanie zsynchronizować aktualizacji, jeśli hasło serwera proxy nie zostanie zastąpione podczas działania kreatora konfiguracji serwera WSUS. Ze względu na to, że kreator konfiguracji jest uruchamiany automatycznie pod koniec procesu instalacji, omawiany problem może spowodować błędy w synchronizacji po uaktualnieniu WSUS do wersji 3.0.

Można uniknąć tego problemu poprzez anulowanie działania kreatora konfiguracji po dokonaniu uaktualnienia lub ponowne wprowadzenie prawidłowego hasła serwera proxy, gdy kreator konfiguracji zostanie uruchomiony. Aby usunąć problem, jeśli wystąpi, przejdź do pozycji **Źródło aktualizacji i ustawienia serwera proxy** na stronie **Opcje**, wprowadź ponownie hasło serwera proxy i zapisz ustawienia.

Wymagania systemowe do instalacji serwera WSUS 3.0
--------------------------------------------------

#### Serwer WSUS 3.0 jest obsługiwany w systemach Windows Server 2003 z dodatkiem Service Pack 1 i Windows Server 2008

Serwer WSUS 3.0 jest obsługiwany w systemach Windows Server 2003 z dodatkiem Service Pack 1 i Windows Server 2008.

#### System Windows 2000 Server nie jest obsługiwany przez serwery WSUS 3.0.

Serwer WSUS 3.0 nie obsługuje systemu Microsoft Windows® 2000 Server.

#### Program WSUS 3.0 nie jest obsługiwany na serwerach z usługami terminalowymi.

Program WSUS 3.0 może działać na serwerach z usługami terminalowymi, jednak takie rozwiązanie nie jest wspierane ani zalecane. Program WSUS 3.0 nie będzie działał na serwerze z usługami terminalowymi w konfiguracjach wykorzystujących zdalne implementacje programu SQL Server. Wszystkie niestandardowe akcje zdalne (w tym instalacja) wykonywane na serwerze licencji z usługami terminalowymi będą uruchamiane jako konto systemowe. Konto systemowe serwera może nie mieć uprawnień w zdalnym programie SQL Server i instalacja może zakończyć się niepowodzeniem.

Wymagania konfiguracyjne do instalacji serwera WSUS 3.0
-------------------------------------------------------

#### Program Internetowe usługi informacyjne (IIS) musi zostać zainstalowany.

Program Microsoft Windows Server Update Services 3.0 (WSUS 3.0) wymaga programu Internetowe usługi informacyjne (IIS), który nie jest zainstalowany domyślnie w systemie Microsoft Windows Server 2003 lub Windows Server 2008. W przypadku próby zainstalowania programu WSUS 3.0 bez programu IIS Instalator programu Windows Server Update Services wyświetli komunikat o błędzie z informacją o braku zainstalowanego programu IIS

#### Instalacja nie powiedzie się, jeśli program IIS działa w trybie izolacji IIS 5.0

Jeśli serwer został uaktualniony z wersji Windows 2000 Server do wersji Windows Server 2003, program IIS może działać w trybie zgodności IIS 5.0. Można także włączyć tryb izolacji IIS 5.0 w Menedżerze usług IIS. Spowoduje to niepowodzenie instalacji. Przed rozpoczęciem instalacji programu WSUS 3.0 konieczne będzie wyłączenie trybu izolacji IIS 5.0.

#### Jeśli którykolwiek ze składników programu IIS został zainstalowany w 32-bitowym trybie zgodności na platformie 64-bitowej, instalacja programu WSUS 3.0 może zakończyć się niepowodzeniem.

Wszystkie składniki programu IIS powinny zostać zainstalowane w trybie macierzystym platform 64-bitowych. Instalacja może zakończyć się niepowodzeniem, jeśli dowolny składnik programu IIS będzie działać w 32-bitowym trybie zgodności.

#### Serwery proxy muszą obsługiwać protokoły HTTP i HTTPS.

Jeśli skonfigurowano główny serwer WSUS (serwer WSUS pobierający aktualizacje bezpośrednio z witryny Microsoft Update), w przypadku występowania serwera proxy pomiędzy serwerem WSUS a strefą internetową ten serwer proxy musi obsługiwać protokoły HTTP i HTTPS.

#### Jeśli na porcie 80 działają już co najmniej dwie witryny sieci Web, usuń je przed rozpoczęciem instalacji programu WSUS, pozostawiając tylko jedną

Jeśli na porcie 80 działają co najmniej dwie witryny sieci Web (na przykład usługi Windows® SharePoint® Services), przed rozpoczęciem instalacji programu WSUS należy usunąć wszystkie poza jedną. W przeciwnym wypadku klienci serwera mogą nie być w stanie dokonać samodzielnej aktualizacji.

#### Podczas instalowania programu WSUS 3.0 może być wymagane wyłączenie programów antywirusowych.

W czasie instalowania programu WSUS 3.0 przed rozpoczęciem procesu może być wymagane wyłączenie programów antywirusowych. Po wyłączeniu programu antywirusowego przed rozpoczęciem instalacji programu WSUS należy uruchomić ponownie komputer. Ponowne uruchomienie komputera zapobiega zablokowaniu plików, do których dostęp będzie wymagany w czasie instalacji. Po ukończeniu instalacji należy włączyć ponownie program antywirusowy. Należy odwiedzić witrynę sieci Web producenta programu antywirusowego, aby uzyskać dokładny opis czynności wyłączania i ponownego włączania tego programu.

> [!Caution]  
> Czynności te mogą spowodować, że komputer lub sieć będą bardziej narażone na ataki złośliwego oprogramowania, na przykład wirusów. Nie zalecamy takiego rozwiązania, ale chcemy wskazać możliwość wykonania takiej procedury wedle uznania użytkownika. Procedurę tą należy przeprowadzać na własną odpowiedzialność. 

> [!note]  
> Program antywirusowy służy do ochrony komputera przed wirusami. Jeżeli program antywirusowy jest wyłączony, nie należy pobierać ani otwierać plików pochodzących z niezaufanych źródeł. Nie wolno także odwiedzać niezaufanych witryn sieci Web ani otwierać załączników wiadomości e-mail. 

#### Program WSUS 3.0 w środowisku SQL Server wymaga włączenia opcji wyzwalaczy zagnieżdżonych.

Opcja wyzwalaczy zagnieżdżonych jest włączana domyślnie, może zostać jednak wyłączona przez administratora programu SQL Server.

Jeśli magazynem danych Windows Server Update Services ma być baza danych programu SQL Server, administrator programu SQL Server powinien włączyć opcję zagnieżdżonych wyzwalaczy, zanim administrator programu WSUS 3.0 zainstaluje program WSUS 3.0 i określi bazę danych podczas instalacji.

Instalator programu WSUS 3.0 włącza opcję RECURSIVE\_TRIGGERS (zależną od ustawień bazy danych), ale nie włącza opcji wyzwalaczy zagnieżdżonych będącej globalną opcją serwera.

Aby sprawdzić, czy opcja wyzwalaczy zagnieżdżonych została włączona, użyj następujących poleceń:

**sp\_configure 'nested triggers'**

W celu włączenia opcji zagnieżdżonych wyzwalaczy w środowisku SQL Server, na komputerze z programem SQL Server wykonaj następujące polecenia z pliku wsadowego:

**sp\_configure 'nested triggers', 1**

**GO**

**RECONFIGURE**

**GO**

Jeśli na serwerze nie zainstalowano programu SQL Server Management Studio, skrypty języka SQL można uruchomić z poziomu wiersza polecenia. Narzędzie Command Line Query Utility dla programu Microsoft SQL Server 2005 można pobrać z witryny [Centrum pobierania firmy Microsoft](http://go.microsoft.com/fwlink/?linkid=70728) (http://go.microsoft.com/fwlink/?LinkId=70728, strona może być w języku angielskim). Aby rozpocząć pracę, uruchom polecenie **sqlcmd**.

Jeżeli użytkownik chce uruchamiać skrypty SQL w Wewnętrzna baza danych systemu Windows, musi także pobrać sterownik SQL Native Client z tej samej witryny pobierania.

#### Ograniczenia i wymagania zdalnej współpracy z bazą SQL.

Program WSUS 3.0 zapewnia obsługę bazy danych działającej na komputerze innym niż komputer z zainstalowaną aplikacją WSUS 3.0. Istnieją pewne wymagania wobec konfiguracji zdalnej instalacji programu SQL

-   Nie można używać serwera skonfigurowanego jako kontroler domeny jako serwera typu back-end zdalnej pary SQL.
-   Na komputerze mającym pełnić rolę serwera frontonu zdalnej instalacji SQL nie może pracować oprogramowanie serwera terminali.
-   Oprogramowanie bazy danych, którego należy użyć na komputerze typu back-end, to przynajmniej Microsoft SQL Server 2005 z dodatkiem Service Pack 1 (dostępne w witrynie [Microsoft Download Center](http://go.microsoft.com/fwlink/?linkid=66143) (http://go.microsoft.com/fwlink/?LinkId=66143), jeśli komputer pracuje pod kontrolą systemu Windows Server 2003, lub SQL Server 2005 z dodatkiem Service Pack 2, jeśli zainstalowano system Windows Server® 2008.
-   Zarówno komputer frontonu, jak i komputer typu back-end muszą zostać przyłączone do domeny Active Directory. W przeciwnym wypadku, jeśli znajdują się one w różnych domenach, przed rozpoczęciem instalacji programu WSUS należy ustanowić zaufanie między domenami.
-   Jeśli na komputerze zdalnym z bazą danych SQL zainstalowano program WSUS 2.0, aby uaktualnić go do wersji WSUS 3.0, odinstaluj program WSUS 2.0 (za pomocą apletu **Dodaj/Usuń programy** w Panelu sterowania) na komputerze wewnętrznym, pozostawiając bez zmian istniejącą bazę danych. Zainstaluj program SQL Server 2005 z dodatkiem Service Pack 1 lub Service Pack 2 i uaktualnij istniejącą bazę danych. Na koniec zainstaluj program WSUS 3.0 na komputerze frontonu.

#### Programu WSUS nie można zainstalować, jeśli wcześniej zainstalowano niektóre wersje wstępne programu Internet Explorer 7 z usługami terminalowymi.

Instalacja programu WSUS nie powiedzie się, jeśli na komputerze zainstalowano niektóre wersje Release Candidate programu Internet Explorer 7 z usługami terminalowymi.

Wymagania systemowe do instalacji konsoli zdalnej WSUS 3.0
----------------------------------------------------------

Konsola zdalna programu WSUS 3.0 może zostać zainstalowana na następujących platformach:

-   Windows Server 2008
-   Windows Vista®
-   Windows Server 2003 z dodatkiem SP1
-   Windows XP z dodatkiem SP2

Wymagania konfiguracyjne dla konsol zdalnych WSUS 3.0
-----------------------------------------------------

#### Pomiędzy zdalną konsolą administracyjną a serwerem WSUS 3.0 powinno być dostępne połączenie szerokopasmowe

Łączenie się z serwerem WSUS 3.0 ze zdalnej konsoli administracyjnej przy użyciu połączenia WAN o wąskim paśmie może powodować problemy z wydajnością. Liczbę widocznych aktualizacji i komputerów można ograniczyć poprzez filtrowanie widoków tych elementów, ale zaleca się, aby pomiędzy zdalną konsolą administracyjną a serwerami WSUS 3.0 dostępne było połączenie szerokopasmowe. Jeśli podczas pracy z konsolą zdalną wystąpią problemy z wydajnością, zaleca się łączenie z serwerem w celu zdalnego zarządzania przy użyciu serwera terminali.

Wymagania systemowe do instalacji klienta
-----------------------------------------

Funkcja Aktualizacje automatyczne należy do oprogramowania klienckiego WSUS. Można używać jej z programem WSUS w następujących systemach operacyjnych:

-   Windows Vista
-   Windows Server 2008
-   Microsoft Windows Server 2003 (dowolna wersja)
-   Microsoft Windows XP Professional z dodatkiem SP2
-   Microsoft Windows 2000 Professional z dodatkiem SP4, Windows 2000 Server z dodatkiem SP4 i Windows 2000 Advanced Server z dodatkiem SP4

Wymagania programowe do instalacji serwera WSUS 3.0
---------------------------------------------------

W poniższej tabeli przedstawiono wymagane oprogramowanie dla platform Windows Server 2003 z dodatkiem Service Pack 1. Oprogramowanie wymagane dla systemu Windows Server 2008 zostanie omówione w sekcji dotyczącej obsługi programu WSUS 3.0 w systemie Windows Server 2008.

Przed uruchomieniem Instalatora programu WSUS 3.0 należy sprawdzić, czy serwer WSUS 3.0 spełnia te wymagania. Jeśli którakolwiek aktualizacja wymaga ponownego uruchomienia komputera po zakończeniu instalacji, należy to zrobić przed rozpoczęciem instalowania programu WSUS 3.0.

<p></p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Wymaganie</th>
<th style="border:1px solid black;" >Szczegóły</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Program Microsoft Internet Information Services (IIS)</td>
<td style="border:1px solid black;">Instalacja z poziomu systemu operacyjnego.
Zobacz: Problem 1: Program Internetowe usługi informacyjne (IIS) musi zostać zainstalowany.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Pakiet redystrybucyjny systemu Microsoft .NET Framework w wersji 2.0 (x86)</td>
<td style="border:1px solid black;">Zobacz stronę z opisem pakietu redystrybucyjnego systemu Microsoft .NET Framework w wersji 2.0 (x86) w witrynie <a href="http://go.microsoft.com/fwlink/?linkid=68935">Centrum pobierania firmy Microsoft</a> (http://go.microsoft.com/fwlink/?LinkId=68935, strona może być w języku angielskim). W przypadku platform 64-bitowych zobacz stronę z opisem pakietu redystrybucyjnego systemu Microsoft .NET Framework w wersji 2.0 (x64) witrynie <a href="http://go.microsoft.com/fwlink/?linkid=70637">Centrum pobierania firmy Microsoft</a> (http://go.microsoft.com/fwlink/?LinkId=7063, strona może być w języku angielskim).</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Program Microsoft Management Console 3.0 dla systemu Windows Server 2003</td>
<td style="border:1px solid black;">To jest wymaganie wstępne dotyczące korzystania z interfejsu użytkownika programu WSUS 3.0. Zobacz stronę z opisem programu Microsoft Management Console 3.0 dla systemu Windows Server 2003 (KB907265) w witrynie <a href="http://go.microsoft.com/fwlink/?linkid=70412">Centrum pobierania firmy Microsoft</a> (http://go.microsoft.com/fwlink/?LinkId=70412, strona może być w języku angielskim). W przypadku platform 64-bitowych zobacz stronę z opisem programu Microsoft Management Console 3.0 dla systemu Windows Server 2003 x64 Edition (KB907265) w witrynie <a href="http://go.microsoft.com/fwlink/?linkid=70638">Centrum pobierania firmy Microsoft</a> (http://go.microsoft.com/fwlink/?LinkId=70638, strona może być w języku angielskim).</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Narzędzie Podgląd raportów firmy Microsoft</td>
<td style="border:1px solid black;">To jest wymaganie wstępne dotyczące korzystania z interfejsu użytkownika programu WSUS 3.0. Zobacz stronę z opisem wersji redystrybucyjnej narzędzia Podgląd raportów firmy Microsoft 2005 w witrynie <a href="http://go.microsoft.com/fwlink/?linkid=70410">Centrum pobierania firmy Microsoft</a> (http://go.microsoft.com/fwlink/?LinkId=70410, strona może być w języku angielskim).</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">SQL Server 2005 (opcjonalnie)</td>
<td style="border:1px solid black;">Program WSUS 3.0 zainstaluje Wewnętrzna baza danych systemu Windows, jeśli zgodna wersja programu SQL Server nie jest już zainstalowana. Użytkownicy planujący użycie pełnej bazy danych SQL Server muszą korzystać z (co najmniej) programu SQL Server 2005 z dodatkiem SP1 (dostępny w witrynie <a href="http://go.microsoft.com/fwlink/?linkid=66143">Microsoft Download Center</a> (http://go.microsoft.com/fwlink/?LinkId=66143) w systemie Windows Server 2003 lub programu SQL Server 2005 z dodatkiem SP2 (dostępny w witrynie <a href="http://go.microsoft.com/fwlink/?linkid=84823">Microsoft Download Center</a> na stronie http://go.microsoft.com/fwlink/?LinkId=84823) w systemie Windows Server 2008.</td>
</tr>
</tbody>
</table>
  
> [!note]  
> Jeśli program WSUS 2.0 został już zainstalowany i korzysta z bazy danych SQL Server 2000, SQL Server Desktop Engine 2000 lub dowolnej bazy danych SQL Server wcześniejszej niż SQL Server 2005 z dodatkiem Service Pack 1 (lub SQL Server 2005 z dodatkiem SP2 w systemie Windows Server 2008), instalator programu WSUS 3.0 zainstaluje program Windows® Internal Database oraz dokona migracji bazy danych do tego formatu. 
  
Wymagania dotyczące minimalnej ilości wolnego miejsca na dysku dla instalacji serwera WSUS 3.0  
----------------------------------------------------------------------------------------------
  
W przypadku instalowania programu Windows Server Update Services konieczne jest spełnienie następujących wymagań dotyczących minimalnej ilości wolnego miejsca na dysku:
  
-   1 GB na partycji systemowej  
-   2 GB dla woluminu, na którym będą przechowywane pliki bazy danych  
-   20 GB dla woluminu, na którym będzie przechowywana zawartość
  
> [!Important]  
> Programu WSUS 3.0 nie można zainstalować na dyskach skompresowanych. Upewnij się, że wybrany dysk nie jest dyskiem skompresowanym. 
  
Wymagania dotyczące uaktualnienia WSUS 3.0  
------------------------------------------
  
#### Przed rozpoczęciem uaktualniania upewnij się, czy zainstalowany program WSUS działa prawidłowo, i wykonaj kopię zapasową bazy danych WSUS
  
W przypadku uaktualniania starszej wersji programu do wersji WSUS 3.0 upewnij się, czy obecnie zainstalowany program działa prawidłowo, i przed rozpoczęciem uaktualniania wykonaj kopię zapasową bazy danych WSUS.
  
1.  Sprawdź, czy w dziennikach zdarzeń nie ma informacji o występujących ostatnio błędach, problemach z synchronizacją między serwerami podrzędnymi a nadrzędnymi i problemach z brakiem raportowania przez klientów. Kontynuuj dopiero po upewnieniu się, że problemy te zostały usunięte.  
2.  Warto uruchomić program DBCC CHECKDB w celu sprawdzenia, czy baza danych WSUS została prawidłowo zaindeksowana. Aby uzyskać więcej informacji o programie CHECKDB, zobacz [DBCC CHECKDB](http://go.microsoft.com/fwlink/?linkid=86948) (http://go.microsoft.com/fwlink/?LinkId=86948).  
3.  Wykonywanie kopii zapasowej bazy danych WSUS.
  
#### Należy odinstalować program Software Update Services 1.0.
  
Instalacja programu WSUS 3.0 zakończy się niepowodzeniem, jeśli na tym samym komputerze jest zainstalowany program Software Update Services 1.0. Przed zainstalowaniem programu WSUS 3.0 należy odinstalować program Software Update Services 1.0.
  
#### Uaktualnianie z wersji beta programu WSUS 3.0 do jego wersji RTM nie jest obsługiwane, ale uaktualnianie z wersji RC do wersji RTM jest dozwolone.
  
Jeśli na komputerze znajduje się już wersja beta programu WSUS 3.0, przed zainstalowaniem wersji RTM tego programu należy odinstalować istniejącą wersję oraz usunąć bazę danych programu. Uaktualnianie można wykonać tylko z wersji RC do wersji RTM.
  
#### Nie można uaktualnić programu WSUS z wersji 2.0 do wersji 3.0 w 64-bitowym systemie operacyjnym.
  
Program WSUS 2.0 jest nieobsługiwany w 64-bitowych systemach operacyjnych. Nie można uaktualnić programu WSUS z wersji 2.0 do wersji 3.0 w 64-bitowych systemach operacyjnych.
  
Parametry wiersza polecenia Instalatora  
---------------------------------------
  
Przy użyciu parametrów wiersza polecenia programu WSUS można wykonać instalacje nienadzorowane programu WSUS 3.0. W tabeli poniżej podano parametry wiersza polecenia programu WSUS 3.0.
  
<p></p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Opcja</th>
<th style="border:1px solid black;" >Opis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>/q</strong></td>
<td style="border:1px solid black;">Przeprowadzenie instalacji dyskretnej.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>/u</strong></td>
<td style="border:1px solid black;">Odinstalowywanie produktu. Odinstalowane zostaną także wystąpienia programu Wewnętrzna baza danych systemu Windows, jeśli jest zainstalowany.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>/p</strong></td>
<td style="border:1px solid black;">Tylko sprawdzenie wymagań wstępnych. Nie instaluje produktu, lecz sprawdza system i zgłasza ewentualne niespełnione wymagania wstępne.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>/?, /h</strong></td>
<td style="border:1px solid black;">Wyświetla parametry wiersza polecenia wraz z opisami.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>/g</strong></td>
<td style="border:1px solid black;">Uaktualnia od wersji 2.0 programu WSUS. Jedyny prawidłowy parametr tej opcji to /q (instalacja dyskretna). Jedyna prawidłowa właściwość tej opcji to DEFAULT_WEBSITE.</td>
</tr>
</tbody>
</table>
  
W tabeli poniżej podano właściwości wiersza polecenia programu WSUS 3.0.
  
<p></p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Właściwość</th>
<th style="border:1px solid black;" >Opis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">CONTENT_LOCAL</td>
<td style="border:1px solid black;">0=zawartość obsługiwana lokalnie, 1=obsługiwana przez usługę Microsoft Update</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CONTENT_DIR</td>
<td style="border:1px solid black;">Ścieżka do katalogu zawartości Wartość domyślna to <em>WSUSInstallationDrive</em><strong>\WSUS\WSUSContent</strong>, gdzie <em>WSUSInstallationDrive</em> to dysk lokalny o największej ilości wolnego miejsca.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">WYUKON_DATA_DIR</td>
<td style="border:1px solid black;">Ścieżka do katalogu danych Wewnętrzna baza danych systemu Windows.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">SQLINSTANCE_NAME</td>
<td style="border:1px solid black;">Nazwa powinna występować w formacie <em>nazwa_serwera</em>\<em>nazwa_wystąpienia_SQL</em>. Jeżeli wystąpienie bazy danych znajduje się na komputerze lokalnym, należy użyć zmiennej środowiskowej %COMPUTERNAME%. Jeżeli istniejące wystąpienie jest nieobecne, nazwą domyślną jest %COMPUTERNAME%\WSUS.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DEFAULT_WEBSITE</td>
<td style="border:1px solid black;">0=port 8530, 1=port 80</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PREREQ_CHECK_LOG</td>
<td style="border:1px solid black;">Ścieżka i nazwa pliku dziennika</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">CONSOLE_INSTALL</td>
<td style="border:1px solid black;">0=zainstaluj serwer WSUS, 1=zainstaluj tylko konsolę</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ENABLE_INVENTORY</td>
<td style="border:1px solid black;">0=bez instalacji funkcji magazynu, 1=instalacja funkcji magazynu</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DELETE_DATABASE</td>
<td style="border:1px solid black;">0=zachowanie bazy danych, 1=usunięcie bazy danych</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DELETE_CONTENT</td>
<td style="border:1px solid black;">0=zachowanie plików zawartości, 1=usunięcie plików zawartości</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DELETE_LOGS</td>
<td style="border:1px solid black;">0=zachowaj pliki dziennika, 1=usuń pliki dziennika (używane z przełącznikiem instalacji /u).</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CREATE_DATABASE</td>
<td style="border:1px solid black;">0=użycie bieżącej bazy danych, 1=utworzenie bazy danych</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PROGRESS_WINDOW_HANDLE</td>
<td style="border:1px solid black;">Uchwyt okna służący do zwracania komunikatów postępu MSI</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">MU_ROLLUP</td>
<td style="border:1px solid black;">1=przystąpienie do Programu poprawy jakości rozszerzenia Microsoft Update, 0=nieprzystąpienie do programu</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">FRONTEND_SETUP</td>
<td style="border:1px solid black;">1=nie zapisuj lokalizacji zawartości w bazie danych, 0=zapisz lokalizację zawartości w bazie danych (dla technologii NLB)</td>
</tr>
</tbody>
</table>
  
#### Przykładowe użycie
  
```  
WSUSSetup.exe /q DEFAULT\_WEBSITE=0 (install in quiet mode using port 8530) 
WSUSSetup.exe /q /u (uninstall WSUS)  
```  
> [!Important]  
> Jeśli program WSUS 3.0 jest instalowany w trybie cichym (/q), a komputer nie spełnia wymagań wstępnych, instalator wygeneruje plik o nazwie WSUSPreReqCheck.xml i zapisze go w katalogu %TEMP%. 
  
Problemy z instalacją  
---------------------
  
#### Program IIS zostanie ponownie uruchomiony podczas instalowania programu WSUS 3.0.
  
Instalator programu WSUS 3.0 uruchomi ponownie program IIS bez powiadomienia. Może to wpłynąć na istniejące witryny sieci Web znajdujące się w organizacji. Jeśli program IIS nie jest uruchomiony, instalator programu WSUS 3.0 spowoduje jego uruchomienie.
  
#### Jeśli połączenia są aktywne dla istniejącej bazy danych programu WSUS, instalacja może zakończyć się niepowodzeniem.
  
W przypadku uaktualniania programu do wersji WSUS 3.0 z istniejącej instalacji, gdy połączenia są nadal aktywne dla istniejącej bazy danych programu WSUS (na przykład, jeśli jest otwarty program SQL Server Management Studio), instalacja może zakończyć się niepowodzeniem. Zamknij wszystkie połączenia i zainstaluj ponownie program WSUS 3.0.
  
#### Instalator programu WSUS wyświetla nieprawidłowy katalog dla plików bazy danych.
  
Na ekranie instalatora WSUS **Gotowy do zainstalowania** jest wyświetlana niewłaściwa informacja, że lokalizacją bazy danych jest katalog nadrzędny. Na przykład zamiast lokalizacji domyślnej %systemdrive%\\WSUS\\UpdateServicesDbFiles instalator podaje ścieżkę %systemdrive%\\WSUS.
  
#### Jeśli program WSUS zostanie zainstalowany na komputerze z pakietami wielojęzycznego interfejsu użytkownika i domyślnym językiem innym niż angielski, Pomoc programu będzie wyświetlania w tym języku
  
Użytkownicy komputerów z pakietami wielojęzycznego interfejsu użytkownika i domyślnym językiem innym niż angielski mogą zainstalować program WSUS, jeśli bieżący użytkownik korzysta z angielskich ustawień regionalnych. Interfejs użytkownika będzie dostępny w wersji angielskiej, ale uzyskanie wyświetlania Pomocy w tym języku wymaga zastosowania obejścia. Należy skopiować plik .chm z Pomocą w języku angielskim (*WSUSInstallDir*\\documentation\\mui\\0409\\WSUS30Help.chm) do głównego katalogu dokumentacji (*WSUSInstallDir*\\documentation\\WSUS30Help.chm). Od tego momentu Pomoc powinna być wyświetlana prawidłowo we wszystkich językach.
  
Problemy dotyczące uaktualniania  
--------------------------------
  
#### Uaktualnienie z wersji WSUS 3.0 RC do WSUS 3.0 RTM spowoduje, że witrynie sieci Web programu WSUS nie zostanie przypisany certyfikat SSL
  
Podczas uaktualnienia z wersji WSUS 3.0 RC do WSUS 3.0 RTM witryna sieci Web programu WSUS jest usuwana i tworzona na nowo. W rezultacie witryna WSUS zostaje pozbawiona przypisanego certyfikatu SSL. Konieczne będzie ponowne przypisanie certyfikatu po zakończeniu uaktualnienia.
  
#### Odzyskiwanie instalacji po błędzie uaktualnienia.
  
Jeśli podczas uaktualniania programu WSUS 2.0 do wersji WSUS 3.0 proces zakończy się niepowodzeniem, należy zainstalować ponownie program WSUS 2.0 i przywrócić jego bazę danych z kopii zapasowej.
  
#### Nie można wykonać uaktualnienia programu WSUS 2.0 do wersji WSUS 3.0, jeśli istnieje baza danych programu WSUS 3.0 pochodząca z poprzedniej instalacji.
  
Jeśli poprzednio zainstalowano program WSUS 3.0, a następnie zainstalowano program WSUS 2.0, przed ponownym zainstalowaniem programu WSUS 3.0 należy usunąć bazę danych programu WSUS 2.0.
  
#### Zmiana nazwy komputera przed uaktualnieniem programu WSUS do wersji 3.0 może spowodować, że uaktualnianie nie powiedzie się.
  
W przypadku zmiany nazwy komputera po zainstalowaniu programu WSUS 2.0, a przed uaktualnieniem programu WSUS do wersji 3.0 uaktualnianie może zakończyć się niepowodzeniem.
  
Użyj następującego skryptu, aby usunąć i dodać ponownie grupy ASPNET i Administratorzy WSUS. Następnie ponownie uruchom uaktualnianie.
  
Nazwę *&lt;lokalizacja\_bazy\_danych&gt;* należy zastąpić nazwą folderu, w którym baza danych jest zainstalowana, a nazwę *&lt;katalog\_zawartosci&gt;* należy zastąpić nazwą folderu przechowywania plików.
  
```  
sqlcmd.exe -S <DBLocation> -E -Q "USE SUSDB DECLARE @asplogin varchar(200) SELECT @asplogin=name from sysusers WHERE name like '%ASPNET' EXEC sp_revokedbaccess @asplogin"
sqlcmd.exe -S <DBLocation> -E -Q "USE SUSDB DECLARE @wsusadminslogin varchar(200) SELECT @wsusadminslogin=name from sysusers WHERE name like '%WSUS Administrators' EXEC sp_revokedbaccess @wsusadminslogin"

sqlcmd.exe -S <DBLocation> -E -Q "USE SUSDB DECLARE @asplogin varchar(200) SELECT @asplogin=HOST_NAME()+'\ASPNET' EXEC sp_grantlogin @asplogin EXEC sp_grantdbaccess @asplogin EXEC sp_addrolemember webService,@asplogin"
sqlcmd.exe -S <DBLocation> -E -Q "USE SUSDB DECLARE @wsusadminslogin varchar(200) SELECT @wsusadminslogin=HOST_NAME()+'\WSUS Administrators' EXEC sp_grantlogin @wsusadminslogin EXEC sp_grantdbaccess @wsusadminslogin EXEC sp_addrolemember webService,@wsusadminslogin"

sqlcmd.exe -S <DBLocation> -E -Q "backup database SUSDB to disk=N'<ContentDirectory>\SUSDB.Dat' with init" 
```
  
#### Instalator może zastąpić kopię zapasową poprzedniej bazy danych.
  
Instalator programu WSUS 3.0 dodaje bazę danych w katalogu określonym w czasie przeprowadzania instalacji. Domyślnie jest to katalog *%systemdrive%*\\WSUS\\UpdateServicesDbFiles. Jeśli w tym katalogu znajduje się kopia zapasowa poprzedniej bazy danych, zostanie ona zastąpiona przez nową bazę danych. Administratorzy powinni wykonać kopię zapasową plików bazy danych przed zastosowaniem aktualizacji na komputerach, na których znajduje się baza danych.
  
#### W przypadku przeprowadzenia migracji z programu MSDE do programu SQL Server 2000 lub SQL Server 2005 w programie WSUS 2.0 konieczna będzie zmiana wartości w rejestrze
  
Jeśli w systemie zainstalowano program WSUS 2.0 i została przeprowadzona migracja z programu SQL Server 2000 lub SQL Server 2005, konieczna będzie zmiana wartości klucza **HKLM\\SOFTWARE\\Microsoft\\Update Services\\Server\\Setup\\WmsdeInstalled** z 1 na 0. Jeśli wartość ta nie zostanie zmieniona przed rozpoczęciem procesu uaktualniania do wersji WSUS 3.0, uaktualnienie nie powiedzie się.
  
#### Uruchomienie i anulowanie działania instalatora programu WSUS 2.0 powoduje usunięcie klucza rejestru programu WSUS.
  
Anulowanie działania instalatora programu WSUS 2.0 wkrótce po jego uruchomieniu powoduje usunięcie klucza rejestru programu WSUS. Może to spowodować występowanie problemów, jeśli na komputerze jest już zainstalowany program WSUS 3.0. Ten sam problem może wystąpić w przypadku rozpoczęcia dezinstalacji programu WSUS 2.0, a następnie anulowania tej operacji i podjęcia próby uaktualnienia programu WSUS z wersji 2.0 do wersji 3.0.
  
#### Po odinstalowaniu programu WSUS 3.0 i pozostawieniu plików dziennika pliki te mogą mieć nieprawidłowe uprawnienia po ponownym zainstalowaniu programu.
  
W czasie odinstalowywania programu WSUS 3.0 użytkownik może zachować pliki dziennika instalacji. Po ponownym zainstalowaniu programu WSUS 3.0 stare pliki dziennika tracą swoje uprawnienia (zwykle są to uprawnienia tylko dla grupy Administratorzy WSUS). Należy przywrócić uprawnienia dla tych plików dziennika.
  
#### Jeżeli program Windows SharePoint Services został zainstalowany później niż program WSUS 3.0 w wersji RC, uaktualnianie do programu WSUS 3.0 w wersji RTM zostanie zakończone pomyślnie dzięki zastosowaniu odpowiedniej procedury.
  
Jeśli na komputerze zainstalowano program WSUS 3.0 w wersji RC, a następnie zainstalowano program Windows SharePoint Services, można dokonać uaktualnienia programu WSUS do wersji 3.0 RTM tylko po wybraniu opcji instalacji przy użyciu portu niestandardowego (portu 8530). Aby wykonać instalację z wiersza polecenia, należy otworzyć powłokę poleceń, a następnie wprowadzić polecenie: **WSUSSetup /q / g/ DEFAULT\_WEBSITE=0**. (Aby wykonać instalację za pomocą interfejsu użytkownika, należy wpisać polecenie **WSUSSetup /g DEFAULT\_WEBSITE=0**.)
  
Jeśli program WSUS zostanie zainstalowany na komputerze z pakietami wielojęzycznego interfejsu użytkownika, Pomoc nie będzie wyświetlana w bieżącym języku użytkownika, lecz w języku domyślnym
  
#### Jeśli dla klientów WSUS 2.0 istnieją aktualizacje o statusie „Nie dotyczy”, przez krótki okres czasu po uaktualnieniu do wersji WSUS 3.0 będą one widoczne jako aktualizacje o statusie „Nieznany”
  
Jeśli serwer WSUS 2.0 ma klientów z aktualizacjami o statusie „Nie dotyczy”, przez krótki okres czasu po uaktualnieniu serwera do wersji WSUS 3.0 dla aktualizacji tych będzie wyświetlany status „Nieznany” Status aktualizacji powróci do wartości „Nie dotyczy” po następnym skanowaniu przeprowadzonym przez klienta.
  
Znane problemy  
--------------
  
#### Rozwiązywanie problemów z wielokrotnymi błędami pobierania lub powtarzającymi się błędami synchronizacji komputerów klienckich.
  
Jeśli klienci WSUS 3.0 zgłaszają przez dłuższy okres wiele błędów pobierania lub jeśli klienci nie mogą przeprowadzić synchronizacji z serwerem programu WSUS 3.0, może być uszkodzona pamięć podręczna pobierania na komputerze klienckim. Aby przywrócić prawidłowy stan, można usunąć pamięć podręczną pobierania z systemu plików.
  
Aby usunąć pamięć podręczną pobierania na komputerze klienckim:
  
1.  Usuń wszystkie pliki i podkatalogi w tej lokalizacji na komputerze klienckim: **%windir%\\SoftwareDistribution\\Download**  
2.  Spróbuj zainstalować aktualizację, synchronizując ponownie komputer kliencki z programem WSUS 3.0. Ta instalacja powinna zakończyć się niepowodzeniem i powinien zostać wyświetlony następujący komunikat o błędzie: **WU\_E\_DM\_NOTDOWNLOADED, „Nie pobrano aktualizacji.”**  
3.  Po wystąpieniu tego błędu komputer kliencki zostanie automatycznie ponownie uruchomiony i będzie można kontynuować instalację.
  
#### W przypadku błędu synchronizacji należy ponownie przeprowadzić ten proces.
  
W przypadku nieudanej synchronizacji, pierwszą czynnością naprawczą powinna być próba wykonania ponownej synchronizacji z serwerem. Jeśli następna synchronizacja zakończy się niepowodzeniem, należy skorzystać z informacji dotyczących rozwiązywania problemów w [Przewodniku obsługi programu Windows Server Update Services 3.0](http://go.microsoft.com/fwlink/?linkid=81072) (http://go.microsoft.com/fwlink/?LinkId=81072, strona może być w języku angielskim).
  
#### Nie można zmienić konfiguracji programu WSUS 3.0 bezpośrednio w bazie danych.
  
Program Windows Server Update Services przechowuje swoje dane konfiguracyjne w bazie danych programu SQL Server. Nie jest jednak możliwa zmiana tych informacji bezpośrednio w bazie danych. Nie należy podejmować prób modyfikowania konfiguracji programu WSUS 3.0 przez uzyskiwanie bezpośredniego dostępu do bazy danych. Konfigurację programu WSUS 3.0 należy zmieniać za pomocą konsoli programu WSUS 3.0 lub przez wywołania API programu WSUS 3.0.
  
#### Błędy pobierania nie są wyświetlane z odpowiednią szybkością, jeśli włączono przydziały dysku.
  
Jeśli włączono przydziały dysku i zostały one osiągnięte, komunikaty o błędach pobierania aktualizacji występujące na serwerze WSUS mogą nie być wyświetlane odpowiednio szybko. Aby uniknąć tego problemu, należy wyłączyć przydziały dysku lub zwiększyć istniejący przydział.
  
#### Jeśli program WSUS 3.0 jest rozmieszczany przy użyciu protokołu SSL, komputery klienckie mogą zwracać kod błędu 0x8024400a.
  
Komputery klienckie zwracają czasami błąd „0x8024400a” w czasie nawiązywania połączenia z serwerem programu WSUS 3.0 przy użyciu protokołu SSL. Aby uzyskać informacje na temat rozwiązania tego problemu, zobacz artykuł [KB 905422](http://go.microsoft.com/fwlink/?linkid=70593) (http://go.microsoft.com/fwlink/?LinkId=70593, strona może być w języku angielskim).
  
#### Konto domeny Administratorzy WSUS nie zostanie usunięte po odinstalowaniu programu WSUS.
  
Grupa Administratorzy WSUS jest utworzona jako konto domeny (nie jako konto lokalne) na kontrolerach domeny, więc wszystkie instalacje korzystające z tego konta domeny mogą zostać wyłączone w przypadku usunięcia podczas dezinstalacji programu WSUS. Dlatego dezinstalacja programu WSUS nie powoduje usunięcia konta domeny Administratorzy WSUS.
  
#### Jeśli serwer podrzędny jest konwertowany na serwer nadrzędny, należy ponownie zaimportować aktualizacje witryny wykazu.
  
W przypadku awansowania serwera podrzędnego do roli serwera nadrzędnego należy także zaimportować ponownie wszystkie aktualizacje witryny wykazu. W przeciwnym razie witryna nie będzie mogła dokonać synchronizacji nowych poprawek aktualizacji witryny wykazu z tym serwerem.
  
#### W przypadku korzystania z programu IIS i protokołu SSL nadal jest możliwy dostęp nieszyfrowany, jeśli nie zaznaczono opcji „Wymagaj bezpiecznego kanału”.
  
W przypadku skonfigurowania programu IIS w celu używania protokołu SSL przez zainstalowanie certyfikatu można nadal uzyskać dostęp do witryny za pomocą niezaszyfrowanego protokołu HTTP, jeśli nie zaznaczono opcji „Wymagaj bezpiecznego kanału”. Aby uzyskać więcej informacji, zobacz artykuł na temat [włączania szyfrowania](http://go.microsoft.com/fwlink/?linkid=70601) (http://go.microsoft.com/fwlink/?LinkId=70601, strona może być w języku angielskim).
  
#### Importowanie witryny wykazu może zakończyć się niepowodzeniem w przypadku nienadania uprawnień odczytu/zapisu dla folderu %windir%\\TEMP.
  
Podczas importowania witryny wykazu proces, jeśli konto Network Service nie ma uprawnień odczytu/zapisu dla folderu %windir%\\TEMP, może zostać wyświetlony następujący komunikat o błędzie: „Serwer nie może przetworzyć żądania. ---&gt; Nie można znaleźć pliku C:\\WINDOWS\\TEMP\\*nazwa\_pliku\_tymczasowego*.dll."
  
#### Wydajność może obniżyć się w czasie synchronizowania programu WSUS 3.0 oraz podrzędnego serwera repliki z programem WSUS 2.0.
  
Jeśli program WSUS 3.0 jest zainstalowany na serwerze nadrzędnym i zostanie dokonana próba synchronizacji z podrzędnym serwerem repliki z programem WSUS 2.0, mogą wystąpić problemy z wydajnością. Aby rozwiązać ten problem, zobacz artykuł [KB 910847](http://go.microsoft.com/fwlink/?linkid=70669) (http://go.microsoft.com/fwlink/?LinkId=70669, strona może być w języku angielskim).
  
#### Jeśli serwer pocztowy nie działa lub nie jest dostępny, funkcja powiadamiania pocztą e-mail nie działa.
  
Jeśli sieciowy serwer poczty e-mail działa w trybie offline, program WSUS 3.0 bez powiadomienia wyłączy tę funkcję w trybie cichym. W dzienniku zdarzeń zostanie jednak zapisane zdarzenie 10052 (HealthCoreEmailNotificationRed).
  
#### Zmienione ustawienia serwera nadrzędnego nie są natychmiast wypychane do serwera podrzędnego.
  
Po zmianie konfiguracji serwera nadrzędnego wprowadzenie zmian konfiguracji może chwilę potrwać. Na przykład, jeśli zmieniane jest ustawienie serwera nadrzędnego, takie jak nowy język, a następnie jest wyzwalana synchronizacja na serwerze podrzędnym, zmiana nie zostanie uwzględniona. Zostanie ona wypchnięta do serwera podrzędnego w czasie następnej zaplanowanej synchronizacji. Czas oczekiwania zwiększa się w zależności od liczby aktualizacji obecnych na serwerze nadrzędnym.
  
#### Odinstalowanie programu WSUS 3.0 nie powoduje odinstalowania wystąpienia bazy danych.
  
Po odinstalowaniu programu WSUS 3.0 wystąpienie bazy danych nie zostanie odinstalowane. Wystąpienie może być używane przez więcej niż jedną aplikację i spowodować wystąpienie błędów innych aplikacji w przypadku jego usunięcia.
  
Jeśli będzie konieczne odinstalowanie programu Wewnętrzna baza danych systemu Windows, następujące polecenia spowodują odinstalowanie tej aplikacji:
  
(platformy 32-bitowe)
  
```  
msiexec /x {CEB5780F-1A70-44A9-850F-DE6C4F6AA8FB} callerid=ocsetup.exe  
```  
(platformy 64-bitowe)
  
```  
msiexec /x {BDD79957-5801-4A2D-B09E-852E7FA64D01} callerid=ocsetup.exe  
```  
Aby odinstalować dodatek Service Pack 2 dla programu Wewnętrzna baza danych systemu Windows w systemie Windows Server 2008, można to zrobić za pomocą programu Server Manager.
  
Usunięcie tej aplikacji nie spowoduje jednak usunięcia domyślnych plików mdf i ldf, co z kolei spowoduje błąd instalacji programu WSUS 3.0. Pliki te można usunąć w katalogu %windir%\\SYSMSI\\SSEE.
  
#### Jeśli serwer podrzędny powoduje zmianę serwera nadrzędnego, stany aktualizacji „Nieznane” są wyświetlane jako „Nie dotyczy”.
  
Jeśli serwer podrzędny uruchamia synchronizację na innym serwerze nadrzędnym, aktualizacje o stanie „Nieznane” zostaną zgłoszone nowemu serwerowi nadrzędnemu jako „Nie dotyczy”. Ten stan jest tymczasowy i zostanie on poprawiony przy następnym przesyłaniu informacji o stanie z serwera podrzędnego po dokonaniu synchronizacji z komputerami klienckimi.
  
#### Jeśli serwer repliki z programem WSUS 3.0 zarządza więcej niż jednym komputerem o tej samej nazwie generowanie zestawienia raportów zostanie zakończone niepowodzeniem.
  
Jeśli serwer repliki z programem WSUS 3.0 zarządza więcej niż jednym komputerem o tej samej nazwie generowanie zestawienia raportów zostanie zakończone niepowodzeniem. W wyniku tego raporty dostępne dla katalogu głównego serwera WSUS będą niepełne. Ten problem można rozwiązać, usuwając wpisy zduplikowanych komputerów znajdujące się na serwerze repliki, pozostawiając przy tym tylko jeden z tych wpisów.
  
#### Jeśli Kreator oczyszczania serwera przekroczył limit czasu na jednym serwerze po uruchomieniu na wielu serwerach z poziomu konsoli zdalnej, połączenia ze wszystkimi serwerami zostaną utracone.
  
Kreatora oczyszczania serwera można uruchomić na wielu serwerach z poziomu pojedynczej konsoli zdalnej. Jeśli jednak proces oczyszczania przekroczy limit czasu na jednym z serwerów, konsola straci połączenie ze wszystkimi serwerami. Nie zostaną utracone żadne dane, ale administrator będzie musiał zresetować zdalne połączenie z każdym z serwerów.
  
#### Kreator oczyszczania serwera usuwa pliki po trzydziestu dniach, a nie po trzech miesiącach.
  
Niektóre informacje w Kreatorze oczyszczania serwera są niedokładne. Polecenie Kreatora brzmi: „Usuń aktualizacje wygasłe i niezatwierdzone od trzech miesięcy oraz usuń stare poprawki aktualizacji, które nie zostały zatwierdzone od trzech miesięcy”. Poprawny okres wynosi trzydzieści dni, a nie trzy miesiące.
  
#### Uruchamianie i zatrzymywanie działania połączenia w krótkim odstępie czasu powoduje wyświetlenie komunikatu o braku błędów w Kreatorze konfiguracji.
  
Podczas konfigurowania programu WSUS należy nawiązać połączenie z serwerem nadrzędnym (serwerem usługi Microsoft Update lub serwerem w sieci intranetowej) w celu przesłania podstawowych informacji o serwerze. Jeśli klikniesz przycisk **Rozpocznij połączenie**, a następnie natychmiast klikniesz przycisk **Zatrzymaj połączenie**, zostanie wyświetlony niewłaściwy komunikat „Brak błędów synchronizacji”.
  
#### Komputery klienckie z programem WSUS działające w systemie Windows Vista w wersji RTM mogą teraz wyszukiwać aktualizacje w witrynie Microsoft Update.
  
W poprzednich wersjach programu WSUS komputery klienckie z systemem Windows Vista w wersji RTM mogły pobierać aktualizacje wyłącznie z serwera WSUS. Po zainstalowaniu programu WSUS 3.0 w wersji RTM komputery klienckie z systemem Windows Vista mogą teraz pobierać aktualizacje także z witryny Microsoft Update. Dla komputerów klienckich z systemem Windows Vista można włączyć przekierowanie do witryny Microsoft Update, otwierając witrynę Windows Update w Panelu sterowania i klikając hiperłącze **Sprawdź aktualizacje w trybie online za pomocą usługi Microsoft Update**. Jeśli została włączona opcja zasad grupy **Usuń dostęp do używania wszystkich funkcji witryny Windows Update**, w witrynie Windows Update to hiperłącze nie będzie wyświetlane.
  
WSUS 3.0 w systemie Windows Server 2008  
---------------------------------------
  
#### Obsługiwane wersje
  
Program WSUS 3.0 obsługuje system Windows Server 2008 w wersjach 32-bitowych i 64-bitowych.
  
#### Wymagania wstępne
  
<p></p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Wymaganie</th>
<th style="border:1px solid black;" >Szczegóły</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Program Microsoft Internet Information Services (IIS)</td>
<td style="border:1px solid black;">Instalacja z poziomu systemu operacyjnego. Należy upewnić się, że następujące składniki są włączone:

Funkcja uwierzytelniania systemu Windows

Funkcja zawartości statycznej

Program ASP.NET

Funkcja zgodności zarządzania z wersją 6.0

Funkcja zgodności metabazy programu IIS</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Pakiet redystrybucyjny systemu Microsoft .NET Framework w wersji 2.0 (x86)</td>
<td style="border:1px solid black;">Włączenie tych składników nie jest konieczne w przypadku systemu Windows Server 2008, ponieważ są one zainstalowane jako elementy systemu operacyjnego.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Program Microsoft Management Console 3.0</td>
<td style="border:1px solid black;">Włączenie tych składników nie jest konieczne w przypadku systemu Windows Server 2008, ponieważ są one zainstalowane jako elementy systemu operacyjnego.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Narzędzie Podgląd raportów firmy Microsoft</td>
<td style="border:1px solid black;">To jest wymaganie wstępne dotyczące korzystania z interfejsu użytkownika programu WSUS. Zobacz stronę z opisem wersji redystrybucyjnej narzędzia Podgląd raportów firmy Microsoft 2005 w witrynie <a href="http://go.microsoft.com/fwlink/?linkid=70410">Centrum pobierania firmy Microsoft</a> (http://go.microsoft.com/fwlink/?LinkId=70410, strona może być w języku angielskim).</td>
</tr>
</tbody>
</table>
  
#### Problem 1: Przed uruchomieniem programu WSUS 3.0 należy zaktualizować plik konfiguracji programu IIS 7.0.
  
Przed uruchomieniem programu WSUS 3.0 w systemie Windows Server 2008 należy zaktualizować plik konfiguracji programu IIS. Należy wykonać następujące czynności:
  
1. Otwórz plik konfiguracji programu IIS: %WINDIR%\\system32\\inetsrv\\applicationhost.config
  
2. W metce &lt;System.webServer&gt;&lt;modules&gt; usuń wpis &lt;add name="CustomErrorMode"&gt;, jeśli występuje.
  
3. W metce &lt;System.webServer&gt;&lt;modules&gt; dodaj wpis &lt;remove name="CustomErrorMode"&gt;.
  
Metka powstała w wyniku tych operacji powinna mieć następującą postać:
  
```  
      <System.webServer>
<modules>
<remove name="CustomErrorMode">
</modules>
</System.webServer>
```
  
#### Problem 2: Aby zainstalować program WSUS 3.0 przy użyciu niestandardowego portu w systemie Windows Server 2008 Beta 3, należy wstępnie utworzyć witrynę sieci Web
  
Jeśli program WSUS 3.0 ma zostać zainstalowany w systemie Windows Server 2008 Beta 3 oraz skonfigurowany do używania niestandardowego portu 8530, przed uruchomieniem instalatora WSUS konieczne będzie utworzenie witryny sieci Web o nazwie „WSUS Administration” na porcie 8530.
  
Program WSUS 3.0 w programie Windows Small Business Server 2003  
---------------------------------------------------------------
  
#### Problem 1: Jeśli wirtualny katalog główny jest ograniczony do określonych adresów IP lub nazw domen, serwer programu WSUS 3.0 nie będzie mógł przeprowadzać samodzielnej aktualizacji.
  
W niektórych instalacjach programu Windows Small Business Server może występować domyślna witryna sieci Web programu IIS skonfigurowana na potrzeby opcji „Ograniczenia adresów IP i nazw domen”. W takim przypadku klient usługi Windows Update na serwerze nie będzie mógł przeprowadzić samodzielnej aktualizacji.
  
#### Problem 2: Instalowanie programu WSUS 3.0 w programie Small Business Server — problemy dotyczące integracji.
  
-   Jeśli w programie Windows Small Business Server 2003 dostęp do Internetu jest uzyskiwany za pośrednictwem serwera proxy ISA, korzystając z interfejsu użytkownika, należy ręcznie wprowadzić następujące dane w obszarze **Ustawienia**: ustawienia serwera proxy, nazwa serwera proxy oraz port.  
-   Jeśli w architekturze ISA jest używana funkcja uwierzytelniania systemu Windows, poświadczenia serwera proxy powinny zostać wprowadzane w formacie „DOMENA\\użytkownik”, a użytkownik powinien należeć do grupy użytkowników internetowych.
  
#### Problem 3: Jeśli do sieci dodano podsieć bez użycia kreatorów programu Windows SBS, należy wykonać poniższą procedurę.
  
W procesie instalacji serwera WSUS na serwerze są instalowane dwa wirtualne katalogi główne programu IIS: SelfUpdate oraz ClientWebService. Instalator umieszcza także niektóre pliki w katalogu głównym domyślnej witryny sieci Web (przy użyciu portu 80), który umożliwia komputerom klienckim przeprowadzanie samodzielnej aktualizacji za pośrednictwem domyślnej witryny sieci Web. Domyślna witryna sieci Web jest skonfigurowana tak, aby blokować dostęp do adresów IP innych niż localhost lub określonych podsieci skojarzonych z serwerem. W wyniku tego komputery klienckie, które nie znajdują się pod adresem localhost lub tych podsieciach, nie mogą przeprowadzać samodzielnej aktualizacji. Jeśli do sieci dodano podsieć bez użycia kreatorów programu Microsoft Windows Small Business Server 2003 (Windows SBS), należy wykonać poniższą procedurę.
  
1.  W obszarze Zarządzanie serwerem, rozwiń kolejno węzły **Zarządzanie zaawansowane**, **Internetowe usługi informacyjne**, **Witryny sieci Web**, **Domyślna witryna sieci Web**, kliknij prawym przyciskiem myszy katalog wirtualny **Selfupdate**, a następnie kliknij polecenie **Właściwości**.  
2.  Kliknij kartę **Ustawienia zabezpieczeń**.  
3.  W obszarze **Ograniczenia adresów IP i nazw domen** kliknij pozycję **Edycja**, a następnie kliknij pozycję **Udzielony dostęp**.  
4.  Kliknij przycisk **OK**, kliknij prawym przyciskiem myszy katalog wirtualny **ClientWebService**, a następnie kliknij polecenie **Właściwości**.  
5.  Kliknij kartę **Ustawienia zabezpieczeń**.  
6.  W obszarze **Ograniczenia adresów IP i nazw domen** kliknij pozycję **Edycja**, a następnie kliknij pozycję **Udzielony dostęp**.
  
#### Prawa autorskie
  
W tym dokumencie opisano wstępne wydanie oprogramowania, które może ulec znacznym zmianom przed ostatecznym wprowadzeniem na rynek. Informacje zawarte w tym dokumencie są poufne i stanowią własność firmy Microsoft Corporation. Dokument jest tajny, zgodnie z umową dotyczącą nieujawniania informacji, zawartą pomiędzy odbiorcą a firmą Microsoft. Ten dokument jest dostarczany wyłącznie w celach informacyjnych i firma Microsoft nie udziela w tym dokumencie żadnych gwarancji wyraźnych ani dorozumianych. Informacje zawarte w tym dokumencie, w tym adresy URL oraz inne odniesienia do witryn sieci Web mogą ulec zmianie bez powiadomienia. Całkowita odpowiedzialność związana z wynikiem użycia tego dokumentu spoczywa na użytkowniku. Jeśli nie określono inaczej, firmy, organizacje, produkty, nazwy domen, adresy e-mail, logo, osoby, miejsca i zdarzenia przedstawione w przykładach są fikcyjne. Żaden związek z jakąkolwiek rzeczywistą firmą, organizacją, produktem, nazwą domeny, adresem e-mail, logo, osobą, miejscem lub zdarzeniem nie był zamierzony ani nie należy go zakładać. Odpowiedzialność za dostosowanie się do stosownych praw autorskich spoczywa na użytkowniku. Bez ograniczania praw objętych prawem autorskim niniejszego dokumentu ani jego części nie wolno w żadnej formie powielać, przechowywać ani wprowadzać do żadnego systemu umożliwiającego odtworzenie, ani przekazywać za pomocą jakichkolwiek nośników (elektronicznych, mechanicznych, fotokopii, nagrania itp.) z wyjątkiem przypadków, w których uzyskano na to pisemną zgodę firmy Microsoft Corporation.
  
Firma Microsoft może mieć patenty lub rozpoczęte postępowania patentowe, znaki towarowe, prawa autorskie lub inne prawa związane z własnością intelektualną, które odnoszą się do treści zawartej w niniejszym dokumencie. Otrzymanie tego dokumentu nie oznacza udzielenia licencji na te patenty, znaki towarowe, prawa autorskie ani inne prawa związane z własnością intelektualną, z wyjątkiem wyraźnie określonych przypadków zawartych w pisemnych umowach licencyjnych firmy Microsoft.
  
© 2007 Microsoft Corporation. Wszelkie prawa zastrzeżone.
  
Microsoft, SQL Server, Windows i Windows Server są zastrzeżonymi znakami towarowymi lub znakami towarowymi firmy Microsoft Corporation zarejestrowanymi w USA i/lub w innych krajach.
  
Wszystkie inne znaki towarowe są własnością ich prawnych właścicieli.
