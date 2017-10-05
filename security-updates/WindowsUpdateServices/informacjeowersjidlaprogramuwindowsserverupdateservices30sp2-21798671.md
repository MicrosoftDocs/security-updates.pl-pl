---
TOCTitle: 'Informacje o wersji dla programu Windows Server Update Services 3.0 SP2'
Title: 'Informacje o wersji dla programu Windows Server Update Services 3.0 SP2'
ms:assetid: 'b3723422-489d-47b7-abfa-663353647da0'
ms:contentKeyID: 21798671
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Dd939886(v=WS.10)'
---

Informacje o wersji dla programu Windows Server Update Services 3.0 SP2
=======================================================================

Te informacje o wersji dotyczą programu Windows Server Update Services 3.0 z dodatkiem Service Pack 2 (WSUS 3.0 z dodatkiem SP2). Ten dokument zawiera następujące sekcje:

1.  Co nowego w tej wersji
2.  Wymagania systemowe dla instalacji serwera programu WSUS 3.0 z dodatkiem SP2
3.  Wymagania wstępne związane z konfiguracją oraz najważniejsze wskazówki dotyczące serwera WSUS
4.  Wymagania wstępne dotyczące produktu Windows Small Business Server
5.  Wymagania systemowe dla instalacji konsoli zdalnej programu WSUS 3.0 z dodatkiem SP2
6.  Wymagania systemowe dla instalacji klienta
7.  Wymagania i zalecenia dotyczące uaktualniania
8.  Instalowanie programu WSUS 3.0 z dodatkiem SP2
9.  Parametry wiersza polecenia dotyczące instalacji nienadzorowanych programu WSUS 3.0 z dodatkiem SP2
10. Znane problemy

Co nowego w tej wersji
----------------------

