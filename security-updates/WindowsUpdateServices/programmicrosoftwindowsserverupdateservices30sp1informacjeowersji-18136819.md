---
TOCTitle: 'Program Microsoft Windows Server Update Services 3.0 SP1 — informacje o wersji'
Title: 'Program Microsoft Windows Server Update Services 3.0 SP1 — informacje o wersji'
ms:assetid: 'a5aa93bf-842b-4ad4-ab0f-fe867843cb02'
ms:contentKeyID: 18136819
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc708525(v=WS.10)'
---

Program Microsoft Windows Server Update Services 3.0 SP1 — informacje o wersji
==============================================================================

Niniejsze informacje o wersji zawierają opis znanych problemów z programem Microsoft® Windows® Server Update Services (WSUS) 3.0 z dodatkiem Service Pack 1 oraz zalecenia i wymagania dotyczące instalowania tej aplikacji. Dokument zawiera następujące sekcje:

-   Wymagania systemowe związane z instalacją serwera WSUS 3.0 SP1
-   Wymagania dotyczące konfiguracji związane z instalacją serwera WSUS 3.0 SP1
-   Wymagania systemowe związane z instalacją konsoli zdalnej programu WSUS 3.0 SP1
-   Wymagania systemowe związane z instalacją klienta
-   Wymagania dotyczące oprogramowania związane z instalacją serwera WSUS SP1
-   Wymagania dotyczące minimalnej ilości miejsca na dysku związane z instalacją serwera WSUS 3.0 SP1
-   Wymagania związane z uaktualnianiem do programu WSUS 3.0 SP1
-   Parametry wiersza polecenia Instalatora
-   Problemy z instalacją
-   Problemy z uaktualnianiem
-   Znane problemy
-   Program WSUS 3.0 SP1 w systemie Windows Server® 2008
-   Program WSUS 3.0 SP1 w systemie Windows Small Business Server 2003

Wymagania systemowe związane z instalacją serwera WSUS 3.0 SP1
--------------------------------------------------------------

#### Serwer WSUS 3.0 SP1 jest obsługiwany w systemach Windows Server 2008 oraz Windows Server 2003 z dodatkiem Service Pack 1

Serwer WSUS 3.0 SP1 jest obsługiwany w systemach Windows Server 2008 i Windows Server 2003 Service Pack 1.

#### Serwery WSUS 3.0 SP1 nie są obsługiwane w systemie Windows 2000 Server

Serwery WSUS 3.0 SP1 nie mogą działać w systemie operacyjnym Windows 2000 Server.

#### Program WSUS 3.0 SP1 nie jest obsługiwany na serwerach, na których działają usługi terminalowe

Mimo że uruchomienie programu WSUS 3.0 SP1 na serwerach z usługami terminalowymi może się powieść, taka konfiguracja nie jest obsługiwana ani zalecana. Program WSUS 3.0 SP1 nie będzie działać na serwerze z uruchomionymi usługami terminalowymi korzystającymi z implementacji zdalnego serwera SQL Server. Ze względu na to, że wszystkie zdalne akcje niestandardowe (w tym instalacja) na serwerze licencji usług terminalowych są uruchamianie w ramach konta systemowego, a konto systemowe serwera może nie mieć uprawnień na zdalnym serwerze SQL Server, instalacja może się nie powieść.

Wymagania dotyczące konfiguracji związane z instalacją serwera WSUS 3.0 SP1
---------------------------------------------------------------------------

#### Muszą być zainstalowane usługi IIS

Program WSUS 3.0 SP1 wymaga internetowych usług informacyjnych (IIS), które nie są domyślnie instalowane w systemach Windows Server 2008 i Microsoft Windows Server 2003. Próba zainstalowania programu WSUS 3.0 SP1 bez usług IIS powoduje wyświetlenie przez Instalatora programu Windows Server Update Services komunikatu o błędzie z informacją, że usługi IIS nie są zainstalowane.

#### Jeśli usługi IIS działają w trybie izolacji usług IIS 5.0, instalacja nie powiedzie się

Po uaktualnieniu serwera z systemem Windows 2000 Server do systemu Windows Server 2003 usługi IIS mogą działać w trybie zgodności usług IIS 5.0. Tryb izolacji usług IIS 5.0 może też zostać włączony w menedżerze usług IIS. Spowoduje to niepowodzenie instalacji. Przed zainstalowaniem programu WSUS 3.0 SP1 należy wyłączyć tryb izolacji usług IIS 5.0.

#### Jeśli jakikolwiek składnik usług IIS jest zainstalowany w trybie zgodności 32-bitowej na platformie 64-bitowej, instalacja programu WSUS 3.0 SP1 może się nie powieść

Na platformach 64-bitowych wszystkie składniki usług IIS powinny być zainstalowane w trybie macierzystym. Działanie jakiegokolwiek składnika usług IIS w trybie zgodności 32-bitowej może spowodować niepowodzenie instalacji.

#### Serwery proxy mogą obsługiwać tylko protokół HTTP lub protokoły HTTP i HTTPS

W programie WSUS 3.0 SP1 jest możliwe, aby serwer proxy obsługiwał tylko protokół HTTP. Drugi serwer proxy, na którym będzie działać protokół HTTPS, należy skonfigurować za pomocą wiersza polecenia (**wsusutil configuresslproxy**) przed skonfigurowaniem serwera WSUS z poziomu konsoli administracji lub Kreatora konfiguracji.

#### Jeśli dwie lub więcej witryn sieci Web używa już portu 80, przed zainstalowaniem programu WSUS należy je usunąć, pozostawiając tylko jedną

Jeśli dwie lub więcej witryn sieci Web używa portu 80 (np. witryny programu Windows® SharePoint® Services), przed zainstalowaniem programu WSUS należy je usunąć, pozostawiając tylko jedną z nich. Pominięcie tej operacji może spowodować niepowodzenie samoaktualizacji klientów serwera.

#### Na czas instalacji programu WSUS 3.0 SP1 może być konieczne wyłączenie programów antywirusowych

Pomyślne przeprowadzenie instalacji programu WSUS 3.0 SP1 może wymagać wyłączenia programów antywirusowych na czas instalacji. Po wyłączeniu programu antywirusowego, a przed rozpoczęciem instalacji programu WSUS należy ponownie uruchomić komputer. Zapobiega to blokowaniu plików, do których proces instalacji może wymagać dostępu. Należy pamiętać o ponownym włączeniu programu antywirusowego po ukończeniu instalacji. Aby uzyskać szczegółowe instrukcje dotyczące wyłączania i ponownego włączania konkretnej wersji programu antywirusowego, odwiedź witrynę dostawcy tego programu w sieci Web.

> [!Caution]  
> Wyłączenie programu antywirusowego może narazić używany komputer lub używaną sieć na ataki złośliwych użytkowników lub złośliwego oprogramowania, na przykład wirusów. Wykonanie tej operacji nie jest zalecane — powyższe informacje są podawane w celu umożliwienia użytkownikowi zastosowania tego rozwiązania, jeśli podejmie taką decyzję. Użytkownik wykonuje tę operację na własne ryzyko. 

