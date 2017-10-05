---
TOCTitle: Migrowanie rozmieszczenia pilotażowego programu RMS do środowiska produkcyjnego
Title: Migrowanie rozmieszczenia pilotażowego programu RMS do środowiska produkcyjnego
ms:assetid: 'ea151946-22fb-4cba-a3ef-fd7a4bf0d292'
ms:contentKeyID: 18123498
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747789(v=WS.10)'
---

Migrowanie rozmieszczenia pilotażowego programu RMS do środowiska produkcyjnego
===============================================================================

Wiele organizacji decyduje się na rozmieszczenie programu RMS w trybie pilotażowym przed zaimplementowaniem technologii w całej swojej strukturze. Program pilotażowy zazwyczaj obejmuje ograniczoną liczbę użytkowników, a serwer może być obsługiwany lokalnie przez przydzielonego administratora, a nie stanowi części centrum przetwarzania danych obsługiwanego przez grupę IT. Jeśli organizacja implementuje program RMS w centrum przetwarzania danych dla wszystkich klientów po zakończeniu programu pilotażowego, nowe serwery programu RMS są rozmieszczane na potrzeby obsługi większej liczby możliwych użytkowników.

Jednak zawartość chroniona technologią RMS jest powiązana z serwerem programu RMS, za pomocą którego została utworzona. Dlatego jeśli serwer zostanie usunięty lub zastąpiony, należy wykonać odpowiednie czynności mające na celu odszyfrowanie i licencjonowanie zawartości zaszyfrowanej za pomocą pilotażowych serwerów programu RMS, korzystając z produkcyjnych serwerów programu RMS.

Jeśli program RMS jest rozmieszczany w ramach programu pilotażowego i serwer programu RMS ma być przeniesiony do środowiska produkcyjnego organizacji, ale ma być także zachowana integralność zawartości chronionej za pomocą pilotażowego serwera programu RMS, należy utworzyć plan migracji, który umożliwi płynną zmianę i wycofanie do programu pilotażowego, jeśli będzie konieczne przywrócenie danych.

