---
TOCTitle: Usługa certyfikacji wstępnej programu RMS
Title: Usługa certyfikacji wstępnej programu RMS
ms:assetid: '09957294-167f-4f98-88e9-ae90fbeb26c1'
ms:contentKeyID: 18123166
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720191(v=WS.10)'
---

Usługa certyfikacji wstępnej programu RMS
=========================================

Usługa certyfikacji wstępnej działa tylko na klastrze głównym programu RMS. Ta usługa umożliwia serwerowi żądanie certyfikatu konta praw w imieniu użytkownika i może być używana do tworzenia niestandardowych aplikacji. Przykładowymi programami, które korzystają z tej usługi są Microsoft Exchange Server 2007 i Microsoft Office SharePoint Server 2007.

Plik aplikacji usługi certyfikacji wstępnej, Precertification.asmx, znajduje się w katalogu wirtualnym Certification w programie IIS.

Aby uzyskać więcej informacji dotyczących tworzenia niestandardowych aplikacji, zobacz temat Dokumentacja technologii programu Usługi zarządzania prawami dostępu w systemie Windows w witrynie MSDN Library [http://go.microsoft.com/fwlink/?LinkId=32972](http://go.microsoft.com/fwlink/?linkid=32972).

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