-   Integracja z systemem Windows Server® 2008 R2.
-   Obsługa funkcji BranchCache w systemie Windows Server 2008 R2.
-   Obsługa klientów z systemem Windows 7.
-   Udoskonalenia klienta usługi Windows Update Agent (WUA). Nowy klient usługi WUA zawiera udoskonalenia dotyczące wydajności i środowiska użytkownika oraz różne poprawki, które wprowadzono, bazując na opiniach klientów.
    -   Czas skanowania klienta jest krótszy niż w poprzednich wersjach.
    -   Komputery zarządzane przez serwery programu WSUS zamiast pełnego skanowania mogą teraz przeprowadzać skanowanie w określonym zakresie w odniesieniu do tych samych serwerów programu WSUS. Dzięki temu skanowanie w poszukiwaniu aplikacji z zastosowaniem interfejsów API usługi Microsoft Update, takich jak Windows Defender, jest znacznie szybsze.
    -   Udoskonalenia dotyczące środowiska użytkownika usługi WUA ułatwiają użytkownikom organizowanie aktualizacji i zapewniają bardziej przejrzyste informacje dotyczące znaczenia i działania aktualizacji.
    -   Komputery skonfigurowane za pomocą obrazów systemów są lepiej widoczne w konsoli programu WSUS. Aby uzyskać więcej informacji, zobacz artykuł opisujący sytuację, w której [komputer z systemem Windows 2000, Windows Server 2003 lub Windows XP skonfigurowany przy użyciu obrazu systemu Windows 2000, Windows Server 2003 lub Windows XP nie jest widoczny w konsoli programu WSUS](http://go.microsoft.com/fwlink/?linkid=159749) (strona może zostać wyświetlona w języku angielskim).
-   Nowe funkcje:
    -   Reguły automatycznego zatwierdzania umożliwiają obecnie określanie terminu ostatecznego (daty i godziny) zatwierdzenia dla wszystkich komputerów lub dla określonych grup komputerów.
    -   Ulepszona obsługa wyboru języka na serwerach podrzędnych udostępnia nowe okno dialogowe z ostrzeżeniem, które jest wyświetlane w przypadku pobierania aktualizacji tylko dla określonych języków.
    -   Nowe raporty dotyczące aktualizacji i stanu komputerów umożliwiają filtrowanie aktualizacji zatwierdzonych do zainstalowania. Można uruchamiać te raporty za pomocą konsoli programu WSUS lub dołączyć tę funkcjonalność do własnych raportów, korzystając z interfejsu programowania aplikacji (API).
-   Dodatki Service Pack 1 i Service Pack 2 dla programu WSUS 3.0 udostępniają zgodny interfejs użytkownika na serwerze i na kliencie.
-   Aktualizacje oprogramowania.
-   W tej wersji rozwiązano znane problemy dotyczące usługi Windows Update Agent:
    1.  Program WSUS 3.0 z dodatkiem SP2 i system Windows 7 zawierają nową wersję usługi Windows Update Agent (dla systemów Windows XP, Windows Vista, Windows Server 2000, Windows Server 2003 i Windows Server 2008). W tej wersji rozwiązano następujący problem: wywołania interfejsów API z poziomu systemu innego niż lokalny w sesji nieinterakcyjnej kończą się niepowodzeniem.
    2.  Problem rozwiązany w wersji 7.2.6001.788 usługi Windows Update Agent. W tej aktualizacji rozwiązano następujący problem: próba jednoczesnego zainstalowania co najmniej 80 aktualizacji z poziomu strony Windows Update lub Microsoft Update może spowodować zwrócenie kodu błędu 0x80070057.
    3.  Ulepszenia i rozwiązane problemy uwzględnione w wersji 7.2.6001.784 usługi Windows Update Agent. Ta aktualizacja obejmuje następujące ulepszenia: krótszy czas skanowania w usłudze Windows Update, szybsze dostarczanie aktualizacji podpisów, obsługa funkcji ponownego instalowania w Instalatorze Windows, ulepszona obsługa komunikatów o błędach.

<span id="BKMK_SysReqWSUS30SP2"></span>
Wymagania systemowe dla instalacji serwera programu WSUS 3.0 z dodatkiem SP2
----------------------------------------------------------------------------

W tej sekcji opisano wymagania dotyczące sprzętu i oprogramowania, które muszą być spełnione, aby można było zainstalować program WSUS 3.0 z dodatkiem SP2.

### Wymagania wstępne dotyczące oprogramowania dla serwera WSUS

-   Na komputerze musi być zainstalowany jeden z następujących obsługiwanych systemów operacyjnych:
    -   Windows Server 2008 R2
    -   Windows Server 2008 z dodatkiem SP1 lub nowsza wersja
 
        <table style="border:1px solid black;">
        <colgroup>
        <col width="100%" />
        </colgroup>
        <thead>
        <tr class="header">
        <th style="border:1px solid black;" ><img src="images/Dd939886.Warning(WS.10).gif" />Ostrzeżenie</th>
        </tr>
        </thead>
        <tbody>
        <tr class="odd">
        <td style="border:1px solid black;">Jeśli program WSUS 3.0 z dodatkiem SP2 został zainstalowany w systemie Windows Server 2008 przed przeprowadzeniem uaktualnienia do systemu Windows Server 2008 R2, próba uaktualnienia do systemu Windows Server 2008 R2 nie powiedzie się. Aby uzyskać więcej informacji, zobacz sekcję <a href="#bkmk_knownissues">Znane problemy</a>.
        </td>
        </tr>
        </tbody>
        </table>
 

    -   Windows Server 2003 SP1 lub nowsza wersja
    -   Windows Small Business Server 2008
    -   Windows Small Business Server 2003

    Należy pamiętać, że istnieją dodatkowe wymagania wstępne dotyczące produktu Windows Small Business Server. Aby uzyskać więcej informacji, zobacz sekcję „Wymagania wstępne dotyczące produktu Windows Small Business Server”.
-   Program Internet Information Services (IIS) w wersji 6.0 lub nowszej
-   Program Microsoft .NET Framework 2.0 lub nowsza wersja
-   Na komputerze musi być zainstalowana jedna z następujących obsługiwanych baz danych:
    -   Microsoft SQL Server 2008 Standard lub Enterprise Edition
    -   Microsoft SQL Server 2005 z dodatkiem SP3 lub nowsza wersja
    -   Wewnętrzna baza danych systemu Windows

    Jeśli nie jest zainstalowana żadna z obsługiwanych wersji programu SQL Server, Kreator instalacji programu WSUS 3.0 z dodatkiem SP2 zainstaluje wewnętrzną bazę danych systemu Windows.
-   Program Microsoft Management Console 3.0
-   Program Microsoft Report Viewer Redistributable 2008

 
<table style="border:1px solid black;">
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" ><img src="images/Dd939886.Important(WS.10).gif" />Ważne</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">System Windows Server 2008 R2 wymaga programu WSUS 3.0 z dodatkiem SP2. Jeśli zainstalowano system Windows Server 2008 R2, należy zainstalować program WSUS 3.0 z dodatkiem SP2. Nie należy instalować programu WSUS 3.0 z dodatkiem SP1 w systemie Windows Server 2008 R2.

Programu WSUS 3.0 z dodatkiem SP2 nie można używać z usługami terminalowymi na serwerze frontonu zdalnej konfiguracji bazy danych SQL.
</td>
</tr>
</tbody>
</table>
 

### Wymagania wstępne dotyczące oprogramowania dla konsoli administracyjnej programu WSUS

-   Jeden z następujących obsługiwanych systemów operacyjnych: Windows Server 2008 R2, Windows Server 2008, Windows Server 2003 z dodatkiem SP2 lub nowsze wersje, Windows Small Business Server 2008 albo Windows Small Business Server 2003, Windows Vista lub Windows XP z dodatkiem SP2
-   Program Microsoft .NET Framework 2.0 lub nowsza wersja
-   Program Microsoft Management Console 3.0
-   Program Microsoft Report Viewer Redistributable 2008

### Minimalne wymagania dotyczące sprzętu dla serwera programu WSUS

Następująca lista zawiera minimalne wymagania dotyczące sprzętu niezbędne do utworzenia podstawowej instalacji serwera. Pełną listę obsługiwanych konfiguracji sprzętowych można znaleźć w przewodniku dotyczącym wdrażania programu WSUS 3.0 z dodatkiem SP2 pod adresem [http://go.microsoft.com/fwlink/?LinkId=139832](http://go.microsoft.com/fwlink/?linkid=139832) (strona może zostać wyświetlona w języku angielskim).

-   Partycja systemowa oraz partycja z zainstalowanym programem WSUS 3.0 z dodatkiem SP2 muszą być sformatowane z użyciem systemu plików NTFS.
-   Co najmniej 1 GB wolnego miejsca na partycji systemowej.
-   Co najmniej 2 GB wolnego miejsca w woluminie, w którym będą przechowywane pliki bazy danych.
-   Co najmniej 20 GB wolnego miejsca w woluminie, w którym będzie przechowywana zawartość (zalecane 30 GB).

 
<table style="border:1px solid black;">
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" ><img src="images/Dd939886.Important(WS.10).gif" />Ważne</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Programu WSUS 3.0 z dodatkiem SP2 nie można zainstalować na dyskach skompresowanych.
</td>
</tr>
</tbody>
</table>
 

Wymagania wstępne związane z konfiguracją oraz najważniejsze wskazówki dotyczące serwera WSUS
---------------------------------------------------------------------------------------------

Przed zainstalowaniem programu WSUS 3.0 SP2 należy upewnić się, że zostały wykonane odpowiednie zadania opisane w tej sekcji.

### Usługi IIS

-   Na stronie Usługi roli serwera sieci Web (IIS) w Menedżerze serwera należy zainstalować wszelkie wymagane funkcje, wszystkie domyślne usługi roli IIS i następujące usługi roli: **ASP.NET**, **Uwierzytelnianie systemu Windows**, **Kompresja zawartości dynamicznej** i **Zgodność z narzędziami zarządzania usługami IIS w wersji 6**.
-   Jeśli usługi IIS są uruchomione w trybie izolacji usług IIS 5.0, instalacja nie powiedzie się. Przed zainstalowaniem programu WSUS 3.0 z dodatkiem SP2 należy wyłączyć tryb izolacji usług IIS 5.0.
-   Jeśli którykolwiek ze składników usług IIS został zainstalowany w 32-bitowym trybie zgodności na platformie 64-bitowej, instalacja programu WSUS 3.0 z dodatkiem SP2 może zakończyć się niepowodzeniem. Wszystkie składniki programu IIS powinny zostać zainstalowane w trybie macierzystym platform 64-bitowych.

### Serwery proxy

Program WSUS 3.0 z dodatkiem SP2 umożliwia serwerowi proxy obsługę wyłącznie protokołu HTTP. Zaleca się skonfigurowanie drugiego serwera proxy z protokołem HTTPS za pomocą wiersza polecenia (**wsusutil configuresslproxy**) przed skonfigurowaniem serwera programu WSUS z poziomu konsoli administracyjnej lub Kreatora konfiguracji.

### Witryny sieci Web uruchomione na porcie 80

Jeśli na porcie 80 są uruchomione co najmniej dwie witryny sieci Web (na przykład oparte na programie Windows SharePoint Services), przed zainstalowaniem programu WSUS należy usunąć je tak, aby została tylko jedna. W przeciwnym razie samoczynna aktualizacja klientów serwera może nie działać.

### Programy antywirusowe

Przed rozpoczęciem instalowania programu WSUS 3.0 z dodatkiem SP2 może być wymagane wyłączenie programów antywirusowych. Gdy oprogramowanie antywirusowe zostanie wyłączone, należy uruchomić ponownie komputer przed rozpoczęciem instalacji programu WSUS. Ponowne uruchomienie komputera zapobiega zablokowaniu plików, do których dostęp będzie wymagany w czasie instalacji. Po ukończeniu instalacji należy włączyć ponownie oprogramowanie antywirusowe. Należy odwiedzić witrynę sieci Web producenta oprogramowania antywirusowego, aby uzyskać dokładny opis wyłączania i ponownego włączania tego oprogramowania.

 
<table style="border:1px solid black;">
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" ><img src="images/Dd939886.Caution(WS.10).gif" />Przestroga</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Zastosowanie tego obejścia może spowodować, że komputer lub sieć będą bardziej narażone na ataki złośliwych użytkowników lub złośliwego oprogramowania, na przykład wirusów. Nie zalecamy takiego rozwiązania, ale chcemy wskazać możliwość wykonania takiej procedury wedle uznania użytkownika. Tę procedurę należy przeprowadzać na własną odpowiedzialność.

Oprogramowanie antywirusowe ułatwia ochronę komputera przed wirusami. Jeśli program antywirusowy jest wyłączony, nie należy pobierać ani otwierać plików pochodzących z niezaufanych źródeł. Nie wolno także odwiedzać niezaufanych witryn sieci Web ani otwierać załączników wiadomości e-mail.
</td>
</tr>
</tbody>
</table>
 

### Opcja wyzwalaczy zagnieżdżonych programu SQL Server

Jeśli magazynem danych programu Windows Server Update Services ma być baza danych programu SQL Server, administrator programu SQL Server powinien sprawdzić, czy opcja wyzwalaczy zagnieżdżonych jest włączona na serwerze, zanim administrator programu WSUS zainstaluje program WSUS 3.0 z dodatkiem SP2. Opcja wyzwalaczy zagnieżdżonych jest włączana domyślnie, może zostać jednak wyłączona przez administratora programu SQL Server. Instalator programu WSUS 3.0 z dodatkiem SP2 włącza opcję RECURSIVE\_TRIGGERS specyficzną dla bazy danych. Instalator programu WSUS 3.0 z dodatkiem SP2 nie włącza jednak opcji wyzwalaczy zagnieżdżonych będącej globalną opcją serwera.

### Ograniczenia i wymagania dotyczące współpracy ze zdalną bazą danych SQL

Program WSUS 3.0 z dodatkiem SP2 umożliwia uruchamianie zgodnej wersji oprogramowania SQL Server na komputerze innym niż komputer, na którym jest uruchomiona aplikacja WSUS 3.0 z dodatkiem SP2. Poniższe wymagania dotyczą zdalnej instalacji bazy danych SQL.

-   Serwera skonfigurowanego jako kontroler domeny nie można używać jako komputera wewnętrznego ze zdalną bazą danych SQL.
-   Na komputerze będącym serwerem frontonu zdalnej instalacji bazy danych SQL nie można uruchamiać usług terminalowych.
-   Zarówno komputer frontonu, jak i komputer wewnętrzny muszą być przyłączone do domeny usługi Active Directory. Jeśli komputer frontonu i komputer wewnętrzny znajdują się w różnych domenach, przed uruchomieniem Instalatora programu WSUS należy ustanowić zaufanie między tymi domenami.
-   Jeśli program WSUS 2.0 zainstalowano już w konfiguracji ze zdalną bazą danych SQL i jest planowane uaktualnienie go do programu WSUS 3.0 z dodatkiem SP2, przed zainstalowaniem programu WSUS wykonaj następujące czynności:
    1.  Odinstaluj program WSUS 2.0 za pomocą apletu **Dodaj lub usuń programy** w Panelu sterowania. Upewnij się przy tym, że istniejąca baza danych pozostała nienaruszona.
    2.  Zainstaluj program SQL Server 2005 z dodatkiem SP2 lub SQL Server 2008 i uaktualnij istniejącą bazę danych.

### Usługi IIS zostaną ponownie uruchomione podczas instalowania programu WSUS 3.0 z dodatkiem SP2

Instalator programu WSUS 3.0 z dodatkiem SP2 uruchomi ponownie usługi IIS bez powiadomienia. Może to wpłynąć na istniejące witryny sieci Web w organizacji. Zaleca się powiadomienie wszystkich użytkowników tych witryn sieci Web przed rozpoczęciem tej instalacji. Należy pamiętać, że Instalator programu WSUS 3.0 z dodatkiem SP2 uruchomi usługi IIS, jeśli nie były uruchomione.

Wymagania wstępne dotyczące produktu Windows Small Business Server
------------------------------------------------------------------

Jeśli program WSUS 3.0 z dodatkiem SP2 jest instalowany w systemie Windows Small Business Server, mają zastosowanie poniższe wymagania wstępne.

### Jeśli w wirtualnym katalogu głównym usług IIS wprowadzono ograniczenie umożliwiające używanie tylko określonych adresów IP lub nazw domen

W niektórych instalacjach produktu Windows Small Business Server może występować domyślna witryna sieci Web usług IIS skonfigurowana na potrzeby opcji **Ograniczenia adresów IP i nazw domen**. W takim przypadku klient usługi Windows Update na serwerze może nie mieć możliwości przeprowadzenia samodzielnej aktualizacji. Przed zainstalowaniem programu WSUS 3.0 z dodatkiem SP2 należy usunąć to ograniczenie.

### Jeśli jest używany serwer proxy programu ISA

-   Jeśli system Windows Small Business Server uzyskuje dostęp do Internetu za pomocą serwera proxy programu ISA, wpisz ciąg **ustawienia serwera proxy, nazwa serwera proxy, port** w interfejsie użytkownika **Ustawienia**.
-   Jeśli program ISA korzysta z uwierzytelniania systemu Windows, wpisz poświadczenia serwera proxy w postaci *DOMENA*\\*użytkownik*. Użytkownik powinien być członkiem grupy Internet Users (Użytkownicy Internetu).

### Jeśli do sieci dodano podsieć i nie użyto kreatorów produktu Windows Small Business Server

W procesie instalacji serwera WSUS na serwerze są instalowane dwa wirtualne katalogi główne programu IIS: SelfUpdate oraz ClientWebService. Instalator umieszcza także niektóre pliki w katalogu głównym domyślnej witryny sieci Web (używającej portu 80), co umożliwia komputerom klienckim przeprowadzanie samodzielnej aktualizacji za pośrednictwem domyślnej witryny sieci Web. Domyślna witryna sieci Web jest skonfigurowana tak, aby blokować dostęp do adresów IP innych niż localhost lub określonych podsieci skojarzonych z serwerem. Dlatego komputery klienckie, które nie używają adresu localhost ani nie znajdują się w tych podsieciach, nie mogą przeprowadzać samodzielnej aktualizacji. Jeśli do sieci dodano podsieć bez użycia kreatorów systemu Microsoft Windows Small Business Server, należy wykonać poniższą procedurę:

1.  W obszarze Zarządzanie serwerem rozwiń kolejno węzły **Zarządzanie zaawansowane**, **Internetowe usługi informacyjne**, **Witryny sieci Web**, **Domyślna witryna sieci Web**, kliknij prawym przyciskiem myszy katalog wirtualny **Selfupdate**, a następnie kliknij polecenie **Właściwości**.
2.  Kliknij kartę **Ustawienia zabezpieczeń**.
3.  W obszarze **Ograniczenia adresów IP i nazw domen** kliknij pozycję **Edytuj**, a następnie kliknij pozycję **Udzielony dostęp**.
4.  Kliknij przycisk **OK**, kliknij prawym przyciskiem myszy katalog wirtualny **ClientWebService**, a następnie kliknij polecenie **Właściwości**.
5.  Kliknij kartę **Ustawienia zabezpieczeń**.
6.  W obszarze **Ograniczenia adresów IP i nazw domen** kliknij pozycję **Edytuj**, a następnie kliknij pozycję **Udzielony dostęp**.

Wymagania systemowe dla instalacji konsoli zdalnej programu WSUS 3.0 z dodatkiem SP2
------------------------------------------------------------------------------------

Konsolę zdalną programu WSUS 3.0 z dodatkiem SP2 można zainstalować w dowolnym z następujących systemów operacyjnych:

-   Windows Server 2008 R2, Windows Server 2008 z dodatkiem SP1 lub nowsze wersje, Windows Server 2003 z dodatkiem SP2 lub nowsze wersje, Windows Small Business Server 2003, Windows Small Business Server 2005 lub Windows Small Business Server 2008, Windows Vista albo Windows XP Professional z dodatkiem SP3 lub nowsze wersje.

Wymagania systemowe dla instalacji klienta programu WSUS
--------------------------------------------------------

Aktualizacje automatyczne (oprogramowanie klienckie programu WSUS) można zainstalować w dowolnym z następujących systemów operacyjnych:

-   Windows Server 2008 R2, Windows Server 2008 z dodatkiem SP1 lub nowsze wersje, Windows Server 2003 z dodatkiem SP2 lub nowsze wersje, Windows Small Business Server 2003, Windows Small Business Server 2005 albo Windows Small Business Server 2008, Windows Vista, Windows XP Professional RTM, Windows XP Professional z dodatkiem SP1, Windows XP Professional z dodatkiem SP2, Windows XP Professional z dodatkiem SP3 lub nowsze wersje, Windows 2000 z dodatkiem SP4 lub Windows 7 (klient).

Wymagania i zalecenia dotyczące uaktualniania
---------------------------------------------

Poniższe wersje programu WSUS można uaktualnić do programu WSUS 3.0 z dodatkiem SP2 bez odinstalowywania starszej wersji:

-   WSUS 2.0, 2.0 z dodatkiem SP1, 3.0 i 3.0 z dodatkiem SP1.

Uaktualnienia programu WSUS z wersji 1.0 do wersji 3.0 z dodatkiem SP2 nie są obsługiwane. Przed zainstalowaniem programu WSUS 3.0 z dodatkiem SP2 należy odinstalować program Software Update Services (SUS) 1.0.

System Windows Server 2008 R2 wymaga programu WSUS 3.0 z dodatkiem SP2. Jeśli zainstalowano system Windows Server 2008 R2, należy zainstalować program WSUS 3.0 z dodatkiem SP2. Nie należy instalować programu WSUS 3.0 z dodatkiem SP1 w systemie Windows Server 2008 R2.

#### Przed przeprowadzeniem uaktualnienia do programu WSUS 3.0 z dodatkiem SP2

1.  Sprawdź błędy zarejestrowane ostatnio w dziennikach zdarzeń, problemy z synchronizacją między serwerami podrzędnymi i nadrzędnymi oraz problemy z raportowaniem dotyczącym klientów. Przed rozpoczęciem uaktualniania rozwiąż te problemy.

2.  Opcjonalnie można uruchomić polecenie DBCC CHECKDB, aby upewnić się, że baza danych programu WSUS jest poprawnie indeksowana. Aby uzyskać więcej informacji o poleceniu DBCC CHECKDB, zobacz [DBCC CHECKDB](http://go.microsoft.com/fwlink/?linkid=86948) (strona może zostać wyświetlona w języku angielskim).

3.  Wykonaj kopię zapasową bazy danych programu WSUS. Zwróć uwagę, że Instalator programu WSUS 3.0 z dodatkiem SP2 doda nową bazę danych do katalogu domyślnego, czyli *dysk*\\WSUS (*dysk* to dysk lokalny z systemem plików NTFS, na którym jest dostępna największa ilość wolnego miejsca). Jeśli w tym katalogu jest już umieszczona kopia zapasowa bazy danych, może zostać zastąpiona. Zaleca się zapisanie kopii zapasowej bazy danych bieżącej wersji programu WSUS w innej lokalizacji przed rozpoczęciem uaktualniania do programu WSUS 3.0 z dodatkiem SP2.

4.  Jeśli ręcznie zmieniono port używany przez program WSUS (bez użycia narzędzia Wsusutil) i jest obecnie używany program SUS 1.0 lub WSUS 2.0, uruchom domyślną witrynę sieci Web przed odinstalowaniem programu SUS 1.0 lub WSUS 2.0 w wersji 64-bitowej.

5.  Otwarte połączenia z istniejącą bazą danych programu WSUS (na przykład związane z otwartym programem SQL Server Management Studio) mogą spowodować niepowodzenie instalacji. Przed zainstalowaniem programu WSUS 3.0 z dodatkiem SP2 zamknij wszystkie połączenia.

### Odzyskiwanie instalacji po błędzie uaktualnienia

Jeśli próba uaktualnienia starszej wersji programu WSUS do wersji 3.0 z dodatkiem SP2 zakończy się niepowodzeniem (z dowolnego powodu innego niż próba przeprowadzenia nieobsługiwanego uaktualnienia programu SUS 1.0), należy wykonać poniższe zadania.

1.  Zainstaluj ponownie starszą wersję programu WSUS.
2.  Przywróć bazę danych na podstawie kopii zapasowej, która została wykonana przed próbą uaktualnienia. Pomyślne ukończenie uaktualniania jest niemożliwe, jeśli istnieje baza danych programu WSUS 3.0 z dodatkiem SP2 związana z poprzednią instalacją. W większości przypadków program WSUS automatycznie wykonuje kopię zapasową. Aby poznać jej lokalizację, zobacz plik WSUSSetup.log.
3.  Sprawdź dzienniki, aby ustalić przyczynę niepowodzenia, a następnie rozwiąż zaistniały problem.
4.  Zainstaluj program WSUS 3.0 z dodatkiem SP2.

### Zmiana nazwy komputera przed przeprowadzeniem uaktualnienia do programu WSUS 3.0 SP2 może spowodować niepowodzenie uaktualnienia

Jeśli nazwa komputera zostanie zmieniona po zainstalowaniu programu WSUS 2.0, ale przed przeprowadzeniem uaktualnienia do programu WSUS 3.0 z dodatkiem SP2, próba uaktualnienia może zakończyć się niepowodzeniem.

Użyj następującego skryptu, aby usunąć i dodać ponownie grupy ASPNET i Administratorzy WSUS. Następnie ponownie uruchom uaktualnianie.

        ```

### Jeśli przeprowadzono migrację z programu MSDE do programu SQL Server 2008 lub SQL Server 2005 w programie WSUS 2.0, należy zmienić odpowiednią wartość rejestru

Jeśli po zainstalowaniu programu WSUS 2.0 przeprowadzono migrację do programu SQL Server 2008 lub SQL Server 2005, należy zmienić wartość **HKLM\\SOFTWARE\\Microsoft\\Update Services\\Server\\Setup\\WmsdeInstalled** z 1 na 0. Jeśli ta czynność nie zostanie wykonana przed rozpoczęciem uaktualniania do programu WSUS 3.0 z dodatkiem SP2, próba uaktualnienia zakończy się niepowodzeniem.

### Odinstalowanie programu WSUS 3.0 i pozostawienie plików dziennika może spowodować, że te pliki będą miały nieprawidłowe uprawnienia po ponownym zainstalowaniu programu

W czasie odinstalowywania programu WSUS 3.0 z dodatkiem SP2 można zachować pliki dziennika instalacji. Po ponownym zainstalowaniu programu WSUS 3.0 z dodatkiem SP2 stare pliki dziennika mogą utracić przypisane do nich uprawnienia (zwykle są to uprawnienia tylko dla grupy administratorów programu WSUS). Zaleca się sprawdzenie uprawnień dla tych plików dziennika po zakończeniu instalacji.

### Jeśli istnieją aktualizacje ze stanem „Nie dotyczy” związane z klientami programu WSUS 2.0, aktualizacje te będą przez krótki czas wyświetlane ze stanem „Nieznany” po uaktualnieniu do programu WSUS 3.0 z dodatkiem SP2

Jeśli istniejący serwer programu WSUS 2.0 ma klientów z aktualizacjami w stanie **Nie dotyczy**, dla tych aktualizacji może być przez krótki czas wyświetlany stan **Nieznany** po przeprowadzeniu uaktualnienia do programu WSUS 3.0 z dodatkiem SP2. Gdy klient przeprowadzi kolejne skanowanie, zostanie przywrócony stan aktualizacji **Nie dotyczy**.

Instalowanie programu WSUS 3.0 z dodatkiem SP2
----------------------------------------------

Przewodnik krok po kroku dotyczący instalowania programu WSUS dostępny pod adresem [http://go.microsoft.com/fwlink/?LinkId=139836](http://go.microsoft.com/fwlink/?linkid=139836) (strona może zostać wyświetlona w języku angielskim) zawiera instrukcje dotyczące instalowania programu WSUS 3.0 z dodatkiem SP2 przy użyciu Menedżera serwera systemu Windows lub programu WSUSSetup.exe.

Aby uzyskać pełne informacje na temat instalowania programu WSUS i korzystania z niego, zobacz:

Przewodnik dotyczący wdrażania programu WSUS: [http://go.microsoft.com/fwlink/?LinkId=139832](http://go.microsoft.com/fwlink/?linkid=139832) (strona może zostać wyświetlona w języku angielskim).

Przewodnik obsługi programu WSUS: [http://go.microsoft.com/fwlink/?LinkId=139838](http://go.microsoft.com/fwlink/?linkid=139838) (strona może zostać wyświetlona w języku angielskim).

Parametry wiersza polecenia dotyczące instalacji nienadzorowanych programu WSUS 3.0 SP2
---------------------------------------------------------------------------------------

Dostępny z poziomu wiersza polecenia Instalator programu WSUS umożliwia przeprowadzanie instalacji nienadzorowanych programu WSUS 3.0 z dodatkiem SP2. W tabeli poniżej podano parametry wiersza polecenia Instalatora programu WSUS 3.0 z dodatkiem SP2.

###  

 
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
<td style="border:1px solid black;">Umożliwia przeprowadzenie instalacji dyskretnej.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>/u</strong></td>
<td style="border:1px solid black;">Umożliwia odinstalowanie programu.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>/p</strong></td>
<td style="border:1px solid black;">Umożliwia sprawdzenie wymagań wstępnych. Służy do przeprowadzania inspekcji systemu i zgłaszania wszelkich wymagań wstępnych, które nie są spełnione.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>/?, /h</strong></td>
<td style="border:1px solid black;">Umożliwia wyświetlenie parametrów wiersza polecenia i ich opisów.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>/g</strong></td>
<td style="border:1px solid black;">Umożliwia uaktualnienie poprzedniej wersji programu WSUS. Uaktualnienia programu SUS 1.0 nie są obsługiwane. W przypadku użycia tej opcji jedynym poprawnym parametrem jest /q (instalacja dyskretna). Razem z tą opcją można użyć jedynie właściwości DEFAULT_WEBSITE.</td>
</tr>
</tbody>
</table>
  
W tabeli poniżej podano właściwości wiersza polecenia dla programu WSUS 3.0 z dodatkiem SP2.
  
###  

 
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
<td style="border:1px solid black;">Ścieżka do katalogu zawartości. Wartość domyślna to <em>dysk_instalacji_programu_WSUS\WSUS\WSUSContent</em>, gdzie <em>dysk_instalacji_programu_WSUS</em> to dysk lokalny, na którym jest dostępna największa ilość wolnego miejsca.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">WYUKON_DATA_DIR</td>
<td style="border:1px solid black;">Ścieżka do katalogu danych wewnętrznej bazy danych systemu Windows.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">SQLINSTANCE_NAME</td>
<td style="border:1px solid black;">Nazwa powinna występować w formacie <em>nazwa_serwera</em>\<em>nazwa_wystąpienia_SQL</em>. Jeżeli wystąpienie bazy danych znajduje się na komputerze lokalnym, należy użyć zmiennej środowiskowej %COMPUTERNAME%. W przypadku braku istniejącego wystąpienia nazwą domyślną jest %COMPUTERNAME%\WSUS.</td>
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
<td style="border:1px solid black;">0=instalacja serwera WSUS, 1=instalacja wyłącznie konsoli</td>
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
<td style="border:1px solid black;">0=zachowanie plików dziennika, 1=usunięcie plików dziennika (opcja używana razem z przełącznikiem instalacji /u)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CREATE_DATABASE</td>
<td style="border:1px solid black;">0=użycie bieżącej bazy danych, 1=utworzenie bazy danych</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PROGRESS_WINDOW_HANDLE</td>
<td style="border:1px solid black;">Dojście do okna służące do zwracania komunikatów postępu Instalatora Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">MU_ROLLUP</td>
<td style="border:1px solid black;">1=przystąpienie do Programu poprawy jakości rozszerzenia Microsoft Update, 0=rezygnacja z przystąpienia do Programu poprawy jakości rozszerzenia Microsoft Update</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">FRONTEND_SETUP</td>
<td style="border:1px solid black;">1=nie zapisuj lokalizacji zawartości w bazie danych, 0=zapisz lokalizację zawartości w bazie danych (dla technologii NLB)</td>
</tr>
</tbody>
</table>
  
### Przykładowe użycie
  
```  
WSUSSetup.exe /q DEFAULT\_WEBSITE=0 (instalacja w trybie cichym przy użyciu portu 8530) WSUSSetup.exe /q /u (dezinstalacja programu WSUS)  
```
 
<table style="border:1px solid black;">
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" ><img src="images/Dd939886.Important(WS.10).gif" />Ważne</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Jeśli program WSUS 3.0 SP2 jest instalowany w trybie cichym (/q), a komputer nie spełnia wszystkich wymagań wstępnych dotyczących zainstalowanych elementów, program instalacyjny wygeneruje plik o nazwie WSUSPreReqCheck.xml i zapisze go w katalogu %TEMP%.
</td>
</tr>
</tbody>
</table>
 

<span id="BKMK_KnownIssues"></span>
Znane problemy
--------------

-   Po pomyślnym ukończeniu pracy Kreatora instalacji programu WSUS użytkownik jest proszony o kliknięcie przycisku **Zakończ**. Sporadycznie pojawia się okno dialogowe z następującym komunikatem o błędzie: „**Wystąpił błąd podczas komunikowania się z serwerem. Praca kreatora musi zostać zakończona. Kreatora konfiguracji serwera WSUS można uruchomić na stronie Opcje w konsoli WSUS 3.0**”. Aby upewnić się, że wybrane opcje instalacji zostały zapisane, należy otworzyć stronę **Opcje** w konsoli administracyjnej programu WSUS i sprawdzić ustawienia w każdej z sekcji.
-   **Zlokalizowane wersje klienta usługi Windows Update Agent (WUA) zostaną wydane po wydaniu programu WSUS 3.0 z dodatkiem SP2**. Jest to spowodowane zależnością od harmonogramu lokalizowania systemu Windows 7. W okresie od wydania programu WSUS 3.0 z dodatkiem SP2 do momentu wydania zlokalizowanej wersji klienta usługi WUA klient ten będzie obsługiwać tylko pięć języków: angielski, francuski, hiszpański, japoński i niemiecki.
-   **Nowe raporty dotyczące aktualizacji i stanu komputerów wprowadzone w tej wersji z dodatkiem SP2 nie działają w środowiskach, w których serwery podrzędne programu WSUS 3.0 z dodatkiem SP1 są zarządzane z serwera programu WSUS 3.0 z dodatkiem SP2**. Jeśli nowe raporty zostają uruchomione na serwerze programu WSUS 3.0 z dodatkiem SP1, pojawia się następujący komunikat o błędzie: „Wystąpił błąd podczas generowania raportu. Spróbuj uruchomić raport ponownie lub skontaktuj się z administratorem sieci, jeśli problem będzie nadal występował”. Ponowne uruchomienie raportu nie rozwiąże problemu. Ten problem nie dotyczy sieci. Nowe raporty są zależne od funkcjonalności interfejsu API, który nie jest dostępny w programie WSUS 3.0 z dodatkiem SP1, jednak konsola administracyjna programu WSUS 3.0 z dodatkiem SP2 nie blokuje nowych raportów podczas zarządzania serwerem programu WSUS 3.0 z dodatkiem SP1.
-   **Próba przeprowadzenia uaktualnienia do programu WSUS 3.0 z dodatkiem SP2 kończy się niepowodzeniem, gdy protokół SSL jest skonfigurowany bez nazwy certyfikatu**. W przypadku konfigurowania protokołu SSL jest wymagana nazwa certyfikatu.
-   **Program WSUS 3.0 z dodatkiem SP2, w którym została uruchomiona Wewnętrzna baza danych systemu Windows zainstalowana w systemie Windows Server 2008, uniemożliwia dokonanie uaktualnienia do systemu Windows Server 2008 R2**. Zanim będzie możliwe kontynuowanie uaktualniania do systemu Windows Server 2008 R2, pojawi się komunikat o błędzie raportu zgodności z informacją, że Wewnętrzna baza danych systemu Windows musi zostać wyłączona. Wewnętrzna baza danych systemu Windows musi zostać uaktualniona, aby można było kontynuować uaktualnianie do systemu Windows Server 2008 R2. Aby uzyskać więcej informacji o uaktualnianiu składnika Wewnętrzna baza danych systemu Windows oraz odpowiednie instrukcje, zobacz artykuł dotyczący [uzyskiwania najnowszego dodatku Service Pack dla wewnętrznej bazy danych systemu Windows](http://go.microsoft.com/fwlink/?linkid=162104) (http://go.microsoft.com/fwlink/?LinkId=162104) (strona może zostać wyświetlona w języku angielskim).

Informacje o prawach autorskich
-------------------------------

Informacje podane w tym dokumencie, w tym adresy URL i inne odwołania do internetowych witryn sieci Web, mogą zostać zmienione bez powiadomienia. Jeśli nie określono inaczej, firmy, organizacje, produkty, nazwy domen, adresy e-mail, logo, osoby, miejsca i zdarzenia przedstawione w przykładach są fikcyjne. Żaden związek z jakąkolwiek rzeczywistą firmą, organizacją, produktem, nazwą domeny, adresem e-mail, logo, osobą, miejscem lub zdarzeniem nie był zamierzony ani nie należy go zakładać. Obowiązek przestrzegania wszystkich stosownych praw autorskich spoczywa na użytkowniku. Niezależnie od praw wchodzących w zakres praw autorskich, żadnej części niniejszego dokumentu nie wolno w żadnej formie powielać, przechowywać, wprowadzać do żadnego systemu umożliwiającego odtworzenie ani przekazywać za pomocą jakichkolwiek metod (urządzeń elektronicznych, mechanicznych, fotokopii, nagrania itp.) i w jakimkolwiek celu — z wyjątkiem przypadków, w których uzyskano na to jawną, pisemną zgodę firmy Microsoft Corporation.

Firma Microsoft może być właścicielem patentów, zgłoszeń patentowych, znaków towarowych, praw autorskich lub innych praw własności intelektualnej dotyczących przedmiotu tego dokumentu. Otrzymanie tego dokumentu nie oznacza udzielenia licencji na te patenty, znaki towarowe, prawa autorskie ani inne prawa związane z własnością intelektualną, z wyjątkiem przypadków wyraźnie określonych w pisemnych umowach licencyjnych firmy Microsoft.

© 2009 Microsoft Corporation. Wszelkie prawa zastrzeżone.

Microsoft, Active Directory, ActiveX, Authenticode, Excel, InfoPath, Internet Explorer, MSDN, Outlook, Visual Studio, Win32, Windows, Windows Server i Windows Vista są znakami towarowymi grupy firm Microsoft.

Wszystkie inne znaki towarowe są własnością ich prawnych właścicieli.
