---
TOCTitle: 'Usługa licencjonowania programu RMS.'
Title: 'Usługa licencjonowania programu RMS.'
ms:assetid: '5cad1baf-0304-4e82-b62d-83a4aac2140b'
ms:contentKeyID: 18123279
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720278(v=WS.10)'
---

Usługa licencjonowania programu RMS.
====================================

Usługa licencjonowania, która wystawia licencje użytkowania, działa klastrze głównym programu RMS, a także na dowolnym klastrze licencji. Licencje użytkowania umożliwiają użytkownikowi korzystanie z zawartości chronionej na podstawie praw.

Plik aplikacji usługi licencjonowania, License.asmx, znajduje się w katalogu wirtualnym Licensing w programie IIS.

> [!note]  
> Można rozmieścić osobny klaster licencji w celu przejęcia żądań licencji kierowanych z klastra głównego. Można również rozmieścić osobny serwer lub klaster licencji dla oddziału, na przykład aby dać oddziałowi możliwość ustanowienia własnych zasad praw dostępu. Aby uzyskać więcej informacji dotyczących tych zagadnień, zobacz „Identyfikowanie podstawowych składników” w części dotyczącej planowania rozmieszczenia programu RMS w tym zestawie dokumentacji. 

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