> [!note]  
> Program antywirusowy służy do ochrony komputera przed wirusami. Przy wyłączonym programie antywirusowym nie należy pobierać ani otwierać plików pochodzących z niezaufanych źródeł, odwiedzać niezaufanych witryn sieci Web ani otwierać załączników do wiadomości e-mail. 

#### Program WSUS 3.0 SP1 wymaga, aby na serwerze SQL Server była włączona opcja zagnieżdżonych wyzwalaczy

Opcja zagnieżdżonych wyzwalaczy jest domyślnie włączona, jednak może zostać wyłączona przez administratora serwera SQL Server.

Jeśli jest planowane stosowanie bazy danych serwera SQL Server jako magazynu danych programu Windows Server Update Services, zanim administrator programu WSUS 3.0 SP1 zainstaluje go i w trakcie instalacji określi bazę danych, administrator serwera SQL Server powinien upewnić się, że opcja zagnieżdżonych wyzwalaczy jest włączona na tym serwerze.

Instalator programu WSUS 3.0 SP1 włącza opcję RECURSIVE\_TRIGGERS, która jest opcją specyficzną dla bazy danych, ale nie włącza opcji zagnieżdżonych wyzwalaczy, która jest globalną opcją serwera.

Aby sprawdzić, czy opcja zagnieżdżonych wyzwalaczy jest włączona, należy uruchomić polecenie:

**sp\_configure 'nested triggers'**

Aby włączyć opcję zagnieżdżonych wyzwalaczy na serwerze SQL Server, należy uruchomić następujące polecenia z poziomu pliku wsadowego na komputerze, na którym działa serwer SQL Server:

**sp\_configure 'nested triggers', 1**

**GO**

**RECONFIGURE**

**GO**

