---
TOCTitle: Listy odwołania w programie RMS
Title: Listy odwołania w programie RMS
ms:assetid: '688d4dfa-c928-4b2f-8116-2f9e87d2b6f7'
ms:contentKeyID: 18123296
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720287(v=WS.10)'
---

Listy odwołania w programie RMS
===============================

Listy odwołania określają zawartość, aplikacje, użytkowników lub inne podmioty, które zostały odwołane. Organizacja może dołączyć jednostkę do listy odwołania z jednego lub kilku poniższych powodów:

-   Wiadomo lub podejrzewa się, że klucz prywatny został złamany.
-   Właściciel żąda odwołania klucza, który według jego wiedzy został złamany.
-   Podmiot nie jest już ważny (na przykład pracownik został zwolniony).
-   Istnieje błąd w systemie zabezpieczeń (na przykład certyfikat wystawiony komputerowi klienckiemu został złamany).
-   Ponowna certyfikacja jest wymagana z powodu zmian w autoryzacji.
-   W aplikacji obsługującej technologię RMS istnieją błędy zabezpieczeń, które uniemożliwiają użytkowanie tej aplikacji do korzystania z cennej zawartości lub w ogóle z zawartości chronionej.
-   Fragment zawartości, który został wcześniej ponownie rozpowszechniony, utracił ważność lub nie jest już przeznaczony do wykorzystania.

W poniższej tabeli przedstawiono jednostki, które można określić na liście odwołania, wraz z informacjami używanymi do zidentyfikowania każdej z nich.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Jednostka</th>
<th>Identyfikator</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Grupa licencji lub certyfikatów</td>
<td style="border:1px solid black;">Identyfikator lub klucz publiczny jednostki wystawiającej</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Grupa manifestów aplikacji</td>
<td style="border:1px solid black;">Identyfikator lub klucz publiczny jednostki wystawiającej</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Określona licencja lub certyfikat</td>
<td style="border:1px solid black;">Identyfikator lub wartość mieszania (hash) licencji</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Określony manifest aplikacji</td>
<td style="border:1px solid black;">Identyfikator lub wartość mieszania (hash) licencji</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Określony podmiot</td>
<td style="border:1px solid black;">Identyfikator lub klucz publiczny podmiotu</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Określony fragment zawartości</td>
<td style="border:1px solid black;">Identyfikator zawartości</td>
</tr>
</tbody>
</table>
  
| ![](images/Cc720287.note(WS.10).gif)Uwaga                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |  
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Dla potrzeb odwołania i wykluczania wszystkie wartości mieszania należą do kategorii SHA-1 \[NIS94c\], wersji algorytmu SHA (Secure Hash Algorithm), określonego przez standard SHS, FIPS 180 (Secure Hash Standard). Kategorię SHA-1 opisano w standardzie ANSI X9.30 (część 2). Aby odwołać za pomocą manifestu aplikacji, konieczne jest wyodrębnienie identyfikatora wystawcy, klucza publicznego wystawcy, identyfikatora licencji lub wartości mieszania licencji z manifestu aplikacji. Jednak manifesty aplikacji są szyfrowane algorytmem Base-64, dlatego też informacje nie są dostępne w czytelnym widoku. Korzystając z pakietu Rights Management Client SDK, za pomocą metod **DRMConstructCertificateChain**, **DRMDeconstructCertificateChain** i **DRMDecode** można opracować program umożliwiający odszyfrowanie manifestu aplikacji i uzyskanie żądanych informacji. Aby uniemożliwić pewnym aplikacjom korzystanie z zawartości chronionej technologią RMS, należy rozważyć zastosowanie wykluczania aplikacji mającego na celu uniemożliwienie serwerowi programu RMS udzielania tym aplikacjom licencji użytkowania. Wykluczanie ma natomiast jedno ograniczenie: uniemożliwienie odszyfrowywania zawartości chronionej technologią RMS osobie z ważną licencją użytkowania jest niemożliwe. Aby uzyskać więcej informacji dotyczących wykluczania aplikacji, zobacz Wykluczanie aplikacji w części „Obsługa serwerów programu RMS” w tym zestawie dokumentacji. |
  
Listy odwołania są plikami XrML, które określają następujące parametry.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Parametr</th>
<th>Opis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">ISSUEDTIME</td>
<td style="border:1px solid black;">Czas systemowy, kiedy utworzono plik XrML. Ten parametr jest używany przez warunek REFRESH w licencji użytkowania w celu określenia wieku listy odwołania.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ISSUER</td>
<td style="border:1px solid black;">Nazwa, identyfikator i adres jednostki wystawiającej listę odwołania.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PUBLICKEY</td>
<td style="border:1px solid black;">Klucz publiczny jednostki wystawiającej listę odwołania.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">REVOCATIONLIST</td>
<td style="border:1px solid black;">Nazwa, typ i identyfikator każdej z odwołanych jednostek.</td>
</tr>
</tbody>
</table>
