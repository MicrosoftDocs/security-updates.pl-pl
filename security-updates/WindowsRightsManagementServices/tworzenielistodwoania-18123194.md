---
TOCTitle: Tworzenie list odwołania
Title: Tworzenie list odwołania
ms:assetid: '1ef75199-3344-4225-84de-a863a777696a'
ms:contentKeyID: 18123194
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720208(v=WS.10)'
---

Tworzenie list odwołania
========================

Do implementacji odwołania wymagane jest rozmieszczenie listy odwołania, a więc dokumentu XML, w którym stosuje się język XrML (eXtensible Rights Markup Language) i wymienia podmioty zabezpieczeń, które od danego momentu nie powinny mieć dostępu do zawartości chronionej na podstawie praw. Tworzone listy odwołania muszą posiadać sygnaturę czasową oraz odpowiedni podpis wstawiony za pomocą narzędzia Podpisywanie listy odwołania (RLsigner.exe) dostarczonego z programem RMS.

> [!Important]  
> Aby podpisać listę odwołania przy użyciu programu RLsigner.exe, należy zapisać ją jako plik unicode. 

Przykład listy odwołania
------------------------

Ten temat zawiera przykład pełnej listy odwołania, w którym przedstawiono każdy z możliwych mechanizmów odwołania. Przykładem tym można posłużyć się jako wzorem przy tworzeniu własnych list odwołania.

Lista odwołania to plik XML wykorzystujący język XrML.

Element BODY zawiera cztery elementy podrzędne:

-   **ISSUEDTIME**. Zawiera datę i godzinę wystawienia listy odwołania. Program RLsigner.exe wstawia ten element do pliku. Element przytoczono wyłącznie jako przykład mający zaprezentować ogólną strukturę pliku listy odwołania.
-   **DESCRIPTOR**. Zawiera dane identyfikujące plik jako listę odwołania.
-   **ISSUER**. Zawiera dane identyfikacyjne jednostki, która wystawia listę odwołania.
-   **REVOCATIONLIST**. Zawiera elementy podrzędne REVOKE, które określają jednostki odwołane przez daną listę.

Poniżej ukazano przykładowy plik listy odwołania.

> [!Note]  
> Elementy ISSUEDTIME, PUBLICKEY i SIGNATURE mogą zostać pominięte, ponieważ program RLsigner.exe wstawia je lub nadpisuje.

```
<?xml version="1.0" ?> 
<XrML xml:space=”preserve” version=”1.2”>
  <BODY type="LICENSE" version="3.0">
    <ISSUEDTIME>...</ISSUEDTIME> 
    <DESCRIPTOR>
      <OBJECT type="Revocation-List">
        <ID type="MS-GUID">{d6373cba-01f1-4f32-ac58-260f580af0f8}</ID>
      </OBJECT>
    </DESCRIPTOR>
<ISSUER>
      <OBJECT type="Revocation-List">
        <ID type="acsii-tag">External revocation authority</ID>
        <NAME>Revocation list name</NAME>
        <ADDRESS type="URL">https://somedomain.com/revocation_list_file</ADDRESS>
      </OBJECT>
      <PUBLICKEY>...</PUBLICKEY>
    </ISSUER>
  <REVOCATIONLIST>
    <REVOKE>...<\REVOKE>
    <REVOKE>...<\REVOKE>
  </REVOCATIONLIST>
  <SIGNATURE>...</SIGNATURE>
</XrML>
```
> [!Caution]  
> Ścieżka UNC nie jest już obsługiwana w programie RMS z dodatkiem SP1 lub SP2 podczas określania adresu URL na liście odwołania. Należy użyć adresu URL. 

Po zdefiniowaniu elementów REVOKE lista odwołania jest gotowa do podpisania.

Korzystanie z elementu REVOKE
-----------------------------

Na przykładowej liście odwołania w sekcji Przykład listy odwołania każdy element REVOKE określa podmiot zabezpieczeń, który ma być odwołany. Tag otwierający ma atrybuty kategorii i typu, które określają, do czego odnosi się odwołanie oraz według jakiego kryterium. Różne elementy REVOKE mają różne elementy podrzędne, zależnie od działania określonego atrybutami kategorii i typu.

