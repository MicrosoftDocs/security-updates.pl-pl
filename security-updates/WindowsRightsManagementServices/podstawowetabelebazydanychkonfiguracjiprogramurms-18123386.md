---
TOCTitle: Podstawowe tabele bazy danych konfiguracji programu RMS
Title: Podstawowe tabele bazy danych konfiguracji programu RMS
ms:assetid: '8f9e15a2-92bc-41f7-a4fd-329567afb142'
ms:contentKeyID: 18123386
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747676(v=WS.10)'
---

Podstawowe tabele bazy danych konfiguracji programu RMS
=======================================================

W tym temacie opisano podstawowe tabele bazy danych konfiguracji programu RMS.

DRMS\_ApplicationExclusionList
------------------------------

Poniższa tabela zawiera informacje o wykluczonych aplikacjach.

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
<td style="border:1px solid black;">ID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">IDENTITY(100,1) nie NULL</td>
<td style="border:1px solid black;">Wewnętrzny indeks</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Nazwa</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Nazwa aplikacji</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">VersionMinMajor</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Minimalny numer wersji głównej aplikacji</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">VersionMinMinor</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Minimalny numer wersji pomocniczej aplikacji</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">VersionMinBuild</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Minimalny numer wersji kompilacji aplikacji</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">VersionMinRevision</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Minimalny numer wersji poprawek aplikacji</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">VersionMaxMajor</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Maksymalny numer wersji głównej aplikacji</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">VersionMaxMinor</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Maksymalny numer wersji pomocniczej aplikacji</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">VersionMaxBuild</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Maksymalny numer wersji kompilacji aplikacji</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">VersionMaxRevision</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Maksymalny numer wersji poprawek aplikacji</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Opis</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Opis aplikacji</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">dt_DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Sygnatura czasowa aktualizacji</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Sygnatura czasowa utworzenia</td>
</tr>
</tbody>
</table>
  
DRMS\_AsynchronousQueue  
-----------------------
  
Poniższa tabela zawiera informacje dotyczące kolejki komunikatów.
  
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
<td style="border:1px solid black;">AsyncQueueID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY(100,1) nie NULL</td>
<td style="border:1px solid black;">Wewnętrzny indeks</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">QueueName</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Ścieżka do kolejki komunikatów</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Sygnatura czasowa aktualizacji</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Sygnatura czasowa utworzenia</td>
</tr>
</tbody>
</table>
  
DRMS\_CaType  
------------
  
Poniższa tabela zawiera informacje dotyczące typu certyfikatu wystawionego klientowi.
  
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
<td style="border:1px solid black;">ID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Identyfikator certyfikatu</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">TypeName</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Stacja robocza, urządzenie przenośne lub serwer</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Sygnatura czasowa aktualizacji</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Sygnatura czasowa utworzenia</td>
</tr>
</tbody>
</table>
  
DRMS\_ClusterConfiguration  
--------------------------
  
Poniższa tabela zawiera informacje na temat bieżącego certyfikatu licencjodawcy serwera znajdującego się w tabeli DRMS\_LicensorCertificate.
  
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
<td style="border:1px solid black;">CurrentLicensorCertID</td>
<td style="border:1px solid black;">int (klucz obcy)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Aktywny certyfikat licencjodawcy</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Sygnatura czasowa aktualizacji</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Sygnatura czasowa utworzenia</td>
</tr>
</tbody>
</table>
  
DRMS\_ClusterPolicies  
---------------------
  
Poniższa tabela zawiera listę lokalizacji, w których przechowywane są zasady klastrów.
  
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
<td style="border:1px solid black;">PolicyID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY(100,1) nie NULL</td>
<td style="border:1px solid black;">Identyfikator zasad</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PolicyName</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Nazwa zasad</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PolicyData</td>
<td style="border:1px solid black;">sql_variant</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Dane zasad</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Sygnatura czasowa aktualizacji</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Sygnatura czasowa utworzenia</td>
</tr>
</tbody>
</table>
  
DRMS\_ClusterServer  
-------------------
  
Poniższa tabela zawiera informacje na temat serwerów znajdujących się w klastrze.
  
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
<td style="border:1px solid black;">ServerID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY(100,1) nie NULL</td>
<td style="border:1px solid black;">Identyfikator serwera</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ServerName</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">Nie określono</td>
<td style="border:1px solid black;">Nazwa komputera odpowiadająca serwerowi</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Sygnatura czasowa aktualizacji</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Sygnatura czasowa utworzenia</td>
</tr>
</tbody>
</table>
  
DRMS\_GICExclusionList  
----------------------
  
