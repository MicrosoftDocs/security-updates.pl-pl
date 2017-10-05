---
TOCTitle: Zarządzanie certyfikatami licencjodawcy serwera
Title: Zarządzanie certyfikatami licencjodawcy serwera
ms:assetid: '549979ad-13ee-4abc-8281-3e002a5a9561'
ms:contentKeyID: 18123274
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720272(v=WS.10)'
---

Zarządzanie certyfikatami licencjodawcy serwera
===============================================

Certyfikaty licencjodawcy serwera wygasają po określonym czasie, zwykle po upływie jednego roku. Aby odnowić certyfikat licencjodawcy serwera, należy zalogować się jako administrator lokalny. Jeśli odnawiany jest certyfikat licencjodawcy serwera dla klastra głównej certyfikacji, program RMS wysyła żądanie odnowienia tego certyfikatu do usługi rejestrowania firmy Microsoft. Jeśli ten certyfikat jest odnawiany dla serwera licencji, program RMS wysyła żądanie odnowienia do serwera głównej certyfikacji, który wystawił wygasający certyfikat.

Istnieją trzy zdarzenia wysyłane przez program RMS do dziennika zdarzeń systemowych, które trzeba monitorować. Zdarzenia te informują, kiedy dany certyfikat licencjodawcy serwera zbliża się do daty odnowienia lub kiedy wygasł. W poniższej tabeli wymieniono identyfikatory zdarzeń i ich nazwy.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Identyfikator zdarzenia</th>
<th>Nazwa zdarzenia</th>
<th>Typ zdarzenia</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">16</td>
<td style="border:1px solid black;">LicensorCertExpiresInOneMonthEvent (Certyfikat licencjodawcy wygasa za miesiąc)</td>
<td style="border:1px solid black;">Ostrzeżenie Usługa w dalszym ciągu działa normalnie</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">17</td>
<td style="border:1px solid black;">LicensorCertExpiresInOneWeekEvent (Certyfikat licencjodawcy wygasa za tydzień)</td>
<td style="border:1px solid black;">Ostrzeżenie Usługa w dalszym ciągu działa normalnie</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">18</td>
<td style="border:1px solid black;">LicensorCertExpiredEvent (Certyfikat licencjodawcy wygasł)</td>
<td style="border:1px solid black;">Błąd. Usługa jest wyłączana</td>
</tr>
</tbody>
</table>
