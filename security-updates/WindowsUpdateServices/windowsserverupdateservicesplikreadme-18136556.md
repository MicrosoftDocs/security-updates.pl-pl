---
TOCTitle: 'Windows Server Update Services — plik ReadMe'
Title: 'Windows Server Update Services — plik ReadMe'
ms:assetid: '4244109a-395a-4ff8-9989-ea55ab0964a3'
ms:contentKeyID: 18136556
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720505(v=WS.10)'
---

Windows Server Update Services — plik ReadMe
============================================

W tym dokumencie zamieszczono opis znanych problemów dotyczących Usług Windows Server Update Services (WSUS). Zawiera on także zalecenia oraz wymagania dotyczące instalacji Usług WSUS.

> [!note]  
> Kopia tego dokumentu w wersji do pobrania jest dostępna w witrynie Microsoft Download Center pod adresem [http://go.microsoft.com/fwlink/?LinkId=48126](http://go.microsoft.com/fwlink/?linkid=48126). 

Zanim rozpoczniesz
------------------

#### Problem 1: Program Internetowe usługi informacyjne (IIS) musi zostać zainstalowany.

Program Microsoft® Windows Server™ Update Services (WSUS) wymaga zainstalowania Internetowych usług informacyjnych (IIS). W przypadku systemów Microsoft Windows Server 2003 i Microsoft Windows® 2000 Server Internetowe usługi informacyjne nie są instalowane domyślnie, w wyniku czego działanie Instalatora programu Windows Server Update Services może zostać przerwane i może zostać wyświetlony komunikat o błędzie, informujący o braku zainstalowanych Internetowych usług informacyjnych.

Aby zainstalować program IIS:

1.  Otwórz Panel sterowania.
2.  Kliknij dwukrotnie aplet **Dodaj lub usuń programy**.
3.  Kliknij przycisk **Dodaj/Usuń składniki systemu Windows**.
4.  Na liście **Składniki** kliknij pozycję **Serwer aplikacji**.
5.  Kliknij przycisk **Szczegóły**.
6.  Zaznacz pole wyboru **ASP.NET**. Pola wyboru **Włącz dostęp sieciowy modelu COM+** i Internetowe usługi informacyjne (IIS) zostaną zaznaczone automatycznie.
7.  Zaznacz pole wyboru **Internetowe usługi informacyjne (IIS)**, a następnie kliknij przycisk **Szczegóły** w celu przejrzenia listy opcjonalnych składników IIS.
8.  Wybierz wszystkie opcjonalne składniki, które chcesz zainstalować. Składnik opcjonalny Usługa World Wide Web zawiera ważne podskładniki, takie jak Strony ASP czy Administracja zdalna (HTML). Aby przejrzeć i wybrać te podskładniki, kliknij pozycję Usługa World Wide Web, a następnie kliknij przycisk Szczegóły. Klikaj przyciski OK, dopóki nie wrócisz do Kreatora składników systemu Windows.
9.  Kliknij przycisk **Dalej** i postępuj zgodnie z instrukcjami kreatora.
10. Po zainstalowaniu Internetowych usług informacyjnych uruchom Instalatora programu Windows Server Update Services.

#### Problem 2: W przypadku serwerów z systemem Windows 2000 Server przed zainstalowaniem programu WSUS w ramach Internetowych usług informacyjnych musi być dostępna co najmniej jedna witryna sieci Web

Jeśli po uruchomieniu Instalatora programu Windows Server Update Services w ramach Internetowych usług informacyjnych nie są dostępne żadne witryny, utworzenie witryny sieci Web przez Instalatora może się nie powieść. Taka sytuacja może wystąpić na przykład wtedy, gdy w ramach Internetowych usług informacyjnych dostępna była jedynie witryna Software Update Services (SUS) 1.0 i została ona usunięta przed zainstalowaniem programu WSUS.

W takim przypadku konieczne jest utworzenie nowej witryny sieci Web za pośrednictwem przystawki Menedżer internetowych usług informacyjnych (IIS). Po wykonaniu tej czynności można wybrać tę witrynę lub określić nową witrynę w trakcie pracy Instalatora programu WSUS.

Jeśli już podjęto próbę zainstalowania programu WSUS i instalacja nie powiodła się z powodu braku witryn, otwórz przystawkę Menedżer internetowych usług informacyjnych (IIS) i usuń witrynę sieci Web nr 1. Następnie wykonaj czynności opisane wcześniej i ponownie uruchom Instalatora.

#### Problem 3: Instalowanie wstępnie wymaganych składników.

#### Wymagania dotyczące oprogramowania

W poniższej tabeli przedstawiono oprogramowanie wymagane dla poszczególnych obsługiwanych systemów operacyjnych. Przed uruchomieniem Instalatora programu WSUS należy upewnić się, czy serwer WSUS spełnia wymagania wymienione na tej liście. Jeśli jakiekolwiek z tych uaktualnień wymagają ponownego uruchomienia komputera po zakończeniu aktualizacji, komputera należy ponownie uruchomić przed zainstalowaniem programu WSUS.

<p></p>
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >System operacyjny</th>
<th style="border:1px solid black;" >Wymagania</th>
<th style="border:1px solid black;" >Pliki pobieralne</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Wszystkie systemy operacyjne</td>
<td style="border:1px solid black;">Microsoft Internet Information Services (IIS) 5.0</td>
<td style="border:1px solid black;">Instalacja z poziomu systemu operacyjnego.
Zobacz: Problem 1: Program Internetowe usługi informacyjne (IIS) musi zostać zainstalowany.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Wszystkie systemy operacyjne</td>
<td style="border:1px solid black;">Usługa inteligentnego transferu w tle (BITS) 2.0</td>
<td style="border:1px solid black;">W przypadku systemów Windows Server 2003 — zobacz <a href="http://go.microsoft.com/fwlink/?linkid=47251">aktualizację usługi Background Intelligent Transfer Service (BITS) 2.0 i WinHTTP 5.1 Windows Server 2003</a>(KB842773) w Centrum pobierania (http://go.microsoft.com/fwlink/?LinkId=47251 (strona może być w języku angielskim)).
W przypadku systemów operacyjnych Windows Server 2000 — zobacz <a href="http://go.microsoft.com/fwlink/?linkid=46794">aktualizację usługi Background Intelligent Transfer Service (BITS) 2.0 i WinHTTP 5.1 Windows 2000</a> (KB842773) w Centrum pobierania (http://go.microsoft.com/fwlink/?LinkId=46794 (strona może być w języku angielskim)).</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Server 2003</td>
<td style="border:1px solid black;">Microsoft .NET Framework 1.1 z dodatkiem Service Pack 1 dla systemu Windows Server 2003</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=47358">Microsoft .NET Framework 1.1 z dodatkiem Service Pack 1 dla systemu Windows Server 2003</a>
Można także przejść do witryny <a href="http://go.microsoft.com/fwlink/?linkid=47370">Windows Update</a> i sprawdzić dostępność krytycznych aktualizacji i dodatków Service Pack; zainstaluj pakiet Microsoft .NET Framework 1.1 z dodatkiem Service Pack 1 dla systemu Windows Server 2003.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows Server 2003</td>
<td style="border:1px solid black;">Oprogramowanie bazy danych w pełni zgodne z językiem Microsoft SQL</td>
<td style="border:1px solid black;">N/D</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows 2000 Server</td>
<td style="border:1px solid black;">Oprogramowanie bazy danych w pełni zgodne z językiem Microsoft SQL</td>
<td style="border:1px solid black;">Jeśli nie jest używany program Microsoft SQL Server 2000, można zainstalować program Microsoft SQL Server 2000 Desktop Engine (MSDE 2000). Wymaga to wykonania kilku czynności. Aby uzyskać więcej informacji, zobacz punkt Instalowanie programu MSDE w systemie Windows 2000 (poniżej).</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows 2000 Server</td>
<td style="border:1px solid black;">Program Microsoft Internet Explorer 6.0 z dodatkiem Service Pack 1</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=47359">Program Internet Explorer 6 z dodatkiem Service Pack 1</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows 2000 Server</td>
<td style="border:1px solid black;">Microsoft .NET Framework w wersji 1.1 do dystrybucji</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=47369">Microsoft .NET Framework w wersji 1.1 do dystrybucji</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows 2000 Server</td>
<td style="border:1px solid black;">Microsoft .NET Framework 1.1 z dodatkiem Service Pack 1</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=47368">Microsoft .NET Framework 1.1 z dodatkiem Service Pack 1</a>
Alternatywnie, przejdź do witryny <a href="http://go.microsoft.com/fwlink/?linkid=47370">Windows Update</a> (strona może być w języku angielskim) i sprawdź dostępność krytycznych aktualizacji i dodatków Service Pack; zainstaluj pakiet Microsoft .NET Framework 1.1 z dodatkiem Service Pack 1 dla systemu Windows Server 2000.</td>
</tr>
</tbody>
</table>
 

Oprócz tych wymagań program WSUS może w razie potrzeby zainstalować lub skonfigurować na serwerze funkcję ASP.NET w wersji 1.1. (Funkcję ASP.NET konfiguruje instalator WSUS).

#### Instalowanie programu MSDE 2000 w systemie Windows 2000

W przypadku używania systemu Windows 2000 dla programu WSUS i braku dostępu do programu Microsoft SQL Server 2000 przed uruchomieniem Instalatora programu WSUS należy zainstalować program Microsoft SQL Server 2000 Desktop Engine (MSDE). Jeśli na serwerze WSUS jest już zainstalowany program MSDE, nie ma potrzeby instalowania jego specjalnej instancji dla programu WSUS. Można po prostu wskazać istniejącą nazwę instancji w trakcie procesu instalacji programu WSUS.

Instalowanie programu MSDE w systemie Windows 2000 Server jest procesem składającym się z czterech etapów. Najpierw należy pobrać i rozwinąć archiwum programu MSDE do folderu znajdującego się na serwerze WSUS. Następnie za pomocą wiersza polecenia i jego opcji należy uruchomić Instalatora programu MSDE, określić hasło administratora systemu i przypisać WSUS jako nazwę instancji. Następnie po zakończeniu instalacji programu MSDE należy sprawdzić, czy instancja programu WSUS jest uruchomiona jako usługa systemu NT. W końcowym etapie należy dodać aktualizację zabezpieczeń do programu MSDE w celu zabezpieczenia serwera WSUS.

#### Krok 1: Pobranie i rozwinięcie archiwum programu MSDE

Pobierz i rozwiń archiwum programu MSDE do folderu znajdującego się na serwerze WSUS. Zobacz [Microsoft SQL Server Desktop Engine (MSDE 2000) wydanie A](http://go.microsoft.com/fwlink/?linkid=47366) (strona może być w języku angielskim).

#### Krok 2. Instalacja programu MSDE

Za pomocą wiersza polecenia i jego opcji uruchom Instalatora programu MSDE, określ hasło i przypisz WSUS jako nazwę instancji. Po zakończeniu instalacji programu MSDE sprawdź, czy instancja programu WSUS jest uruchomiona jako usługa NT.

Aby zainstalować program MSDE, określ hasło administratora systemu i przypisz nazwę instancji:

1.  W wierszu polecenia przejdź do folderu instalacji programu MSDE podanego w „Kroku 1: Pobranie i rozwinięcie archiwum programu MSDE”.
2.  Wpisz następujące polecenie: **setup sapwd="***hasło***" nazwa\_instancji=WSUS***,*
    gdzie zmienna *hasło* jest silnym hasłem do konta administratora systemu w tej instancji programu MSDE, natomiast zmienna **nazwa\_instancji** jest nazwą instancji bazy danych. Alternatywnie, dla bazy danych WSUS można użyć domyślnej nazwy instancji (zamiast „WSUS”). W przypadku wybrania tego rozwiązania nie ma potrzeby wpisywania polecenia **instancename=WSUS** jako parametru w wierszu polecenia. To polecenie umożliwia uruchomienie programu instalacyjnego MSDE, podanie wartości dla hasła administratora systemu oraz nazw instancji programu MSDE.

#### Krok 3: Sprawdzenie instalacji instancji WSUS programu MSDE

Należy upewnić się, czy widoczne jest wystąpienie WSUS programu MSDE.

1.  Kliknij przycisk **Start**, a następnie polecenie **Uruchom**.
2.  W polu **Otwórz** wpisz **services.msc**, a następnie kliknij przycisk **OK**.

Przewiń listę usług i sprawdź, czy usługa SSQL$WSUS (jeśli nazwa instancji to „WSUS”) lub MSSQLSERVER (jeśli użyto domyślnej nazwy instancji) istnieje.

#### Krok 4: Uruchomienie instancji programu MSDE

Na końcu procesu instalacji programu MSDE należy uruchomić instancję. Jeśli jako nazwę instancji została podana wartość „WSUS”, uruchom usługę „MSSQL$WSUS”. W przypadku użycia domyślnej nazwy instancji uruchom usługę MSSQLSERVER. Dopóki te usługa nie zostanie uruchomiona, program nie będzie mógł korzystać z instancji bazy danych.

#### Krok 5: Uaktualnienie programu MSDE

Wymagane jest pobranie i zainstalowanie aktualizacji zabezpieczeń opisanej w biuletynie [MS03-031: Cumulative Security Patch for SQL Server (Skumulowany pakiet zabezpieczeń dla programu SQL Server)](http://go.microsoft.com/fwlink/?linkid=47364) (strona może być w języku angielskim).

Aby pobrać aktualizację zabezpieczeń, zobacz artykuł dotyczący [pakietu poprawek dla programu SQL Server 2000 (32-bitowy) MS03-031](http://go.microsoft.com/fwlink/?linkid=47363).

#### Problem 4: Wymagania dotyczące minimalnej ilości wolnego miejsca na dysku.

W przypadku instalowania programu Windows Server Update Services konieczne jest spełnienie następujących wymagań dotyczących minimalnej ilości wolnego miejsca na dysku:

-   1 gigabajt (GB) w partycji systemowej
-   2 GB dla woluminu, na którym będą przechowywane pliki bazy danych
-   6 GB, co jest wartością oszacowaną na podstawie przewidywanej objętości zawartości

#### Problem 5: Przed zainstalowaniem najnowszej wersji programu WSUS należy odinstalować wcześniejsze wersje tego programu za pomocą apletu Dodaj lub usuń programy

W przypadku zamiaru zainstalowania programu Windows Server Update Services na serwerze, na którym jest zainstalowany program Windows Update Services w wersji beta 1 lub beta 2 należy najpierw odinstalować wcześniejszą wersję programu za pomocą apletu Dodaj lub usuń programy w Panelu sterowania.

#### Problem 6: Program WSUS wymaga włączenia opcji zagnieżdżonych wyzwalaczy w programie SQL Server

Ta opcja jest domyślnie włączona; jednak może zostać wyłączona przez administratora programu SQL Server.

W przypadku zamiaru używania bazy danych programu SQL Server jako magazynu danych programu Windows Server Update Services administrator serwera SQL powinien sprawdzić, czy opcja zagnieżdżonych wyzwalaczy na serwerze jest włączona zanim administrator WSUS zainstaluje program WSUS i wskaże bazę danych w trakcie instalacji.

Instalator programu WSUS powoduje włączenie opcji RECURSIVE\_TRIGGERS właściwej dla bazy danych; jednak nie powoduje włączenia opcji zagnieżdżonych wyzwalaczy będącej globalną opcją serwera.

Aby sprawdzić, czy opcja wyzwalaczy zagnieżdżonych jest włączona, użyj następującego polecenia:

**sp\_configure 'nested triggers'**

W celu włączenia opcji zagnieżdżonych wyzwalaczy w środowisku SQL Server, na komputerze z programem SQL Server wykonaj następujące polecenia z pliku wsadowego:

**sp\_configure 'nested triggers', 1**

**GO**

**RECONFIGURE**

**GO**

#### Problem 7: Parametry wiersza polecenia Instalatora programu WSUS

Istnieje możliwość wykonania instalacji nienadzorowanej programu WSUS. Aby uzyskać więcej informacji oraz parametry wiersza polecenia, zobacz „Dodatek A: Instalacja nienadzorowana” w części dotyczącej [wdrażania programu Microsoft Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=41777) (strona może być w języku angielskim).

Znane problemy
--------------

#### Problem 1: Kreator IIS Lockdown

W przypadku uruchamiania Internetowych usług informacyjnych (IIS) na komputerze z zainstalowanym systemem Windows 2000 Server zainstaluj najnowszą wersję Kreatora IIS Lockdown (zawierającej narzędzie URLScan) ze strony IIS Lockdown Tool (Narzędzie IIS Lockdown) w bazie informacji technicznych Microsoft TechNet. Firma Microsoft zdecydowanie zaleca zainstalowanie tego narzędzia w celu zabezpieczenia serwerów Internetowych usług informacyjnych. Działanie Kreatora IIS Lockdown polega na wyłączeniu zbędnych funkcji Internetowych usług informacyjnych, co ogranicza zagrożenie dla bezpieczeństwa.

> [!note]  
> Instalator programu WSUS nie instaluje tych składników. Te składniki muszą zostać zainstalowane ręcznie. Nie ma potrzeby instalowania narzędzia IIS Lockdown na komputerach z systemem Windows Server 2003, ponieważ ta funkcja jest częścią tego systemu. 

#### Problem 2: Zmiana konfiguracji programu WSUS bezpośrednio w bazie danych nie jest obsługiwana

Dane konfiguracji programu Windows Server Update Services są przechowywane w bazie danych (programu MSDE lub SQL Server). Nie jest jednak możliwa zmiana tych informacji bezpośrednio w bazie danych. Administratorzy nie powinni podejmować prób modyfikacji konfiguracji programu WSUS w ten sposób. Konfigurację programu WSUS można zmieniać za pośrednictwem konsoli WSUS lub przez wywoływanie interfejsów API programu WSUS.

#### Problem 3: Aby można było uzyskać dostęp do witryny administracyjnej programu WSUS, należy włączyć opcję wykonywania skryptów aktywnych

Aby można było uzyskać dostęp do witryny administracyjnej programu WSUS za pośrednictwem programu Internet Explorer, na stacji roboczej administratora należy skonfigurować program Internet Explorer w taki sposób, aby zezwalał na wykonywanie skryptów aktywnych.

#### Problem 4: Usługa IIS zostanie ponownie uruchomiona podczas instalacji programu WSUS

Instalator programu Windows Server Update Services ponownie uruchomi usługę IIS bez powiadomienia. Może to mieć wpływ na istniejące witryny sieci Web w danej organizacji.

#### Problem 5: Zmiana dostępu do katalogu wirtualnego punktów zarządzania programem WSUS lub SMS

Domyślnie dostęp do zawartości katalogu wirtualnego programu Windows Server Update Services jest możliwy w trybie anonimowym. W przypadku zmiany tego ustawienia i żądania uwierzytelniania klienci będą otrzymywać błędy dotyczące uwierzytelniania oraz nie będą mogli pobierać aktualizacji. Jest to znany problem wynikający z faktu, że biblioteka Winhttp.dll używa niewłaściwego kontekstu uwierzytelniania, gdy wymagane jest uwierzytelnianie niejawne, a w konsekwencji wezwanie do uwierzytelnienia kończy się niepowodzeniem. Aby uniknąć tego problemu, upewnij się, że dla serwera WSUS oraz punktów zarządzania (MP) programem SMS został skonfigurowany dostęp anonimowy do katalogów wirtualnych usług IIS.

#### Problem 6: W przypadku instalowania programu WSUS w systemie Windows Small Business Server 2003 należy zmodyfikować domyślne ustawienia dostępu do wirtualnych katalogów głównych programu WSUS w witrynie sieci Web w taki sposób, aby klienci WSUS mogli dokonywać autoaktualizacji z serwera

W trakcie instalacji serwera WSUS są instalowane dwa wirtualne katalogi główne, SelfUpdate i ClientWebService, oraz określone pliki w katalogu głównym domyślnej witryny sieci Web (na porcie 80). Dzięki temu klienci mogą dokonywać autoaktualizacji za pośrednictwem domyślnej witryny sieci Web. Domyślnie w systemie Windows Small Business Server 2003 konfiguracja domyślnej witryny sieci Web zezwala tylko na dostęp do adresu IP i hosta lokalnego tego serwera. Oznacza to odmowę dostępu do wirtualnych katalogów głównych SelfUpdate i ClientWebService oraz brak możliwości wykonywania autoaktualizacji przez klientów. Aby zezwolić klientom na wykonywanie autoaktualizacji, wykonaj poniższe czynności w wirtualnych katalogach głównych SelfUpdate i ClientWebService w domyślnej witrynie sieci Web.

1.  W wirtualnym katalogu głównym kliknij polecenie **Właściwości**, kliknij polecenie **Zabezpieczenia katalogów**, kliknij polecenie **Ograniczenia adresów IP i nazw domen**, a następnie kliknij polecenie **Edytuj**.
2.  Wybierz opcję **Udzielony dostęp**, a następnie kliknij przycisk **OK**. Zamknij wszystkie strony właściwości.

#### Problem 7: Instalowanie programu WSUS w systemie Small Business Server — problemy z integracją

-   Jeśli system Windows Small Business Server 2003 uzyskuje dostęp do Internetu za pośrednictwem serwera proxy ISA, w interfejsie użytkownika **Ustawienia** należy ręcznie wprowadzić następujące ustawienia: ustawienia serwera proxy, nazwa serwera proxy oraz port.
-   Jeśli program ISA korzysta z uwierzytelniania systemu Windows, poświadczenia serwera proxy muszą zostać wprowadzone w postaci „DOMENA\\użytkownik” (użytkownik należący do grupy „Użytkownicy Internetu”).

#### Problem 8: W przypadku przenoszenia komputera z jednej grupy komputerów do drugiej opóźnienie przeniesienia komputera do nowej grupy widoczne z konsoli administracyjnej może wynosić maksymalnie godzinę

Gdy komputer zostanie po raz pierwszy przypisany do grupy docelowej, dane na komputerze są modyfikowane informacjami o grupie. Te dane są odświeżane systematycznie lub co godzinę. W związku z tym przy przenoszeniu komputera z jednej grupy komputerów do drugiej opóźnienie odświeżenia tych informacji na kliencie i wyświetlenie zmian na konsoli administracyjnej programu WSUS może wynosić maksymalnie godzinę.

#### Problem 9: W przypadku instalowania programu WSUS na serwerze członkowskim i zamiaru podwyższenia poziomu serwera członkowskiego do kontrolera domeny należy najpierw odinstalować program WSUS

W przypadku instalowania programu WSUS na serwerze członkowskim i zamiaru podwyższenia poziomu serwera członkowskiego do kontrolera domeny należy wykonać następujące czynności:

1.  Odinstaluj program WSUS.
2.  Podwyższ poziom serwera do kontrolera domeny.
3.  Ponownie zainstaluj program WSUS.

#### Problem 10: Aby obniżyć poziom serwera WSUS z kontrolera domeny na serwer członkowski, należy najpierw odinstalować program WSUS

W przypadku uruchomienia serwera WSUS na kontrolerze domeny i zamiaru obniżenia poziomu kontrolera domeny do serwera członkowskiego, należy wykonać następujące czynności:

1.  Odinstaluj program WSUS i zachowaj bazę danych.
2.  Utwórz konto użytkownika ASPNET.
3.  W wierszu polecenia wpisz polecenie **aspnet\_regiis -i**.
4.  Ponownie zainstaluj program WSUS i użyj zachowanej bazy danych.

#### Problem 11: Jeśli platforma .NET Framework 1.0 lub 2.0 została zainstalowana po zainstalowaniu programu WSUS, konsola administracyjna programu WSUS nie będzie wyświetlana

Wynika to z tego, że platforma .NET Framework 1.0 jest rejestrowana za pośrednictwem usług IIS, a serwer WSUS wymaga platformy .NET Framework 1.1. Aby rozwiązać ten problem, otwórz plik aspnet\_regiis.exe i uruchom poniższe polecenia, w których zmienna *id\_witryny\_sieci\_Web* jest wartością znajdującą się w następującym kluczu rejestru:

HKLM\\Software\\Microsoft\\WindowsUpdateServices\\Server\\Setup\\IISTargetWebsiteIndex

-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*id\_witryny\_sieci\_Web*&gt;\\ROOT\\ReportingWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*id\_witryny\_sieci\_Web*&gt;\\ROOT\\ClientWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*id\_witryny\_sieci\_Web*&gt;\\ROOT\\SimpleAuthWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*id\_witryny\_sieci\_Web*&gt;\\ROOT\\WSUSAdmin
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*id\_witryny\_sieci\_Web*&gt;\\ROOT\\AdministrationWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*id\_witryny\_sieci\_Web*&gt;\\ROOT\\ServrSyncWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*id\_witryny\_sieci\_Web*&gt;\\ROOT\\DssAuthWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*id\_witryny\_sieci\_Web*&gt;\\ROOT\\Content

#### Problem 12: Ograniczenia zdalnego serwera SQL

Program WSUS oferuje ograniczoną obsługę uruchamiania oprogramowania baz danych na komputerze innym niż komputer zawierający pozostałe aplikacje WSUS.

-   Nie można używać serwera Windows 2000 Server jako komputera frontonu w zdalnej parze SQL.
-   Nie można używać serwera skonfigurowanego jako kontroler domeny jako serwera frontonu lub serwera typu back-end zdalnej pary SQL.
-   Nie można używać programu WMSDE ani MSDE dla oprogramowania bazy danych na komputerach typu back-end.
-   Instalacja zdalnego serwera SQL (który ma być używany jako baza danych WSUS) nie powiedzie się, jeśli usługi terminalowe są zainstalowane na serwerze zdalnym i działają w trybie aplikacji. Podczas instalowania programu SQL Server na serwerze usług terminalowych należy wykonać następujące czynności:
    1.  Przed uruchomieniem instalatora otwórz wiersz polecenia i wpisz polecenie: **change user /install**
    2.  Uruchom Instalatora programu SQL Server.
    3.  Po uruchomieniu instalatora w wierszu polecenia wpisz polecenie: **change user /execute**
-   Aby można było zainstalować bazę danych WSUS na serwerze zdalnym SQL, użytkownik musi należeć do lokalnej grupy zabezpieczeń Administratorzy zarówno na komputerze frontonu, jak i komputerze typu back-end.
-   Aby uzyskać więcej informacji na temat problemów ze zdalnym serwerem SQL, zobacz „Dodatek C: Zdalny serwer SQL” w części dotyczącej [&gt;wdrażania programu Microsoft Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=41777) (strona może być w języku angielskim).

#### Problem 13: Następny serwer replik może mieć mniej zatwierdzeń niż poprzedni serwer nadrzędny.

Następny serwer replik może mieć mniej zatwierdzeń niż poprzedni serwer nadrzędny. Wynika to z faktu, że zatwierdzenia instalacji nie przepływają do następnego serwera, dopóki pobieranie zawartości nie zakończy się na poprzednim serwerze.

#### Problem 14: W przypadku błędu synchronizacji należy ponownie przeprowadzić ten proces.

W przypadku błędu synchronizacji może zostać wyświetlony komunikat o błędzie. W takim wypadku należy najpierw spróbować synchronizacji.

#### Problem 15: Przy próbie uzyskania dostępu do konsoli administracyjnej programu WSUS jest wyświetlany komunikat o błędzie System.IO.FileNotFoundException

W przypadku wyświetlenia poniższego komunikatu o błędzie konieczna może być zmiana uprawnień na kontach usługi sieciowej lub ASP.NET:

System.IO.FileNotFoundException: File or Assembly name *xxxxxx*.dll, or one of its dependencies, was not found

Zmienna *xxxx* jest nazwą losową.

Aby rozwiązać ten problem w systemach operacyjnych Windows Server 2003, nadaj dla konta usługi sieciowej uprawnienie odczytu/zapisu do folderu to %systemroot%\\Temp. W systemie Windows 2000 Server nadaj dla konta ASP.NET uprawnienie odczytu/zapisu dla folderu %systemroot%\\Temp.

#### Problem 16: Aktualizacja zabezpieczeń SQL MS03-031 (KB815495)

Ta aktualizacja może być wskazywana jako zainstalowana na serwerze WSUS, nawet wtedy, gdy instalacja na kliencie nie powiodła się. Z tego powodu pakiet może być ponownie oferowany klientowi. Ten problem można obejść, cofając zatwierdzenie aktualizacji na serwerze.

#### Problem 17: Utrata ustawień usług IIS podczas uaktualniania wersji RTM.

W przypadku instalacji programu WSUS RTM na serwerze z zainstalowaną poprzednią wersją programu WSUS (na przykład RC) program WSUS RTM spowoduje odinstalowanie wcześniejszej wersji, a następnie zainstalowanie nowej wersji. Oznacza to, że wirtualne katalogi główne i pliki skojarzone z programem WSUS w ramach Internetowych usług informacyjnych zostaną usunięte.

W przypadku zainstalowania programu WSUS w domyślnej witrynie sieci Web ustawienia katalogów wirtualnych programu WSUS charakterystyczne dla tego programu zostaną utracone. Na przykład, jeśli wirtualne katalogi główne programu WSUS zostały skonfigurowane dla protokołu SSL w celu zabezpieczenia programu WSUS, konieczne będzie ich ponowne skonfigurowanie po zainstalowaniu wersji RTM programu WSUS. Uwaga: w konsoli programu WSUS zostanie wyświetlone powiadomienie o włączeniu obsługi protokołu SSL.

Jeśli program WSUS nie został zainstalowany w domyślnej witrynie sieci Web, wszystkie ustawienia dodatkowe na poziomie witryny sieci Web programu WSUS zostaną utracone.

#### Problem 18: Korzystanie z nagłówków hostów

Aby przypisać wartości nagłówków hosta do domyślnej witryny sieci Web (witryna sieci Web programu WSUS) w ramach Internetowych usług informacyjnych, należy dodać „wszystkie nieprzypisane” lub przypisany adres IP do listy adresów IP bez wartości nagłówka hosta w domyślnej witrynie sieci Web. Informacje te należy także dodać do witryny sieci Web innej niż domyślna.

**Ostrzeżenie**: Może to spowodować zakłócenia pracy programów Windows® SharePoint® Services i Exchange.

#### Problem 19: Konieczne jest dodanie adresu URL konsoli programu WSUS do listy stref zawartości sieci Web Zaufane witryny lub Lokalny intranet na komputerach z włączoną opcją ograniczenia funkcjonalności programu Internet Explorer

Jeśli opcja ograniczenia funkcjonalności programu Internet Explorer (znana także jako składnik Konfiguracja zwiększonych zabezpieczeń programu Internet Explorer w systemie Microsoft Windows Server 2003 Internet Explorer) jest włączona na komputerze i konsola programu WSUS nie zostanie dodana do stref zawartości sieci Web Zaufane witryny lub Lokalny intranet, przy każdej próbie otwarcia strony w konsoli programu WSUS będzie wyświetlany monit z prośbą o podanie poświadczeń użytkownika.

Aby dodać konsolę programu WSUS do stref zawartości sieci Web **Lokalny intranet** oraz **Zaufane witryny**:

1.  Otwórz aplet **Opcje internetowe** (na przykład kliknij przycisk **Start**, wskaż polecenie **Panel sterowania**, a następnie kliknij polecenie **Opcje internetowe**).
2.  Na karcie **Zabezpieczenia** kliknij polecenie **Lokalny intranet**, kliknij polecenie **Witryny**, kliknij opcję **Zaawansowane**, dodaj adres URL (http://*nazwa\_serwera\_WSUS*/WSUSAdmin), a następnie kliknij przycisk **OK**.
3.  Kliknij polecenie **Zaufane witryny**, kliknij polecenie **Witryny**, dodaj adres URL konsoli programu WSUS, kliknij przycisk **OK**, a następnie ponownie kliknij przycisk **OK**, aby zamknąć aplet **Opcje internetowe**.

#### Problem 20: Niepowodzenie uaktualnienia z wersji WSUS Release Candidate

Uaktualnienie z wersji WSUS Release Candidate może nie udać się ze względu na problem z drzewem SelfUpdate. Może do tego dojść, jeśli wielu klientów dokonuje samodzielnej aktualizacji w momencie, gdy użytkownik próbuje dokonać uaktualnienia.

Rozwiązanie problemu:

1.  Odłącz serwer WSUS od sieci i upewnij się, że klienci nie mogą się z nim połączyć.
2.  W wierszu polecenia wpisz: **iisrestart /reset** i naciśnij klawisz ENTER.
3.  Uruchom uaktualnienie.

#### Problem 21: Niektóre zatwierdzenia SUS 1.0 nie mogą być migrowane do WSUS.

Podczas migracji z SUS 1.0 do WSUS niektóre zatwierdzenia serwera SUS 1.0 nie będą mogły być migrowane do serwera WSUS. Wynika to z faktu, że niektóre aktualizacje, które były dostępne dla serwera SUS 1.0, nie są dostępne dla programu WSUS. Ponadto program WSUS obsługuje większą liczbę aktualizacji niż SUS, dlatego też na serwerze WSUS mogą znaleźć się ważne aktualizacje, które po zakończeniu procesu migracji pozostaną niezatwierdzone.

Firma Microsoft zdecydowanie zaleca, aby po migracji z programu SUS 1.0 sprawdzić niezatwierdzone aktualizacje.

Aby uzyskać więcej informacji na temat migracji z programu SUS 1.0 do programu WSUS, zobacz [poradnik poświęcony migracji z programu Software Update Services do programu Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=48042) na stronie http://go.microsoft.com/fwlink/?LinkId=48042.

#### Problem 22: Przed uaktualnieniem do programu WSUS 2.0 z dodatkiem Service Pack 1 należy naprawić ten wpis rejestru, jeśli dokonano migracji z programu WMSDE do SQL Server

Planując uaktualnienie programu WSUS 2.0 do wersji z dodatkiem Service Pack 1 należy zadbać o zmianę poniższego wpisu rejestru, jeśli instalacja WMSDE została przeniesiona do programu SQL Server (zdalnego lub lokalnego), :

HKLM\\Software\\Microsoft\\Update Services\\Server\\Setup\\WmsdeInstalled 

Należy zmienić wartość z 1 na 0.

#### Problem 23: Migrowanie zdalnej instalacji programu SQL do programu WSUS 2.0 z dodatkiem Service Pack 1

W przypadku migracji do programu WSUS 2.0 z dodatkiem Service Pack 1 ze zdalną konfiguracją SQL należy wykonać następujące czynności:

1) Uruchom pakiet instalacyjny serwera frontonu bez przełączników i wybierz opcję uaktualnienia

2) Uruchom pakiet instalacyjny serwera typu back end bez przełączników i wybierz opcję uaktualnienia

#### Prawa autorskie

Informacje znajdujące się w tym dokumencie przedstawiają aktualne stanowisko firmy Microsoft Corporation dotyczące zagadnień omówionych do daty publikacji. Ponieważ firma Microsoft zmuszona jest reagować na zmieniające się warunki rynkowe, dokumentu tego nie należy interpretować jako zobowiązania ze strony firmy Microsoft, a firma Microsoft nie może zagwarantować dokładności informacji zaprezentowanych po dacie publikacji.

Niniejszy dokument ma charakter wyłącznie informacyjny. FIRMA MICROSOFT NIE UDZIELA ŻADNYCH GWARANCJI, BEZPOŚREDNICH, DOMNIEMANYCH LUB PRZEWIDZIANYCH PRZEZ PRAWO, DOTYCZĄCYCH INFORMACJI ZNAJDUJĄCYCH SIĘ W TYM DOKUMENCIE.

Odpowiedzialność za dostosowanie się do stosownych praw autorskich spoczywa na użytkowniku. Bez ograniczania praw objętych prawem autorskim niniejszego dokumentu ani jego części nie wolno w żadnej formie powielać, przechowywać ani wprowadzać do żadnego systemu umożliwiającego odtworzenie, ani przekazywać za pomocą jakichkolwiek nośników (elektronicznych, mechanicznych, fotokopii, nagrania itp.) z wyjątkiem przypadków, w których uzyskano na to pisemną zgodę firmy Microsoft Corporation.

Firma Microsoft może mieć patenty lub rozpoczęte postępowania patentowe, znaki towarowe, prawa autorskie lub inne prawa związane z własnością intelektualną, które odnoszą się do treści zawartej w niniejszym dokumencie. Otrzymanie tego dokumentu nie oznacza udzielenia licencji na te patenty, znaki towarowe, prawa autorskie ani inne prawa związane z własnością intelektualną, z wyjątkiem wyraźnie określonych przypadków zawartych w pisemnych umowach licencyjnych firmy Microsoft.

O ile nie podano inaczej, wymienione w przykładach firmy, organizacje, produkty, nazwy domen, adresy e-mail, znaki logo, osoby, miejsca i zdarzenia są fikcyjne i nie mają żadnego związku z jakimikolwiek rzeczywistymi firmami, organizacjami, produktami, nazwami domen, adresami e-mail, znakami logo, osobami, miejscami lub zdarzeniami.

© 2005 Microsoft Corporation. Wszelkie prawa zastrzeżone.

Microsoft, SQL Server, Windows i Windows Server są zastrzeżonymi znakami towarowymi lub znakami towarowymi firmy Microsoft Corporation zarejestrowanymi w USA i/lub w innych krajach.

Nazwy rzeczywistych firm i produktów wymienione w niniejszym dokumencie mogą być znakami towarowymi zarejestrowanymi przez ich prawnych właścicieli.
