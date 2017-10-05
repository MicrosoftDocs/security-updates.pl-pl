---
TOCTitle: Zastępowanie odnajdowania usługi Active Directory
Title: Zastępowanie odnajdowania usługi Active Directory
ms:assetid: '9d97e7fb-5b05-4853-ad7b-6cc82b9729f0'
ms:contentKeyID: 18123360
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747614(v=WS.10)'
---

Zastępowanie odnajdowania usługi Active Directory
=================================================

Usługi RMS i klienci wykrywają lokalizacje usług, sprawdzając najpierw lokalny rejestr. Jeśli określone klucze rejestru nie mają wartości, usługi RMS i klienci będą szukać punktu połączenia usługi w katalogu Active Directory. Oznacza to, że można zastąpić domyślne ustawienia wykrywania usług Active Directory, wpisując określone klucze do rejestru klienta lub serwera.

| ![](images/Cc747614.note(WS.10).gif)Uwaga                                                                                                                                         |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Jeśli klaster główny programu RMS został skonfigurowany tak, aby nie publikować punktu połączenia usługi w katalogu Active Directory, przy użyciu tych kluczy można wskazać właściwą lokalizację klientom RMS. |

Niniejsza sekcja zawiera opis wpisów w rejestrze oraz szczegółowe informacje na temat ich tworzenia.

Zastępowanie wykrywania usług dla rejestrowania podrzędnego klastra przeznaczonego tylko do licencjonowania
-----------------------------------------------------------------------------------------------------------

Jeśli użytkownik zastrzega klaster przeznaczony tylko do licencjonowania i chce, aby został on zarejestrowany podrzędnie w innym klastrze głównym niż klaster główny wdrożony w lesie Active Directory klastra przeznaczonego tylko do licencjonowania, konieczne jest zastąpienie wykrywania usług rejestrowania podrzędnego i certyfikowania konta.

#### Opisy wpisów rejestru

Do zastąpienia usług rejestrowania podrzędnego i certyfikowania konta służą następujące wpisy do rejestru.

-   **SubEnrollmentURL**. Ten wpis określa ścieżkę do klastra głównego, z której korzysta serwer licencji, żądając swego certyfikatu licencjodawcy serwera.
-   **GicURL**. Ten wpis określa ścieżkę do usługi certyfikowania konta dla danego klastra przeznaczonego tylko do licencjonowania.

#### Szczegóły wpisu

Na komputerach z 32-bitową wersją systemu Windows Server 2003 pełna ścieżka do podklucza rejestru dla wpisów dotyczących wykrywania usług dla rejestrowania podrzędnego klastra przeznaczonego tylko do licencjonowania ma postać:

**HKEY\_LOCAL\_MACHINE\\Software\\Microsoft\\DRMS\\1.0**

Na komputerach z 64-bitową wersją systemu Windows Server 2003 pełna ścieżka do podklucza rejestru dla wpisów dotyczących wykrywania usług dla rejestrowania podrzędnego klastra przeznaczonego tylko do licencjonowania ma postać:

**HKEY\_LOCAL\_MACHINE\\SoftwareWOW6432Node\\Microsoft\\DRMS\\1.0**

W poniższej tabeli znajduje się lista wpisów, które można dodać w celu zastąpienia wykrywania usług.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Nazwa</th>
<th style="border:1px solid black;" >Typ</th>
<th style="border:1px solid black;" >wartość</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">SubEnrollmentURL</td>
<td style="border:1px solid black;">Ciąg</td>
<td style="border:1px solid black;">http(lub https)://<em>nazwa_serwera</em>/_wmcs/certification/subenrollservice.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">GicURL</td>
<td style="border:1px solid black;">Ciąg</td>
<td style="border:1px solid black;">http(lub https)://<em>nazwa_serwera</em>/_wmcs/certification/certification.asmx</td>
</tr>
</tbody>
</table>
  
Zastępowanie wykrywania usług po stronie klienta do celów publikacji  
--------------------------------------------------------------------
  
Jeśli użytkownicy będą publikować zawartość pochodzącą z ich komputerów, w zależności od topologii zastosowanej w przedsiębiorstwie może być potrzebne zastąpienie lokalizacji serwerów używanych do publikowania. Standardowo, lokalizacje serwerów używanych do publikowania są wykrywane przez klienta przy użyciu usługi Active Directory. Dodanie odpowiednich kluczy rejestru na komputerach klienckich spowoduje, że klienci obejdą te metody i zamiast tego użyją adresów URL, które zostaną zdefiniowane w wartościach wpisów rejestru.
  
