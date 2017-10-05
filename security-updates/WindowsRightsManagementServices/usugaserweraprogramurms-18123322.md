---
TOCTitle: Usługa serwera programu RMS
Title: Usługa serwera programu RMS
ms:assetid: '772d0a89-c9fb-4430-9434-38cd5add1e86'
ms:contentKeyID: 18123322
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747566(v=WS.10)'
---

Usługa serwera programu RMS
===========================

Usługa serwera działa tylko na klastrze głównym programu RMS. Usługa serwera udostępnia żądanie zgłoszone przez klienta korzystającego z publikacji w trybie online, aby pobrać certyfikat licencjodawcy serwera.

Plik aplikacji usługi serwera, Server.asmx, znajduje się w katalogu wirtualnym Certification w programie IIS.

W poniższej tabeli przedstawiono domyślną listę kontroli dostępu w ramach tej usługi:

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Użytkownik lub grupa</th>
<th>Uprawnienie domyślne</th>
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
