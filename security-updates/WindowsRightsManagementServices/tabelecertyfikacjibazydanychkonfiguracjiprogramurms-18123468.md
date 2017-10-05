---
TOCTitle: Tabele certyfikacji bazy danych konfiguracji programu RMS
Title: Tabele certyfikacji bazy danych konfiguracji programu RMS
ms:assetid: 'd392663a-1a46-42f6-a71d-f0f2c1843566'
ms:contentKeyID: 18123468
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747760(v=WS.10)'
---

Tabele certyfikacji bazy danych konfiguracji programu RMS
=========================================================

W tym temacie opisano tabele certyfikacji, które znajdują się w bazie danych konfiguracji programu RMS. Tabele te zawierają informacje na temat certyfikatów kont praw wystawionych użytkownikom danej instalacji.

UD\_Machines
------------

Poniższa tabela zawiera informacje o identyfikatorach sprzętu odpowiadających wszystkim komputerom.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Nazwa</th>
<th>Typ danych</th>
<th>Wartości NULL</th>
<th>Opis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">i_MachineId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">IDENTITY(1,1) nie NULL</td>
<td style="border:1px solid black;">Wewnętrzny indeks</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">b_PubKeyHash</td>
<td style="border:1px solid black;">binary(20)</td>
<td style="border:1px solid black;">(20) Nie NULL</td>
<td style="border:1px solid black;">Mieszanie identyfikatora sprzętu</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_CreateDate</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Data i godzina dodania wpisu do tabeli</td>
</tr>
</tbody>
</table>
  
UD\_PassportAuthIdentities  
--------------------------
  
Poniższa tabela zawiera informacje o usłudze Microsoft® .NET Passport dotyczące użytkowników.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Nazwa</th>
<th>Typ danych</th>
<th>Wartości NULL</th>
<th>Opis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">i_UserId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Wewnętrzny indeks</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i64_Puid</td>
<td style="border:1px solid black;">bigint</td>
<td style="border:1px solid black;">(50) NULL</td>
<td style="border:1px solid black;">Identyfikator użytkownika usługi .NET Passport</td>
</tr>
</tbody>
</table>
  
UD\_UserMachine  
---------------
  
Poniższa tabela łączy dane certyfikowanych użytkowników z odpowiadającymi im informacjami o komputerach.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Nazwa</th>
<th>Typ danych</th>
<th>Wartości NULL</th>
<th>Opis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">i_MachineId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Wewnętrzny indeks</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i_UserId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Wewnętrzny indeks</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_CreateDate</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Data i godzina dodania wpisu do tabeli</td>
</tr>
</tbody>
</table>
  
UD\_Users  
---------
  
Poniższa tabela zawiera informacje dotyczące danych użytkowników.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Nazwa</th>
<th>Typ danych</th>
<th>Wartości NULL</th>
<th>Opis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">i_UserId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">IDENTITY(1,1) nie NULL</td>
<td style="border:1px solid black;">Wewnętrzny indeks</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">b_KeyData</td>
<td style="border:1px solid black;">varbinary(2000)</td>
<td style="border:1px solid black;">(2000) Nie NULL</td>
<td style="border:1px solid black;">Zaszyfrowany klucz publiczny/prywatny użytkownika</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">i_KeyDataLength</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Długość niezaszyfrowanego klucza publicznego/prywatnego</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">b_PublicKey</td>
<td style="border:1px solid black;">PublicKey</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Klucz publiczny użytkownika</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">i_EncryptionDbId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Wskazanie certyfikatu licencjodawcy używanego w szyfrowaniu danej pary kluczy publiczny-prywatny</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_Certificate</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">Nie określono</td>
<td style="border:1px solid black;">Nieużywane</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_Expiration</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Data wygaśnięcia klucza użytkownika</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">dt_TemporaryExpiration</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Data i godzina wygaśnięcia tymczasowego użytkowania klucza</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">f_Modified</td>
<td style="border:1px solid black;">bit</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Nieużywane</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i_Quota</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Bieżący poziom przydziału danego użytkownika</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">i_WaitDays</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Liczba dni, które muszą upłynąć, aby żądania dodatkowego przydziału mogły kończyć się powodzeniem</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">dt_LastConsumption</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Data i godzina ostatniej dodatkowej certyfikacji użytkownika</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_CreateDate</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Data i godzina dodania wpisu do tabeli</td>
</tr>
</tbody>
</table>
  
UD\_Windows AuthIdentities  
--------------------------
  
Poniższa tabela zawiera listę identyfikatorów wszystkich uwierzytelnionych i certyfikowanych użytkowników systemu Windows.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Nazwa</th>
<th>Typ danych</th>
<th>Wartości NULL</th>
<th>Opis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">i_UserId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Wewnętrzny indeks</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_Sid</td>
<td style="border:1px solid black;">Sid</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Identyfikator zabezpieczeń (SID) użytkownika</td>
</tr>
</tbody>
</table>
