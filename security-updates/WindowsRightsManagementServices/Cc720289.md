---
TOCTitle: Usługa podrejestrowywania programu RMS
Title: Usługa podrejestrowywania programu RMS
ms:assetid: '6b05e71c-5e7d-467c-9e13-35ac14d3718a'
ms:contentKeyID: 18123303
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720289(v=WS.10)'
---

Usługa podrejestrowywania programu RMS
======================================

Usługa podrejestrowywania działa tylko na klastrze głównym programu RMS. Odpowiada na żądania dotyczące certyfikatów licencjodawcy serwera, zgłaszane przez serwery klastrów licencji podczas zastrzegania.

Plik aplikacji usługi podrejestrowywania, SubEnrollService.asmx, znajduje się w katalogu wirtualnym Certification o ścieżce *witryna\_sieci\_Web\_programu\_RMS*\\\_wmcs\\Certification\\, przy czym *witryna\_sieci\_Web\_programu\_RMS* należy zastąpić nazwą witryny sieci Web, na której został zastrzeżony program RMS.

Domyślnie dostęp do tej usługi jest ograniczony do lokalnego konta SYSTEM. W celu zastrzeżenia oraz zarejestrowania podrzędnego serwera w klastrze licencji należy dodać konto użytkownika dla administratora serwera licencji, z pełnymi uprawnieniami, do listy arbitralnej kontroli dostępu (DACL) usługi SubEnrollService.asmx.

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
<td style="border:1px solid black;">SYSTEM</td>
<td style="border:1px solid black;">Pełna kontrola</td>
</tr>
</tbody>
</table>