Poniżej przedstawiono przykładowe elementy, które powinien zawierać plan migracji. Każde rozmieszczenie może mieć inne wymagania.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Serwer</th>
<th>Krok</th>
<th>Uwagi</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Program pilotażowy</td>
<td style="border:1px solid black;">Tworzenie kopii zapasowej bazy danych konfiguracji programu RMS.</td>
<td style="border:1px solid black;">Dzięki temu w razie konieczności można przywrócić serwer pilotażowy.
Baza danych konfiguracji zawiera klucz prywatny programu RMS.
Należy znać hasło klucza prywatnego.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Program pilotażowy</td>
<td style="border:1px solid black;">Jeśli do zabezpieczenia klucza prywatnego programu RMS użyto sprzętowego modułu zabezpieczeń, należy utworzyć kopię zapasową konfiguracji tego modułu zgodnie z zaleceniami jego producenta.</td>
<td style="border:1px solid black;">Sprzętowy moduł zabezpieczeń jest przywracany na nowym serwerze.
Sprawdź, czy masz wszystkie składniki niezbędne do instalacji i konfiguracji sprzętowego modułu zabezpieczeń.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Program pilotażowy</td>
<td style="border:1px solid black;">Eksportowanie pliku zaufanej domeny publikacji.</td>
<td style="border:1px solid black;">W ten sposób inny serwer programu RMS może odszyfrować licencje publikacji utworzone przez ten serwer i wystawiać licencje użytkowania zawartości chronionej.
Zaufana domena publikacji obejmuje certyfikat licencjodawcy serwera, klucz prywatny programu RMS i wszystkie szablony zasad praw dostępu utworzone przez ten serwer.
Plik zaufanej domeny publikacji jest plikiem XML zaszyfrowanym za pomocą silnego hasła zdefiniowanego podczas tworzenia tego pliku. Hasło to jest także niezbędne do zaimportowania zaufanego pliku domeny publikacji.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Program pilotażowy</td>
<td style="border:1px solid black;">Eksportowanie zaufanych domen użytkowników.</td>
<td style="border:1px solid black;">W ten sposób inny serwer programu RMS może udzielać licencji użytkowania użytkownikom, których certyfikaty kont praw dostępu zostały udzielone przez pilotażowy serwer programu RMS.
Zaufana domena użytkownika jest tworzona przez zaimportowanie certyfikatu licencjodawcy tego serwera do innego serwera programu RMS.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Środowisko produkcyjne</td>
<td style="border:1px solid black;">Przygotuj nowy serwer, który będzie serwerem głównej certyfikacji.</td>
<td style="border:1px solid black;">Sprawdź ,czy ma on dostęp do serwera bazy danych oraz czy są zainstalowane usługi IIS i usługa kolejkowania wiadomości.
Jeśli to możliwe, używaj tej samej nazwy serwera.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Środowisko produkcyjne</td>
<td style="border:1px solid black;">Jeśli używasz sprzętowego modułu zabezpieczeń, zainstaluj sprzętowy moduł zabezpieczeń i przywróć jego konfigurację z kopii zapasowej utworzonej na serwerze pilotażowym.</td>
<td style="border:1px solid black;">Tworzy poświadczenia wymagane do odszyfrowania klucza prywatnego programu RMS.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Środowisko produkcyjne</td>
<td style="border:1px solid black;">Zainstaluj program RMS.</td>
<td style="border:1px solid black;">Program RMS sprawdzi, czy zainstalowano wszystkie wymagane usługi i czy zostały one prawidłowo skonfigurowane.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Środowisko produkcyjne</td>
<td style="border:1px solid black;">Rozmieszczenie programu RMS za pomocą nowego klucza prywatnego. Jeśli używane jest rejestrowanie w trybie online, serwer zostanie zarejestrowany podczas rozmieszczania za pomocą Internetu, aby połączyć się z usługą rejestracji firmy Microsoft. Jeśli połączenie internetowe z tego serwera nie jest dostępne, należy użyć funkcji rejestrowania w trybie offline.</td>
<td style="border:1px solid black;">Jeśli nazwa tego serwera jest inna niż nazwa serwera pilotażowego, można zmodyfikować adres URL klastra, tak by był on taki sam jak adres URL serwera pilotażowego.
Jeśli adres ten nie zostanie zmodyfikowany, należy skonfigurować adres URL przekierowania z adresu URL poprzedniego klastra do nowego adresu URL klastra, aby umożliwić użytkownikom istniejącej zawartości uzyskanie licencji użytkowania.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Środowisko produkcyjne</td>
<td style="border:1px solid black;">Jeśli używana jest funkcja rejestrowania w trybie offline, należy wykonać ręczną rejestrację nowego serwera RMS. Aby uzyskać więcej informacji, zobacz „Ręczne rejestrowanie serwera głównej certyfikacji” w części „Obsługa serwerów programu RMS” w tym zestawie dokumentacji.</td>
<td style="border:1px solid black;">Serwera programu RMS nie można używać, dopóki nie zostanie on zarejestrowany.
Dopóki serwer nie zostanie zarejestrowany, nie można także uzyskać dostępu do stron administracyjnych programu RMS.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Środowisko produkcyjne</td>
<td style="border:1px solid black;">Importowanie pliku zaufanej domeny publikacji wyeksportowanej w punkcie 3.</td>
<td style="border:1px solid black;">Aby pomyślnie zaimportować plik, konto usługi programu RMS musi mieć uprawnienia do odczytu do lokalizacji, w której jest przechowywany plik.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Środowisko produkcyjne</td>
<td style="border:1px solid black;">Ponowne podpisanie każdego szablonu zaimportowanego do zaufanej domeny publikacji.</td>
<td style="border:1px solid black;">Szablony są podpisywane za pomocą klucza prywatnego serwera. Ponieważ ten serwer ma nowy klucz prywatny, szablony muszą zostać ponownie podpisane, aby były ważne. Aby uzyskać więcej informacji, zobacz „Ponowne podpisywanie szablonu zasad praw” w części „Obsługa serwerów programu RMS” w tym zestawie dokumentacji.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Środowisko produkcyjne</td>
<td style="border:1px solid black;">Ponowna dystrybucja szablonów na komputerach klienckich, które były objęte programem pilotażowym.</td>
<td style="border:1px solid black;">Należy usunąć stare szablony. Trzeba je zastąpić szablonami podpisanymi przez ten serwer.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Środowisko produkcyjne</td>
<td style="border:1px solid black;">Importowanie pliku zaufanej domeny publikacji wyeksportowanej w punkcie 4.</td>
<td style="border:1px solid black;">Umożliwia korzystanie ze starych certyfikatów licencjodawcy klienta i certyfikatów RAC.
Jeśli konta użytkowników są przenoszone między lasami w ramach tej migracji, należy pamiętać, że konta muszą mieć zgodne serwery SMTP proxy.</td>
</tr>
</tbody>
</table>
 

Po skonfigurowaniu serwera produkcyjnego należy upewnić się, że użytkownicy pilotażowi mogą nadal tworzyć i czytać wcześniej zabezpieczone wiadomości pocztowe. Możesz później dodać odpowiednią liczbę serwerów programu RMS do klastra, aby obsłużyć wszystkich użytkowników w organizacji