| ![](images/Cc747614.note(WS.10).gif)Uwaga                                                                                                               |  
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Wymienione w tych sekcjach zastąpienia dla klientów powinny być utworzone jako klucze, a nie indywidualne wpisy. Ich wartości należy utworzyć w domyślnych wpisach każdego z kluczy. |
  
#### Opisy kluczy rejestru
  
Do zastąpienia automatycznego wykrywania klastra RMS można użyć następujących kluczy rejestru.
  
-   **Activation**. Ten klucz rejestru definiuje adres URL usługi aktywacji danego komputera. Jeśli użytkownik korzysta z klienta RMS z dodatkiem Service Pack 1 lub nowszym, ten wpis jest nieużywany.  
-   **EnterprisePublishing**. Ten klucz rejestru definiuje adres URL instalacji RMS, której dany klient powinien używać w odniesieniu do żądań licencji.  
-   **CloudPublishing**. Ten klucz rejestru definiuje adres URL udostępnianej przez firmę Microsoft usługi licencjonowania, która może być użyta, gdy klient nie ma dostępu do instalacji RMS, ale ma dostęp do Internetu.
  
#### Szczegóły klucza
  
Pełna ścieżka do podklucza rejestru dla wpisów dotyczących wykrywania usług po stronie klienta dla publikowania ma postać:
  
**HKEY\_LOCAL\_MACHINE\\Software\\Microsoft\\MSDRM\\ServiceLocation\\**
  
W poniższej tabeli znajduje się lista kluczy rejestru, które można dodać na komputerze klienckim RMS w celu zastąpienia wykrywania usług.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Nazwa</th>
<th style="border:1px solid black;" >Typ</th>
<th style="border:1px solid black;" >wartość</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Aktywacja</td>
<td style="border:1px solid black;">Ciąg</td>
<td style="border:1px solid black;">http(lub https)://<em>nazwa_klastra_RMS</em>/_wmcs/Certification (<em>nazwa_klastra_RMS</em> to nazwa klastra użytkownika).</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">EnterprisePublishing</td>
<td style="border:1px solid black;">Ciąg</td>
<td style="border:1px solid black;">http(lub https)://<em>nazwa_klastra_RMS</em>/_wmcs/Licensing (<em>nazwa_klastra_RMS</em> to nazwa klastra użytkownika).</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">CloudPublishing</td>
<td style="border:1px solid black;">Ciąg</td>
<td style="border:1px solid black;">http(lub https)://<em>nazwa_klastra_FQDN</em>/_wmcs/Licensing (<em>nazwa_klastra_FQDN</em> to w pełni kwalifikowana nazwa domeny klastra RMS).</td>
</tr>
</tbody>
</table>
  
Zaleca się, aby omawiane klucze rejestru były wdrażane przy użyciu programu Systems Management Server lub Zasad grupy, co pozwoli mieć pewność, że wszyscy klienci w przedsiębiorstwie korzystają z prawidłowych serwerów publikowania.
  
| ![](images/Cc747614.Caution(WS.10).gif)Przestroga                                                                                                                             |  
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Niewłaściwe modyfikacje rejestru mogą powodować poważne uszkodzenie systemu. Przed wprowadzeniem zmian w rejestrze należy utworzyć kopie zapasowe wszystkich ważnych danych przechowywanych na komputerze. |
  
Do zaimportowania właściwych kluczy rejestru do każdego serwera w klastrze RMS można użyć przykładowego pliku rejestru (.reg).
  
**Aby zaimportować właściwe klucze rejestru do wszystkich serwerów w klastrze RMS**  
1.  Skopiuj poniższy plik rejestru do Notatnika.
  
    `Windows Registry Editor Version 5.00`
  
    `[HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\MSDRM\ServiceLocation]`
  
    `[HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\MSDRM\ServiceLocation\Activation]`
  
    `@="http://<RMS_cluster_name>/_wmcs/certification"`
  
    `[HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\MSDRM\ServiceLocation\EnterprisePublishing]`
  
    `@="http://<RMS_cluster_name>/_wmcs/licensing"`
  
2.  Zastąp ciąg &lt;nazwa\_klastra\_RMS&gt; nazwą klastra RMS.
  
3.  Zapisz plik z rozszerzeniem .reg.
  
4.  Kliknij dwukrotnie nazwę tego pliku w programie Eksplorator Windows.
  
5.  Jeśli wyświetlone zostanie okno dialogowe **Kontrola konta użytkownika**, potwierdź chęć wyświetlenia akcji, a następnie kliknij przycisk **Kontynuuj**.. Kliknij opcję **Tak**, gdy zostanie wyświetlone pytanie, czy chcesz dodać informacje do rejestru.