Aby uzyskać więcej informacji dotyczących określania elementów REVOKE, zobacz następujące przykłady:

-   [Odwołanie podmiotów zabezpieczeń na podstawie klucza publicznego](#bkmk_1)
-   [Odwołanie certyfikatów i licencji na podstawie identyfikatora GUID](#bkmk_2)
-   [Odwołanie certyfikatów i licencji na podstawie wartości mieszania](#bkmk_3)
-   [Odwołanie certyfikatów i licencji na podstawie klucza publicznego wystawcy](#bkmk_4)
-   [Odwołanie certyfikatów i licencji na podstawie identyfikatora wystawcy](#bkmk_5)
-   [Odwołanie zawartości na podstawie identyfikatora zawartości](#bkmk_6)
-   [Odwołanie certyfikatów na podstawie identyfikatora podmiotu zabezpieczeń](#bkmk_10)
-   [Odwołanie podmiotów zabezpieczeń na podstawie Windows Live ID](#bkmk_7)

<span id="BKMK_1"></span>
#### Odwołanie podmiotów zabezpieczeń na podstawie klucza publicznego

W tym przykładzie przedstawiono odwołanie podmiotu zabezpieczeń na podstawie jego klucza publicznego. Zawartość tagu &lt;PUBLICKEY&gt; pochodzi tutaj z węzła &lt;BODY&gt;&lt;ISSUEDPRINCIPALS&gt;&lt;PRINCIPAL&gt;&lt;PUBLICKEY&gt; certyfikatu, który spowodował wystawienie klucza.

```
      <REVOKE category="principal" type="principal-key">
        <PUBLICKEY>
          <ALGORITHM>RSA-1024</ALGORITHM>
          <PARAMETER name="public exponent">
            <VALUE encoding="integer32">65537</VALUE>
          </PARAMETER>
          <PARAMETER name="modulus">
            <VALUE encoding="base64" size="1024">
6Jn0kEAWU+1AFWtuUmBYL8Jza8tLhUv/BCmgcq/Pc08Au3DvXkH65s+0MEyZjM+71j3F1xaXUSst+wH2FjApkY1RxgL8VAKIuEvIy9hRrvY1YhJx/0Ite5fZeg2crUFrmoQgZzaJ50FvoakA2QMgZZgxoQmwiGE0y40cEJtIlE0=
            </VALUE>
          </PARAMETER>
        </PUBLICKEY>
      </REVOKE>
```

<span id="BKMK_2"></span>
#### Odwołanie certyfikatów i licencji na podstawie identyfikatora GUID

W tym przykładzie przedstawiono odwołanie certyfikatu lub licencji na podstawie ich unikatowego identyfikatora globalnego (GUID). Użycie tej listy odwołania powoduje, że nie można korzystać z certyfikatu lub licencji o pasującym identyfikatorze GUID. W tym przykładzie zawartość tagu &lt;ID&gt; pochodzi z węzła &lt;BODYDESCRIPTOROBJECTID&gt;&lt;DESCRIPTOR&gt;&lt;OBJECT&gt;&lt;ID&gt; odwoływanego certyfikatu lub licencji. (Za pomocą tego mechanizmu można także odwołać aplikacje przez określenie identyfikatora manifestu aplikacji.)

```
	<REVOKE category="license" type="license-id">
        <OBJECT>
          <ID type="MS-GUID">{06BCB94D-43E5-419f-B180-AA9FD321ED7A}</ID>
        </OBJECT>
      </REVOKE>
```
#### Odwołanie poprzez manifest aplikacji

Aby odwołać za pomocą manifestu aplikacji, konieczne jest wyodrębnienie identyfikatora wystawcy, klucza publicznego wystawcy, identyfikatora licencji lub wartości mieszania licencji z manifestu aplikacji. Jednak manifesty aplikacji są szyfrowane algorytmem Base-64, dlatego też informacje nie są dostępne w postaci zwykłego tekstu. Korzystając z pakietu SDK Windows Rights Management Services, za pomocą metod DRMConstructCertificateChain, DRMDeconstructCertificateChain i DRMDecode można opracować program umożliwiający odszyfrowanie manifestu aplikacji i uzyskanie żądanych informacji.

Aby uniemożliwić pewnym aplikacjom korzystanie z zawartości chronionej na podstawie praw, należy rozważyć zastosowanie wykluczania aplikacji mającego na celu uniemożliwienie klastrowi programu RMS udzielania tym aplikacjom licencji użytkowania. Wykluczanie ma natomiast jedno ograniczenie: uniemożliwienie odszyfrowywania zawartości chronionej na podstawie praw osobie z ważną licencją użytkowania jest niemożliwe. Aby uzyskać więcej informacji dotyczących wykluczania aplikacji, zobacz [Wykluczanie aplikacji](https://technet.microsoft.com/b68ae4b2-b9ba-44ae-90cb-c88df600ec86) we wcześniejszej części tego tematu.

<span id="BKMK_3"></span>
#### Odwołanie certyfikatów i licencji na podstawie wartości mieszania

W tym przykładzie przedstawiono odwołanie certyfikatu lub licencji na podstawie jej wartości mieszania. Zawartość tagu &lt;VALUE&gt; pochodzi tutaj z wartości mieszania SHA-1 znaków UNICODE z &lt;BODY&gt; do &lt;/BODY&gt; włącznie w certyfikacie lub licencji. Tę wartość mieszania można znaleźć w części &lt;SIGNATURE&gt; certyfikatu lub licencji. (Za pomocą tego mechanizmu można także odwołać aplikacje przez określenie wartości mieszania manifestu aplikacji.)

```
	<REVOKE category="license" type="license-hash">
        <DIGEST>
          <ALGORITHM>SHA1</ALGORITHM>
          <VALUE encoding="base64" size="160">
            ABfB4mcEslVCMEZR9reACqXHCoQ=
          </VALUE>
        </DIGEST>
      </REVOKE>
```
#### Odwołanie poprzez manifest aplikacji

Aby odwołać za pomocą manifestu aplikacji, konieczne jest wyodrębnienie identyfikatora wystawcy, klucza publicznego wystawcy, identyfikatora licencji lub wartości mieszania licencji z manifestu aplikacji. Jednak manifesty aplikacji są szyfrowane algorytmem Base-64, dlatego też informacje nie są dostępne w postaci zwykłego tekstu. Korzystając z pakietu SDK Rights Management Services, za pomocą metod DRMConstructCertificateChain, DRMDeconstructCertificateChain i DRMDecode można opracować program umożliwiający odszyfrowanie manifestu aplikacji i uzyskanie żądanych informacji.

Aby uniemożliwić pewnym aplikacjom korzystanie z zawartości chronionej na podstawie praw, należy rozważyć zastosowanie wykluczania aplikacji mającego na celu uniemożliwienie klastrowi programu RMS udzielania tym aplikacjom licencji użytkowania. Wykluczanie ma natomiast jedno ograniczenie: uniemożliwienie odszyfrowywania zawartości chronionej technologią RMS osobie z ważną licencją użytkowania jest niemożliwe. Aby uzyskać więcej informacji dotyczących wykluczania aplikacji, zobacz [Wykluczanie aplikacji](https://technet.microsoft.com/b68ae4b2-b9ba-44ae-90cb-c88df600ec86) we wcześniejszej części tego tematu.

<span id="BKMK_4"></span>
#### Odwołanie certyfikatów i licencji na podstawie klucza publicznego wystawcy

W tym przykładzie przedstawiono odwołanie wszystkich certyfikatów i licencji wystawionych przez właściciela określonego klucza publicznego. Zawartość tagu &lt;PUBLICKEY&gt; pochodzi z węzła &lt;BODY&gt;&lt;ISSUER&gt;&lt;PUBLICKEY&gt; odwoływanych certyfikatów lub licencji.

```
	<REVOKE category="license" type="issuer-key">
        <PUBLICKEY>
          <ALGORITHM>RSA-1024</ALGORITHM>
          <PARAMETER name="public exponent">
            <VALUE encoding="integer32">65537</VALUE>
          </PARAMETER>
          <PARAMETER name="modulus">
            <VALUE encoding="base64" size="1024">
AAn0kEAWU+1AFWtuUmBYL8Jza8tLhUv/BCmgcq/Pc08Au3DvXkH65s+0MEyZjM+71j3F1xaXUSst+wH2FjApkY1RxgL8VAKIuEvIy9hRrvY1YhJx/0Ite5fZeg2crUFrmoQgZzaJ50FvoakA2QMgZZgxoQmwiGE0y40cEJtIlE0=
            </VALUE>
          </PARAMETER>
        </PUBLICKEY>
      </REVOKE>
```

<span id="BKMK_5"></span>
#### Odwołanie certyfikatów i licencji na podstawie identyfikatora wystawcy

W tym przykładzie przedstawiono odwołanie zestawu certyfikatów lub licencji na podstawie identyfikatora wystawcy. Zawartość tagu &lt;ID&gt; pochodzi tutaj z węzła &lt;BODY&gt;&lt;ISSUER&gt;&lt;OBJECT&gt;&lt;ID&gt; odwoływanych certyfikatów lub licencji.

```
	      <REVOKE category="license" type="issuer-id">
        <OBJECT type="MS-DRM-Server">
          <ID type="MS-GUID">{2BE9E200-3040-41B9-8832-D4D0445EBBD6}</ID> 
        </OBJECT>
      </REVOKE>
```
	
> [!note]  
> Przy określaniu typu identyfikatora należy zwrócić uwagę, aby pomiędzy unikatowym identyfikatorem globalnym (GUID) a tagiem zamykającym nie występował znak powrotu karetki. W razie przypadkowego wstawienia znaku powrotu karetki klient RMS nie będzie mógł przetworzyć listy odwołania. 

<span id="BKMK_6"></span>
#### Odwołanie zawartości na podstawie identyfikatora zawartości

W tym przykładzie przedstawiono odwołanie chronionej zawartości na podstawie jej identyfikatora. Jest to zalecana metoda odwołania zawartości, ponieważ we wszystkich licencjach użytkowania utworzonych na podstawie danej licencji publikacji identyfikator zawartości jest taki sam. Wartość występującego tutaj węzła &lt;OBJECT&gt; można znaleźć w węźle &lt;BODY&gt;&lt;WORK&gt;&lt;OBJECT&gt; licencji publikacji lub licencji użytkowania danej zawartości.

```
<REVOKE category="content" type="content-id">
        <OBJECT type="Microsoft Office Document">
          <ID type="MS-GUID">{8702641D-3512-4AA4-A584-84C703A5B5C0}</ID>
        </OBJECT>
      </REVOKE>
```
        
> [!note]  
> Przy określaniu typu identyfikatora należy zwrócić uwagę, aby pomiędzy unikatowym identyfikatorem globalnym (GUID) a tagiem zamykającym nie występował znak powrotu karetki. W razie przypadkowego wstawienia znaku powrotu karetki klient RMS nie będzie mógł przetworzyć listy odwołania. 

<span id="BKMK_10"></span>
#### Odwołanie podmiotów zabezpieczeń na podstawie konta systemu Windows

W tym przykładzie przedstawiono odwołanie użytkownika lub włączającego podmiotu zabezpieczeń na podstawie jego konta Windows. Zawartość elementu &lt;OBJECT&gt; pochodzi tutaj z węzła &lt;BODY&gt;&lt;ISSUEDPRINCIPALS&gt;&lt;PRINCIPAL&gt;&lt;OBJECT&gt; certyfikatu konta praw lub licencji użytkowania.

```
<REVOKE category="principal" type="principal-id">
        <OBJECT type="Group-Identity">
          <ID type="Windows">{Windows account SID}</ID> 
          <NAME>{E-mail address}</NAME> 
        </OBJECT>
      </REVOKE>
```	  
   
> [!note]  
> Przy określaniu typu identyfikatora należy zwrócić uwagę, aby pomiędzy identyfikatorem SID konta Windows a tagiem zamykającym nie występował znak powrotu karetki. W razie przypadkowego wstawienia znaku powrotu karetki klient RMS nie będzie mógł przetworzyć listy odwołania. 

<span id="BKMK_7"></span>
#### Odwołanie podmiotów zabezpieczeń na podstawie Windows Live ID

W tym przykładzie przedstawiono odwołanie użytkownika lub włączającego podmiotu zabezpieczeń na podstawie jego identyfikatora Windows Live™ ID. Zawartość elementu &lt;OBJECT&gt; pochodzi tutaj z węzła &lt;BODY&gt;&lt;ISSUEDPRINCIPALS&gt;&lt;PRINCIPAL&gt;&lt;OBJECT&gt; certyfikatu konta praw lub licencji użytkowania.

```
<REVOKE category="principal" type="principal-id">
        <OBJECT type="Group-Identity">
          <ID type="Passport">{PUID}</ID> 
          <NAME>michael@contoso.com</NAME> 
        </OBJECT>
      </REVOKE>
```

> [!note]  
> Przy określaniu typu identyfikatora należy zwrócić uwagę, aby pomiędzy unikatowym identyfikatorem podmiotu (PUID) a tagiem zamykającym nie występował znak powrotu karetki. W razie przypadkowego wstawienia znaku powrotu karetki klient RMS nie będzie mógł przetworzyć listy odwołania. 

<span id="BKMK_8"></span>
Wstawianie podpisu do listy odwołania
-------------------------------------

Po utworzeniu listy odwołania należy do niej wstawić podpis w sposób opisany w tym temacie. Następnie listę odwołania można udostępnić użytkownikom w lokalizacji określonej adresem URL w odpowiednim szablonie zasad praw dostępu.

Pierwszym krokiem, który należy wykonać w celu wstawienia podpisu, jest wygenerowanie pary kluczy i pliku kluczy dla listy odwołania za pomocą narzędzia silnych nazw (Sn.exe). Narzędzie Sn.exe wchodzi w skład zestawu SDK 1.1 platformy Microsoft .NET Framework, który jest dostępny w witrynie firmy Microsoft w sieci Web [http://go.microsoft.com/fwlink/?LinkId=104796](http://go.microsoft.com/fwlink/?linkid=104796).

Aby możliwe było podpisanie za pomocą narzędzia RLsigner.exe, plik listy odwołania musi być zapisany jako plik unicode.

**Aby za pomocą narzędzia Sn.exe wygenerować nową parę kluczy i wpisać tę parę do pliku:**
1.  Utwórz klucz prywatny. W wierszu polecenia wpisz poniższe polecenie, a następnie naciśnij klawisz ENTER:

    **sn -k** *plik\_klucza\_prywatnego***.snk**

    gdzie *plik\_klucza\_prywatnego* to nazwa pliku klucza.

2.  Za pomocą narzędzia Sn.exe wyodrębnij klucz publiczny z pliku pary kluczy utworzonego w kroku 1 i wyeksportuj go do osobnego pliku. Wpisz następujące polecenie, a następnie naciśnij klawisz ENTER:

    **sn -p** *plik\_klucza\_prywatnego plik\_klucza\_publicznego*

    gdzie *plik\_klucza\_prywatnego* to nazwa pliku klucza prywatnego utworzonego w kroku 1, a *plik\_klucza\_publicznego* to nazwa pliku, w którym zostanie zapisany wyeksportowany klucz publiczny.

3.  Do użycia z programem RLsigner.exe należy zmienić rozszerzenie nazwy pliku klucza prywatnego (utworzonego w kroku 1) z .snk na .dat.

4.  Użyj narzędzia RLsigner.exe, aby wstawić podpis do pliku listy odwołań. Narzędzie to jest dołączone do programu RMS. Domyślnie znajduje się ono w katalogu %systemdrive%\\Program Files\\Windows Rights Management Services\\Tools.

> [!note]  
> Narzędzie RLsigner.exe nie obsługuje nazw plików, które zawierają spacje. 

<span id="BKMK_9"></span>
Korzystanie z narzędzia RLsigner.exe
------------------------------------

Po uruchomieniu narzędzia RLsigner.exe najpierw tworzy ono podpis przy użyciu klucza prywatnego dostarczonego w pliku kluczy. Następnie tworzy ono plik wyjściowy w oparciu o dostarczony plik listy odwołania.

> [!Important]  
> Aby możliwe było podpisanie za pomocą narzędzia RLsigner.exe, plik listy odwołania musi być zapisany jako plik unicode. 

Aby podpisać listę odwołania za pomocą narzędzia RLsigner.exe, wpisz następujące polecenie w wierszu polecenia:

**rlsigner.exe** *plik\_wej* **{-f** *plik\_kluczy* **| -h** *nazwa\_kontenera* **CSP}** *plik\_wyj*

W uzupełnianiu parametrów wejściowych polecenia pomocne będą następujące informacje:


<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Parametr</th>
<th style="border:1px solid black;" >Opis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><em>plik-wej</em></td>
<td style="border:1px solid black;">Nazwa przygotowanego pliku listy odwołania zgodnego z językiem XrML</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><em>plik_kluczy</em></td>
<td style="border:1px solid black;">Nazwa pliku zawierającego zarówno wygenerowany klucz publiczny, jak i prywatny</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><em>nazwa_kontenera</em></td>
<td style="border:1px solid black;">Nazwa kontenera klucza</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><em>plik_wyj</em></td>
<td style="border:1px solid black;">Nazwa podpisanego pliku listy odwołania, który zostanie utworzony przez narzędzie</td>
</tr>
</tbody>
</table>
  
> [!note]  
> Narzędzie RLsigner.exe nie obsługuje nazw plików, które zawierają spacje. 
  
W poniższych przykładach opisano, jak w wierszu polecenia można użyć narzędzia RLsigner.exe z różnymi dostawcami usług kryptograficznych:
  
-   Przykładowa składnia wiersza polecenia z zastosowaniem pliku kluczy:  
    **rlsigner.exe lo.xml -f klucz.dat wyjscie.xml**  
-   Przykładowa składnia wiersza polecenia z zastosowaniem sprzętowego modułu zabezpieczeń:  
    **rlsigner.exe lo.xml -h Kontener CSP wyjscie.xml**
  
W kodzie zwracanym przez narzędzie RLsigner.exe znajdują się podstawowe informacje na temat błędów i powodzenia. Możliwe kody zwracane przez narzędzie opisano w poniższej tabeli.
  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Zwrócony kod</th>
<th style="border:1px solid black;" >Opis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">0</td>
<td style="border:1px solid black;">Powodzenie</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">-1</td>
<td style="border:1px solid black;">Nie można odczytać pliku źródłowego</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">-2</td>
<td style="border:1px solid black;">Nie można odczytać pliku kluczy</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">-3</td>
<td style="border:1px solid black;">Nieprawidłowy plik kluczy</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">-4</td>
<td style="border:1px solid black;">Nieprawidłowy plik źródłowy</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">-5</td>
<td style="border:1px solid black;">Nie można zapisać danych do pliku źródłowego</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">-6</td>
<td style="border:1px solid black;">Nieznany błąd</td>
</tr>
</tbody>
</table>
  
Podpisywanie list odwołania można zaplanować zgodnie z częstotliwością odświeżania określoną na serwerze.
  
Proces podpisywania list odwołania można zautomatyzować za pomocą skryptów. Poniższy przykładowy skrypt VBScript powoduje wywołanie narzędzia RLsigner.exe i wpisanie wyników do dziennika zdarzeń systemowych.
  
```VB
const EVT_SUCCESS       = 0
const EVT_ERROR         = 1
const EVT_WARNING       = 2
const EVT_INFORMATION   = 4
const EVT_AUDIT_SUCCESS = 8
const EVT_AUDIT_FAILURE = 16

Dim WshShell, oExec

Set WshShell = CreateObject( "WScript.Shell" )
Set oExec = WshShell.Exec("rlsigner.exe input_file key_file output_file")
Do While oExec.Status = 0
     WScript.Sleep 100
Loop

if WshShell.ExitCode <> 0 Then
    WshShell.LogEvent EVT_ERROR, "RLsigner failed with error """ + WshShell.ExitCode + """"
else
    WshShell.LogEvent EVT_SUCCESS, "RLsigner completed successfully"
end if
```
