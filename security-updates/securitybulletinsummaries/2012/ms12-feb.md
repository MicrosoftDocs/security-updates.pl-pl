---
TOCTitle: 'MS12-FEB'
Title: 'Podsumowanie biuletynów zabezpieczeń firmy Microsoft za luty 2012 r.'
ms:assetid: 'ms12-feb'
ms:contentKeyID: 61233134
ms:mtpsurl: 'https://technet.microsoft.com/pl-PL/library/ms12-feb(v=Security.10)'
---
Podsumowanie biuletynów zabezpieczeń firmy Microsoft za luty 2012 r.
====================================================================

Opublikowano: 14 lutego 2012

**Wersja:** 1.0

Niniejsze podsumowanie biuletynów zabezpieczeń zawiera spis biuletynów za luty 2012 r.

Z chwilą opublikowania biuletynów zabezpieczeń za luty 2012 r. niniejsze podsumowanie biuletynów zastępuje powiadomienie o biuletynach zabezpieczeń wydane 9 lutego 2012 r. Aby uzyskać więcej informacji na temat usługi powiadamiania o biuletynach, zobacz [Powiadomienia o biuletynach zabezpieczeń firmy Microsoft (j. ang.)](http://go.microsoft.com/fwlink/?linkid=217213).

Aby dowiedzieć się, jak otrzymywać automatyczne powiadomienia o publikacji biuletynów zabezpieczeń firmy Microsoft, odwiedź stronę [Microsoft Technical Security Notifications](http://go.microsoft.com/fwlink/?linkid=21163).

15 lutego 2012 r. o godz. 11:00 czasu Pacyfiku (godz. 20:00 czasu środkowoeuropejskiego) firma Microsoft udostępni emisję internetową, w której znajdą się odpowiedzi na pytania klientów dotyczące tych biuletynów (USA i Kanada). Zarejestruj się, aby zobaczyć [emisję internetową dotyczącą biuletynów zabezpieczeń za luty](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032499501). Po tym dniu emisja internetowa będzie dostępna na żądanie. Aby uzyskać więcej informacji, zobacz [Podsumowania biuletynów zabezpieczeń i emisje internetowe firmy Microsoft](http://go.microsoft.com/fwlink/?linkid=217214).

Firma Microsoft udostępnia także informacje, dzięki którym klienci mogą ustalić priorytety dla aktualizacji zabezpieczeń w związku z niezwiązanymi z zabezpieczeniami aktualizacjami, które publikowane są w tym samym dniu, co comiesięczne aktualizacje zabezpieczeń. Zapoznaj się z sekcją **Inne informacje**.

### Informacje o biuletynie

Streszczenia
------------

<span></span>
Następująca tabela zawiera podsumowanie biuletynów zabezpieczeń za ten miesiąc (uporządkowanych według wskaźnika ważności).

Szczegółowe informacje o programach, których dotyczy luka, znajdują się w następnej sekcji, **Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki**.

 
<table style="border:1px solid black;">
<thead>
<tr class="header">
<th style="border:1px solid black;" >Identyfikator biuletynu</th>
<th style="border:1px solid black;" >Tytuł biuletynu i streszczenie</th>
<th style="border:1px solid black;" >Maksymalny wskaźnik ważności oraz wpływ luki</th>
<th style="border:1px solid black;" >Wymaganie dotyczące ponownego uruchomienia</th>
<th style="border:1px solid black;" >Programy, których dotyczy problem</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=238387">MS12-008</a></td>
<td style="border:1px solid black;"><strong>Luki w zabezpieczeniach sterowników trybu jądra systemu Windows umożliwiają zdalne wykonanie kodu (2660465)</strong><br />
<br />
Ta aktualizacja zabezpieczeń usuwa dwie luki w zabezpieczeniach systemu Microsoft Windows — jedną zgłoszoną przez użytkowników, a jedną przez organizację publiczną. Poważniejsza z tych luk umożliwia zdalne wykonanie kodu, jeśli użytkownik odwiedzi witrynę sieci Web zawierającą specjalnie spreparowaną treść albo lokalnie uruchomi specjalnie spreparowaną aplikację. Osoba atakująca nie może w żaden sposób zmusić użytkowników do odwiedzenia złośliwej witryny. Musi przekonać użytkowników do odwiedzenia takiej witryny, najczęściej zachęcając do kliknięcia łącza w wiadomości e-mail lub wiadomości błyskawicznej, które przekieruje ich do witryny osoby atakującej.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Krytyczny</a><br />
Zdalne wykonanie kodu</td>
<td style="border:1px solid black;">Wymaga ponownego uruchomienia komputera</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=236989">MS12-010</a></td>
<td style="border:1px solid black;"><strong>Zbiorcza aktualizacja zabezpieczeń dla programu Internet Explorer (2647516)</strong><br />
<br />
Niniejsza aktualizacja zabezpieczeń usuwa cztery luki w zabezpieczeniach programu Internet Explorer, które zostały zgłoszone przez użytkowników. Najpoważniejsze z tych luk umożliwiają zdalne wykonanie kodu, jeśli użytkownik wyświetli specjalnie spreparowaną stronę sieci Web przy użyciu programu Internet Explorer. Osoba atakująca, której uda się wykorzystać jedną z tych luk, może uzyskać takie same uprawnienia jak zalogowany użytkownik. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Krytyczny</a><br />
Zdalne wykonanie kodu</td>
<td style="border:1px solid black;">Wymaga ponownego uruchomienia komputera</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=238617">MS12-013</a></td>
<td style="border:1px solid black;"><strong>Luka w zabezpieczeniach biblioteki wykonawczej dla języka C umożliwia zdalne wykonanie kodu (2654428)</strong><br />
<br />
Ta aktualizacja zabezpieczeń usuwa lukę w zabezpieczeniach systemu Microsoft Windows. Luka może pozwalać na zdalne wykonanie kodu, jeśli użytkownik otworzy specjalnie spreparowany plik multimedialny umieszczony w witrynie sieci Web lub wysłany jako załącznik do poczty e-mail. Osoba atakująca, której uda się wykorzystać lukę, może uzyskać takie same prawa użytkownika, jak użytkownik lokalny. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Krytyczny</a><br />
Zdalne wykonanie kodu</td>
<td style="border:1px solid black;">Wymaga ponownego uruchomienia komputera</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=235370">MS12-016</a></td>
<td style="border:1px solid black;"><strong>Luki w zabezpieczeniach systemu .NET Framework i programu Microsoft Silverlight umożliwiają zdalne wykonanie kodu (2651026)</strong><br />
<br />
Niniejsza aktualizacja zabezpieczeń usuwa dwie luki w zabezpieczeniach programów Microsoft .NET Framework i Microsoft Silverlight, z których jedną zgłosiły organizacje publiczne, a drugą użytkownicy. Luki w zabezpieczeniach umożliwiają zdalne wykonanie kodu w systemie klienta, jeśli użytkownik wyświetli specjalnie spreparowaną stronę sieci Web w przeglądarce sieci Web obsługującej aplikacje przeglądarki XAML (XBAP) lub aplikacje Silverlight. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Krytyczny</a><br />
Zdalne wykonanie kodu</td>
<td style="border:1px solid black;">Może wymagać ponownego uruchomienia</td>
<td style="border:1px solid black;">Microsoft .NET Framework,<br />
Microsoft Silverlight</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=238474">MS12-009</a></td>
<td style="border:1px solid black;"><strong>Luki w zabezpieczeniach pomocniczego sterownika funkcji umożliwia podniesienie uprawnień (2645640)</strong><br />
<br />
Ta aktualizacja zabezpieczeń usuwa dwie luki w zabezpieczeniach systemu Windows, które zostały zgłoszone przez użytkowników. Luki te mogą umożliwić podniesienie uprawnień, jeśli osoba atakująca zaloguje się do systemu użytkownika i uruchomi specjalnie spreparowaną aplikację. Osoba atakująca musi dysponować prawidłowymi poświadczeniami logowania oraz być w stanie zalogować się lokalnie, aby wykorzystać możliwości stwarzane przez luki.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Ważny</a><br />
Podniesienie uprawnień</td>
<td style="border:1px solid black;">Wymaga ponownego uruchomienia komputera</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=238500">MS12-011</a></td>
<td style="border:1px solid black;"><strong>Luki w zabezpieczeniach programu Microsoft SharePoint umożliwiają podniesienie poziomu uprawnień (2663841)</strong><br />
<br />
Ta aktualizacja zabezpieczeń usuwa trzy luki w zabezpieczeniach programów Microsoft SharePoint i Microsoft SharePoint Foundation, które zostały zgłoszone przez użytkowników. Luki te umożliwiają podniesienie poziomu uprawnień lub ujawnienie informacji, jeśli użytkownik kliknie specjalnie spreparowany adres URL.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Ważny</a><br />
Podniesienie uprawnień</td>
<td style="border:1px solid black;">Może wymagać ponownego uruchomienia</td>
<td style="border:1px solid black;">Microsoft Office,<br />
Oprogramowanie serwerów firmy Microsoft</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=239941">MS12-012</a></td>
<td style="border:1px solid black;"><strong>Luka w zabezpieczeniach apletu Panel sterowania kolorami może pozwolić na zdalne wykonanie kodu (2643719)</strong><br />
<br />
Ta aktualizacja zabezpieczeń usuwa lukę w zabezpieczeniach systemu Microsoft Windows ujawnioną przez organizację publiczną. Luka ta umożliwia zdalne wykonanie kodu, gdy użytkownik otworzy prawidłowy plik (na przykład plik .icm lub .icc), który znajduje się w tym samym katalogu, co specjalnie spreparowany plik biblioteki dołączanej dynamicznie (DLL). Osoba atakująca, której uda się wykorzystać tę lukę, może uzyskać takie same uprawnienia, jak zalogowany użytkownik. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Ważny</a><br />
Zdalne wykonanie kodu</td>
<td style="border:1px solid black;">Może wymagać ponownego uruchomienia</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=239945">MS12-014</a></td>
<td style="border:1px solid black;"><strong>Luka w zabezpieczeniach kodera-dekodera Indeo umożliwia zdalne wykonanie kodu (2661637)</strong><br />
<br />
Ta aktualizacja zabezpieczeń usuwa lukę w zabezpieczeniach systemu Microsoft Windows ujawnioną przez organizację publiczną. Luka ta umożliwia zdalne wykonanie kodu, gdy użytkownik otworzy prawidłowy plik (na przykład .avi) znajdujący się w tym samym katalogu, co specjalnie spreparowany plik biblioteki dołączanej dynamicznie (DLL). Osoba atakująca, której uda się wykorzystać tę lukę, może uruchomić dowolny kod jako użytkownik zalogowany. Osoba taka mogłaby wówczas instalować programy, przeglądać, zmieniać i usuwać dane oraz tworzyć nowe konta z pełnymi uprawnieniami. Jeśli użytkownik jest zalogowany jako administrator, osoba atakująca może uzyskać pełną kontrolę nad systemem podlegającym luce. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Ważny</a><br />
Zdalne wykonanie kodu</td>
<td style="border:1px solid black;">Może wymagać ponownego uruchomienia</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=238400">MS12-015</a></td>
<td style="border:1px solid black;"><strong>Luki w zabezpieczeniach programu Microsoft Visio Viewer 2010 umożliwiają zdalne wykonanie kodu (2663510)</strong><br />
<br />
Ta aktualizacja zabezpieczeń usuwa pięć luk w zabezpieczeniach pakietu Microsoft Office, które zostały zgłoszone przez użytkowników. Luki te mogą umożliwić zdalne wykonanie kodu, jeśli użytkownik otworzy specjalnie spreparowany plik programu Visio. Osoba atakująca, której uda się wykorzystać te luki, może uzyskać takie same uprawnienia jak zalogowany użytkownik. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Ważny</a><br />
Zdalne wykonanie kodu</td>
<td style="border:1px solid black;">Może wymagać ponownego uruchomienia</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
</tbody>
</table>
  
Wskaźnik możliwości wykorzystania luki  
--------------------------------------
  
<span></span>
Poniższa tabela przedstawia ocenę możliwości wykorzystania luk dla każdej luki opisywanej w tym miesiącu. Luki są wymienione wg identyfikatora biuletynu, a następnie identyfikatora CVE. Uwzględniono wyłącznie te luki, które w biuletynach mają nadany wskaźnik ważności „krytyczny” lub „ważny”.
  
**W jaki sposób korzystać z tej tabeli?**
  
Tabela ta pozwala sprawdzić prawdopodobieństwo, że w ciągu 30 dni od wydania biuletynu zabezpieczeń dla każdej z aktualizacji zabezpieczeń, których zainstalowanie może być potrzebne, wykorzystane zostaną możliwości wykonania kodu lub doprowadzenia do odmowy usług z wykorzystaniem luk w zabezpieczeniach. Aby ustalić priorytety wdrażania wydanych w tym miesiącu aktualizacji, zapoznaj się z dostępnymi poniżej ocenami, rozpatrując je w kontekście posiadanej konfiguracji. Więcej informacji na temat znaczenia tych ocen oraz sposobu ich dokonywania można znaleźć na stronie sieci Web [Microsoft Exploitability Index](http://technet.microsoft.com/security/cc998259.aspx).
  
W poniższych kolumnach sformułowanie „Najnowsza wersja programu” odnosi się do wersji omawianego oprogramowania, a sformułowanie „Starsze wersje programu” dotyczy wszystkich starszych, obsługiwanych wersji omawianego oprogramowania, wymienionych w biuletynie w tabelach „Programy, których dotyczy problem” lub „Programy, których nie dotyczy problem”
  
| Identyfikator biuletynu                                   | Nazwa luki w zabezpieczeniach                                                                        | CVE ID                                                                           | Ocena możliwości wykorzystania luki w najnowszej wersji programu                                              | Ocena możliwości wykorzystania luki w poprzedniej wersji programu                                             | Ocena możliwości wykorzystania luki w celu wytworzenia sytuacji typu „odmowa usługi” | Najważniejsze uwagi                                                                                                                                |  
|-----------------------------------------------------------|------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------|  
| [MS12-008](http://go.microsoft.com/fwlink/?linkid=238387) | Luka w zabezpieczeniach związana z użyciem układu klawiatury po zwolnieniu                           | [CVE-2012-0154](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0154) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny kod wykorzystujący lukę        | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny kod wykorzystujący lukę        | Nie dotyczy                                                                          | (Brak)                                                                                                                                             |  
| [MS12-008](http://go.microsoft.com/fwlink/?linkid=238387) | Luka w zabezpieczeniach związana z naruszeniem zasad dostępu do interfejsu GDI                       | [CVE-2011-5046](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-5046) | [2](http://technet.microsoft.com/en-us/security/cc998259.aspx) — kod wykorzystujący lukę trudny do utworzenia | [2](http://technet.microsoft.com/en-us/security/cc998259.aspx) — kod wykorzystujący lukę trudny do utworzenia | Stałe                                                                                | Informacje o tej luce są znane publicznie.                                                                                                         |  
| [MS12-009](http://go.microsoft.com/fwlink/?linkid=238474) | Luka w zabezpieczeniach modułu AfdPoll umożliwiająca podniesienie poziomu uprawnień                  | [CVE-2012-0148](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0148) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny kod wykorzystujący lukę        | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) — kod wykorzystujący lukę mało prawdopodobny   | Stałe                                                                                | W systemach opartych na procesorach x64 luka może zostać wykorzystana, w systemach z procesorami x86 — nie.                                        |  
| [MS12-009](http://go.microsoft.com/fwlink/?linkid=238474) | Luka w zabezpieczeniach pomocniczego sterownika funkcji umożliwiająca podniesienie uprawnień         | [CVE-2012-0149](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0149) | Brak zagrożenia                                                                                               | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny kod wykorzystujący lukę        | Stałe                                                                                | Działaniu luki podlega jedynie system Windows Server 2003.                                                                                         |  
| [MS12-010](http://go.microsoft.com/fwlink/?linkid=236989) | Luka w zabezpieczeniach układów stron HTML umożliwiająca zdalne wykonanie kodu                       | [CVE-2012-0011](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0011) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny kod wykorzystujący lukę        | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny kod wykorzystujący lukę        | Tymczasowy                                                                           | (Brak)                                                                                                                                             |  
| [MS12-010](http://go.microsoft.com/fwlink/?linkid=236989) | Luka w zabezpieczeniach związana z bajtem niezerowym umożliwiająca ujawnienie informacji             | [CVE-2012-0012](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0012) | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) — kod wykorzystujący lukę mało prawdopodobny   | Brak zagrożenia                                                                                               | Nie dotyczy                                                                          | Ta luka może doprowadzić do ujawnienia informacji.                                                                                                 |  
| [MS12-010](http://go.microsoft.com/fwlink/?linkid=236989) | Luka w zabezpieczeniach języka VML umożliwiająca zdalne wykonanie kodu                               | [CVE-2012-0155](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0155) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny kod wykorzystujący lukę        | Brak zagrożenia                                                                                               | Tymczasowy                                                                           | (Brak)                                                                                                                                             |  
| [MS12-011](http://go.microsoft.com/fwlink/?linkid=238500) | Luka w zabezpieczeniach dotycząca skryptów krzyżowych na stronie inplview.aspx                       | [CVE-2012-0017](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0017) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny kod wykorzystujący lukę        | Brak zagrożenia                                                                                               | Nie dotyczy                                                                          | (Brak)                                                                                                                                             |  
| [MS12-011](http://go.microsoft.com/fwlink/?linkid=238500) | Luka w zabezpieczeniach dotycząca skryptów krzyżowych na stronie themeweb.aspx                       | [CVE-2012-0144](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0144) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny kod wykorzystujący lukę        | Brak zagrożenia                                                                                               | Nie dotyczy                                                                          | (Brak)                                                                                                                                             |  
| [MS12-011](http://go.microsoft.com/fwlink/?linkid=238500) | Luka w zabezpieczeniach dotycząca skryptów krzyżowych na stronie wizardlist.aspx                     | [CVE-2012-0145](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0145) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny kod wykorzystujący lukę        | Brak zagrożenia                                                                                               | Nie dotyczy                                                                          | (Brak)                                                                                                                                             |  
| [MS12-012](http://go.microsoft.com/fwlink/?linkid=239941) | Luka w zabezpieczeniach Panelu sterowania kolorami związana z niebezpiecznym ładowaniem biblioteki   | [CVE-2010-5082](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-5082) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny kod wykorzystujący lukę        | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny kod wykorzystujący lukę        | Nie dotyczy                                                                          | Informacje o tej luce są znane publicznie.                                                                                                         |  
| [MS12-013](http://go.microsoft.com/fwlink/?linkid=238617) | Luka w zabezpieczeniach biblioteki Msvcrt.dll związana z przepełnieniem buforu                       | [CVE-2012-0150](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0150) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny kod wykorzystujący lukę        | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny kod wykorzystujący lukę        | Tymczasowy                                                                           | (Brak)                                                                                                                                             |  
| [MS12-014](http://go.microsoft.com/fwlink/?linkid=239945) | Luka w zabezpieczeniach kodera-dekodera dźwięku Indeo związana z niebezpiecznym ładowaniem bibliotek | [CVE-2010-3138](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3138) | Brak zagrożenia                                                                                               | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny kod wykorzystujący lukę        | Nie dotyczy                                                                          | Informacje o tej luce są znane publicznie.                                                                                                         |  
| [MS12-015](http://go.microsoft.com/fwlink/?linkid=238400) | Luka w zabezpieczeniach związana z uszkodzeniem pamięci formatu plików VSD                           | [CVE-2012-0019](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0019) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny kod wykorzystujący lukę        | Brak zagrożenia                                                                                               | Nie dotyczy                                                                          | Luka ta dotyczy programu Visio Viewer 2010 i Visio Viewer 2010 z dodatkiem Service Pack 1 (są to jedyne obsługiwane wersje programu Visio Viewer). |  
| [MS12-015](http://go.microsoft.com/fwlink/?linkid=238400) | Luka w zabezpieczeniach związana z uszkodzeniem pamięci formatu plików VSD                           | [CVE-2012-0020](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0020) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny kod wykorzystujący lukę        | Brak zagrożenia                                                                                               | Nie dotyczy                                                                          | Luka ta dotyczy programu Visio Viewer 2010 i Visio Viewer 2010 z dodatkiem Service Pack 1 (są to jedyne obsługiwane wersje programu Visio Viewer). |  
| [MS12-015](http://go.microsoft.com/fwlink/?linkid=238400) | Luka w zabezpieczeniach związana z uszkodzeniem pamięci formatu plików VSD                           | [CVE-2012-0136](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0136) | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) — kod wykorzystujący lukę mało prawdopodobny   | Brak zagrożenia                                                                                               | Nie dotyczy                                                                          | Luka ta dotyczy programu Visio Viewer 2010 i Visio Viewer 2010 z dodatkiem Service Pack 1 (są to jedyne obsługiwane wersje programu Visio Viewer). |  
| [MS12-015](http://go.microsoft.com/fwlink/?linkid=238400) | Luka w zabezpieczeniach związana z uszkodzeniem pamięci formatu plików VSD                           | [CVE-2012-0137](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0137) | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) — kod wykorzystujący lukę mało prawdopodobny   | Brak zagrożenia                                                                                               | Nie dotyczy                                                                          | Luka ta dotyczy programu Visio Viewer 2010 i Visio Viewer 2010 z dodatkiem Service Pack 1 (są to jedyne obsługiwane wersje programu Visio Viewer). |  
| [MS12-015](http://go.microsoft.com/fwlink/?linkid=238400) | Luka w zabezpieczeniach związana z uszkodzeniem pamięci formatu plików VSD                           | [CVE-2012-0138](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0138) | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) — kod wykorzystujący lukę mało prawdopodobny   | Brak zagrożenia                                                                                               | Nie dotyczy                                                                          | Luka ta dotyczy programu Visio Viewer 2010 i Visio Viewer 2010 z dodatkiem Service Pack 1 (są to jedyne obsługiwane wersje programu Visio Viewer). |  
| [MS12-016](http://go.microsoft.com/fwlink/?linkid=235370) | Luka w zabezpieczeniach systemu .NET Framework związana z niezarządzanymi obiektami                  | [CVE-2012-0014](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0014) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny kod wykorzystujący lukę        | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny kod wykorzystujący lukę        | Nie dotyczy                                                                          | (Brak)                                                                                                                                             |  
| [MS12-016](http://go.microsoft.com/fwlink/?linkid=235370) | Luka w zabezpieczeniach systemu .NET Framework związana z uszkodzeniem stosu                         | [CVE-2012-0015](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0015) | Brak zagrożenia                                                                                               | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny kod wykorzystujący lukę        | Nie dotyczy                                                                          | Informacje o tej luce są znane publicznie.                                                                                                         |
  
Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki  
---------------------------------------------------------------------------------
  
<span></span>
Poniższe tabele wymieniają biuletyny według najważniejszych kategorii programów i wskaźnika ważności.
  
**Jak korzystać z tych tabel?**
  
Tabele te pozwalają odczytać informacje o aktualizacjach zabezpieczeń, których zainstalowanie może być konieczne. Należy zapoznać się z informacjami dotyczącymi każdego wymienionego programu lub składnika oprogramowania w celu sprawdzenia, czy aktualizacje zabezpieczeń odnoszą się do danej instalacji. Jeśli program lub składnik znajduje się na liście, dostępne jest łącze prowadzące do aktualizacji oprogramowania i podana jest informacja o wskaźniku ważności tej aktualizacji.
  
**Uwaga** Konieczne może być zainstalowanie kilku aktualizacji zabezpieczeń dotyczących jednej luki. Przejrzyj całą kolumnę dla każdego wymienionego identyfikatora biuletynu, aby sprawdzić, jakie aktualizacje musisz zainstalować, w oparciu o programy bądź składniki zainstalowane w systemie.
  
#### System operacyjny Windows i jego składniki:

 
<table style="border:1px solid black;">
<tr>
<th colspan="8">
Windows XP  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS12-008**](http://go.microsoft.com/fwlink/?linkid=238387)
</td>
<td style="border:1px solid black;">
[**MS12-010**](http://go.microsoft.com/fwlink/?linkid=236989)
</td>
<td style="border:1px solid black;">
[**MS12-013**](http://go.microsoft.com/fwlink/?linkid=238617)
</td>
<td style="border:1px solid black;">
[**MS12-016**](http://go.microsoft.com/fwlink/?linkid=235370)
</td>
<td style="border:1px solid black;">
[**MS12-009**](http://go.microsoft.com/fwlink/?linkid=238474)
</td>
<td style="border:1px solid black;">
[**MS12-012**](http://go.microsoft.com/fwlink/?linkid=239941)
</td>
<td style="border:1px solid black;">
[**MS12-014**](http://go.microsoft.com/fwlink/?linkid=239945)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Zbiorczy wskaźnik ważności**
</td>
<td style="border:1px solid black;">
[**Krytyczny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Krytyczny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Brak
</td>
<td style="border:1px solid black;">
[**Krytyczny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Brak
</td>
<td style="border:1px solid black;">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP z dodatkiem Service Pack 3
</td>
<td style="border:1px solid black;">
[Windows XP z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=832afe5e-d61e-4554-b889-9174df042b32)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=a7d59fa8-0a49-4985-9f14-92218d3b5cea)  
(Umiarkowany)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=6025c5d6-696c-49cd-9264-96af5766d318)  
(Krytyczny)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=5b37f5b1-207f-4fa1-9769-c873d672e80c)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5269e18b-d4f0-4c64-8df8-283a2ca66c59)  
(KB2633880)  
(Krytyczny)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=70aadf34-abdc-4577-8da9-a0669dccc119)<sup>[1]</sup>
(KB2633870)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows XP z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=32e5c9ad-b610-4afb-b6f0-bb0b5fbdd1f6)  
(Ważny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ff2c141c-08b4-42c6-9f66-580f8678c01f)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=96d404e7-8928-494e-8a3c-3897817cda7b)  
(Umiarkowany)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=b40bc334-edbc-48d5-9196-b7fb0e19966e)  
(Krytyczny)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=2fc9d519-94b3-4b56-92fd-4c0ccf8210fe)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5269e18b-d4f0-4c64-8df8-283a2ca66c59)  
(KB2633880)  
(Krytyczny)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=70aadf34-abdc-4577-8da9-a0669dccc119)<sup>[1]</sup>
(KB2633870)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=82f5c503-d2ea-4fed-8f9d-f30bee2f60b3)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr>
<th colspan="8">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS12-008**](http://go.microsoft.com/fwlink/?linkid=238387)
</td>
<td style="border:1px solid black;">
[**MS12-010**](http://go.microsoft.com/fwlink/?linkid=236989)
</td>
<td style="border:1px solid black;">
[**MS12-013**](http://go.microsoft.com/fwlink/?linkid=238617)
</td>
<td style="border:1px solid black;">
[**MS12-016**](http://go.microsoft.com/fwlink/?linkid=235370)
</td>
<td style="border:1px solid black;">
[**MS12-009**](http://go.microsoft.com/fwlink/?linkid=238474)
</td>
<td style="border:1px solid black;">
[**MS12-012**](http://go.microsoft.com/fwlink/?linkid=239941)
</td>
<td style="border:1px solid black;">
[**MS12-014**](http://go.microsoft.com/fwlink/?linkid=239945)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Zbiorczy** **wskaźnik ważności**
</td>
<td style="border:1px solid black;">
[**Krytyczny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Umiarkowany**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Brak
</td>
<td style="border:1px solid black;">
[**Krytyczny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Brak
</td>
<td style="border:1px solid black;">
Brak
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f0e6e06d-89db-45ad-9660-7959c6f9b546)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=c4642890-2fba-45da-bbe9-fcaa84e4aa0c)  
(Brak wskaźnika ważności<sup>[1]</sup>)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=9e157b88-2c11-44dc-b13d-1051f9c39890)  
(Umiarkowany)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=bf8ad019-e710-4e16-be4f-8168df5c5343)  
(Umiarkowany)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5269e18b-d4f0-4c64-8df8-283a2ca66c59)  
(KB2633880)  
(Krytyczny)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=70aadf34-abdc-4577-8da9-a0669dccc119)<sup>[1]</sup>
(KB2633870)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5ee4bef7-b355-4aae-8bba-834a16d44744)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b81decda-9d82-4ffb-baae-78b190e553ea)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=c4a52801-55b5-4eef-9db3-c29a45863198)  
(Brak wskaźnika ważności<sup>[1]</sup>)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=f162ad36-c096-43ba-a440-ec4d3fb54c21)  
(Umiarkowany)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=ef4a9002-b2da-40af-abc0-737565fea179)  
(Umiarkowany)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5269e18b-d4f0-4c64-8df8-283a2ca66c59)  
(KB2633880)  
(Krytyczny)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=70aadf34-abdc-4577-8da9-a0669dccc119)<sup>[1]</sup>
(KB2633870)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b53cf810-0ea3-4cb0-91f9-de1406ccfc96)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=8dcd71c8-82ad-4f86-b386-7f1ea09e157f)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=3b42f935-7f59-4871-a01f-480033c3ad40)  
(Brak wskaźnika ważności<sup>[1]</sup>)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=24fe7c08-4736-455b-9b98-1b6a65718143)  
(Umiarkowany)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5269e18b-d4f0-4c64-8df8-283a2ca66c59)  
(KB2633880)  
(Krytyczny)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=70aadf34-abdc-4577-8da9-a0669dccc119)<sup>[1]</sup>
(KB2633870)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=3b18d22d-e192-498b-a105-b946a5f5bfad)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr>
<th colspan="8">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS12-008**](http://go.microsoft.com/fwlink/?linkid=238387)
</td>
<td style="border:1px solid black;">
[**MS12-010**](http://go.microsoft.com/fwlink/?linkid=236989)
</td>
<td style="border:1px solid black;">
[**MS12-013**](http://go.microsoft.com/fwlink/?linkid=238617)
</td>
<td style="border:1px solid black;">
[**MS12-016**](http://go.microsoft.com/fwlink/?linkid=235370)
</td>
<td style="border:1px solid black;">
[**MS12-009**](http://go.microsoft.com/fwlink/?linkid=238474)
</td>
<td style="border:1px solid black;">
[**MS12-012**](http://go.microsoft.com/fwlink/?linkid=239941)
</td>
<td style="border:1px solid black;">
[**MS12-014**](http://go.microsoft.com/fwlink/?linkid=239945)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Zbiorczy wskaźnik ważności**
</td>
<td style="border:1px solid black;">
[**Krytyczny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Krytyczny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Krytyczny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Krytyczny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Brak
</td>
<td style="border:1px solid black;">
Brak
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5852118c-fc39-45e2-8b44-ce1401d310e2)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=6ec23c7e-0166-47dc-ae86-c49b505206bb)  
(Krytyczny)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=bbf627df-0bc0-478f-aa34-a7e5f039e589)  
(Krytyczny)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=d287496a-411c-4c1b-9d98-bacc553041ae)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Vista z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c503c7b1-24f8-40a4-8283-c1e4abf90b57)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=aab7826d-539b-4e36-b3a1-afa94b37dbe7)  
(KB2633874)  
(Krytyczny)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=70aadf34-abdc-4577-8da9-a0669dccc119)<sup>[1]</sup>
(KB2633870)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5161d16d-1037-49d5-8d4d-c353288cb41c)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=b30a8cc5-b9ad-476f-928c-c49c993d0e80)  
(Krytyczny)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=3a8b966a-bf34-42fd-8758-9a5e8e3c7689)  
(Krytyczny)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=22cc0245-1877-4c76-914f-dd68f6cd45f0)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ddbd9fcf-10c4-4089-88c0-c2a6c288222b)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=aab7826d-539b-4e36-b3a1-afa94b37dbe7)  
(KB2633874)  
(Krytyczny)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=70aadf34-abdc-4577-8da9-a0669dccc119)<sup>[1]</sup>
(KB2633870)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=73e240a6-2d5e-4ceb-8500-8dacca0e4a43)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr>
<th colspan="8">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS12-008**](http://go.microsoft.com/fwlink/?linkid=238387)
</td>
<td style="border:1px solid black;">
[**MS12-010**](http://go.microsoft.com/fwlink/?linkid=236989)
</td>
<td style="border:1px solid black;">
[**MS12-013**](http://go.microsoft.com/fwlink/?linkid=238617)
</td>
<td style="border:1px solid black;">
[**MS12-016**](http://go.microsoft.com/fwlink/?linkid=235370)
</td>
<td style="border:1px solid black;">
[**MS12-009**](http://go.microsoft.com/fwlink/?linkid=238474)
</td>
<td style="border:1px solid black;">
[**MS12-012**](http://go.microsoft.com/fwlink/?linkid=239941)
</td>
<td style="border:1px solid black;">
[**MS12-014**](http://go.microsoft.com/fwlink/?linkid=239945)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Zbiorczy wskaźnik ważności**
</td>
<td style="border:1px solid black;">
[**Krytyczny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Umiarkowany**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Krytyczny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Krytyczny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Brak
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 z dodatkiem Service Pack 2 dla systemów 32-bitowych
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów 32-bitowych z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=45c6c511-a4fa-4c3b-af26-6c113f6f5f5e)\*\*\*\*  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=21f7dba4-fe97-487e-8b37-45914e106db0)\*\*  
(Umiarkowany)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=98d5b024-0eda-4e5d-ba9d-b828ad3d048e)\*\*  
(Umiarkowany)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=025a5af0-39f1-481c-920c-43d2b3d85dc5)\*\*  
(Umiarkowany)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów 32-bitowych z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0c1812af-f57d-455d-a81d-5e03db99b2f7)\*  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=aab7826d-539b-4e36-b3a1-afa94b37dbe7)  
(KB2633874)  
(Krytyczny)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=70aadf34-abdc-4577-8da9-a0669dccc119)<sup>[1]</sup>
(KB2633870)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów 32-bitowych z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3f6f89b3-3bc8-4325-b8d8-9a5a398b99c6)\*\*  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem x64
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów opartych na procesorze x64 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=046932cf-0671-49e6-8ddf-98abfc97c5f0)\*\*\*\*  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=2cd8e296-dae8-41ce-8373-f8a71b4555e9)\*\*  
(Umiarkowany)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=246f9995-fe19-43d0-8f67-0e91eb961bab)\*\*  
(Umiarkowany)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=c216e01d-2f46-4a46-bdc7-9d0fe98193a3)\*\*  
(Umiarkowany)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem x64 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e1b66bb5-ea12-44a5-807a-f21ede0dc76d)\*  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=aab7826d-539b-4e36-b3a1-afa94b37dbe7)  
(KB2633874)  
(Krytyczny)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=70aadf34-abdc-4577-8da9-a0669dccc119)<sup>[1]</sup>
(KB2633870)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem x64 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0e06e77d-7e5d-4d57-98b2-0817f68a1ebb)\*  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=35e6bd04-594f-42ef-97f8-abcf578b4f10)\*\*  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem Itanium
</td>
<td style="border:1px solid black;">
[Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=304bd0c5-f4ee-4f8c-89b4-4cbaaf418679)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=05c0e6eb-c641-43ab-958a-f43933cdbba7)  
(Umiarkowany)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=3a96ab34-8f45-48bf-a98b-9e683b50aaa0)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=aab7826d-539b-4e36-b3a1-afa94b37dbe7)  
(KB2633874)  
(Krytyczny)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=70aadf34-abdc-4577-8da9-a0669dccc119)<sup>[1]</sup>
(KB2633870)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=56cbeba9-0c39-4418-9042-7244ac9d03db)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=d1d51b26-2d01-42a9-9bb1-9fb82c1fb914)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr>
<th colspan="8">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS12-008**](http://go.microsoft.com/fwlink/?linkid=238387)
</td>
<td style="border:1px solid black;">
[**MS12-010**](http://go.microsoft.com/fwlink/?linkid=236989)
</td>
<td style="border:1px solid black;">
[**MS12-013**](http://go.microsoft.com/fwlink/?linkid=238617)
</td>
<td style="border:1px solid black;">
[**MS12-016**](http://go.microsoft.com/fwlink/?linkid=235370)
</td>
<td style="border:1px solid black;">
[**MS12-009**](http://go.microsoft.com/fwlink/?linkid=238474)
</td>
<td style="border:1px solid black;">
[**MS12-012**](http://go.microsoft.com/fwlink/?linkid=239941)
</td>
<td style="border:1px solid black;">
[**MS12-014**](http://go.microsoft.com/fwlink/?linkid=239945)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Zbiorczy wskaźnik ważności**
</td>
<td style="border:1px solid black;">
[**Krytyczny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Krytyczny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Krytyczny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Krytyczny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Brak
</td>
<td style="border:1px solid black;">
Brak
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 dla systemów 32-bitowych i Windows 7 z dodatkiem Service Pack 1 dla systemów 32-bitowych
</td>
<td style="border:1px solid black;">
[Windows 7 dla systemów 32-bitowych i Windows 7 z dodatkiem Service Pack 1 dla systemów 32-bitowych](http://www.microsoft.com/downloads/details.aspx?familyid=3e5ca1bf-9415-412c-9dff-dd1abc57e74d)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=8b423683-cd29-4049-82d6-f0845842e7f0)  
(Krytyczny)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=c83a9c74-a5a7-4b3e-ba36-7a7024d99fd8)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows 7 dla systemów 32-bitowych i Windows 7 z dodatkiem Service Pack 1 dla systemów 32-bitowych](http://www.microsoft.com/downloads/details.aspx?familyid=403f355c-2273-42ac-8263-d662f5d7740c)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Windows 7 dla systemów 32-bitowych:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=5a5f3ee7-ca49-41c8-aeec-7c76b66712fc)  
(KB2633879)  
(Krytyczny)  
Tylko Windows 7 z dodatkiem Service Pack 1 dla systemów 32-bitowych:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=243e8c64-8b6e-4cea-9e99-58d4b1ad35b5)  
(KB2633873)  
(Krytyczny)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=70aadf34-abdc-4577-8da9-a0669dccc119)<sup>[1]</sup>
(KB2633870)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 dla systemów opartych na procesorach x64 i Windows 7 z dodatkiem Service Pack 1 dla systemów opartych na procesorach x64
</td>
<td style="border:1px solid black;">
[Windows 7 dla systemów opartych na procesorach x64 i Windows 7 z dodatkiem Service Pack 1 dla systemów opartych na procesorach x64](http://www.microsoft.com/downloads/details.aspx?familyid=78cbbe02-a3d3-4cef-9b54-a3e78c1b885a)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=a5d00138-4e24-4a07-92dd-3d8a14476197)  
(Krytyczny)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=bbc9d6ae-9ec5-401f-bf16-4811b63709d1)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows 7 dla systemów opartych na procesorach x64 i Windows 7 z dodatkiem Service Pack 1 dla systemów opartych na procesorach x64](http://www.microsoft.com/downloads/details.aspx?familyid=8bd8e804-ca4d-4326-bc60-345e2975b7aa)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Windows 7 dla systemów z procesorem x64:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=5a5f3ee7-ca49-41c8-aeec-7c76b66712fc)  
(KB2633879)  
(Krytyczny)  
Tylko Windows 7 z dla systemów z procesorem x64 z dodatkiem Service Pack 1:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=243e8c64-8b6e-4cea-9e99-58d4b1ad35b5)  
(KB2633873)  
(Krytyczny)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=70aadf34-abdc-4577-8da9-a0669dccc119)<sup>[1]</sup>
(KB2633870)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows 7 dla systemów opartych na procesorach x64 i Windows 7 z dodatkiem Service Pack 1 dla systemów opartych na procesorach x64](http://www.microsoft.com/downloads/details.aspx?familyid=299d107d-ab9f-42b6-8f94-a2f1d242c127)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr>
<th colspan="8">
System Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS12-008**](http://go.microsoft.com/fwlink/?linkid=238387)
</td>
<td style="border:1px solid black;">
[**MS12-010**](http://go.microsoft.com/fwlink/?linkid=236989)
</td>
<td style="border:1px solid black;">
[**MS12-013**](http://go.microsoft.com/fwlink/?linkid=238617)
</td>
<td style="border:1px solid black;">
[**MS12-016**](http://go.microsoft.com/fwlink/?linkid=235370)
</td>
<td style="border:1px solid black;">
[**MS12-009**](http://go.microsoft.com/fwlink/?linkid=238474)
</td>
<td style="border:1px solid black;">
[**MS12-012**](http://go.microsoft.com/fwlink/?linkid=239941)
</td>
<td style="border:1px solid black;">
[**MS12-014**](http://go.microsoft.com/fwlink/?linkid=239945)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Zbiorczy wskaźnik ważności**
</td>
<td style="border:1px solid black;">
[**Krytyczny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Umiarkowany**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Krytyczny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Krytyczny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Brak
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 dla systemów opartych na procesorach x64 i Windows Server 2008 R2 z dodatkiem Service Pack 1 dla systemów opartych na procesorach x64
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach x64 i Windows Server 2008 R2 dla systemów opartych na procesorach x64 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6b228ad6-d5a4-4b91-8aa8-0874deb22116)\*\*\*\*  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=3074a898-54bb-44ff-a8f4-77f831c28771)\*\*  
(Umiarkowany)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=1896a6da-f7ee-484b-a97c-455fce7b82b8)\*\*  
(Umiarkowany)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach x64 i Windows Server 2008 R2 z dodatkiem Service Pack 1 dla systemów opartych na procesorach x64](http://www.microsoft.com/downloads/details.aspx?familyid=d868c5ef-165a-46a0-b832-e6ca55a910f9)\*  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Tylko Windows Server 2008 R2 dla systemów opartych na procesorach x64:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=5a5f3ee7-ca49-41c8-aeec-7c76b66712fc)\*  
(KB2633879)  
(Krytyczny)  
Tylko Windows Server 2008 R2 dla systemów opartych na procesorach x64:  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=70aadf34-abdc-4577-8da9-a0669dccc119)<sup>[1]</sup>
(KB2633870)  
(Krytyczny)  
Tylko Windows Server 2008 R2 dla systemów opartych na procesorach x64 z dodatkiem Service Pack 1:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=243e8c64-8b6e-4cea-9e99-58d4b1ad35b5)\*  
(KB2633873)  
(Krytyczny)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=70aadf34-abdc-4577-8da9-a0669dccc119)\*<sup>[1]</sup>
(KB2633870)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach x64 i Windows Server 2008 R2 z dodatkiem Service Pack 1 dla systemów opartych na procesorach x64](http://www.microsoft.com/downloads/details.aspx?familyid=576192d3-f050-4718-a7da-c84fce6bf744)\*  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach x64 i Windows Server 2008 R2 z dodatkiem Service Pack 1 dla systemów opartych na procesorach x64](http://www.microsoft.com/downloads/details.aspx?familyid=8c51e09b-51c3-4860-836e-6bcffde75f04)\*\*  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 dla systemów opartych na procesorach Itanium i Windows Server 2008 R2 z dodatkiem Service Pack 1 dla systemów opartych na procesorach Itanium
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach Itanium i Windows Server 2008 R2 z dodatkiem Service Pack 1 dla systemów opartych na procesorach Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=922b2438-0cfc-49e3-b9a0-52c68b69126a)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=7f7c0bc3-fc26-4ee8-aedb-c251247cbeb5)  
(Umiarkowany)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach Itanium i Windows Server 2008 R2 z dodatkiem Service Pack 1 dla systemów opartych na procesorach Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=e5416371-495b-4dc7-a239-f9185f968969)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Tylko Windows Server 2008 R2 dla systemów z procesorem Itanium:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=5a5f3ee7-ca49-41c8-aeec-7c76b66712fc)  
(KB2633879)  
(Krytyczny)  
Tylko Windows Server 2008 R2 dla systemów z procesorem Itanium z dodatkiem Service Pack 1:  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=243e8c64-8b6e-4cea-9e99-58d4b1ad35b5)  
(KB2633873)  
(Krytyczny)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=70aadf34-abdc-4577-8da9-a0669dccc119)<sup>[1]</sup>
(KB2633870)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach Itanium i Windows Server 2008 R2 z dodatkiem Service Pack 1 dla systemów opartych na procesorach Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=d6a9b2c9-7582-4953-8ab1-a55c63fcc8dc)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach Itanium i Windows Server 2008 R2 z dodatkiem Service Pack 1 dla systemów opartych na procesorach Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=fba58a1b-9d9f-4a10-b1df-08a0ebfa2358)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
</table>
 
