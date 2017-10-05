---
TOCTitle: Usługa administrowania programem RMS
Title: Usługa administrowania programem RMS
ms:assetid: '4bd3e142-f0f6-40e9-a160-deab28ce5b88'
ms:contentKeyID: 18123264
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747560(v=WS.10)'
---

Usługa administrowania programem RMS
====================================

Usługa administracji działa na klastrze głównym programu RMS, a także na dowolnym klastrze licencji. Usługa administracji obsługuje administracyjną witrynę sieci Web oraz umożliwia zarządzanie programem RMS.

Plik aplikacji usługi administracji, Default.aspx, znajduje się w katalogu wirtualnym Admin o ścieżce *witryna sieci Web programu RMS*\\\_wmcs\\Admin. Przy czym ciąg *witryna\_sieci\_Web\_programu\_RMS* należy zastąpić nazwą witryny sieci Web, na której został zastrzeżony program RMS.

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
</tbody>
</table>
