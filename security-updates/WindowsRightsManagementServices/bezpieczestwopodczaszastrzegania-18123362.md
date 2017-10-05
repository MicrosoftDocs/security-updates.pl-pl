---
TOCTitle: Bezpieczeństwo podczas zastrzegania
Title: Bezpieczeństwo podczas zastrzegania
ms:assetid: '9f1282c5-5642-4870-a9a4-c3a485f8ff76'
ms:contentKeyID: 18123362
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747616(v=WS.10)'
---

Bezpieczeństwo podczas zastrzegania
===================================

Administracyjnej witryny sieci Web programu RMS można używać w celu zastrzegania zasobów programu RMS w istniejącej witrynie sieci Web. Podczas zastrzegania w tej witrynie sieci Web tworzone są katalogi wirtualne i pule aplikacji, natomiast na serwerze bazy danych tworzone i konfigurowane są bazy danych programu RMS. Dodatkowo serwer może zostać zarejestrowany w usłudze rejestrowania firmy Microsoft podczas procesu zastrzegania, jeśli jest on podłączony do Internetu.

Podczas zastrzegania program RMS używa kont opisanych w poniższej tabeli.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Konto</th>
<th>Funkcja</th>
<th>Uprawnienia</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Konto zalogowanego użytkownika</td>
<td style="border:1px solid black;">Tworzy katalogi wirtualne i pule aplikacji. Usługi IIS wymagają uwierzytelniania systemu Windows, a program RMS personifikuje zalogowanego użytkownika, który musi być zalogowany lokalnie.</td>
<td style="border:1px solid black;">Pełna kontrola (zalogowany użytkownik musi być administratorem lokalnym).</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Konto System</td>
<td style="border:1px solid black;">Tworzy tymczasowy zestaw dla szeregowania.</td>
<td style="border:1px solid black;">Uprawnienia do odczytu i zapisu w folderze tymczasowym systemu Windows, C:\Windows\Temp.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Konto ASPNET</td>
<td style="border:1px solid black;">Tworzy tymczasowy zestaw dla plików *.aspx.</td>
<td style="border:1px solid black;">Dostęp do katalogu tymczasowej pamięci podręcznej zestawu, domyślnie C:\Windows\Microsoft.NET\Framework\v1.1.4322\Temporary ASP.NET Files.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Konto Usługi sieciowe</td>
<td style="border:1px solid black;">Rejestruje punkt połączenia usługi w usłudze Active Directory</td>
<td style="border:1px solid black;"><ul>
<li>Uprawnienia tylko do odczytu w witrynie zastrzegania (zwykle C:\Inetpub\Wwwroot\Provisioning).<br />
<br />
</li>
<li>Uprawnienia do odczytu i zapisu dla klucza rejestru <strong>DRMS</strong>. Uprawnienia są udzielane przez Instalatora programu RMS, który również tworzy następujący klucz rejestru.<br />
<br />
W komputerach z 32-bitową wersją systemu Windows Server 2003<br />
<br />
<code>HKEY_LOCAL_MACHINE\Software\Microsoft\DRMS\1.0</code><br />
<br />
W komputerach z 64-bitową wersją systemu Windows Server 2003<br />
<br />
<code>HKEY_LOCAL_MACHINE\Software\WOW6432Node\Microsoft\DRMS\1.0</code><br />
<br />
</li>
</ul></td>
</tr>
</tbody>
</table>
 

Podczas zastrzegania program RMS wykonuje następujące zadania:

-   Na serwerze bazy danych:
    -   Tworzy bazy danych konfiguracji, usług katalogowych i rejestrowania.
    -   Udziela uprawnień logowania grupie RMS Service Group.
    -   Instaluje procedury przechowywane w bazach danych oraz udziela uprawnień do wykonywania grupie RMS Service Group.
    -   Wykonuje kwerendy w głównej bazie danych.
-   Dodaje grupę RMS Service Group do grupy IIS\_WPG.
-   W katalogu C:\\Inetpub\\Wwwroot\\\_wmcs tworzy hierarchię katalogów wirtualnych, plików oraz puli aplikacji dla usług sieci Web oraz administracyjnej witryny sieci Web programu RMS.
-   Ustawia listy DACL dla katalogów wirtualnych, plików oraz puli aplikacji.
-   Udziela grupie RMS Service Group dostępu do folderu tymczasowego.
-   W przypadku określenia programowej ochrony kluczy, szyfruje klucz prywatny licencjodawcy serwera przed zapisaniem go w bazie danych. Program RMS żąda hasła podczas zastrzegania i uzyskuje dostęp do interfejsu DPAPI na poziomie komputera.
-   Instaluje usługę odbiornika rejestrowania.
-   Tworzy kolejkę wiadomości rejestrowania.
-   W przypadku zastrzegania serwera głównej certyfikacji ustawia punkt połączenia usługi w usłudze Active Directory.
