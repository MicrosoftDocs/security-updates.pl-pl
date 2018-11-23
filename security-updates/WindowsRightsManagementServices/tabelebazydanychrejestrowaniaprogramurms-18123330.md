---
TOCTitle: Tabele bazy danych rejestrowania programu RMS
Title: Tabele bazy danych rejestrowania programu RMS
ms:assetid: '7ab2104c-b12d-4807-8a4b-bcabb145ff9b'
ms:contentKeyID: 18123330
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747569(v=WS.10)'
---

Tabele bazy danych rejestrowania programu RMS
=============================================

W tym temacie opisano tabele bazy danych rejestrowania programu RMS.

DRMS\_Log\_Master
-----------------

Poniższa tabela zawiera wpis odpowiadający każdemu rekordowi rejestrowania.


<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Nazwa</th>
<th style="border:1px solid black;" >Typ danych</th>
<th style="border:1px solid black;" >Wartości NULL</th>
<th style="border:1px solid black;" >Opis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">i_LogID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">IDENTITY(100,1) nie NULL</td>
<td style="border:1px solid black;">Unikatowy identyfikator danego rekordu rejestrowania</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_HostMachineName</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Serwer, który wygenerował rekord</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_HostMachineRequestId</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Identyfikator żądania</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">dt_RequestTime</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Data i godzina żądania</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_RequestPath</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Ścieżka URL żądania</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_RequestType</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Typ żądania</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_RequestUserAddress</td>
<td style="border:1px solid black;">nvarchar(32)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Adres IP klienta</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_RequestUserAgent</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Nagłówek agenta użytkownika odpowiadający klientowi</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_AuthenticatedState</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Stan uwierzytelniania żądania</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_SecureConnectionState</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Ochrona SSL żądania</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_AuthenticatedId</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Identyfikator uwierzytelnionego użytkownika</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_ReceivedXrML</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Zawartość w języku XrML otrzymana od klienta w żądaniu</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_IssuedXrML</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Licencja XrML wystawiona w żądaniu</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_Metadata</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Metadane</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_SuccessOrFailure</td>
<td style="border:1px solid black;">nvarchar(32)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Powodzenie lub niepowodzenie żądania</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_ErrorInformation</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Dane błędu</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_LogCreateTime</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Godzina utworzenia dziennika</td>
</tr>
</tbody>
</table>
  
DRMS\_Log\_Detail  
-----------------
  
Poniższa tabela zawiera dodatkowe dane dotyczące rekordu rejestrowania. Zwykle w tej tabeli rejestrowane są dane XrML.
  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Nazwa</th>
<th style="border:1px solid black;" >Typ danych</th>
<th style="border:1px solid black;" >Wartości NULL</th>
<th style="border:1px solid black;" >Opis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">i_LogDetailID</td>
<td style="border:1px solid black;">int (PK)</td>
<td style="border:1px solid black;">IDENTITY(100,1)</td>
<td style="border:1px solid black;">Wewnętrzny indeks</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i_LogID</td>
<td style="border:1px solid black;">int (klucz obcy)</td>
<td style="border:1px solid black;">Nie NULL (FK)</td>
<td style="border:1px solid black;">Identyfikator nadrzędnego rekordu rejestrowania</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_Name</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Nazwa właściwości</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_Value</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Wartość właściwości</td>
</tr>
</tbody>
</table>
  
DRMS\_Log\_Filter  
-----------------
  
Poniższa tabela zawiera listę pól rejestrowanych w usłudze odbiornika rejestrowania.
  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Nazwa</th>
<th style="border:1px solid black;" >Typ danych</th>
<th style="border:1px solid black;" >Wartości NULL</th>
<th style="border:1px solid black;" >Opis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">i_ID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">IDENTITY(100,1) nie NULL</td>
<td style="border:1px solid black;">Wewnętrzny indeks</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_FieldName</td>
<td style="border:1px solid black;">nvarchar(255)</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Nazwa pola</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_FieldDescription</td>
<td style="border:1px solid black;">nvarchar(1024)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Opis pola</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i_IsIncluded</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Określa, czy pole jest rejestrowane</td>
</tr>
</tbody>
</table>
