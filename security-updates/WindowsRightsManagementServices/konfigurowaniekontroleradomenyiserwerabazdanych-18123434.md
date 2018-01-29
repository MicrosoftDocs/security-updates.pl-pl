---
TOCTitle: Konfigurowanie kontrolera domeny i serwera baz danych
Title: Konfigurowanie kontrolera domeny i serwera baz danych
ms:assetid: 'd20f8305-9f9e-4760-bfbf-82824db60d1f'
ms:contentKeyID: 18123434
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747681(v=WS.10)'
---

Konfigurowanie kontrolera domeny i serwera baz danych
=====================================================

Przed zainstalowaniem serwera certyfikacji lub serwera licencji należy upewnić się, że zaimplementowano odpowiednią obsługę domen i baz danych za pomocą usługi Active Directory i serwera bazy danych, np. SQL Server 2000 z dodatkiem Service Pack 3 (SP3) lub Microsoft® SQL Server 2000 Desktop Engine (MSDE 2000) w wersji A. Środowisko produkcyjne może już zawierać wymagane składniki, jednak nie zaleca się wykorzystywania środowiska produkcyjnego do testowania.

Poniższe procedury dotyczą konfiguracji kontrolera domeny i serwera bazy danych na jednym komputerze w odizolowanej sieci do celów testowania środowiska serwera.

> [!note]  
> W tym przykładzie serwer bazy danych działa na kontrolerze domeny. W środowisku produkcyjnym zwykle nie zaleca się obsługi dodatkowych składników na kontrolerze domeny. W tym przykładzie usługa Active Directory i serwer bazy danych są zainstalowane na tym samym komputerze, aby umożliwić instalację pełnej infrastruktury na minimalnej liczbie komputerów. 