**Uwagi dotyczące systemu Windows Server 2008 i Windows Server 2008 R2**

**\*Luka w zabezpieczeniach dotyczy instalacji Server Core.** Ta aktualizacja ma zastosowanie, z takim samym wskaźnikiem ważności, w przypadku obsługiwanych wersji systemu Windows Server 2008 lub Windows Server 2008 R2, niezależnie od tego, czy zostały zainstalowane przy użyciu opcji instalacji Server Core. Więcej informacji na temat tej opcji instalacji można znaleźć w artykułach TechNet, [Managing a Server Core Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) i [Servicing a Server Core Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) (jęz. ang.). Należy pamiętać, że opcja instalacji Server Core nie dotyczy niektórych wersji systemu Windows Server 2008 i Windows Server 2008 R2. Zobacz [Porównanie opcji instalacji Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Luka w zabezpieczeniach nie dotyczy instalacji Server Core.** Luki usuwane przez tę aktualizację zabezpieczeń nie dotyczą obsługiwanych wersji systemu Windows Server 2008 ani Windows Server 2008 R2, jeżeli systemy te zostały zainstalowane przy użyciu opcji instalacji Server Core. Więcej informacji na temat tej opcji instalacji można znaleźć w artykułach TechNet, [Managing a Server Core Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) i [Servicing a Server Core Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) (jęz. ang.). Należy pamiętać, że opcja instalacji Server Core nie dotyczy niektórych wersji systemu Windows Server 2008 i Windows Server 2008 R2. Zobacz [Porównanie opcji instalacji Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*\*\*Luka w zabezpieczeniach dotyczy instalacji Server Core.** Ta aktualizacja ma zastosowanie, z niższym wskaźnikiem ważności, w przypadku obsługiwanych wersji systemu Windows Server 2008 lub Windows Server 2008 R2, jeśli zostały zainstalowane przy użyciu opcji instalacji Server Core. Więcej informacji na temat tej opcji instalacji można znaleźć w artykułach TechNet, [Managing a Server Core Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) i [Servicing a Server Core Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) (jęz. ang.). Należy pamiętać, że opcja instalacji Server Core nie dotyczy niektórych wersji systemu Windows Server 2008 i Windows Server 2008 R2. Zobacz [Porównanie opcji instalacji Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**Uwaga dotycząca biuletynu MS12-010**

<sup>[1]</sup>Do tej aktualizacji nie stosuje się wskaźników ważności, ponieważ znane kierunki ataku dla luk omówionych w niniejszym biuletynie są blokowane w konfiguracji domyślnej. Jednak ze względu na istnienie kompleksowej aktualizacji zabezpieczeń firma Microsoft zaleca, aby użytkownicy tego oprogramowania zainstalowali omawianą aktualizację zabezpieczeń.

**Uwaga dotycząca biuletynu MS12-016**

<sup>[1]</sup>**Dotyczy systemu .NET Framework 4 i .NET Framework 4 Client Profile.** Pakiety redystrybucyjne systemu .NET Framework w wersji 4 są dostępne w dwóch profilach: .NET Framework 4 i .NET Framework 4 Client Profile. Aplikacja .NET Framework 4 Client Profile jest składnikiem systemu .NET Framework 4. Luka, do której odnosi się ta aktualizacja zabezpieczeń, dotyczy zarówno wersji .NET Framework 4, jak i .NET Framework 4 Client Profile. Więcej informacji znajduje się w artykule MSDN [Instalowanie systemu .NET Framework](http://msdn.microsoft.com/en-us/library/5a4x27ek.aspx) (j. ang.).

Zobacz także pozostałe kategorie oprogramowania w sekcji **Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki**, aby uzyskać więcej plików aktualizacji w ramach tego samego identyfikatora biuletynu. Ten biuletyn obejmuje więcej niż jedną kategorię oprogramowania.

#### Pakiety i oprogramowanie Office

 
<table style="border:1px solid black;">
<tr>
<th colspan="2">
Inne programy pakietu Microsoft Office
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS12-015**](http://go.microsoft.com/fwlink/?linkid=238400)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Zbiorczy wskaźnik ważności**
</td>
<td style="border:1px solid black;">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visio Viewer 2010 i Microsoft Visio Viewer 2010 z dodatkiem Service Pack 1 (wersja 32-bitowa)
</td>
<td style="border:1px solid black;">
[Microsoft Visio Viewer 2010 i Microsoft Visio Viewer 2010 z dodatkiem Service Pack 1 (wersja 32-bitowa)](http://www.microsoft.com/downloads/details.aspx?familyid=173dc4e6-31b4-42ec-808c-f8cd005517ab)  
(KB2597170)  
(Ważny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visio Viewer 2010 i Microsoft Visio Viewer 2010 z dodatkiem Service Pack 1 (wersja 64-bitowa)
</td>
<td style="border:1px solid black;">
[Microsoft Visio Viewer 2010 i Microsoft Visio Viewer 2010 z dodatkiem Service Pack 1 (wersja 64-bitowa)](http://www.microsoft.com/downloads/details.aspx?familyid=34b234e1-1322-4edc-829c-7bc2fbd99338)  
(KB2597170)  
(Ważny)
</td>
</tr>
</table>
 

#### Oprogramowanie serwerów firmy Microsoft

 
<table style="border:1px solid black;">
<tr>
<th colspan="2">
Microsoft SharePoint Server
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS12-011**](http://go.microsoft.com/fwlink/?linkid=238500)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Zbiorczy wskaźnik ważności**
</td>
<td style="border:1px solid black;">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SharePoint Server 2010 i Microsoft SharePoint Server 2010 z dodatkiem Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft SharePoint Server 2010 i Microsoft SharePoint Server 2010 z dodatkiem Service Pack 1 (moss)](http://www.microsoft.com/downloads/details.aspx?familyid=44a8eb5a-e469-4d36-b5a0-7e030c1d3244)  
(KB2597124)  
(Ważny)
</td>
</tr>
<tr>
<th colspan="2">
Microsoft SharePoint Foundation
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS12-011**](http://go.microsoft.com/fwlink/?linkid=238500)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Zbiorczy wskaźnik ważności**
</td>
<td style="border:1px solid black;">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft SharePoint Foundation 2010 i Microsoft SharePoint Foundation 2010 z dodatkiem Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft SharePoint Foundation 2010 i Microsoft SharePoint Foundation 2010 z dodatkiem Service Pack 1 (sts)](http://www.microsoft.com/downloads/details.aspx?familyid=dd348109-953b-4154-b265-85e4694238e6)  
(KB2553413)  
(Ważny)
</td>
</tr>
</table>
 

#### Narzędzia i oprogramowanie firmy Microsoft dla deweloperów

 
<table style="border:1px solid black;">
<tr>
<th colspan="2">
Microsoft Silverlight
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS12-016**](http://go.microsoft.com/fwlink/?linkid=235370)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Zbiorczy wskaźnik ważności**
</td>
<td style="border:1px solid black;">
[**Krytyczny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Silverlight 4
</td>
<td style="border:1px solid black;">
[Microsoft Silverlight 4](http://www.microsoft.com/downloads/details.aspx?familyid=4c3602f0-9781-4374-8fef-669ddd2c0d40) na komputerach Macintosh  
(KB2668562)  
(Krytyczny)  
[Microsoft Silverlight 4](http://www.microsoft.com/downloads/details.aspx?familyid=4c3602f0-9781-4374-8fef-669ddd2c0d40) we wszystkich obsługiwanych wersjach klientów systemu Microsoft Windows  
(KB2668562)  
(Krytyczny)  
[Microsoft Silverlight 4](http://www.microsoft.com/downloads/details.aspx?familyid=4c3602f0-9781-4374-8fef-669ddd2c0d40) we wszystkich obsługiwanych wersjach serwerów Microsoft Windows  
(KB2668562)  
(Krytyczny)
</td>
</tr>
</table>
 
**Uwaga dotycząca biuletynu MS12-016**

Zobacz także pozostałe kategorie oprogramowania w sekcji **Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki**, aby uzyskać więcej plików aktualizacji w ramach tego samego identyfikatora biuletynu. Ten biuletyn obejmuje więcej niż jedną kategorię oprogramowania.

Narzędzia wykrywania i wdrażania oraz wskazówki
-----------------------------------------------

<span></span>
**Centrum zabezpieczeń**

Zarządzanie oprogramowaniem oraz aktualizacjami zabezpieczeń, które należy zainstalować na serwerach oraz komputerach stacjonarnych i przenośnych w organizacji. Więcej informacji można znaleźć w [Centrum TechNet Update Management Center](http://go.microsoft.com/fwlink/?linkid=69903). Witryna [TechNet Security Center](http://go.microsoft.com/fwlink/?linkid=21171) zawiera dodatkowe informacje na temat zabezpieczeń w produktach firmy Microsoft. Użytkownicy mogą także uzyskać dostęp do tych informacji w witrynie [Bezpieczeństwo w domu](http://go.microsoft.com/fwlink/?linkid=85102), klikając łącze „Najnowsze aktualizacje zabezpieczeń”.

Aktualizacje zabezpieczeń dostępne są w witrynach [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747) i [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130). Aktualizacje zabezpieczeń są także dostępne w witrynie [Centrum pobierania Microsoft](http://go.microsoft.com/fwlink/?linkid=21129). Najłatwiej je znaleźć, wyszukując wyrażenie „aktualizacja zabezpieczeń”.

Użytkownicy pakietu Microsoft Office dla komputerów Macintosh mogą skorzystać z funkcji automatycznej aktualizacji firmy Microsoft, aby zapewnić aktualność posiadanego oprogramowania firmy Microsoft. Więcej informacji na temat korzystania z funkcji automatycznych aktualizacji dla komputerów Macintosh można znaleźć w artykule [Automatyczne sprawdzanie aktualizacji oprogramowania](http://mac2.microsoft.com/help/office/14/en-us/word/item/ffe35357-8f25-4df8-a0a3-c258526c64ea).

Aktualizacje zabezpieczeń można także pobierać z [Wykazu usługi Microsoft Update](http://go.microsoft.com/fwlink/?linkid=96155). Wykaz usługi Microsoft Update zawiera katalog zawartości z możliwością przeszukiwania, który udostępniany jest poprzez usługi Windows Update i Microsoft Update i obejmuje aktualizacje zabezpieczeń, sterowniki i dodatki Service Pack. Wyszukiwanie przy użyciu numeru biuletynu zabezpieczeń (np. „MS07-036”) pozwala dodać do koszyka wszystkie odpowiednie aktualizacje (w tym różne wersje językowe aktualizacji) i pobrać pliki do wybranego folderu. Więcej informacji na temat Wykazu usługi Microsoft Update można znaleźć w [Często zadawanych pytaniach dotyczących Wykazu usługi Microsoft Update](http://go.microsoft.com/fwlink/?linkid=97900).

**Porady dotyczące wykrywania i wdrażania**

Firma Microsoft udziela porad dotyczących wykrywania i wdrażania aktualizacji zabezpieczeń. Porady takie zawierają zalecenia i informacje ułatwiające specjalistom IT poznanie obsługi różnych narzędzi do wykrywania i wdrażania aktualizacji zabezpieczeń. Więcej informacji na ten temat można znaleźć w [artykule 961747 bazy wiedzy Microsoft Knowledge Base](http://support.microsoft.com/kb/961747).

**Narzędzie Microsoft Baseline Security Analyzer**

Narzędzie Microsoft Baseline Security Analyzer umożliwia administratorom skanowanie lokalnych i zdalnych systemów w poszukiwaniu brakujących aktualizacji zabezpieczeń oraz typowych błędów konfiguracji zabezpieczeń. Więcej informacji na temat narzędzia MBSA można znaleźć w witrynie sieci Web [Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134).

**Windows Server Update Services**

Korzystając z programu Windows Server Update Services (WSUS), administratorzy mogą szybko i niezawodnie wdrożyć najnowsze aktualizacje krytyczne i aktualizacje zabezpieczeń przeznaczone dla systemów operacyjnych Microsoft Windows 2000 i nowszych, pakietów Office XP i nowszych, programu Exchange Server 2003 oraz SQL Server 2000 w systemach operacyjnych Microsoft Windows 2000 i nowszych.

Więcej informacji na temat sposobu wdrażania tej aktualizacji zabezpieczeń za pomocą programu Windows Server Update Services można znaleźć w [witrynie sieci Web programu Windows Server Update Services](http://technet.microsoft.com/en-us/wsus/default.aspx).

**System Center Configuration Manager 2007**

Program Configuration Manager 2007 Software Update Management ułatwia realizację złożonych zadań dostarczania aktualizacji do systemów IT w firmie i zarządzania nimi. Dzięki programowi Configuration Manager 2007 administratorzy mogą dostarczać aktualizacje produktów firmy Microsoft do całej gamy urządzeń, takich jak komputery stacjonarne, laptopy, serwery i urządzenia mobilne.

System zautomatyzowanej oceny zagrożeń w programie Configuration Manager 2007 wykrywa potrzebne aktualizacje i sporządza raporty dotyczące zalecanych czynności. Funkcja Software Update Management w programie Configuration Manager 2007 powstała w oparciu o usługi Microsoft Windows Software Update Services (WSUS) — dobrze sprawdzoną infrastrukturę aktualizacji znaną administratorom na całym świecie. Więcej informacji na temat możliwości wykorzystania przez administratorów programu Configuration Manager 2007 do wdrażania aktualizacji zawiera dokument [Software Update Management](http://www.microsoft.com/systemcenter/en/us/configuration-manager/cm-software-update-management.aspx). Więcej informacji dotyczących programu Configuration Manager znajduje się na stronie [System Center Configuration Manager](http://www.microsoft.com/systemcenter/en/us/configuration-manager.aspx).

**Systems Management Server 2003**

Program Systems Management Server (SMS) jest przeznaczonym dla przedsiębiorstw i w znacznym stopniu konfigurowalnym rozwiązaniem służącym do zarządzania aktualizacjami. Program SMS umożliwia administratorom znalezienie komputerów z systemem Windows, na których należy zainstalować aktualizację zabezpieczeń, a także przeprowadzić kontrolowane wdrożenie tych aktualizacji w całym przedsiębiorstwie, w minimalnym stopniu zakłócając przy tym pracę użytkowników końcowych.

**Uwaga** Program System Management Server 2003 od 12 stycznia 2010 roku nie jest objęty podstawową pomocą techniczną. Więcej informacji na temat cyklu pomocy technicznej dla produktów można znaleźć w witrynie zasad [cyklu pomocy technicznej firmy Microsoft](http://support.microsoft.com/common/international.aspx?rdpath=dm;en-us;lifecycle). Dostępne jest kolejne wydanie programu System Center Configuration Manager 2007 (SMS); zobacz wcześniejszą sekcję **System Center Configuration Manager 2007**.

Więcej informacji na temat możliwości wykorzystania przez administratorów programu SMS 2003 do wdrażania aktualizacji zabezpieczeń można znaleźć w artykule [Scenarios and Procedures for Microsoft Systems Management Server 2003: Software Distribution and Patch Management](http://www.microsoft.com/downloads/en/details.aspx?familyid=32f2bb4c-42f8-4b8d-844f-2553fd78049f&displaylang=en). Więcej informacji na temat programu SMS można znaleźć w witrynie sieci Web [Microsoft Systems Management Server TechCenter](http://technet.microsoft.com/en-us/systemcenter/bb545936.aspx).

**Uwaga** Program SMS zapewnia obsługę rozwiązań zawartych w biuletynach zabezpieczeń dzięki narzędziu Microsoft Baseline Security Analyzer. Narzędzia te mogą nie wykrywać wszystkich aktualizacji oprogramowania. W takich przypadkach administratorzy mogą wykorzystywać dostępne w programie SMS funkcje zarządzania zasobami do przyporządkowania poszczególnych aktualizacji określonym systemom. Aby uzyskać więcej informacji dotyczących tej procedury, zobacz [Wdrażanie aktualizacji oprogramowania za pomocą funkcji Software Distribution programu SMS](http://go.microsoft.com/fwlink/?linkid=33341). Niektóre aktualizacje oprogramowania wymagają od użytkownika uprawnień administratora po ponownym uruchomieniu systemu. Do zainstalowania tych aktualizacji administratorzy mogą użyć narzędzia Elevated Rights Deployment Tool (dostępnego w dodatku [SMS 2003 Administration Feature Pack](http://www.microsoft.com/downloads/en/details.aspx?familyid=7bd3a16e-1899-4e0b-bb99-1320e816167d&displaylang=en)).

**Tester zgodności aktualizacji i zestaw narzędzi do sprawdzania zgodności aplikacji**

Często aktualizacje zapisują informacje w tych samych plikach i ustawieniach rejestru niezbędnych do działania określonych aplikacji użytkownika. Może to prowadzić do niezgodności i wydłużyć czas wdrażania aktualizacji zabezpieczeń. Dzięki składnikom narzędzia [Tester zgodności aplikacji](http://technet2.microsoft.com/windowsvista/en/library/4279e239-37a4-44aa-aec5-4e70fe39f9de1033.mspx?mfr=true) znajdującego się w [Zestawie narzędzi do sprawdzania zgodności aplikacji](http://www.microsoft.com/downloads/details.aspx?familyid=24da89e9-b581-47b0-b45e-492dd6da2971&displaylang=en) można usprawnić proces testowania i sprawdzania poprawności aktualizacji systemu Windows.

W Zestawie narzędzi do sprawdzania zgodności aplikacji znajdują się niezbędne narzędzia i dokumentacja, które umożliwiają ocenę zgodności aplikacji przed wdrożeniem systemu Windows Vista, aktualizacji dla systemu Windows, aktualizacji zabezpieczeń firmy Microsoft lub nowej wersji programu Windows Internet Explorer w środowisku użytkownika, oraz ograniczenie problemów ze zgodnością aplikacji.

### Inne informacje:

#### Narzędzie Microsoft Windows do usuwania złośliwego oprogramowania

Firma Microsoft opublikowała zaktualizowaną wersję narzędzia Microsoft Windows Malicious Software Removal Tool, która dostępna jest w witrynach sieci Web Windows Update i Microsoft Update, poprzez usługi Windows Server Update Services i w witrynie Centrum pobierania Microsoft.

#### Aktualizacje niezwiązane z zabezpieczeniami, dostępne w witrynach MU, WU oraz usługach WSUS

Aby uzyskać informacje na temat publikacji niezwiązanych z zabezpieczeniami, dostępnych w witrynach Windows Update i Microsoft Update, zobacz:

-   [Artykuł 894199 bazy wiedzy Microsoft Knowledge Base](http://support.microsoft.com/kb/894199): Opis zmian zawartości Usług aktualizacji oprogramowania i usług Windows Server Update Services. Zawiera wszystkie treści dotyczące systemu Windows.
-   [Aktualizacje z poprzednich miesięcy dla usług Windows Server Update Services](http://technet.microsoft.com/en-us/wsus/bb456965.aspx). Wyświetla nowe, zmienione i opublikowane ponownie aktualizacje dla produktów firmy Microsoft innych niż Microsoft Windows.

#### Microsoft Active Protections Program (MAPP)

W celu zwiększenia poziomu bezpieczeństwa swoich klientów firma Microsoft dostarcza informacje na temat luk w zabezpieczeniach największym dostawcom oprogramowania zabezpieczającego przed publikacją comiesięcznej aktualizacji zabezpieczeń. Dzięki informacjom dotyczącym luk w zabezpieczeniach dostawcy oprogramowania zabezpieczającego mogą zaoferować swoim klientom zaktualizowane poprawki za pośrednictwem programów lub urządzeń zabezpieczających np. programów antywirusowych, sieciowych systemów wykrywania włamań lub hostowych systemów zapobiegania włamaniom. Aby sprawdzić, czy dostawcy oprogramowania zabezpieczającego zapewniają aktywną ochronę, odwiedź witryny poszczególnych partnerów programu, których listę znaleźć można w sekcji [Microsoft Active Protections Program (MAPP) Partners](http://go.microsoft.com/fwlink/?linkid=215201).

#### Strategie i społeczność związane z zabezpieczeniami

**Strategie zarządzania aktualizacjami**

Na stronie [Security Guidance for Update Management](http://go.microsoft.com/fwlink/?linkid=21168) (Wskazówki z zakresu bezpieczeństwa dotyczące zarządzania aktualizacjami) znajdują się dodatkowe informacje o zalecanych przez firmę Microsoft najlepszych sposobach stosowania aktualizacji zabezpieczeń.

**Uzyskiwanie innych aktualizacji zabezpieczeń**

Aktualizacje dotyczące innych problemów związanych z zabezpieczeniami można uzyskać w następujących lokalizacjach:

-   Aktualizacje zabezpieczeń są dostępne w witrynie [Centrum pobierania Microsoft](http://go.microsoft.com/fwlink/?linkid=21129). Najłatwiej je znaleźć, wyszukując wyrażenie „aktualizacja zabezpieczeń”.
-   Aktualizacje dla poszczególnych platform są dostępne w [witrynie sieci Web Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747).
-   Aktualizacje zabezpieczeń dostępne w tym miesiącu w witrynie Windows Update można otrzymać w witrynie Centrum pobierania Microsoft w postaci plików obrazu dysku CD zawierającego zabezpieczenia i aktualizacje krytyczne. Więcej informacji na ten temat można znaleźć w [artykule 913086 bazy wiedzy Microsoft Knowledge Base](http://support.microsoft.com/kb/913086).

**Społeczność IT Pro Security Community**

Dowiedz się, jak poprawić bezpieczeństwo i zoptymalizować infrastrukturę informatyczną oraz weź udział w dyskusjach dotyczących zabezpieczeń wraz z innymi specjalistami z branży IT, odwiedzając witrynę sieci Web społeczności [IT Pro Security Community](http://go.microsoft.com/fwlink/?linkid=21164) (jęz. ang.).

#### Podziękowania

Firma Microsoft [dziękuje](http://go.microsoft.com/fwlink/?linkid=21127) wymienionym poniżej organizacjom i osobom za współpracę w dziedzinie ochrony klientów:

-   Tarjei Mandt z firmy [Azimuth Security](http://www.azimuthsecurity.com/), za zgłoszenie problemu opisanego w biuletynie MS12-008
-   Tarjei Mandt z firmy [Azimuth Security](http://www.azimuthsecurity.com/), za zgłoszenie dwóch problemów opisanych w biuletynie MS12-009
-   [Jan Schejbal](http://janschejbal.wordpress.com/), za zgłoszenie problemu opisanego w biuletynie MS12-010
-   Stephen Fewer z firmy [Harmony Security](http://www.harmonysecurity.com/), współpracujący z oddziałem [Zero Day Initiative](http://www.zerodayinitiative.com/) firmy [TippingPoint](http://www.tippingpoint.com/), za zgłoszenie dwóch problemów opisanych w biuletynie MS12-010
-   Jason Hullinger z firmy [HP Cloud Services](http://www.hpcloud.com/), za zgłoszenie problemu opisanego w biuletynie MS12-010
-   Jan Hollenberger, za zgłoszenie problemu opisanego w biuletynie MS12-011
-   Rocco Calvi z firmy stratsec, za zgłoszenie problemu opisanego w biuletynie MS12-011
-   Giorgio Fedon z firmy Minded Security, za współpracę przy wprowadzaniu gruntownych zmian zawartych w biuletynie MS12-011
-   Alexander Gavrun, współpracujący z oddziałem [Zero Day Initiative](http://www.zerodayinitiative.com/) firmy [TippingPoint](http://www.tippingpoint.com/), za zgłoszenie problemu opisanego w biuletynie MS12-013
-   Xin Ouyang z firmy [Palo Alto Networks](http://www.paloaltonetworks.com/), za zgłoszenie pięciu problemów opisanych w biuletynie MS12-015
-   Jeroen Frijters z firmy [Sumatra](http://www.sumatra.nl/), za zgłoszenie problemu opisanego w biuletynie MS12-016

#### Pomoc techniczna

-   Wymienione oprogramowanie zostało przetestowane w celu ustalenia, których wersji dotyczy problem. Dla pozostałych wersji upłynął okres pomocy technicznej. Aby zapoznać się z zasadami cyklu pomocy technicznej dotyczącymi używanej wersji oprogramowania, odwiedź [witrynę zasad cyklu pomocy technicznej firmy Microsoft](http://go.microsoft.com/fwlink/?linkid=21742).
-   Klienci mogą uzyskać pomoc techniczną w [Biurze Obsługi Klienta Microsoft](http://go.microsoft.com/fwlink/?linkid=21131) pod numerem 0 801 802 000 (opłata według stawek Twojego operatora) lub (0-22) 594 19 99 w godzinach od 9:00 do 17:00, od poniedziałku do piątku. Połączenia z działem pomocy technicznej związane z aktualizacjami zabezpieczeń są bezpłatne. Dodatkowe informacje dotyczące możliwości skorzystania z pomocy technicznej można znaleźć w witrynie [Pomoc i obsługa techniczna firmy Microsoft](http://support.microsoft.com/).
-   Klienci międzynarodowi mogą uzyskać pomoc w lokalnych przedstawicielstwach firmy Microsoft. Pomoc techniczna związana z aktualizacjami zabezpieczeń jest bezpłatna. Informacje o sposobie kontaktowania się z pomocą techniczną firmy Microsoft są dostępne w [międzynarodowej witrynie sieci Web pomocy i obsługi technicznej](http://go.microsoft.com/fwlink/?linkid=21155).

#### Zrzeczenie odpowiedzialności

Informacje w bazie wiedzy Microsoft Knowledge Base są dostarczane „tak jak są” bez jakiejkolwiek gwarancji. Firma Microsoft odrzuca wszelkie gwarancje, wyraźne i dorozumiane, w tym gwarancje dotyczące wartości handlowej i przydatności do określonego celu. Firma Microsoft Corporation ani jej dostawcy w żadnym wypadku nie ponoszą odpowiedzialności za jakiekolwiek szkody, w tym bezpośrednie, pośrednie, przypadkowe, wynikowe, utratę zysków handlowych lub szkody specjalne, nawet jeżeli firmę Microsoft Corporation lub jej dostawców powiadomiono o możliwości zaistnienia takich szkód. W niektórych stanach wyłączenie lub ograniczenie odpowiedzialności za straty wynikowe lub przypadkowe, a więc i powyższe ograniczenia, nie mają zastosowania.

#### Wersje

-   Wersja 1.0 (14 lutego 2012 r.): Opublikowane podsumowanie biuletynów zabezpieczeń.

*Built at 2014-04-18T01:50:00Z-07:00*
