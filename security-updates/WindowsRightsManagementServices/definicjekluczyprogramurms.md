---
TOCTitle: Definicje kluczy programu RMS
Title: Definicje kluczy programu RMS
ms:assetid: 'b052305c-1db7-434a-bad9-26d704156776'
ms:contentKeyID: 18123427
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747729(v=WS.10)'
---

Definicje kluczy programu RMS
=============================

W poniższej tabeli przedstawiono klucze stosowane w systemie RMS.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Klucz</th>
<th style="border:1px solid black;" >Użycie</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Klucze serwera</td>
<td style="border:1px solid black;"><strong>Klucz publiczny</strong>
Szyfruje klucz zawartości w licencji publikacji, aby tylko serwer programu RMS mógł pobrać klucz zawartości i wystawić licencję użytkowania dla tej licencji publikacji.
<strong>Klucz prywatny</strong>
Podpisuje wszystkie certyfikaty i licencje wystawione przez ten serwer.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Klucze komputera</td>
<td style="border:1px solid black;"><strong>Klucz publiczny</strong>
Szyfruje klucz prywatny certyfikatu konta praw.
<strong>Klucz prywatny</strong>
Deszyfruje certyfikat konta praw.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Klucze licencjodawcy klienta</td>
<td style="border:1px solid black;"><strong>Klucz publiczny</strong>
Szyfruje symetryczny klucz zawartości w wystawianej licencji publikacji.
<strong>Klucz prywatny</strong>
Podpisuje licencje publikacji wystawiane lokalnie, gdy użytkownik nie jest podłączony do sieci.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Klucze użytkownika</td>
<td style="border:1px solid black;"><strong>Klucz publiczny</strong>
Szyfruje klucz zawartości w licencji użytkowania, tak aby dzięki tej licencji tylko określony użytkownik mógł korzystać z zawartości chronionej technologią RMS.
<strong>Klucz prywatny</strong>
Umożliwia użytkownikowi korzystanie z zawartości chronionej technologią RMS.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Klucze zawartości</td>
<td style="border:1px solid black;">Szyfruje zawartość chronioną technologią RMS, gdy autor ją publikuje.</td>
</tr>
</tbody>
</table>