Poniższa tabela zawiera informacje o wykluczonych certyfikatach kont praw.
  
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
<td style="border:1px solid black;">PublicKeyIndex</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY(100,1) nie NULL</td>
<td style="border:1px solid black;">Wewnętrzny indeks</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PublicKey</td>
<td style="border:1px solid black;">PublicKey</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Bajty klucza publicznego</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">UserID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Indeks identyfikatora użytkownika</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ExpirationDate</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Data wygaśnięcia certyfikatu konta praw</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Opis</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Nazwa skojarzona z danym kluczem wykluczonego certyfikatu konta praw</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">dt_DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Sygnatura czasowa aktualizacji</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Sygnatura czasowa utworzenia</td>
</tr>
</tbody>
</table>
  
DRMS\_LicensorCertificate  
-------------------------
  
Poniższa tabela zawiera informacje o aktywnym certyfikacie licencjodawcy serwera.
  
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
<td style="border:1px solid black;">i_CertID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY(100,1) nie NULL</td>
<td style="border:1px solid black;">Identyfikator zasad</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_CertGUIDType</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Typ identyfikatora pary kluczy</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_CertGUID</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Identyfikator GUID odpowiadający identyfikatorowi pary kluczy</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i_CertificateID</td>
<td style="border:1px solid black;">int (klucz obcy)</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Wartość wskazująca rzeczywisty certyfikat</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Sygnatura czasowa aktualizacji</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">dt_DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Sygnatura czasowa utworzenia</td>
</tr>
</tbody>
</table>
  
DRMS\_LicensorPrivateKey  
------------------------
  
Poniższa tabela zawiera informacje o kluczu prywatnym aktywnego certyfikatu licencjodawcy serwera.
  
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
<td style="border:1px solid black;">PrivateKeyID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY(100,1) nie NULL</td>
<td style="border:1px solid black;">Wewnętrzny indeks</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CertGUIDType</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Typ identyfikatora pary kluczy</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">CertGUID</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Identyfikator GUID odpowiadający identyfikatorowi pary kluczy</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PrivateKey</td>
<td style="border:1px solid black;">varbinary(2048)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Binarna postać klucza</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">CSP</td>
<td style="border:1px solid black;">nvarchar(512)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Nazwa dostawcy usług kryptograficznych (CSP)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CSPType</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Typ dostawcy CSP</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">KeyContainerName</td>
<td style="border:1px solid black;">nvarchar(512)</td>
<td style="border:1px solid black;">Nie określono</td>
<td style="border:1px solid black;">Nazwa kontenera klucza</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">KeyNumber</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Numer klucza</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Sygnatura czasowa aktualizacji</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Sygnatura czasowa utworzenia</td>
</tr>
</tbody>
</table>
  
DRMS\_PassportDenyList  
----------------------
  
Poniższa tabela zawiera informacje o kontach usługi Microsoft® .NET Passport, którym należy odmówić licencji.
  
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
<td style="border:1px solid black;">DenyID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY(100,1) nie NULL</td>
<td style="border:1px solid black;">Wewnętrzny indeks</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DenyAddressPattern</td>
<td style="border:1px solid black;">nvarchar(500)</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Nazwa użytkownika/nazwa domeny</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Sygnatura czasowa aktualizacji</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Sygnatura czasowa utworzenia</td>
</tr>
</tbody>
</table>
  
DRMS\_Plugin  
------------
  
Poniższa tabela zawiera informacje o dodatkach.
  
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
<td style="border:1px solid black;">PluginID</td>
<td style="border:1px solid black;">Int</td>
<td style="border:1px solid black;">IDENTITY(100,1) nie NULL</td>
<td style="border:1px solid black;">Wewnętrzny indeks</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PluginTypeID</td>
<td style="border:1px solid black;">int (klucz obcy)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Typ dodatku</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">NameSpace</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Przestrzeń nazw danego dodatku</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PluginName</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Nazwa danego dodatku</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Ordinal</td>
<td style="border:1px solid black;">Int</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Numer sekwencji, zgodnie z którym wykonywany jest dodatek</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Path</td>
<td style="border:1px solid black;">nvarchar(512)</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Ścieżka do pliku DLL</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">ObjectTypeName</td>
<td style="border:1px solid black;">nvarchar(50)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Nieużywane</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DebugMode</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Określa, czy należy uruchomić dodatek w trybie debugowania</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PublicKey</td>
<td style="border:1px solid black;">PublicKey</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Klucz publiczny dodatku</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Version</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Wersja dodatku</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Sygnatura czasowa aktualizacji</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Sygnatura czasowa utworzenia</td>
</tr>
</tbody>
</table>
  
DRMS\_AllowedPluginVersions  
---------------------------
  
Poniższa tabela zawiera informacje o wersjach dodatków, które można wykorzystać w systemie RMS.
  
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
<td style="border:1px solid black;">RowID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Wewnętrzny indeks</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PluginID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">IDENTITY(100,1) nie NULL</td>
<td style="border:1px solid black;">Wewnętrzny indeks</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">VersionInfo</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">Nie określono</td>
<td style="border:1px solid black;">Wersja dodatku</td>
</tr>
</tbody>
</table>
  
DRMS\_PluginProperties  
----------------------
  
