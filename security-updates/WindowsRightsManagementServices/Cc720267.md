---
TOCTitle: 'Usługa publikacji programu RMS.'
Title: 'Usługa publikacji programu RMS.'
ms:assetid: '4c0c8fe3-695c-4b2c-a2d3-cab9b52bbb25'
ms:contentKeyID: 18123253
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720267(v=WS.10)'
---

Usługa publikacji programu RMS.
===============================

Usługa publikacji, która wystawia licencje publikowania, działa klastrze głównym programu RMS, a także na dowolnym klastrze licencji. Licencje publikacji definiują zasady, według których są dostarczane licencje.

Plik aplikacji usługi publikacji, Publish.asmx, znajduje się w katalogu wirtualnym Licensing w programie IIS.

W poniższej tabeli przedstawiono domyślną listę kontroli dostępu w ramach tej usługi:


<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Użytkownik lub grupa</th>
<th style="border:1px solid black;" >Uprawnienie domyślne</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Administratorzy</td>
<td style="border:1px solid black;">Pełna kontrola</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Grupa RMS Service Group</td>
<td style="border:1px solid black;">Odczyt i Wykonywanie</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">SYSTEM</td>
<td style="border:1px solid black;">Pełna kontrola</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Użytkownicy</td>
<td style="border:1px solid black;">Odczyt i Wykonywanie</td>
</tr>
</tbody>
</table>
