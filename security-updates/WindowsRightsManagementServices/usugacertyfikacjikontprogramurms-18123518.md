---
TOCTitle: Usługa certyfikacji kont programu RMS
Title: Usługa certyfikacji kont programu RMS
ms:assetid: 'fb294969-850e-44b4-8f6a-ca5d5cec1bf1'
ms:contentKeyID: 18123518
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747802(v=WS.10)'
---

Usługa certyfikacji kont programu RMS
=====================================

Usługa certyfikacji kont działa tylko na klastrze głównym. Usługa certyfikacji kont tworzy certyfikaty kont praw, które kojarzą konta użytkowników z określonymi komputerami. Certyfikat konta praw umożliwia użytkownikowi publikowanie lub używanie zawartości chronionej na podstawie praw podczas pracy na określonym komputerze.

Plik aplikacji usługi certyfikacji kont, Certification.asmx, znajduje się w katalogu wirtualnym Certification w programie IIS.

W poniższej tabeli przedstawiono domyślną listę kontroli dostępu w ramach tej usługi:

###  

 
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
