---
TOCTitle: Przygotowanie do instalacji serwera głównej certyfikacji
Title: Przygotowanie do instalacji serwera głównej certyfikacji
ms:assetid: 'ed51605e-8b17-4155-8d83-f6777f499b7b'
ms:contentKeyID: 18123486
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747726(v=WS.10)'
---

Przygotowanie do instalacji serwera głównej certyfikacji
========================================================

W przykładowej instalacji testowej jest tylko jeden serwer głównej certyfikacji. W razie potrzeby można skonfigurować dodatkowe serwery jako część klastra głównej certyfikacji lub jako osobny klaster serwera licencji. Konfiguracja infrastruktury dla wszystkich tych serwerów jest taka sama, więc należy wykonać procedurę podaną w tym temacie na każdym z serwerów.

Po zainstalowaniu kontrolera domeny i skonfigurowaniu serwerów bazy danych (tak jak to opisano w poprzedniej części) oraz po wykonaniu czynności z poniższej tabeli, użytkownik będzie gotowy do zainstalowania programu RMS.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Składnik infrastruktury</th>
<th>Aby przygotować serwer do instalacji programu RMS</th>
<th>Uwagi dotyczące rozmieszczania w środowisku produkcyjnym</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">System operacyjny</td>
<td style="border:1px solid black;">Zainstaluj system operacyjny Windows Server 2003 na komputerze spełniającym wymagania sprzętowe programu RMS, który nie jest jeszcze podłączony do sieci. Użyj systemu plików NTFS dla partycji.</td>
<td style="border:1px solid black;">Zawsze zaleca się instalowanie najnowszych dodatków Service Pack oraz poprawek. Należy używać partycji sformatowanych z użyciem systemu plików NTFS.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Połączenie internetowe
(opcjonalne)</td>
<td style="border:1px solid black;">Doprowadź połączenie do sieci Ethernet umożliwiającej dostęp do Internetu, ale odizolowanej od środowiska produkcyjnego. Jeśli będzie używana funkcja rejestracji w trybie online w celu zarejestrowania serwera programu RMS w ramach procesu zastrzegania, serwer musi być podłączony do Internetu.</td>
<td style="border:1px solid black;">Jeśli używana jest funkcja rejestracji w trybie online, połączenie internetowe musi być chronione za pomocą odpowiedniej zapory.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Adres IP</td>
<td style="border:1px solid black;">Przypisz temu komputerowi statyczny adres IP.</td>
<td style="border:1px solid black;">Należy zawsze używać statycznych adresów IP dla serwerów.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Dołączenie tego komputera do domeny</td>
<td style="border:1px solid black;">Zaloguj się na komputerze jako administrator lokalny. Kliknij przycisk <strong>Start</strong>, prawym przyciskiem myszy kliknij polecenie <strong>Mój komputer</strong>, kliknij polecenie <strong>Właściwości</strong>, kliknij kartę <strong>Nazwa komputera</strong>, a następnie kliknij przycisk <strong>Zmień</strong>.</td>
<td style="border:1px solid black;">Należy użyć tej samej domeny dla wszystkich serwerów.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Nie zmieniaj nazwy komputera. Kliknij opcję <strong>Domena</strong> i wpisz nazwę domeny, na przykład Contoso.com, a następnie kliknij przycisk <strong>OK</strong>. Podaj poświadczenia użytkownika umożliwiające dołączenie do domeny, kliknij przycisk <strong>OK</strong>, a następnie ponownie uruchom komputer po wyświetleniu odpowiedniego monitu. Po ponownym uruchomieniu komputera i wyświetleniu monitu o podanie poświadczeń logowania, podaj odpowiednią domenę, nazwę użytkownika i hasło.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Użytkownik i konto logowania</td>
<td style="border:1px solid black;">Kliknij prawym przyciskiem myszy polecenie <strong>Mój komputer</strong>, kliknij polecenie <strong>Zarządzaj</strong>, rozwiń element <strong>Użytkownicy i grupy lokalne</strong>, kliknij pozycję <strong>Grupy</strong>, a następnie kliknij dwukrotnie pozycję <strong>Administratorzy</strong>.
Kliknij przycisk <strong>Dodaj</strong>, określ nazwę dodawanego konta użytkownika (na przykład Michael@contoso.com), a następnie kliknij przycisk <strong>OK</strong>. Nadaj kontu użytkownika uprawnienia administratora. Po wyświetleniu monitu o podanie poświadczeń, podaj odpowiednie poświadczenia, na przykład Contoso\Administrator.
Zaloguj się jako użytkownik domeny z uprawnieniami administratora na komputerze.</td>
<td style="border:1px solid black;">Prawa administratora są wymagane do dodawania składników do komputera. Niektórych kroków instalacji nie można wykonać z użyciem konta administratora lokalnego. Na serwerze musi istnieć co najmniej jeden użytkownik domeny będący administratorem. Program SQL Server wymaga także praw administratora systemu do tworzenia nowych baz danych.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Połączenie internetowe
(opcjonalne)</td>
<td style="border:1px solid black;">Otwórz przeglądarkę internetową i przejdź do lokalizacji http://uddi.microsoft.com/, aby sprawdzić, czy masz dostęp do Internetu. Na komputerach z systemem operacyjnym Windows Server 2003 może być konieczna edycja plików Lmhosts i Hosts, tak aby zawierały kontroler domeny.</td>
<td style="border:1px solid black;">Przejdź do witryny http://uddi.microsoft.com, aby sprawdzić dostęp do Internetu.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Aktywacja systemu Windows</td>
<td style="border:1px solid black;">Użyj Kreatora aktywacji w celu aktywacji systemu Windows w firmie Microsoft za pomocą połączenia internetowego. System Windows możesz także aktywować telefonicznie. Więcej informacji na temat aktywacji produktu Windows Server 2003 można znaleźć w Centrum pomocy i obsługi technicznej systemu Windows Server 2003.</td>
<td style="border:1px solid black;">System Windows Server 2003 musi być aktywowany w ciągu 14 dni od instalacji.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Aktualizacje oprogramowania</td>
<td style="border:1px solid black;">Pamiętaj o konieczności instalowania najnowszych aktualizacji oprogramowania zainstalowanego na komputerze.</td>
<td style="border:1px solid black;">Zainstaluj najnowsze aktualizacje oprogramowania.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Konfiguracja programu Internet Explorer</td>
<td style="border:1px solid black;">Program RMS korzysta z interfejsu sieci Web do celów administracyjnych. Niektóre domyślne ustawienia zabezpieczeń mogą uniemożliwiać prawidłowe wyświetlanie stron. Na pewnych stronach w administracyjnej witrynie sieci Web programu RMS niektóre opcje konfiguracji ustawia się w oknach podręcznych.</td>
<td style="border:1px solid black;"> </td>
</tr>
</tbody>
</table>
  
Po wykonaniu wszystkich powyższych czynności na obu serwerach można zainstalować i zastrzec program RMS na serwerach.
