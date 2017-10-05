---
TOCTitle: Usługa serwera proxy aktywacji programu RMS
Title: Usługa serwera proxy aktywacji programu RMS
ms:assetid: '6b9d33ef-466b-405b-a768-54e5615d6770'
ms:contentKeyID: 18123299
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747608(v=WS.10)'
---

Usługa serwera proxy aktywacji programu RMS
===========================================

Wszystkie żądania aktywacji komputera programu RMS w wersji 1.0 przechodzą przez usługę serwera proxy aktywacji, która działa tylko na klastrze głównym programu RMS. Komputer kliencki musi zostać aktywowany, zanim będzie można go używać wraz z programem RMS w celu publikowania lub używania zawartości chronionej na podstawie praw. Począwszy od programu RMS z dodatkiem Service Pack 1 klient ma funkcję automatycznej aktywacji i nie musi korzystać z serwera proxy aktywacji ani z usługi aktywacji firmy Microsoft w celu wygenerowania skrytki i certyfikatu komputera.

Usługa serwera proxy aktywacji przesyła żądania aktywacji komputera od klientów programu RMS w wersji 1.0 do usługi aktywacji firmy Microsoft. Następnie ta usługa zwraca indywidualnie wygenerowaną skrytkę oraz odpowiedni certyfikat komputera RMS, które są unikatowe dla określonego użytkownika i komputera. Usługa serwera proxy aktywacji następnie przesyła te elementy z powrotem do klienta zgłaszającego żądanie.

Plik aplikacji usługi serwera proxy aktywacji, Activation.asmx, znajduje się w katalogu wirtualnym Certification w programie IIS. W poniższej tabeli przedstawiono domyślną listę kontroli dostępu w ramach tej usługi:

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
<td style="border:1px solid black;">Goście</td>
<td style="border:1px solid black;">Odczyt i Wykonywanie</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Grupa RMS Service Group</td>
<td style="border:1px solid black;">Odczyt i Wykonywanie</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">SYSTEM</td>
<td style="border:1px solid black;">Pełna kontrola</td>
</tr>
</tbody>
</table>
