---
TOCTitle: Podsumowanie informacji o certyfikatach i licencjach w programie RMS
Title: Podsumowanie informacji o certyfikatach i licencjach w programie RMS
ms:assetid: '637ccfca-318e-4346-85b5-0945b058fb9c'
ms:contentKeyID: 18123292
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747595(v=WS.10)'
---

Podsumowanie informacji o certyfikatach i licencjach w programie RMS
====================================================================

W poniższej tabeli przedstawiono certyfikaty i licencje używane przez program RMS. Zostały one szczegółowo omówione w pozostałych tematach tej części.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Certyfikat lub licencja</th>
<th style="border:1px solid black;" >Funkcja</th>
<th style="border:1px solid black;" >Zawartość</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Certyfikaty licencjodawcy serwera</td>
<td style="border:1px solid black;">Certyfikat licencjodawcy serwera wystawiony dla serwerów licencji udziela prawa do wystawiania:
<ul>
<li>Licencje publikacji<br />
<br />
</li>
<li>Licencje użytkowania<br />
<br />
</li>
<li>Certyfikaty licencjodawcy klienta<br />
<br />
</li>
<li>Szablony zasad praw dostępu<br />
<br />
</li>
</ul>
Certyfikat licencjodawcy serwera wystawiony dla klastra głównej certyfikacji dodatkowo udziela prawa do wystawiania:
<ul>
<li>Certyfikatów kont praw dla klientów<br />
<br />
</li>
<li>Certyfikatów licencjodawcy serwera dla serwerów licencji<br />
<br />
</li>
</ul></td>
<td style="border:1px solid black;">Certyfikat licencjodawcy serwera wystawiony dla serwera licencji zawiera klucz publiczny serwera licencji.
Certyfikat licencjodawcy serwera wystawiony dla serwera głównej certyfikacji zawiera klucz publiczny serwera głównej certyfikacji.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Certyfikaty licencjodawcy klienta</td>
<td style="border:1px solid black;">Udzielają użytkownikowi prawa do publikowania zawartości chronionej technologią RMS bez konieczności bycia podłączonym do sieci firmowej.</td>
<td style="border:1px solid black;">Zawierają klucz publiczny certyfikatu oraz klucz prywatny certyfikatu, zaszyfrowane kluczem publicznym użytkownika, który zażądał certyfikatu. Zawierają również klucz publiczny serwera, który wystawił certyfikat.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Certyfikaty komputerów RMS</td>
<td style="border:1px solid black;">Identyfikują komputer lub urządzenie zaufane w systemie RMS.</td>
<td style="border:1px solid black;">Zawierają klucz publiczny aktywowanego komputera. Odpowiadający mu klucz prywatny znajduje się w skrytce komputera.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Certyfikaty kont praw</td>
<td style="border:1px solid black;">Identyfikują użytkownika w kontekście danego komputera lub urządzenia.</td>
<td style="border:1px solid black;">Zawierają klucz publiczny użytkownika oraz klucz prywatny użytkownika zaszyfrowany kluczem publicznym aktywowanego komputera.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Licencje publikacji</td>
<td style="border:1px solid black;">Określają prawa dla zawartości chronionej technologią RMS.</td>
<td style="border:1px solid black;">Zawierają symetryczny klucz zawartości do deszyfrowania zawartości zaszyfrowanej kluczem publicznym serwera, który wystawił licencję.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Licencje użytkowania</td>
<td style="border:1px solid black;">Określają prawa dla zawartości chronionej technologią RMS w kontekście danego uwierzytelnionego użytkownika.</td>
<td style="border:1px solid black;">Zawierają symetryczny klucz zawartości do deszyfrowania zawartości zaszyfrowanej kluczem publicznym użytkownika.</td>
</tr>
</tbody>
</table>
