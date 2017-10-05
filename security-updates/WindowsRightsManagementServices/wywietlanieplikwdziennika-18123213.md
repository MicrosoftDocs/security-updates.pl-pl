---
TOCTitle: Wyświetlanie plików dziennika
Title: Wyświetlanie plików dziennika
ms:assetid: '2dc9ed54-76d8-4721-ba93-194845de726a'
ms:contentKeyID: 18123213
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720228(v=WS.10)'
---

Wyświetlanie plików dziennika
=============================

Zależnie od sposobu rozmieszczenia programu RMS pliki dziennika są przechowywane na serwerze bazy danych, np. SQL Server lub Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) wersja A. Za pomocą specjalnie napisanych filtrów można zmniejszyć ilość informacji przechowywanych w plikach dziennika. Aby uzyskać instrukcje, zobacz Pomoc programu SQL Server Enterprise Manager.

Rozmiar przeciętnego wpisu dziennika wynosi około 300 bajtów. Rejestrowane pola opisano w poniższej tabeli.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Pole</th>
<th>Opis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">HostMachineName</td>
<td style="border:1px solid black;">Komputer, który obsługiwał żądanie.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">HostMachineRequestId</td>
<td style="border:1px solid black;">Unikatowy identyfikator danego żądania na tym komputerze. Kombinacja wartości HostMachineName i HostMachineRequestId stanowi unikatowy identyfikator żądania w klastrze.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">RequestTime</td>
<td style="border:1px solid black;">Godzina otrzymania żądania, wyrażona w skoordynowanym czasie uniwersalnym (czasie uniwersalnym Greenwich).</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">RequestPath</td>
<td style="border:1px solid black;">Względny adres URL do pliku.asmx, na przykład: /_wmcs/licensing/License.asmx.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">RequestType</td>
<td style="border:1px solid black;">Nazwa wywołanej metody sieci Web, na przykład AcquireLicense.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">RequestUserAddress</td>
<td style="border:1px solid black;">Źródłowy adres IP obiektu zgłaszającego żądanie.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">RequestUserAgent</td>
<td style="border:1px solid black;">Wartość agenta użytkownika z nagłówka HTTP.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">AuthenticatedState</td>
<td style="border:1px solid black;">Określa, czy połączenie HTTP było uwierzytelnione (Prawda/Fałsz).</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">SecureConnectionState</td>
<td style="border:1px solid black;">Określa, czy jest to połączenie SSL (Prawda/Fałsz).</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">AuthenticatedId</td>
<td style="border:1px solid black;">Nazwa logowania odpowiadająca uwierzytelnionym żądaniom. Pole puste, jeśli AuthenticatedState=Fałsz.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">ReceivedXrMLDocument</td>
<td style="border:1px solid black;">Dokument XrML otrzymany od obiektu zgłaszającego żądanie.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ReceivedXrMLDocumentIssuerChain</td>
<td style="border:1px solid black;">Łańcuch wystawcy odpowiadający otrzymanemu dokumentowi XrML.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">IssuedXrMLDocument</td>
<td style="border:1px solid black;">Dokument XrML zwrócony obiektowi zgłaszającemu żądanie.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">IssuedXrMLDocumentIssuerChain</td>
<td style="border:1px solid black;">Łańcuch wystawcy odpowiadający wystawionemu dokumentowi XrML.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">SuccessOrFailure</td>
<td style="border:1px solid black;">Określa, czy żądanie zakończyło się powodzeniem, czy niepowodzeniem (Powodzenie/Niepowodzenie).</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Metadane</td>
<td style="border:1px solid black;">Pole metadanych.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">ErrorInformation</td>
<td style="border:1px solid black;">Opisowy komunikat o błędzie, wyświetlany w przypadku wystąpienia błędu.</td>
</tr>
</tbody>
</table>