Poniższa tabela zawiera informacje o właściwościach dodatku.
  
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
<td style="border:1px solid black;">PropertyID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">IDENTITY(100,1) nie NULL</td>
<td style="border:1px solid black;">Wewnętrzny indeks</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PluginID</td>
<td style="border:1px solid black;">int (klucz obcy)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Identyfikator dodatku, do którego należy właściwość</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PropertyName</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Nazwa właściwości odpowiadająca danym konfiguracji</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PropertyValue</td>
<td style="border:1px solid black;">text</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Wartość właściwości odpowiadająca danym konfiguracji</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Sygnatura czasowa aktualizacji</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Sygnatura czasowa utworzenia</td>
</tr>
</tbody>
</table>
  
DRMS\_PluginType  
----------------
  
Poniższa tabela zawiera informacje o typie dodatku.
  
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
<td style="border:1px solid black;">PluginTypeID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Wewnętrzny indeks</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PluginTypeName</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Nazwa danego dodatku</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Sygnatura czasowa aktualizacji</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Sygnatura czasowa utworzenia</td>
</tr>
</tbody>
</table>
  
DRMS\_RightsTemplate  
--------------------
  
Poniższa tabela zawiera informacje o szablonach zasad praw.
  
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
<td style="border:1px solid black;">Guid</td>
<td style="border:1px solid black;">nvarchar(128) (PK)</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Identyfikator GUID szablonu zasad praw</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">TemplateData</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">To pole zawiera dane szablonu XrML.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Sygnatura czasowa aktualizacji</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Sygnatura czasowa utworzenia</td>
</tr>
</tbody>
</table>
  
DRMS\_TrustedCertificateAuthorities  
-----------------------------------
  
Poniższa tabela zawiera informacje o zaufanych urzędach certyfikacji.
  
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
<td style="border:1px solid black;">ID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY(1,1) nie NULL</td>
<td style="border:1px solid black;">Wewnętrzny indeks</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CertificateID</td>
<td style="border:1px solid black;">int (klucz obcy)</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Identyfikator certyfikatu</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">CertificateGUID</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Identyfikator GUID certyfikatu</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CaTypeID</td>
<td style="border:1px solid black;">int (klucz obcy)</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Typ urzędu certyfikacji</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Sygnatura czasowa aktualizacji</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Sygnatura czasowa utworzenia</td>
</tr>
</tbody>
</table>
  
DRMS\_TrustedEmailDomains  
-------------------------
  
Poniższa tabela zawiera informacje o zaufanych domenach poczty e-mail w środowisku RMS
  
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
<td style="border:1px solid black;">ID</td>
<td style="border:1px solid black;">int (PK)</td>
<td style="border:1px solid black;">IDENTITY(100,1) nie NULL</td>
<td style="border:1px solid black;">Wewnętrzny indeks</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i_TrustedIdentityDomainID</td>
<td style="border:1px solid black;">int (FK)t</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Wewnętrzny indeks</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_EmailDomainName</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Lista nazw domen poczty e-mail należących do zaufanych domen użytkowników</td>
</tr>
</tbody>
</table>
  
DRMS\_TrustedIdentityDomain  
---------------------------
  
Poniższa tabela zawiera informacje o zaufanych domenach użytkownika i zaufanych domenach publikacji.
  
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
<td style="border:1px solid black;">i_TrustedIdentityDomainID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY(100,1) nie NULL</td>
<td style="border:1px solid black;">Wewnętrzny indeks</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_DomainType</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Typ domeny</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">CertGUIDType</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Typ identyfikatora GUID certyfikatu</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CertGUID</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Identyfikator GUID certyfikatu</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">i_CertificateID</td>
<td style="border:1px solid black;">int (klucz obcy)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Identyfikator certyfikatu</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i_allowSID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Identyfikator SID domeny</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">S_friendlyname</td>
<td style="border:1px solid black;">nvarchar(255)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Przyjazna nazwa certyfikatu</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">dt_DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Sygnatura czasowa aktualizacji</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Sygnatura czasowa utworzenia</td>
</tr>
</tbody>
</table>
  
DRMS\_XrML\_Certificate  
-----------------------
  
Poniższa tabela zawiera informacje o certyfikatach licencjodawcy serwera XrML, do których odwołuje się tabela DRMS\_LicensorCertificate. Zawiera ona również odwzorowanie łańcucha certyfikatów.
  
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
<td style="border:1px solid black;">i_CertificateID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY(100,1) nie NULL</td>
<td style="border:1px solid black;">Wartość wskazująca rzeczywisty certyfikat</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_Certificate</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">Nie NULL</td>
<td style="border:1px solid black;">Wartość wskazująca rzeczywisty certyfikat</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">i_ParentCertificateID</td>
<td style="border:1px solid black;">int (klucz obcy)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Wartość wskazująca rzeczywisty certyfikat</td>
</tr>
</tbody>
</table>