Jeśli jako serwer bazy danych wybrano program MSDE 2000, należy pamiętać, że nie obsługuje on żadnych interfejsów sieciowych oraz że warunki jego użytkowania stanowią, że nie można używać narzędzi klienckich programu SQL Server do obsługi bazy danych programu MSDE. To ograniczenie uniemożliwi przeglądanie informacji rejestrowania lub zmienianie danych przechowywanych w bazie danych konfiguracji. Dlatego zaleca się używanie programu MSDE 2000 tylko do obsługi baz danych programu RMS w środowiskach testowych.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Składnik infrastruktury</th>
<th style="border:1px solid black;" >Kroki potrzebne do skonfigurowania kontrolera domeny i serwera bazy danych</th>
<th style="border:1px solid black;" >Uwagi dotyczące rozmieszczania w środowisku produkcyjnym</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">System operacyjny</td>
<td style="border:1px solid black;">Zainstaluj system operacyjny Windows 2000 Server z dodatkiem SP3 lub nowszy albo system Windows Server 2003 na komputerze spełniającym wymagania sprzętowe programu RMS, który nie jest jeszcze podłączony do sieci. Użyj systemu plików NTFS na partycjach dysku.</td>
<td style="border:1px solid black;">Zawsze zaleca się instalowanie najnowszych dodatków Service Pack oraz aktualizacji. Należy używać partycji sformatowanych z użyciem systemu plików NTFS.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Połączenie sieciowe</td>
<td style="border:1px solid black;">Doprowadź połączenie sieciowe umożliwiające dostęp do Internetu, ale odizolowane od środowiska produkcyjnego.</td>
<td style="border:1px solid black;">Połączenie internetowe powinno dysponować odpowiednią zaporą.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Adres IP</td>
<td style="border:1px solid black;">Przypisz temu komputerowi statyczny adres IP.</td>
<td style="border:1px solid black;">Należy zawsze używać statycznych adresów IP dla serwerów.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">usługę Active Directory.</td>
<td style="border:1px solid black;">Zaloguj się jako administrator lokalny.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Kliknij przycisk <strong>Start</strong>, kliknij polecenie <strong>Uruchom</strong>, wpisz polecenie <code>dcpromo</code> w oknie <strong>Otwórz</strong>, a następnie kliknij przycisk <strong>OK</strong>.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Po uruchomieniu Kreatora konfiguracji usługi Active Directory wykonaj czynności potrzebne do utworzenia nowej domeny w nowym lesie, akceptując opcje domyślne oprócz poniższych:
Określ nazwę domeny, na przykład contoso.com.
Pozwól kreatorowi skonfigurować usługę DNS na komputerze.
Zaznacz pole wyboru <strong>Uprawnienia zgodne tylko z serwerami systemu Windows 2000</strong>, jeśli na wszystkich kontrolerach domeny jest zainstalowany system Windows 2000 lub nowszy.
Podaj silne hasło administratora lokalnego.</td>
<td style="border:1px solid black;">Jeśli do zaimplementowania programu RMS wymagane są nowe domeny, należy je skonfigurować w usłudze Active Directory.
Należy zawsze używać silnych haseł dla wszystkich kont.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Ponownie uruchom komputer po wyświetleniu odpowiedniego monitu.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Zweryfikuj poziom funkcjonalny, otwierając przystawkę <strong>Użytkownicy i komputery usługi Active Directory</strong>, a następnie klikając prawym przyciskiem myszy nazwę domeny i klikając polecenie <strong>Właściwości</strong>. Sprawdź ustawienie w polu <strong>Tryb działania domeny</strong>. Jeśli nie ma kontrolerów domeny starszych niż kontroler domeny systemu Windows 2000, kliknij polecenie <strong>Zmień tryb</strong> i wybierz opcję <strong>Tryb macierzysty</strong>.
Uwaga: W systemach operacyjnych Windows Server 2003 ustawienie <strong>Tryb działania domeny</strong> zostało zastąpione przez ustawienie <strong>Poziom funkcjonalny domeny</strong>.</td>
<td style="border:1px solid black;">W celu zapewnienia optymalnego bezpieczeństwa i możliwości zarządzania nie należy używać różnych poziomów funkcjonalnych systemu Windows 2000 do obsługi programu RMS.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Konta użytkowników</td>
<td style="border:1px solid black;">Utwórz konto użytkownika domeny, które będzie używane jako konto usługi RMS programu RMS, np. ContosoRMS@contoso.com. Określ silne hasło. Upewnij się, że określono adres e-mail dla użytkownika. Jeśli w usłudze Active Directory nie określono adresu e-mail, użytkownik nie będzie mógł pobierać licencji i certyfikatów z programu RMS.
Uwaga: Jako konta usługi programu RMS nie można użyć konta, za pomocą którego instalowano program RMS.</td>
<td style="border:1px solid black;">Należy utworzyć osobne konto w usłudze Active Directory do użytku jako konto usługi programu RMS. Należy podać adres e-mail. Nie należy przypisywać specjalnych uprawnień dla tego konta.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Program SQL Server 2000</td>
<td style="border:1px solid black;">Zaloguj się do serwera, na którym chcesz zainstalować bazę danych. Jeśli jest to serwer będący kontrolerem domeny, należy zalogować się jako administrator domeny.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Postępuj zgodnie ze wskazówkami wyświetlanymi w programie bazy danych, aby zainstalować oprogramowanie serwera bazy danych.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Zainstaluj serwer bazy danych, pamiętając o najważniejszych wskazówkach, np.:
<ul>
<li>Podaj nazwę konta administratora systemu bazy danych oraz nazwę organizacji, na przykład Contoso.<br />
<br />
</li>
<li>Podaj silne hasło administratora systemu.<br />
<br />
</li>
<li>Korzystaj ze zintegrowanych metod uwierzytelniania systemu Windows.<br />
<br />
</li>
</ul></td>
<td style="border:1px solid black;">Używaj zintegrowanego trybu uwierzytelniania systemu Windows. Jeśli nie można uruchomić serwera bazy danych w tym trybie, skontaktuj się z administratorem domeny i administratorem serwera bazy danych, aby określić zmiany, które mogą być konieczne w konfiguracji programu RMS.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Sprawdź, czy usługa bazy danych została zatrzymana.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Zainstaluj wszystkie aktualizacje oprogramowania serwera bazy danych. Po wyświetleniu monitu o podanie hasła użyj hasła podanego podczas instalacji.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Ponownie uruchom komputer. Sprawdź, czy usługa bazy danych została uruchomiona.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Sprawdź, czy w ustawieniach kont użytkowników w usłudze Active Directory podano prawidłowe atrybuty adresu e-mail.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Upewnij się, że użytkownik domeny, który będzie administrować programem RMS (oraz zastrzegać główne serwery certyfikacji i licencji), posiada wymagane uprawnienia na serwerze bazy danych. Jeśli jako serwer bazy danych używasz programu SQL Server, możesz dodać identyfikator logowania użytkownika, który używa przystawki <strong>SQL Server Enterprise Manager</strong>. W przystawce rozwiń węzeł serwera i grupę serwera, a następnie rozwiń element <strong>Zabezpieczenia</strong>. Kliknij element <strong>Logins</strong> (Nazwy logowania), dodaj nową nazwę logowania dla konta domeny użytkownika, kliknij kartę <strong>Server Roles</strong> (Role serwera), a następnie zaznacz pole wyboru <strong>Server Administrators</strong> (Administratorzy serwera).</td>
<td style="border:1px solid black;">Ważne: Wszyscy użytkownicy i grupy korzystający z programu RMS w celu uzyskania licencji i publikowania zawartości muszą mieć skonfigurowany adres e-mail w swoich kontach w przystawce Użytkownicy i grupy usługi Active Directory konsoli MMC na karcie <strong>Ogólne</strong> w oknie <strong>Właściwości</strong>.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Połączenie internetowe
(opcjonalne)</td>
<td style="border:1px solid black;">Sprawdź, czy przeglądarka i serwer (z uwzględnieniem wszystkich wymaganych konfiguracji serwerów proxy), protokół TCP/IP i pliki LMHOSTS/HOSTS są prawidłowo skonfigurowane na potrzeby dostępu do Internetu. Możesz to sprawdzić, otwierając stronę http://uddi.microsoft.com. Jeśli możesz ją otworzyć, program RMS może połączyć się z usługą rejestracji firmy Microsoft.</td>
<td style="border:1px solid black;">Przejdź do witryny http://uddi.microsoft.com, aby sprawdzić dostęp do Internetu.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Aktualizacje oprogramowania</td>
<td style="border:1px solid black;">Pobierz i zainstaluj najnowsze aktualizacje oprogramowania zainstalowanego na tym komputerze (w tym najnowsze aktualizacje systemu Windows z witryny www.microsoft.com).</td>
<td style="border:1px solid black;">Zawsze należy pobierać i instalować najnowsze aktualizacje.</td>
</tr>
</tbody>
</table>
  
Po wykonaniu powyższych czynności można przystąpić do wstępnej instalacji (w tym instalacji wymaganego oprogramowania) na komputerach, które będą pracowały z programem RMS.
