---
TOCTitle: Usługa lokalizatora usług programu RMS
Title: Usługa lokalizatora usług programu RMS
ms:assetid: '6f410cc9-5d5b-4df3-bf4f-7b13811eb52f'
ms:contentKeyID: 18123311
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747548(v=WS.10)'
---

Usługa lokalizatora usług programu RMS
======================================

Usługa lokalizatora usług działa na klastrze głównym oraz klastrach licencji programu RMS. Usługa lokalizatora usług dostarcza adres URL połączenia usługi dla klastra do usługi Active Directory, tak aby mógł być odnajdowany przez klientów obsługujących technologię RMS.

Plik aplikacji usługi lokalizatora usług, ServiceLocator.asmx, znajduje się w katalogach wirtualnych Certification i Licensing w programie IIS.

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