Jeśli na serwerze nie ma programu SQL Server Management Studio, należy uruchomić skrypty SQL z poziomu wiersza polecenia. Narzędzie Command Line Query Utility dla programu Microsoft SQL Server 2005 można pobrać z [Centrum pobierania Microsoft](http://go.microsoft.com/fwlink/?linkid=70728) (http://go.microsoft.com/fwlink/?LinkId=70728) (strona może zostać wyświetlona w języku angielskim). Aby rozpocząć, należy uruchomić polecenie **sqlcmd**.

Jeśli skrypty SQL mają korzystać z programu Wewnętrzna baza danych systemu Windows, należy pobrać również oprogramowanie klienckie SQL Server Native Client z tej samej strony pobierania.

#### Wymagania i ograniczenia zdalnego serwera SQL

Program WSUS 3.0 SP1 obsługuje rozwiązania, w których oprogramowanie bazy danych działa na komputerze innym niż komputer, na którym jest zainstalowana pozostała część aplikacji WSUS 3.0 SP1. Poniżej wymieniono wymagania dotyczące konfiguracji zdalnej instalacji serwera SQL:

-   Jako wewnętrznej bazy danych w parze instalacji zdalnej serwera SQL nie można używać serwera skonfigurowanego w charakterze kontrolera domeny.
-   Na komputerze, który ma być serwerem frontonu instalacji zdalnej serwera SQL, nie może działać serwer usług terminalowych.
-   Na komputerze z wewnętrzną bazą danych jako oprogramowania bazy danych należy użyć programu Microsoft SQL Server 2005 z dodatkiem Service Pack 1 dostępnego w [Centrum pobierania Microsoft](http://go.microsoft.com/fwlink/?linkid=66143) (http://go.microsoft.com/fwlink/?LinkId=66143) (strona może zostać wyświetlona w języku angielskim) lub nowszej wersji, jeśli jest to komputer z systemem Windows Server 2003, oraz programu SQL Server 2005 z dodatkiem Service Pack 2 lub nowszej wersji w przypadku komputera z systemem Windows Server® 2008.
-   Zarówno komputer będący serwerem frontonu, jak i komputer z wewnętrzną bazą danych muszą być przyłączone do domeny usługi Active Directory. W przeciwny przypadku — jeśli należą do różnych domen — przed uruchomieniem instalacji programu WSUS należy ustanowić relację zaufania między tymi domenami.
-   Jeśli istnieje już instalacja programu WSUS 2.0 w konfiguracji ze zdalnym serwerem SQL i jest planowane uaktualnienie do wersji WSUS 3.0 SP1, należy odinstalować program WSUS 2.0 (za pomocą apletu **Dodawanie lub usuwanie programów** w Panelu sterowania) na komputerze z wewnętrzną bazą danych, nie naruszając przy tym istniejącej bazy danych. Następnie należy zainstalować program SQL Server 2005 z dodatkiem SP1 lub SP2 i uaktualnić istniejącą bazę danych. Na końcu należy zainstalować program WSUS 3.0 SP1 na komputerze frontonu.

Wymagania systemowe związane z instalacją konsoli zdalnej programu WSUS 3.0 SP1
-------------------------------------------------------------------------------

Konsolę zdalną programu WSUS 3.0 SP1 można zainstalować na następujących platformach:

-   Windows Server 2008
-   Windows Vista® lub nowszej
-   Windows Server 2003 z dodatkiem SP1 lub nowszej
-   Windows XP z dodatkiem SP2 lub nowszej

Wymagania systemowe związane z instalacją klienta
-------------------------------------------------

Oprogramowanie klienckie programu WSUS to Aktualizacje automatyczne. Tego klienta można używać razem z programem WSUS w dowolnym z następujących systemów operacyjnych:

-   Windows Vista lub nowszy
-   Windows Server 2008 lub nowszy
-   Microsoft Windows Server 2003 (dowolne wydanie)
-   Microsoft Windows XP Professional z dodatkiem SP2 lub nowszy
-   Microsoft Windows 2000 Professional z dodatkiem SP4, Windows 2000 Server z dodatkiem SP4 lub Windows 2000 Advanced Server z dodatkiem SP4

Wymagania dotyczące oprogramowania związane z instalacją serwera WSUS 3.0 SP1
-----------------------------------------------------------------------------

W poniższej tabeli wymieniono oprogramowanie wymagane dla platform Windows Server 2003 z dodatkiem SP1. Oprogramowanie wymagane dla systemu Windows Server 2008 zostanie omówione w sekcji poświęconej programowi WSUS 3.0 SP1 w systemie Windows Server 2008.

Przed uruchomieniem instalacji programu WSUS 3.0 SP1 należy upewnić się, że serwer, na którym ten program ma działać, spełnia wymienione tu wymagania. Jeśli którakolwiek z tych aktualizacji wymaga ponownego uruchomienia komputera po ukończeniu instalacji, należy wykonać tę czynność przed zainstalowaniem programu WSUS 3.0 SP1.

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
<td style="border:1px solid black;">Internetowe usługi informacyjne (IIS) firmy Microsoft</td>
<td style="border:1px solid black;">Instalacja z poziomu systemu operacyjnego.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Pakiet dystrybucyjny środowiska .NET Framework 2.0 firmy Microsoft</td>
<td style="border:1px solid black;">Więcej informacji można znaleźć w opisie pakietu dystrybucyjnego środowiska Microsoft .NET Framework 2.0 dla architektury x86 w <a href="http://go.microsoft.com/fwlink/?linkid=68935">Centrum pobierania Microsoft</a> (http://go.microsoft.com/fwlink/?LinkId=68935) (strona może zostać wyświetlona w języku angielskim). W przypadku platform 64-bitowych więcej informacji można znaleźć w opisie pakietu dystrybucyjnego środowiska Microsoft .NET Framework 2.0 dla architektury x64 w <a href="http://go.microsoft.com/fwlink/?linkid=70637">Centrum pobierania Microsoft</a> (http://go.microsoft.com/fwlink/?LinkId=70637) (strona może zostać wyświetlona w języku angielskim).</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Program Microsoft Management Console 3.0 dla systemu Windows Server 2003</td>
<td style="border:1px solid black;">Wymaganie wstępne dotyczące interfejsu użytkownika programu WSUS 3.0 SP1. Więcej informacji można znaleźć w opisie programu Microsoft Management Console 3.0 dla systemu Windows Server 2003 (KB907265) w <a href="http://go.microsoft.com/fwlink/?linkid=70412">Centrum pobierania Microsoft</a> (http://go.microsoft.com/fwlink/?LinkId=70412) (strona może zostać wyświetlona w języku angielskim). W przypadku platform 64-bitowych więcej informacji można znaleźć w opisie programu Microsoft Management Console 3.0 dla systemu Windows Server 2003 x64 Edition (KB907265) w <a href="http://go.microsoft.com/fwlink/?linkid=70638">Centrum pobierania Microsoft</a> (http://go.microsoft.com/fwlink/?LinkId=70638) (strona może zostać wyświetlona w języku angielskim).</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Podgląd raportów firmy Microsoft</td>
<td style="border:1px solid black;">Wymaganie wstępne dotyczące interfejsu użytkownika programu WSUS 3.0 SP1. Więcej informacji można znaleźć w opisie pakietu dystrybucyjnego Podglądu raportów firmy Microsoft 2005 w <a href="http://go.microsoft.com/fwlink/?linkid=70410">Centrum pobierania Microsoft</a> (http://go.microsoft.com/fwlink/?LinkId=70410) (strona może zostać wyświetlona w języku angielskim).</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Program SQL Server 2005 (opcjonalnie)</td>
<td style="border:1px solid black;">Program WSUS 3.0 SP1 zainstaluje program Wewnętrzna baza danych systemu Windows, jeśli zgodna wersja programu SQL Server nie została jeszcze zainstalowana. Jeśli jest planowane korzystanie z bazy danych pełnej wersji serwera SQL Server, w systemie Windows Server 2003 należy użyć programu SQL Server 2005 SP1 (dostępnego w <a href="http://go.microsoft.com/fwlink/?linkid=66143">Centrum pobierania Microsoft</a> pod adresem http://go.microsoft.com/fwlink/?LinkId=66143) (strona może zostać wyświetlona w języku angielskim) lub nowszej wersji, natomiast w systemie Windows Server 2008 — programu SQL Server 2005 SP2 (dostępnego w <a href="http://go.microsoft.com/fwlink/?linkid=84823">Centrum pobierania Microsoft</a> pod adresem http://go.microsoft.com/fwlink/?LinkId=84823) (strona może zostać wyświetlona w języku angielskim) lub nowszej wersji.</td>
</tr>
</tbody>
</table>
  
> [!note]  
> Jeśli wcześniej zainstalowano program WSUS 2.0 i program ten używa bazy danych programu SQL Server 2000, SQL Server Desktop Engine 2000 lub innej bazy danych programu SQL Server starszej niż SQL Server 2005 z dodatkiem SP1 (albo SQL Server 2005 z dodatkiem SP2 w systemie Windows Server 2008), program instalacyjny aplikacji WSUS 3.0 SP1 instaluje program Windows® Internal Database i migruje do niego bazę danych. 
  
Wymagania dotyczące minimalnej ilości miejsca na dysku związane z instalacją serwera WSUS 3.0 SP1  
-------------------------------------------------------------------------------------------------
  
Poniżej wymieniono wymagania dotyczące minimalnej ilości miejsca na dysku związane z instalowaniem programu Windows Server Update Services:
  
-   1 GB na partycji systemowej  
-   2 GB na potrzeby woluminu do przechowywania plików bazy danych  
-   20 GB na potrzeby woluminu do przechowywania zawartości
  
> [!Important]  
> Nie można zainstalować programu WSUS 3.0 SP1 na dyskach skompresowanych. Należy upewnić się, że wybrany dysk nie jest skompresowany. 
  
Wymagania związane z uaktualnianiem do programu WSUS 3.0 SP1  
------------------------------------------------------------
  
#### Sprawdzanie poprawności działania instalacji programu WSUS i wykonywanie kopii zapasowej bazy danych programu WSUS przed uaktualnieniem
  
W przypadku uaktualniania starszej wersji programu do wersji WSUS 3.0 SP1 należy upewnić się, że bieżąca instalacja działa poprawnie, i wykonać kopię zapasową bazy danych programu WSUS przed uaktualnieniem.
  
1.  Sprawdź dzienniki zdarzeń pod kątem ostatnio występujących błędów oraz upewnij się, że nie występują problemy z synchronizacją między serwerami podrzędnymi i nadrzędnymi ani problemy z niezgłaszającymi się klientami. Przed kontynuowaniem upewnij się, że te problemy są rozwiązane.  
2.  Może być konieczne uruchomienie narzędzia DBCC CHECKDB w celu zapewnienia poprawnej indeksacji bazy danych programu WSUS. Więcej informacji można znaleźć na stronie poświęconej narzędziu [DBCC CHECKDB](http://go.microsoft.com/fwlink/?linkid=86948) (http://go.microsoft.com/fwlink/?LinkId=86948) (strona może zostać wyświetlona w języku angielskim).  
3.  Wykonaj kopię zapasową bazy danych programu WSUS.
  
#### Jeśli ręcznie zmodyfikowano port używany przez program WSUS, przed uaktualnieniem należy odinstalować program
  
W przypadku potrzeby zmodyfikowania portu programu WSUS nigdy nie należy robić tego ręcznie, lecz używając narzędzia wsusutil. Jeśli zmodyfikowano port ręcznie, a wcześniej uaktualniono program Software Update Services 1.0 do programu WSUS 2.0, należy postępować zgodnie z poniższymi instrukcjami:
  
1.  Jeśli jeszcze nie zainstalowano programu WSUS 3.0, odinstaluj program WSUS 2.0, zachowując bazę danych i zawartość. (Jeśli już zainstalowano program WSUS 3.0, odinstaluj go, zachowując bazę danych i zawartość).  
2.  Uruchom domyślną witrynę sieci Web, tymczasowo ponownie włączając program SUS 1.0, ale udostępniając go dezinstalatorowi.  
3.  Odinstaluj program SUS 1.0.  
4.  Zainstaluj program WSUS 3.0.
  
#### Należy odinstalować program Software Update Services 1.0
  
Instalacja programu WSUS 3.0 SP1 nie powiedzie się, jeśli na tym samym komputerze będzie zainstalowany program Software Update Services 1.0. Przed zainstalowaniem programu WSUS 3.0 SP1 należy odinstalować program Software Update Services 1.0.
  
#### W 64-bitowym systemie operacyjnym nie ma możliwości uaktualnienia programu WSUS 2.0 do wersji WSUS 3.0 SP1
  
Program WSUS 2.0 nie jest obsługiwany w 64-bitowych systemach operacyjnych. Dlatego w takich systemach nie ma możliwości uaktualnienia programu WSUS 2.0 do wersji WSUS 3.0 SP1.
  
Parametry wiersza polecenia Instalatora  
---------------------------------------
  
Za pomocą Instalatora aplikacji WSUS dla wiersza polecenia można przeprowadzać nienadzorowane instalacje programu WSUS 3.0 SP1. W poniższej tabeli przedstawiono parametry wiersza polecenia Instalatora aplikacji WSUS 3.0 SP1.
  
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
<td style="border:1px solid black;">Instalacja dyskretna.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>/u</strong></td>
<td style="border:1px solid black;">Odinstalowanie produktu. Jeśli zainstalowano wystąpienie programu Wewnętrzna baza danych systemu Windows, jest ono również odinstalowywane.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>/p</strong></td>
<td style="border:1px solid black;">Tylko sprawdzenie warunków wstępnych. Produkt nie jest instalowany. Zamiast tego jest przeprowadzana inspekcja systemu i są zgłaszane wszelkie odstępstwa od warunków wstępnych.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>/?, /h</strong></td>
<td style="border:1px solid black;">Wyświetlenie parametrów wiersza polecenia i ich opisów.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>/g</strong></td>
<td style="border:1px solid black;">Uaktualnienie z poprzedniej wersji programu WSUS. (Nie należy podejmować prób uaktualnienia z programu SUS 1.0). Jedynym prawidłowym parametrem stosowanym z tą opcją jest /q (instalacja dyskretna). Jedyną prawidłową właściwością stosowaną z tą opcją jest DEFAULT_WEBSITE.</td>
</tr>
</tbody>
</table>
  
W poniższej tabeli przedstawiono właściwości wiersza polecenia dotyczące aplikacji WSUS 3.0 SP1.
  
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
<td style="border:1px solid black;">0=zawartość obsługiwana lokalnie, 1=obsługa w witrynie Microsoft Update</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CONTENT_DIR</td>
<td style="border:1px solid black;">Ścieżka do katalogu zawartości. Domyślna: <em>dysk_instalacji_WSUS</em><strong>\WSUS\WSUSContent</strong>, gdzie <em>dysk_instalacji_WSUS</em> to dysk lokalny z największą ilością wolnego miejsca.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">WYUKON_DATA_DIR</td>
<td style="border:1px solid black;">Ścieżka do katalogu danych programu Wewnętrzna baza danych systemu Windows.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">SQLINSTANCE_NAME</td>
<td style="border:1px solid black;">Nazwa powinna mieć postać: <em>nazwa_serwera</em>\<em>nazwa_wystąpienia_SQL</em>. Jeśli wystąpienie bazy danych znajduje się na komputerze lokalnym, należy użyć zmiennej środowiskowej %COMPUTERNAME%. W przypadku braku istniejącego wystąpienia domyślna wartość to %COMPUTERNAME%\WSUS.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DEFAULT_WEBSITE</td>
<td style="border:1px solid black;">0=port 8530, 1=port 80</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PREREQ_CHECK_LOG</td>
<td style="border:1px solid black;">Ścieżka i nazwa pliku dziennika.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">CONSOLE_INSTALL</td>
<td style="border:1px solid black;">0=instaluj serwer WSUS, 1=instaluj tylko konsolę</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ENABLE_INVENTORY</td>
<td style="border:1px solid black;">0=nie instaluj funkcji spisu, 1=instaluj funkcje spisu</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DELETE_DATABASE</td>
<td style="border:1px solid black;">0=zachowaj bazę danych, 1=usuń bazę danych</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DELETE_CONTENT</td>
<td style="border:1px solid black;">0=zachowaj pliki zawartości, 1=usuń pliki zawartości</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DELETE_LOGS</td>
<td style="border:1px solid black;">0=zachowaj pliki dziennika, 1=usuń pliki dziennika (stosowane z przełącznikiem instalacyjnym /u).</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CREATE_DATABASE</td>
<td style="border:1px solid black;">0=użyj bieżącej bazy danych, 1=utwórz bazę danych</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PROGRESS_WINDOW_HANDLE</td>
<td style="border:1px solid black;">Uchwyt okna do zwracania komunikatów o postępie programu MSI.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">MU_ROLLUP</td>
<td style="border:1px solid black;">1=dołącz do programu poprawy jakości usługi Microsoft Update, 0=nie dołączaj do programu poprawy jakości usługi Microsoft Update</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">FRONTEND_SETUP</td>
<td style="border:1px solid black;">1=nie zapisuj lokalizacji zawartości w bazie danych, 0=zapisz lokalizację zawartości w bazie danych (na potrzeby równoważenia obciążenia sieciowego)</td>
</tr>
</tbody>
</table>
  
#### Przykładowe użycie
  
```  
WSUSSetup.exe /q DEFAULT\_WEBSITE=0 (install in quiet mode using port 8530) WSUSSetup.exe /q /u (uninstall WSUS)  
```  
> [!Important]  
> W przypadku instalowania programu WSUS 3.0 SP1 w trybie dyskretnym (/q) na komputerze, na którym brakuje oprogramowania wymienionego w warunkach wstępnych, podczas instalacji jest generowany plik o nazwie WSUSPreReqCheck.xml zapisywany w katalogu %TEMP%. 
  
Problemy z instalacją  
---------------------
  
#### W trakcie instalacji programu WSUS 3.0 SP1 usługi IIS są ponownie uruchamianie
  
Program instalacyjny aplikacji WSUS 3.0 SP1 bez żadnego powiadomienia uruchamia ponownie usługi IIS, co może wpływać na istniejące witryny sieci Web w organizacji użytkownika. Jeśli usługi IIS nie są uruchomione, Instalator programu WSUS 3.0 SP1 uruchamia je.
  
#### Jeśli są otwarte połączenia z istniejącą bazą danych programu WSUS, instalacja może się nie powieść
  
Jeśli istniejąca instalacja jest uaktualniana do programu WSUS 3.0 SP1 i nadal są otwarte połączenia z istniejącą bazą danych programu WSUS (na przykład jest otwarty program SQL Server Management Studio), instalacja może zakończyć się niepowodzeniem. Należy zamknąć wszystkie połączenia i ponownie zainstalować program WSUS 3.0 SP1.
  
#### Instalator programu WSUS wskazuje niewłaściwy katalog plików bazy danych
  
W Instalatorze programu WSUS na ekranie **Gotowy do instalacji** jest zgłaszana niepoprawna lokalizacja bazy danych w postaci katalogu nadrzędnego tej lokalizacji. Na przykład w przypadku domyślnej lokalizacji %systemdrive%\\WSUS\\UpdateServicesDbFiles jest niepoprawnie zgłaszana lokalizacja %systemdrive%\\WSUS.
  
#### Jeśli program WSUS jest zainstalowany na komputerze z pakietami językowymi wielojęzycznego interfejsu użytkownika i z językiem domyślnym innym niż angielski, Pomoc jest wyświetlana w języku domyślnym, a nie w języku angielskim
  
Jeśli na używanym komputerze są zainstalowane pakiety językowe wielojęzycznego interfejsu użytkownika i językiem domyślnym nie jest angielski, nadal można zainstalować program WSUS, o ile w ustawieniach regionalnych bieżącego użytkownika określono język angielski. Interfejs użytkownika jest wyświetlany w języku angielskim, ale w celu wyświetlania Pomocy w tym języku trzeba dokonać pewnych dostosowań. Należy skopiować plik Pomocy w języku angielskim (plik chm; *katalog\_instalacyjny\_WSUS*\\documentation\\mui\\0409\\WSUS30Help.chm) do katalogu głównego dokumentacji (*katalog\_instalacyjny\_WSUS*\\documentation\\WSUS30Help.chm). Po wykonaniu tej operacji Pomoc powinna być wyświetlana poprawnie we wszystkich językach.
  
Problemy z uaktualnianiem  
-------------------------
  
#### Przywracanie sprawności po nieudanym uaktualnianiu
  
Jeśli wykonywane jest uaktualnianie z poprzedniej wersji programu WSUS (WSUS 3.0, WSUS 2.0 SP1 lub WSUS 2.0) do programu WSUS 3.0 SP1 i z jakiejś przyczyny uaktualnianie nie powiedzie się:
  
1.  Zainstaluj ponownie poprzednią wersję programu WSUS.  
2.  Przywróć bazę danych z kopii zapasowej wykonanej przed podjęciem próby uaktualnienia. W większości przypadków program WSUS też automatycznie tworzy kopię zapasową. Aby poznać jej lokalizację, przejrzyj plik WSUSSetup.log.  
3.  W celu określenia przyczyny niepowodzenia zapoznaj się z zawartością dzienników, a następnie usuń problem.  
4.  Ponów próbę uaktualnienia programu WSUS.
  
#### Nie można wykonać uaktualnienia z programu WSUS 2.0 do programu WSUS 3.0 SP1, jeśli istnieje baza danych programu WSUS 3.0 SP1 z poprzedniej instalacji
  
Jeśli wcześniej był zainstalowany program WSUS 3.0 SP1, a następnie zainstalowano program WSUS 2.0, to przed przystąpieniem do próby ponownego zainstalowania programu WSUS 3.0 SP1 należy usunąć z komputera bazę danych programu WSUS 3.0 SP1.
  
#### Zmienianie nazwy komputera przed uaktualnieniem do programu WSUS 3.0 SP1 może spowodować niepowodzenie uaktualniania
  
Jeśli nazwa komputera zostanie zmieniona po zainstalowaniu programu WSUS 2.0 i przed uaktualnieniem do programu WSUS 3.0 SP1, to uaktualnienie może się nie powieść.
  
Użyj następującego skryptu, aby usunąć i ponownie dodać grupy administratorów programów ASPNET i WSUS. Następnie ponownie uruchom uaktualnianie.
  
Parametr *&lt;lokalizacja\_BD&gt;* zastąp folderem z zainstalowaną bazą danych, a parametr *&lt;katalog\_zawartości&gt;* — lokalnym folderem przechowywania.
  
```  
sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "USE SUSDB DECLARE @asplogin varchar(200) SELECT @asplogin=name from sysusers WHERE name like '%ASPNET' EXEC sp\_revokedbaccess @asplogin" sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "USE SUSDB DECLARE @wsusadminslogin varchar(200) SELECT @wsusadminslogin=name from sysusers WHERE name like '%WSUS Administrators' EXEC sp\_revokedbaccess @wsusadminslogin"   sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "USE SUSDB DECLARE @asplogin varchar(200) SELECT @asplogin=HOST\_NAME()+'\\ASPNET' EXEC sp\_grantlogin @asplogin EXEC sp\_grantdbaccess @asplogin EXEC sp\_addrolemember webService,@asplogin" sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "USE SUSDB DECLARE @wsusadminslogin varchar(200) SELECT @wsusadminslogin=HOST\_NAME()+'\\WSUS Administrators' EXEC sp\_grantlogin @wsusadminslogin EXEC sp\_grantdbaccess @wsusadminslogin EXEC sp\_addrolemember webService,@wsusadminslogin"   sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "backup database SUSDB to disk=N'*&lt;ContentDirectory&gt;*\\SUSDB.Dat' with init"  
```
  
#### Instalator zastąpi poprzednią kopię zapasową bazy danych
  
Instalator programu WSUS 3.0 SP1 doda bazę danych do katalogu domyślnego o ścieżce *dysk*\\WSUS (gdzie *dysk* jest lokalnym dyskiem NTFS z największą ilością wolnego miejsca). Jeśli w tym katalogu znajduje się kopia zapasowa bazy danych, to może ona zostać zastąpiona. Przed rozpoczęciem uaktualniania do programu WSUS 3.0 SP1 administratorzy powinni zapisać kopię zapasową bieżącej wersji bazy danych w innej lokalizacji.
  
#### Jeśli przeprowadzono migrację z programu MSDE do programu SQL Server 2000 lub SQL Server 2005 przy zainstalowanym programie WSUS 2.0, konieczna będzie zmiana wartości rejestru
  
Jeśli jest zainstalowany program WSUS 2.0 i została przeprowadzona migracja do programu SQL Server 2000 lub SQL Server 2005, konieczna będzie zmiana wartości **HKLM\\SOFTWARE\\Microsoft\\Update Services\\Server\\Setup\\WmsdeInstalled** z 1 na 0. Jeśli zmiana ta nie zostanie wprowadzona przed rozpoczęciem uaktualniania do programu WSUS 3.0 SP1, uaktualnianie nie powiedzie się.
  
#### Jeśli instalator programu WSUS 2.0 zostanie uruchomiony i anulowany, usunie klucz rejestru programu WSUS
  
Jeśli instalator programu WSUS 2.0 zostanie uruchomiony, a następnie anulowany, klucz rejestru programu WSUS zostanie usunięty. Jeśli program WSUS 3.0 SP1 jest już zainstalowany, może to powodować problemy. Ten sam problem wystąpi, jeśli rozpocznie się odinstalowywanie programu WSUS 2.0, anuluje je, a następnie spróbuje przeprowadzić uaktualnienie z programu WSUS 2.0 do programu WSUS 3.0 SP1.
  
#### Jeśli program WSUS 3.0 SP1 zostanie odinstalowany, ale pozostawi się pliki dzienników, to po ponownym zainstalowaniu mogą one nie mieć poprawnych uprawnień
  
Podczas odinstalowywania programu WSUS 3.0 SP1 dostępna jest opcja zachowania plików dzienników instalacji. Przy ponownej instalacji programu WSUS 3.0 SP1 stare pliki dzienników tracą uprawnienia (zwykle są przeznaczone wyłącznie dla administratorów programu WSUS). Uprawnienia dla tych plików powinny zostać przywrócone.
  
#### Jeśli klienci programu WSUS 2.0 mają aktualizacje ze stanem Nie dotyczy, to po uaktualnieniu do programu WSUS 3.0 SP1 aktualizacje te będą przez krótki czas wyświetlane ze stanem Nieznane
  
Jeśli serwer WSUS 2.0 ma klientów z aktualizacjami o stanie **Nie dotyczy**, to po uaktualnieniu serwera do wersji WSUS 3.0 SP1 aktualizacje te będą przez krótki czas wyświetlane ze stanem **Nieznane**. Stan aktualizacji powróci do wartości **Nie dotyczy** po następnym wykonaniu skanowania przez klienta.
  
Znane problemy  
--------------
  
#### Rozwiązywanie problemów z wielokrotnymi błędami operacji pobierania lub powtarzającymi się niepowodzeniami synchronizacji klienta
  
Jeśli przez dłuższy czas klienci programu WSUS 3.0 SP1 zgłaszają wiele błędów pobierania lub nie mogą wykonać synchronizacji z serwerem WSUS 3.0 SP1, uszkodzona mogła zostać pamięć podręczna klienta dotycząca pobierania. Aby przywrócić prawidłowe działanie, można spróbować usunąć z systemu plików pamięć podręczną klienta dotyczącą pobierania.
  
Aby usunąć pamięć podręczną klienta dotyczącą pobierania:
  
1.  Usuń wszystkie pliki i podkatalogi w następującej lokalizacji na komputerze klienta: **%windir%\\SoftwareDistribution\\Download**  
2.  Spróbuj zainstalować aktualizację, ponownie synchronizując komputer kliencki z programem WSUS 3.0 SP1. Ta próba instalacji powinna zakończyć się niepowodzeniem i wyświetleniem następującego komunikatu: **WU\_E\_DM\_NOTDOWNLOADED, "Aktualizacja nie została pobrana."**  
3.  Po tym błędzie komputer kliencki automatycznie ponownie uruchomi pobieranie i będzie można kontynuować instalację.
  
#### Jeśli synchronizacja nie powiedzie się, należy spróbować ponownie
  
Jeśli synchronizacja nie powiedzie się, w pierwszej kolejności należy spróbować jeszcze raz zsynchronizować serwer. Jeśli kolejne próby synchronizacji kończą się niepowodzeniem, postępuj zgodnie z informacjami dotyczącymi rozwiązywania problemów w [przewodniku użytkownika programu Windows Server Update Services 3.0](http://go.microsoft.com/fwlink/?linkid=81072) (http://go.microsoft.com/fwlink/?LinkId=81072) (strona może zostać wyświetlona w języku angielskim).
  
#### Nie można zmieniać konfiguracji programu WSUS 3.0 SP1 bezpośrednio w bazie danych
  
Program Windows Server Update Services przechowuje swoje dane konfiguracji w bazie danych programu SQL Server. Nie wolno jednak zmieniać danych konfiguracji programu WSUS 3.0 SP1 przez bezpośrednie uzyskanie dostępu do bazy danych. Konfigurację programu WSUS 3.0 SP1 można zmieniać za pośrednictwem konsoli tego programu oraz za pomocą wywołań jego interfejsu API.
  
#### Niepowodzenia pobierania nie są szybko zgłaszane przy włączonych przydziałach dysku
  
Jeśli włączone są przydziały dysków i osiągnięty zostanie maksymalny rozmiar przydziału, niepowodzenia pobierania aktualizacji mogą nie być zgłaszane na serwerze WSUS w odpowiednio krótkim czasie. Aby uniknąć tego problemu, wyłącz przydziały dysku lub zwiększ przydział.
  
#### Jeśli program WSUS 3.0 SP1 został wdrożony z użyciem protokołu SSL, komputery klienckie mogą zgłaszać błąd o kodzie 0x8024400a
  
Komputery klienckie mogą czasem zgłaszać błąd o kodzie 0x8024400a podczas komunikowania się z serwerem WSUS 3.0 SP1 poprzez połączenie SSL. Aby uzyskać aktualizację rozwiązującą ten problem, zobacz artykuł [KB 905422](http://go.microsoft.com/fwlink/?linkid=70593) (http://go.microsoft.com/fwlink/?LinkId=70593) (strona może zostać wyświetlona w języku angielskim).
  
#### Konto domeny administratorów programu WSUS nie zostanie usunięte po odinstalowaniu programu WSUS
  
Grupa administratorów programu WSUS jest tworzona jako konto domeny (a nie konto lokalne) na kontrolerach domeny, więc jeśli to konto domeny zostałoby usunięte po odinstalowaniu programu WSUS, wszystkie instalacje korzystające z tego konta domeny zostałyby wyłączone. Z tego powodu odinstalowanie programu WSUS nie powoduje usunięcia konta domeny administratorów programu WSUS.
  
#### Po przekształceniu serwera podrzędnego w serwer nadrzędny aktualizacje witryny wykazu muszą zostać zaimportowane ponownie
  
Po przekształceniu serwera podrzędnego w serwer nadrzędny konieczne jest ponowne zaimportowanie wszystkich aktualizacji witryny wykazu. W przeciwnym razie witryna nie będzie mogła zsynchronizować nowych wersji aktualizacji w witrynie wykazu z tym serwerem.
  
#### Jeśli używane są usługi IIS z protokołem SSL, nieszyfrowany dostęp jest nadal możliwy, chyba że zaznaczono opcję Wymagaj bezpiecznego kanału
  
Jeśli usługi IIS zostały skonfigurowane do korzystania z połączeń SSL przez zainstalowanie certyfikatu, nadal można uzyskiwać dostęp do witryny poprzez nieszyfrowane połączenie HTTP, o ile nie została zaznaczona opcja **Wymagaj bezpiecznego kanału**. Więcej informacji można znaleźć w dokumentacji usług [IIS](http://go.microsoft.com/fwlink/?linkid=98084) (http://go.microsoft.com/fwlink/?LinkId=98084) (strona może zostać wyświetlona w języku angielskim).
  
#### Importowanie witryny wykazu może nie powieść się bez uprawnień do odczytu/zapisu folderu %windir%\\TEMP
  
Jeśli konto usługi sieciowej nie ma uprawnienia do odczytu/zapisu folderu %windir%\\TEMP, importowanie witryny wykazu może nie powieść się i może zostać wyświetlony następujący komunikat o błędzie: Serwer nie może przetworzyć żądania. ---&gt; Nie można odnaleźć pliku "C:\\WINDOWS\\TEMP\\*nazwa\_pliku\_tymczasowego*.dll".
  
#### Możliwa niska wydajność podczas synchronizowania programu WSUS 3.0 SP1 z podrzędnym serwerem repliki z uruchomionym programem WSUS 2.0
  
Jeśli na serwerze nadrzędnym zostanie zainstalowany program WSUS 3.0 SP1 i zostanie podjęta próba wykonania synchronizacji z podrzędnym serwerem repliki, na którym działa program WSUS 2.0, mogą wystąpić problemy z wydajnością. Aby rozwiązać ten problem, zapoznaj się z artykułem [KB 910847](http://go.microsoft.com/fwlink/?linkid=70669) (http://go.microsoft.com/fwlink/?LinkId=70669) (strona może zostać wyświetlona w języku angielskim).
  
#### Jeśli serwer poczty e-mail nie działa lub jest nieosiągalny, powiadomienia przesyłane pocztą e-mail przestaną działać bez żadnego ostrzeżenia
  
Jeśli sieciowy serwer poczty e-mail przejdzie w tryb offline, program WSUS 3.0 SP1 nie będzie mógł wysyłać powiadomień pocztą e-mail, przy czym użytkownik nie zostanie o tym poinformowany. W dzienniku zdarzeń zostanie jednak zapisane zdarzenie 10052 (HealthCoreEmailNotificationRed).
  
#### Zmienione ustawienia na serwerze nadrzędnym nie są natychmiast przekazywane do serwera podrzędnego
  
Po zmianie konfiguracji serwera nadrzędnego może upłynąć nieco czasu, zanim zmiany te zaczną rzeczywiście obowiązywać. Przykładowo po zmianie polegającej na wybraniu nowego języka na serwerze nadrzędnym i natychmiastowym wyzwoleniu synchronizacji na serwerze podrzędnym zmiana ta nie będzie widoczna. Zamiast tego zostanie przekazana do serwera podrzędnego przy następnej zaplanowanej synchronizacji. Czas oczekiwania jest tym większy, im większa jest liczba aktualizacji na serwerze nadrzędnym.
  
#### Odinstalowanie programu WSUS 3.0 SP1 nie powoduje odinstalowania wystąpienia bazy danych
  
Odinstalowaniu programu WSUS 3.0 SP1 nie będzie towarzyszyć odinstalowanie wystąpienia bazy danych. Wystąpienie to może być współużytkowane przez kilka aplikacji, więc jego usunięcie może uniemożliwić ich poprawne działanie.
  
Jeśli konieczne jest odinstalowanie aplikacji Wewnętrzna baza danych systemu Windows, następujące polecenia spowodują jej odinstalowanie:
  
Platformy 32-bitowe:
  
```  
msiexec /x {CEB5780F-1A70-44A9-850F-DE6C4F6AA8FB} callerid=ocsetup.exe  
```  
Platformy 64-bitowe:
  
```  
msiexec /x {BDD79957-5801-4A2D-B09E-852E7FA64D01} callerid=ocsetup.exe  
```  
Jeśli chcesz odinstalować program Wewnętrzna baza danych systemu Windows z dodatkiem Service Pack 2 z systemu Windows Server 2008, możesz to zrobić za pośrednictwem Menedżera serwerów.
  
Usunięcie aplikacji może jednak nie pociągać za sobą usunięcia domyślnych plików mdf i ldf, które spowodują, że kolejna próba instalacji programu WSUS 3.0 SP1 nie powiedzie się. Pliki te można usunąć w katalogu %windir%\\SYSMSI\\SSEE.
  
#### Jeśli serwer podrzędny zmieni swój serwer nadrzędny, aktualizacje o stanie Nieznane są zgłaszane ze stanem Nie dotyczy
  
Jeśli serwer podrzędny rozpocznie synchronizację z innym serwerem nadrzędnym, aktualizacje o stanie **Nieznane** będą zgłaszane na nowym serwerze nadrzędnym ze stanem **Nie dotyczy**. Ten stan jest jedynie tymczasowy i zostanie poprawiony przy następnym zgłaszaniu stanu przez serwer podrzędny, gdy jego klienci zostaną z nim zsynchronizowani.
  
#### Jeśli kreator oczyszczania serwera przekroczy limit czasu na jednym z serwerów podczas pracy na wielu serwerach za pośrednictwem konsoli zdalnej, utracone zostanie połączenie ze wszystkimi serwerami
  
Kreator oczyszczania serwera można uruchamiać na wielu serwerach, używając do tego jednej konsoli zdalnej. Jeśli jednak proces oczyszczania przekroczy limit czasu na jednym z serwerów, konsola utraci połączenie ze wszystkimi serwerami. Żadne dane nie zostaną utracone, ale administrator będzie musiał uruchomić ponownie połączenie zdalne z każdym z serwerów.
  
#### Uruchomienie i natychmiastowe zatrzymanie połączenia powoduje komunikat o błędzie „Nie było błędu synchronizacji” w kreatorze konfiguracji
  
Podczas konfigurowania programu WSUS wymagane jest połączenie się z serwerem nadrzędnym (witryną Microsoft Update lub serwerem nadrzędnym w intranecie) w celu przesłania podstawowych informacji o serwerze. Jeśli zostanie kliknięta opcja **Rozpocznij łączenie**, a zaraz po niej opcja **Zatrzymaj łączenie**, wyświetlony zostanie niepoprawny komunikat o błędzie „Nie było błędu synchronizacji”.
  
Program WSUS 3.0 SP1 w systemie Windows Server 2008  
---------------------------------------------------
  
#### Obsługiwane wersje
  
Program WSUS 3.0 SP1 obsługuje system Windows Server 2008 zarówno w wersji 32-bitowej, jak i 64-bitowej.
  
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
<td style="border:1px solid black;">Internetowe usługi informacyjne (IIS) firmy Microsoft</td>
<td style="border:1px solid black;">Instalacja z poziomu systemu operacyjnego. Należy upewnić się, że włączone są następujące składniki:
<ul>
<li>Uwierzytelnianie systemu Windows<br />
<br />
</li>
<li>Zawartość statyczna<br />
<br />
</li>
<li>ASP.NET<br />
<br />
</li>
<li>Zgodność z narzędziami zarządzania usługami IIS w wersji 6<br />
<br />
</li>
<li>Zgodność z metabazą usług IIS 6<br />
<br />
</li>
</ul></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Pakiet dystrybucyjny środowiska Microsoft .NET Framework 2.0 (x86)</td>
<td style="border:1px solid black;">Nie jest potrzebny w systemie Windows Server 2008, ponieważ jest instalowany jako część systemu operacyjnego.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Program Microsoft Management Console 3.0</td>
<td style="border:1px solid black;">Nie jest potrzebny w systemie Windows Server 2008, ponieważ jest instalowany jako część systemu operacyjnego.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Podgląd raportów firmy Microsoft</td>
<td style="border:1px solid black;">Stanowi wymaganie wstępne dla korzystania z interfejsu użytkownika programu WSUS. Więcej informacji można znaleźć w opisie pakietu dystrybucyjnego Podglądu raportów firmy Microsoft 2005 w <a href="http://go.microsoft.com/fwlink/?linkid=70410">Centrum pobierania Microsoft</a> (http://go.microsoft.com/fwlink/?LinkId=70410) (strona może zostać wyświetlona w języku angielskim).</td>
</tr>
</tbody>
</table>
  
#### Korzystanie z kreatora konfiguracji zabezpieczeń
  
W systemie Windows Server 2008 po uruchomieniu kreatora konfiguracji zabezpieczeń można wybrać rolę programu WSUS i włączyć jej zależności. Aby uruchomić tego kreatora, kliknij przycisk **Start**, wskaż polecenie **Narzędzia administracyjne** i kliknij polecenie **Kreator konfiguracji zabezpieczeń**.
  
Następujące znane problemy ujawniają się podczas równoczesnego korzystania z kreatora konfiguracji zabezpieczeń i roli programu WSUS:
  
-   **Usługa wewnętrznej bazy danych systemu Windows jest włączona nawet wtedy, gdy nie jest używana przez program WSUS.** Program WSUS jest konfigurowany do korzystania z bazy danych — wewnętrznej bazy danych systemu Windows bądź bazy danych SQL Server. Jeśli program WSUS jest zainstalowany z bazą danych SQL Server, w kreatorze konfiguracji zabezpieczeń zostanie wybrana rola programu WSUS, a usługa wewnętrznej bazy danych systemu Windows jest zainstalowana, to usługa ta zostanie włączona, ale nie będzie używana przez program WSUS. Usługę wewnętrznej bazy danych systemu Windows należy wyłączyć, jeśli zamiast z niej korzysta się z bazy danych SQL Server.  
-   **Reguły zapory dla programu WSUS w niestandardowej witrynie sieci Web nie są wybrane domyślnie.** Jeśli program WSUS zostanie zainstalowany w niestandardowej witrynie sieci Web (port 8530 lub 8531), to wymagane reguły zapory nie zostaną automatycznie wybrane nawet po wybraniu roli programu WSUS w kreatorze konfiguracji zabezpieczeń. Właściwe reguły zapory dla programu WSUS należy włączyć, opierając się na informacji, czy protokół SSL (Secure Sockets Layer) został skonfigurowany dla serwera WSUS.
  
Program WSUS 3.0 SP1 w systemie Windows Small Business Server 2003  
------------------------------------------------------------------
  
#### Jeśli wirtualny katalog główny usług IIS jest ograniczony do konkretnych adresów IP lub nazw domen, serwer WSUS 3.0 SP1 nie będzie mógł aktualizować samego siebie
  
Niektóre instalacje systemu Windows Small Business Server mogą w konfiguracji domyślnej witryny usług IIS zawierać ograniczenia dotyczące **adresów IP i nazw domen**. W takich przypadkach klient usługi Windows Update na serwerze może nie być w stanie przeprowadzić aktualizacji samego siebie.
  
#### Instalowanie programu WSUS 3.0 SP1 w systemie Small Business Server — problemy z integracją
  
-   Jeśli system Windows Small Business Server 2003 korzysta z serwera proxy ISA do łączenia się z siecią Internet, następujące informacje muszą zostać podane w interfejsie użytkownika **Ustawienia**: **ustawienia serwera proxy, nazwa serwera proxy, port**.  
-   Jeśli usługa ISA korzysta z uwierzytelniania systemu Windows, referencje serwera proxy powinny zostać wpisane w formacie *DOMENA*\\*nazwa\_użytkownika*, a użytkownik powinien być członkiem grupy użytkowników Internetu.
  
#### Jeśli do sieci została dodana podsieć i nie użyto do tego celu kreatorów systemu Windows SBS, konieczne jest wykonanie tej procedury
  
W procesie instalacji serwera WSUS na serwerze instalowane są dwa wirtualne katalogi główne usług IIS: SelfUpdate i ClientWebService. Instalator umieszcza też kilka plików w katalogu głównym domyślnej witryny sieci Web (na porcie 80), co pozwala komputerom klienckim na samoaktualizacje za pośrednictwem domyślnej witryny sieci Web. Domyślna witryna sieci Web jest domyślnie skonfigurowana do odmawiania dostępu dowolnym adresom IP innym niż localhost oraz do akceptowania konkretnych podsieci przyłączonych do serwera. W rezultacie komputery klienckie znajdujące się poza hostem localhost oraz poza określonymi podsieciami nie mogą wykonywać samoaktualizacji. Jeśli do sieci została dodana podsieć i nie użyto do tego celu kreatorów systemu Windows SBS, konieczne jest wykonanie następującej procedury:
  
1.  W Menedżerze serwerów rozwiń opcję **Zarządzanie zaawansowane**, rozwiń opcję **Internetowe usługi informacyjne**, rozwiń opcję **Witryny sieci Web**, rozwiń opcję **Domyślna witryna sieci Web**, kliknij prawym przyciskiem myszy katalog wirtualny **Selfupdate** i kliknij polecenie **Właściwości**.  
2.  Kliknij opcję **Zabezpieczenia katalogów**.  
3.  W obszarze **Ograniczenia adresów IP i nazw domen** kliknij przycisk **Edytuj**, a następnie kliknij przycisk **Udzielony dostęp**.  
4.  Kliknij przycisk **OK**, kliknij prawym przyciskiem myszy katalog wirtualny **ClientWebService** i kliknij polecenie **Właściwości**.  
5.  Kliknij opcję **Zabezpieczenia katalogów**.  
6.  W obszarze **Ograniczenia adresów IP i nazw domen** kliknij przycisk **Edytuj**, a następnie kliknij przycisk **Udzielony dostęp**.
  
Prawa autorskie  
---------------
  
Informacje zawarte w tym dokumencie, w tym również adresy URL i inne odwołania do witryn sieci Web, mogą ulec zmianie bez powiadomienia. Wszystkie firmy, organizacje, produkty, nazwy domen, adresy e-mail, logo, osoby, miejsca i zdarzenia przedstawione w przykładach są fikcyjne, o ile nie zaznaczono, że jest inaczej. Wymienionych firm, organizacji, produktów, nazw domen, adresów e-mail, logo, osób, miejsc i zdarzeń nie należy kojarzyć z podobnymi podmiotami występującymi w rzeczywistości. Użytkownik niniejszego dokumentu jest zobowiązany do przestrzegania wszelkich obowiązujących przepisów w zakresie ochrony praw autorskich. Niezależnie od praw wchodzących w zakres praw autorskich, żadnej części tego dokumentu nie można powielać, przechowywać lub wprowadzać do systemów wyszukiwania informacji ani też przekazywać w żadnej formie lub za pomocą jakichkolwiek urządzeń (elektronicznych, mechanicznych, fotokopiujących, rejestrujących lub innych) w jakimkolwiek celu bez pisemnej zgody firmy Microsoft Corporation.
  
Firma Microsoft może posiadać patenty, zgłoszenia patentowe, znaki towarowe, prawa autorskie lub inne prawa własności intelektualnej dotyczące treści tego dokumentu. Z wyjątkiem przypadków wyraźnie określonych w jakiejkolwiek pisemnej umowie licencyjnej firmy Microsoft, udostępnienie tego dokumentu nie jest równoznaczne z udzieleniem użytkownikowi jakichkolwiek licencji na wymienione patenty, znaki towarowe, prawa autorskie lub inną własność intelektualną.
  
© 2007 Microsoft Corporation. Wszelkie prawa zastrzeżone.
  
Microsoft, SQL Server, Windows i Windows Server są zastrzeżonymi znakami towarowymi lub znakami towarowymi firmy Microsoft Corporation w Stanach Zjednoczonych i/lub innych krajach.
  
Pozostałe znaki towarowe należą do odpowiednich właścicieli.
