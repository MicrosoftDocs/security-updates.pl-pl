---
TOCTitle: Certyfikaty licencjodawcy serwera
Title: Certyfikaty licencjodawcy serwera
ms:assetid: '0b35fbcd-25a9-4587-898d-9a30fd1d3c5b'
ms:contentKeyID: 18123176
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720184(v=WS.10)'
---

Certyfikaty licencjodawcy serwera
=================================

Certyfikat licencjodawcy serwera udziela serwerowi programu RMS prawa do wystawiania certyfikatów i licencji. Podczas zastrzegania pierwszy serwer głównej certyfikacji w rozmieszczeniu programu RMS otrzymuje certyfikat licencjodawcy serwera od usługi rejestrowania firmy Microsoft. Proces ten jest nazywany rejestrowaniem. Ten certyfikat zawiera klucz publiczny serwera głównej certyfikacji i jest podpisywany kluczem prywatnym usługi rejestrowania. Inne serwery dodane do klastra głównej certyfikacji współużytkują ten certyfikat.

Podczas zastrzegania pierwszy serwer licencji w klastrze otrzymuje certyfikat licencjodawcy serwera od serwera lub klastra głównej certyfikacji programu RMS podczas procesu nazywanego podrejestrowywaniem. Ten certyfikat zawiera klucz publiczny serwera licencji i jest podpisywany kluczem prywatnym głównego serwera lub klastra certyfikacji. Inne serwery dodane do klastra licencji współużytkują ten certyfikat.

W poniższej tabeli zawarto prawa udzielane serwerom przez certyfikaty licencjodawcy serwera.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Udziela prawa do wystawiania</th>
<th style="border:1px solid black;" >Certyfikat licencjodawcy serwera jest wystawiany dla serwera głównej certyfikacji</th>
<th style="border:1px solid black;" >Certyfikat licencjodawcy serwera jest wystawiany dla serwera licencji</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Certyfikaty kont praw</td>
<td style="border:1px solid black;">Tak</td>
<td style="border:1px solid black;">Nie</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Licencje publikacji</td>
<td style="border:1px solid black;">Tak</td>
<td style="border:1px solid black;">Tak</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Licencje użytkowania</td>
<td style="border:1px solid black;">Tak</td>
<td style="border:1px solid black;">Tak</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Certyfikaty licencjonowania serwera podrzędnego</td>
<td style="border:1px solid black;">Tak</td>
<td style="border:1px solid black;">Nie</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Certyfikaty licencjodawcy klienta</td>
<td style="border:1px solid black;">Tak</td>
<td style="border:1px solid black;">Tak</td>
</tr>
</tbody>
</table>
  
> [!note]  
> Program RMS nie wymaga osobnych serwerów lub klastrów licencji, ale można użyć osobnych serwerów lub klastrów licencji w celu przejęcia żądań licencji od klastra głównej certyfikacji. Administratorzy mogą również skonfigurować serwery licencji, tak aby spełniały wymagania organizacji w zakresie bezpośredniej kontroli nad publikowaniem bezpiecznej zawartości. Na przykład ogólne zasady w firmie zaimplementowane w szablonach zasad praw serwera lub klastra głównej certyfikacji mogą nie określać wszystkich praw wymaganych przez dany oddział firmy. W takim przypadku dany oddział może rozmieścić oddzielny serwer lub klaster licencji w celu przechowywania własnych szablonów zasad praw dostępu i obsługi żądań licencji. 
