---
TOCTitle: Odwołanie w szablonach zasad praw dostępu
Title: Odwołanie w szablonach zasad praw dostępu
ms:assetid: '287c5b92-fcb5-4295-9c2b-4e37e643beb2'
ms:contentKeyID: 18123206
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720226(v=WS.10)'
---

Odwołanie w szablonach zasad praw dostępu
=========================================

Warunki odwołania są określone w szablonach zasad praw dostępu. Wartości warunków odwołania wpisane w szablony zasad praw dostępu są przechwytywane w tagu REFRESH języka XrML w licencji publikacji wystawianej dla tego szablonu. Wynikowa licencja użytkowania wystawiona przez serwer będzie również zawierać tag REFRESH.

W poniższej tabeli zawarto listę parametrów znajdujących się w tagu REFRESH.

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Parametr</th>
<th style="border:1px solid black;" >Opis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">ID</td>
<td style="border:1px solid black;">Identyfikator listy odwołania.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ADDRESS</td>
<td style="border:1px solid black;">Adres URL lub ścieżka UNC, gdzie można uzyskać listę odwołania.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PUBLICKEY</td>
<td style="border:1px solid black;">Klucz publiczny jednostki wystawiającej listę odwołania. Ten klucz publiczny odpowiada kluczowi prywatnemu użytemu do podpisania listy odwołania.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">INTERVALTIME</td>
<td style="border:1px solid black;">Maksymalny wiek listy odwołania, podany w dniach. Jeśli lista odwołania przechowywana w pamięci podręcznej jest starsza niż to wskazuje parametr INTERVALTIME, klient programu RMS uzyskuje najnowszą listę odwołania za pomocą adresu URL wskazanego w parametrze ADDRESS. Dzięki temu używana jest aktualna lista odwołania.</td>
</tr>
</tbody>
</table>
  
Aby uzyskać więcej informacji dotyczących tworzenia szablonów zasad praw dostępu, zobacz „Tworzenie i modyfikowanie szablonów zasad praw dostępu” w części „Obsługa serwerów programu RMS” w tym zestawie dokumentacji.
