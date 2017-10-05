---
TOCTitle: Planowanie wymagań dotyczących klastrów dla programu RMS
Title: Planowanie wymagań dotyczących klastrów dla programu RMS
ms:assetid: 'ec4023eb-4d39-4551-9789-c8a2d973a55b'
ms:contentKeyID: 18123507
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747792(v=WS.10)'
---

Planowanie wymagań dotyczących klastrów dla programu RMS
========================================================

Jeśli program RMS jest używany w środowisku klastrowym, należy rozważyć sposób spełniania następujących warunków, które mogą istnieć w danej organizacji.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Warunek</th>
<th>Zalecenie</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Duża liczba komputerów, na których używany jest program RMS.</td>
<td style="border:1px solid black;">Używanie usługi Windows Update, skryptu lub jednej z metod rozpowszechniania oprogramowania (np. programu Systems Management Server (SMS) lub zasad grupy) w celu zainstalowania i uaktywnienia klienta programu Usługi zarządzania prawami dostępu w systemie Microsoft Windows.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Duża liczba żądań klientów.</td>
<td style="border:1px solid black;">Używanie serwera równoważenia obciążenia, usługi równoważenia obciążenia sieci (NLB) lub sprzętu równoważącego obciążenie w celu rozpowszechniania żądań w klastrze.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Dwie karty sieciowe, w których używane są wirtualne adresy IP w celu obsługi żądań z sieci ekstranet i intranet.</td>
<td style="border:1px solid black;">Należy upewnić się, że rejestrowanie DNS, wykonywane w celu prezentacji wirtualnego adresu IP w sieci ekstranet, jest także wykonywane w celu prezentacji adresu w sieci intranet.
Jeśli w przypadku sieci intranet nie wykonano rejestracji DNS, wewnętrzne żądania licencji użytkowania nie powiodą się. Jeśli nie można zmodyfikować rekordów zasobów DNS, można zmodyfikować tabelę hostów na każdym serwerze w klastrze w celu zmapowania adresu URL klastra na wirtualny adres IP klastra. Rejestrację DNS należy wykonać przed zastrzeżeniem programu RMS. Jeśli zastrzeżono już program RMS, należy usunąć zastrzeżenie, a następnie powtórzyć proces zastrzegania.</td>
</tr>
</tbody>
</table>
