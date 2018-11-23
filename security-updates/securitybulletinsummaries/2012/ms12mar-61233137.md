---
TOCTitle: 'MS12-MAR'
Title: 'Podsumowanie biuletynów zabezpieczeń firmy Microsoft za marzec 2012 r.'
ms:assetid: 'ms12-mar'
ms:contentKeyID: 61233137
ms:mtpsurl: 'https://technet.microsoft.com/pl-PL/library/ms12-mar(v=Security.10)'
---
Podsumowanie biuletynów zabezpieczeń firmy Microsoft za marzec 2012 r.
======================================================================

Opublikowano: 13 marca 2012

**Wersja:** 1.0

Niniejsze podsumowanie biuletynów zabezpieczeń zawiera spis biuletynów za marzec 2012 r.

Z chwilą opublikowania biuletynów zabezpieczeń za marzec 2012 r. niniejsze podsumowanie biuletynów zastępuje powiadomienie o biuletynach zabezpieczeń wydane 8 marca 2012 r. Aby uzyskać więcej informacji na temat usługi powiadamiania o biuletynach, zobacz [Powiadomienia o biuletynach zabezpieczeń firmy Microsoft (j. ang.)](http://go.microsoft.com/fwlink/?linkid=217213).

Aby dowiedzieć się, jak otrzymywać automatyczne powiadomienia o publikacji biuletynów zabezpieczeń firmy Microsoft, odwiedź stronę [Microsoft Technical Security Notifications](http://go.microsoft.com/fwlink/?linkid=21163).

14 marca 2012 r. o godz. 11:00 czasu Pacyfiku (godz. 20:00 czasu środkowoeuropejskiego) firma Microsoft udostępni emisję internetową, w której znajdą się odpowiedzi na pytania klientów dotyczące tych biuletynów (USA i Kanada). Zarejestruj się, aby zobaczyć [emisję internetową dotyczącą biuletynów zabezpieczeń za marzec](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032499508). Po tym dniu emisja internetowa będzie dostępna na żądanie. Aby uzyskać więcej informacji, zobacz [Podsumowania biuletynów zabezpieczeń i emisje internetowe firmy Microsoft](http://go.microsoft.com/fwlink/?linkid=217214).

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=232664">MS12-020</a></td>
<td style="border:1px solid black;"><strong>Luki w zabezpieczeniach pulpitu zdalnego umożliwiają zdalne wykonanie kodu (2671387)</strong><br />
<br />
Niniejsza aktualizacja zabezpieczeń usuwa dwie zgłoszone przez osoby prywatne luki w zabezpieczeniach protokołu RDP (Remote Desktop Protocol). Najpoważniejsza z tych luk umożliwia zdalne wykonanie kodu, jeśli osoba atakująca wyśle do zagrożonego systemu sekwencję specjalnie spreparowanych pakietów RDP. Protokół RDP (Remote Desktop Protocol) nie jest domyślnie włączony w żadnym systemie operacyjnym Windows. Luka nie dotyczy systemów, w których nie włączono protokołu RDP.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Krytyczny</a><br />
Zdalne wykonanie kodu</td>
<td style="border:1px solid black;">Wymaga ponownego uruchomienia komputera</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=235401">MS12-017</a></td>
<td style="border:1px solid black;"><strong>Luka w zabezpieczeniach serwera DNS umożliwia przeprowadzenie ataku typu „odmowa usługi” (2647170)</strong><br />
<br />
Ta aktualizacja zabezpieczeń usuwa lukę w zabezpieczeniach systemu Microsoft Windows. Luka w zabezpieczeniach umożliwia przeprowadzenie ataku typu „odmowa usługi”, jeśli nieuwierzytelniona osoba atakująca zdalnie wyśle specjalnie spreparowaną kwerendę DNS do atakowanego serwera DNS.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Ważny</a><br />
Odmowa usługi</td>
<td style="border:1px solid black;">Wymaga ponownego uruchomienia komputera</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=235364">MS12-018</a></td>
<td style="border:1px solid black;"><strong>Luka w zabezpieczeniach sterowników trybu jądra systemu Windows umożliwia podniesienie uprawnień (2641653)</strong><br />
<br />
Ta aktualizacja zabezpieczeń usuwa lukę w zabezpieczeniach systemu Microsoft Windows. Luka ta może umożliwić podniesienie uprawnień, jeśli osoba atakująca zaloguje się do systemu i uruchomi specjalnie spreparowaną aplikację. Osoba atakująca musi dysponować prawidłowymi poświadczeniami logowania oraz być w stanie zalogować się lokalnie, aby wykorzystać możliwości stwarzane przez lukę.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Ważny</a><br />
Podniesienie uprawnień</td>
<td style="border:1px solid black;">Wymaga ponownego uruchomienia komputera</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=235362">MS12-021</a></td>
<td style="border:1px solid black;"><strong>Luka w zabezpieczeniach programu Visual Studio umożliwia podniesienie poziomu uprawnień (2651019)</strong><br />
<br />
Ta aktualizacja zabezpieczeń usuwa lukę w zabezpieczeniach programu Visual Studio zgłoszoną przez użytkowników. Luka w zabezpieczeniach może pozwolić na podniesienie poziomu uprawnień, jeśli osoba atakująca umieści w ścieżce używanej przez program Visual Studio specjalnie spreparowany dodatek i przekona użytkownika, który posiada wyższy poziom uprawnień, do uruchomienia tej aplikacji. Osoba atakująca musi dysponować prawidłowymi poświadczeniami logowania oraz być w stanie zalogować się lokalnie, aby wykorzystać możliwości stwarzane przez lukę. Nie jest możliwe wykorzystanie luki w sposób zdalny lub przez użytkowników anonimowych.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Ważny</a><br />
Podniesienie uprawnień</td>
<td style="border:1px solid black;">Może wymagać ponownego uruchomienia</td>
<td style="border:1px solid black;">Microsoft Visual Studio</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=235361">MS12-022</a></td>
<td style="border:1px solid black;"><strong>Luka w zabezpieczeniach programu Expression Design umożliwia zdalne wykonanie kodu (2651018)</strong><br />
<br />
Ta aktualizacja zabezpieczeń usuwa lukę w zabezpieczeniach programu Microsoft Expression Design zgłoszoną przez użytkowników. Luka ta umożliwia zdalne wykonanie kodu, gdy użytkownik otworzy prawidłowy plik (na przykład plik .xpr lub .DESIGN), który znajduje się w tym samym katalogu sieciowym, co specjalnie spreparowany plik biblioteki dołączanej dynamicznie (DLL). Wówczas podczas otwierania prawidłowego pliku program Microsoft Expression Design mógłby próbować załadować plik DLL i wykonać dowolny zawarty w nim kod. Aby atak mógł się powieść, użytkownik musi odwiedzić niezaufaną zdalną lokalizację systemu plików lub udział WebDAV i z takiej lokalizacji otworzyć prawidłowy plik (na przykład plik .xpr lub .DESIGN), który następnie zostanie załadowany przez aplikację zagrożoną przez omawianą lukę.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Ważny</a><br />
Zdalne wykonanie kodu</td>
<td style="border:1px solid black;">Może wymagać ponownego uruchomienia</td>
<td style="border:1px solid black;">Microsoft Expression Design</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=239573">MS12-019</a></td>
<td style="border:1px solid black;"><strong>Luka w zabezpieczeniach</strong> <strong>programu DirectWrite</strong> <strong>umożliwia przeprowadzenie ataku typu „odmowa usługi” (2665364)</strong><br />
<br />
Niniejsza aktualizacja zabezpieczeń ma na celu usunięcie zgłoszonej przez organizację publiczną luki w zabezpieczeniach programu Windows DirectWrite. W scenariuszu ataku z wykorzystaniem wiadomości błyskawicznych luka umożliwia atak typu „odmowa usługi”, jeśli osoba atakująca wyśle specjalnie spreparowaną sekwencję znaków Unicode bezpośrednio do klienta wiadomości błyskawicznych. Aplikacja docelowa może przestać reagować podczas próby renderowania specjalnie spreparowanej sekwencji znaków Unicode przez program DirectWrite.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Umiarkowany</a><br />
Odmowa usługi</td>
<td style="border:1px solid black;">Może wymagać ponownego uruchomienia</td>
<td style="border:1px solid black;">Microsoft Windows</td>
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

 
<table style="border:1px solid black;">
<thead>
<tr class="header">
<th style="border:1px solid black;" >Identyfikator biuletynu</th>
<th style="border:1px solid black;" >Nazwa luki w zabezpieczeniach</th>
<th style="border:1px solid black;" >CVE ID</th>
<th style="border:1px solid black;" >Ocena możliwości wykorzystania luki w najnowszej wersji programu</th>
<th style="border:1px solid black;" >Ocena możliwości wykorzystania luki w poprzedniej wersji programu</th>
<th style="border:1px solid black;" >Ocena możliwości wykorzystania luki w celu wytworzenia sytuacji typu „odmowa usługi”</th>
<th style="border:1px solid black;" >Najważniejsze uwagi</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=235401">MS12-017</a></td>
<td style="border:1px solid black;">Luka w zabezpieczeniach DNS umożliwiająca atak typu „odmowa usługi”</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0006">CVE-2012-0006</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> — kod wykorzystujący lukę mało prawdopodobny</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> — kod wykorzystujący lukę mało prawdopodobny</td>
<td style="border:1px solid black;">Stałe</td>
<td style="border:1px solid black;">Ta luka powoduje awarię typu odmowa usługi.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=235364">MS12-018</a></td>
<td style="border:1px solid black;">Luka w zabezpieczeniach związana z funkcją PostMessage</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0157">CVE-2012-0157</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> — kod wykorzystujący lukę trudny do utworzenia</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> — kod wykorzystujący lukę trudny do utworzenia</td>
<td style="border:1px solid black;">Stałe</td>
<td style="border:1px solid black;">(Brak)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=232664">MS12-020</a></td>
<td style="border:1px solid black;">Luka w zabezpieczeniach protokołu RDP (Remote Desktop Protocol)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0002">CVE-2012-0002</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> — prawdopodobny kod wykorzystujący lukę</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> — prawdopodobny kod wykorzystujący lukę</td>
<td style="border:1px solid black;">Stałe</td>
<td style="border:1px solid black;">Jest to luka umożliwiająca zdalne wykonanie nieuwierzytelnionego kodu.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=232664">MS12-020</a></td>
<td style="border:1px solid black;">Luka w zabezpieczeniach serwerów terminali umożliwiająca atak typu „odmowa usługi”</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0152">CVE-2012-0152</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> — kod wykorzystujący lukę mało prawdopodobny</td>
<td style="border:1px solid black;">Brak zagrożenia</td>
<td style="border:1px solid black;">Tymczasowy</td>
<td style="border:1px solid black;">Ta luka powoduje awarię typu odmowa usługi.<br />
<br />
Tylko najnowsza wersja podlega atakom typu DoS.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=235362">MS12-021</a></td>
<td style="border:1px solid black;">Luka w zabezpieczeniach dodatków programu Visual Studio</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0008">CVE-2012-0008</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> — prawdopodobny kod wykorzystujący lukę</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> — prawdopodobny kod wykorzystujący lukę</td>
<td style="border:1px solid black;">Nie dotyczy</td>
<td style="border:1px solid black;">(Brak)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=235361">MS12-022</a></td>
<td style="border:1px solid black;">Luka w zabezpieczeniach programu Expression Design związana z niebezpiecznym ładowaniem bibliotek</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0016">CVE-2012-0016</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> — prawdopodobny kod wykorzystujący lukę</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> — prawdopodobny kod wykorzystujący lukę</td>
<td style="border:1px solid black;">Nie dotyczy</td>
<td style="border:1px solid black;">(Brak)</td>
</tr>
</tbody>
</table>
  
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
<th colspan="5">
Windows XP  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS12-020**](http://go.microsoft.com/fwlink/?linkid=232664)
</td>
<td style="border:1px solid black;">
[**MS12-017**](http://go.microsoft.com/fwlink/?linkid=235401)
</td>
<td style="border:1px solid black;">
[**MS12-018**](http://go.microsoft.com/fwlink/?linkid=235364)
</td>
<td style="border:1px solid black;">
[**MS12-019**](http://go.microsoft.com/fwlink/?linkid=239573)
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
Brak
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
Windows XP z dodatkiem Service Pack 3
</td>
<td style="border:1px solid black;">
[Windows XP z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=18a1fe48-1318-4b93-afad-206950bb1ae5)  
(KB2621440)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows XP z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=2922411c-9755-461b-9904-f6940322af19)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=eccf865d-399a-4862-b26f-f35580419875)  
(KB2621440)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e72b6b1f-68f5-4e1a-878e-290a5f03ca30)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr>
<th colspan="5">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS12-020**](http://go.microsoft.com/fwlink/?linkid=232664)
</td>
<td style="border:1px solid black;">
[**MS12-017**](http://go.microsoft.com/fwlink/?linkid=235401)
</td>
<td style="border:1px solid black;">
[**MS12-018**](http://go.microsoft.com/fwlink/?linkid=235364)
</td>
<td style="border:1px solid black;">
[**MS12-019**](http://go.microsoft.com/fwlink/?linkid=239573)
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
Windows Server 2003 z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b69b4b9b-c0a1-4c1e-b081-8529eaf1536a)  
(KB2621440)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b04da098-666f-4760-90da-d2a17e78bf47)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=599e5db1-3bf1-4d44-bc7c-81bc545c58ec)  
(Ważny)
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
[Windows Server 2003 x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8081e67f-288c-4714-bff8-e0ff9777692f)  
(KB2621440)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=647eaf09-3959-439e-8418-fd25221eb6b9)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=482c2890-8d4c-4e13-820f-d5ff256b6a3a)  
(Ważny)
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
[Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=521baa02-5d7a-4cba-8a1a-2af1b6e4cbe4)  
(KB2621440)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=92f3af60-9a9b-4419-9e95-55f5cb54cf00)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=ccd0f116-73c2-4471-a6d9-e07d1dbdd406)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr>
<th colspan="5">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS12-020**](http://go.microsoft.com/fwlink/?linkid=232664)
</td>
<td style="border:1px solid black;">
[**MS12-017**](http://go.microsoft.com/fwlink/?linkid=235401)
</td>
<td style="border:1px solid black;">
[**MS12-018**](http://go.microsoft.com/fwlink/?linkid=235364)
</td>
<td style="border:1px solid black;">
[**MS12-019**](http://go.microsoft.com/fwlink/?linkid=239573)
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
Brak
</td>
<td style="border:1px solid black;">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Umiarkowany**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=39abdf7b-ea9d-4b95-a28d-4140374d531d)  
(KB2621440)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Vista z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f4e73a92-583b-4352-b19d-7a8e3ef162b7)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Vista z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7da5b341-6a6f-46de-8d01-448da38e9908)  
(Umiarkowany)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e5970daf-4440-42fa-8efc-e6190c6a22aa)  
(KB2621440)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ead9d29b-becf-448e-bff4-d5bb12d02c64)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1ba25d9c-0fef-471f-8e30-045fe9586a9c)  
(Umiarkowany)
</td>
</tr>
<tr>
<th colspan="5">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS12-020**](http://go.microsoft.com/fwlink/?linkid=232664)
</td>
<td style="border:1px solid black;">
[**MS12-017**](http://go.microsoft.com/fwlink/?linkid=235401)
</td>
<td style="border:1px solid black;">
[**MS12-018**](http://go.microsoft.com/fwlink/?linkid=235364)
</td>
<td style="border:1px solid black;">
[**MS12-019**](http://go.microsoft.com/fwlink/?linkid=239573)
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
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Umiarkowany**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 z dodatkiem Service Pack 2 dla systemów 32-bitowych
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów 32-bitowych z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fef2c1d7-2004-43d7-aa49-673c6f374670)\*  
(KB2621440)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów 32-bitowych z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=233c62b7-f2b1-49ce-9a7f-e51435be0d26)\*  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów 32-bitowych z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=dd547364-f6bb-453c-9e4d-6b80dfc47fbb)\*  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów 32-bitowych z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=45a4784e-5051-4628-9a19-d53f30c1fdf3)\*\*  
(Umiarkowany)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem x64
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem x64 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4ffae13f-3432-4849-a2da-a76f96d7ceb3)\*  
(KB2621440)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem x64 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=56eae770-5990-4e1b-8b48-3d0602fcc72b)\*  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem x64 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5ff65fc2-5969-4d7e-9c72-9a2096dafdcf)\*  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=503cb9c0-d6db-4deb-a555-67af0b25739b)\*\*  
(Umiarkowany)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem Itanium
</td>
<td style="border:1px solid black;">
[Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=67581250-50fd-4f4c-a3cc-45ce2662b0c3)  
(KB2621440)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=eeb5385c-fb81-4d33-af2a-986e6cf14ee2)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr>
<th colspan="5">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS12-020**](http://go.microsoft.com/fwlink/?linkid=232664)
</td>
<td style="border:1px solid black;">
[**MS12-017**](http://go.microsoft.com/fwlink/?linkid=235401)
</td>
<td style="border:1px solid black;">
[**MS12-018**](http://go.microsoft.com/fwlink/?linkid=235364)
</td>
<td style="border:1px solid black;">
[**MS12-019**](http://go.microsoft.com/fwlink/?linkid=239573)
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
Brak
</td>
<td style="border:1px solid black;">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Umiarkowany**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 dla systemów 32-bitowych i Windows 7 z dodatkiem Service Pack 1 dla systemów 32-bitowych
</td>
<td style="border:1px solid black;">
[Windows 7 dla systemów 32-bitowych i Windows 7 z dodatkiem Service Pack 1 dla systemów 32-bitowych](http://www.microsoft.com/downloads/details.aspx?familyid=16b0195c-84d3-4c08-8b98-ff2c80d144e1)  
(KB2621440)  
(Krytyczny)  
[Windows 7 dla systemów 32-bitowych i Windows 7 z dodatkiem Service Pack 1 dla systemów 32-bitowych](http://www.microsoft.com/downloads/details.aspx?familyid=3a6c7fdf-105a-4886-ad52-c892f37e32d1)  
(KB2667402)  
(Umiarkowany)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows 7 dla systemów 32-bitowych i Windows 7 z dodatkiem Service Pack 1 dla systemów 32-bitowych](http://www.microsoft.com/downloads/details.aspx?familyid=75fd93ff-5be5-42b5-ab00-3378e545c271)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows 7 dla systemów 32-bitowych i Windows 7 z dodatkiem Service Pack 1 dla systemów 32-bitowych](http://www.microsoft.com/downloads/details.aspx?familyid=f3a14012-38ae-490e-a48e-7c851f82a7e6)  
(Umiarkowany)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 dla systemów opartych na procesorach x64 i Windows 7 z dodatkiem Service Pack 1 dla systemów opartych na procesorach x64
</td>
<td style="border:1px solid black;">
[Windows 7 dla systemów opartych na procesorach x64 i Windows 7 z dodatkiem Service Pack 1 dla systemów opartych na procesorach x64](http://www.microsoft.com/downloads/details.aspx?familyid=40b62d08-d2a2-4900-b01c-46fc761973d0)  
(KB2621440)  
(Krytyczny)  
[Windows 7 dla systemów opartych na procesorach x64 i Windows 7 z dodatkiem Service Pack 1 dla systemów opartych na procesorach x64](http://www.microsoft.com/downloads/details.aspx?familyid=1bbe7cda-4bee-4d65-8127-3c13624a1168)  
(KB2667402)  
(Umiarkowany)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows 7 dla systemów opartych na procesorach x64 i Windows 7 z dodatkiem Service Pack 1 dla systemów opartych na procesorach x64](http://www.microsoft.com/downloads/details.aspx?familyid=71ffba4c-d816-45a9-abef-131915885bc8)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows 7 dla systemów opartych na procesorach x64 i Windows 7 z dodatkiem Service Pack 1 dla systemów opartych na procesorach x64](http://www.microsoft.com/downloads/details.aspx?familyid=760b5aa4-4e65-4ff1-9ae2-771234803bf0)  
(Umiarkowany)
</td>
</tr>
<tr>
<th colspan="5">
System Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS12-020**](http://go.microsoft.com/fwlink/?linkid=232664)
</td>
<td style="border:1px solid black;">
[**MS12-017**](http://go.microsoft.com/fwlink/?linkid=235401)
</td>
<td style="border:1px solid black;">
[**MS12-018**](http://go.microsoft.com/fwlink/?linkid=235364)
</td>
<td style="border:1px solid black;">
[**MS12-019**](http://go.microsoft.com/fwlink/?linkid=239573)
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
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Umiarkowany**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 dla systemów opartych na procesorach x64 i Windows Server 2008 R2 z dodatkiem Service Pack 1 dla systemów opartych na procesorach x64
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach x64 i Windows Server 2008 R2 z dodatkiem Service Pack 1 dla systemów opartych na procesorach x64](http://www.microsoft.com/downloads/details.aspx?familyid=7c1774cc-e00c-47f3-97a2-bc90de857793)\*  
(KB2621440)  
(Krytyczny)  
[Windows Server 2008 R2 dla systemów opartych na procesorach x64 i Windows Server 2008 R2 z dodatkiem Service Pack 1 dla systemów opartych na procesorach x64](http://www.microsoft.com/downloads/details.aspx?familyid=7ec21f41-1673-4592-b45c-6438ad57e08c)\*  
(KB2667402)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach x64 i Windows Server 2008 R2 z dodatkiem Service Pack 1 dla systemów opartych na procesorach x64](http://www.microsoft.com/downloads/details.aspx?familyid=19a4f3d1-24d2-41af-a41a-e5cc2c6232e8)\*  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach x64 i Windows Server 2008 R2 z dodatkiem Service Pack 1 dla systemów opartych na procesorach x64](http://www.microsoft.com/downloads/details.aspx?familyid=22d6a234-6447-4854-8119-4fddd3c6e1bb)\*  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach x64 i Windows Server 2008 R2 z dodatkiem Service Pack 1 dla systemów opartych na procesorach x64](http://www.microsoft.com/downloads/details.aspx?familyid=86095b20-5869-4b55-8777-ee0af82aaf37)\*\*  
(Umiarkowany)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 dla systemów opartych na procesorach Itanium i Windows Server 2008 R2 z dodatkiem Service Pack 1 dla systemów opartych na procesorach Itanium
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach Itanium i Windows Server 2008 R2 z dodatkiem Service Pack 1 dla systemów opartych na procesorach Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=6a07f99c-8ab4-4e44-8d48-6ac787dd2b51)  
(KB2621440)  
(Krytyczny)  
[Windows Server 2008 R2 dla systemów opartych na procesorach Itanium i Windows Server 2008 R2 z dodatkiem Service Pack 1 dla systemów opartych na procesorach Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=469aa1f6-ed89-4649-8736-eaa5e2ad44ee)  
(KB2667402)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach Itanium i Windows Server 2008 R2 z dodatkiem Service Pack 1 dla systemów opartych na procesorach Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=cb5ac981-e8e5-4df7-84bb-7a2a916d0ce9)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach Itanium i Windows Server 2008 R2 z dodatkiem Service Pack 1 dla systemów opartych na procesorach Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=dc5c336f-329c-4a56-8b24-555e3c8afd50)  
(Umiarkowany)
</td>
</tr>
</table>
 
**Uwagi dotyczące systemu Windows Server 2008 i Windows Server 2008 R2**

**\*Luka w zabezpieczeniach dotyczy instalacji Server Core.** Ta aktualizacja ma zastosowanie, z takim samym wskaźnikiem ważności, w przypadku obsługiwanych wersji systemu Windows Server 2008 lub Windows Server 2008 R2, niezależnie od tego, czy zostały zainstalowane przy użyciu opcji instalacji Server Core. Więcej informacji na temat tej opcji instalacji można znaleźć w artykułach TechNet, [Managing a Server Core Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) i [Servicing a Server Core Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) (jęz. ang.). Należy pamiętać, że opcja instalacji Server Core nie dotyczy niektórych wersji systemu Windows Server 2008 i Windows Server 2008 R2. Zobacz [Porównanie opcji instalacji Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Luka w zabezpieczeniach nie dotyczy instalacji Server Core.** Luki usuwane przez tę aktualizację zabezpieczeń nie dotyczą obsługiwanych wersji systemu Windows Server 2008 ani Windows Server 2008 R2, jeżeli systemy te zostały zainstalowane przy użyciu opcji instalacji Server Core. Więcej informacji na temat tej opcji instalacji można znaleźć w artykułach TechNet, [Managing a Server Core Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) i [Servicing a Server Core Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) (jęz. ang.). Należy pamiętać, że opcja instalacji Server Core nie dotyczy niektórych wersji systemu Windows Server 2008 i Windows Server 2008 R2. Zobacz [Porównanie opcji instalacji Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

#### Narzędzia i oprogramowanie firmy Microsoft dla deweloperów

 
<table style="border:1px solid black;">
<tr>
<th colspan="3">
Microsoft Visual Studio
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS12-021**](http://go.microsoft.com/fwlink/?linkid=235362)
</td>
<td style="border:1px solid black;">
[**MS12-022**](http://go.microsoft.com/fwlink/?linkid=235361)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Zbiorczy wskaźnik ważności**
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
Microsoft Visual Studio 2008 z dodatkiem Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio 2008 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=99d7c39a-14f1-4e7e-8a4f-2466b16821eb)  
(KB2669970)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual Studio 2010
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio 2010](http://www.microsoft.com/downloads/details.aspx?familyid=f80235ae-da15-4527-93b3-c2f31ec2f387)  
(KB2644980)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visual Studio 2010 z dodatkiem Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio 2010 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=e2aaec35-b2c0-48f0-8a51-34e44f6d12fb)  
(KB2645410)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr>
<th colspan="3">
Microsoft Expression Design
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS12-021**](http://go.microsoft.com/fwlink/?linkid=235362)
</td>
<td style="border:1px solid black;">
[**MS12-022**](http://go.microsoft.com/fwlink/?linkid=235361)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Zbiorczy wskaźnik ważności**
</td>
<td style="border:1px solid black;">
Brak
</td>
<td style="border:1px solid black;">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Expression Design
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Microsoft Expression Design](http://www.microsoft.com/downloads/details.aspx?familyid=49e12f3a-718d-4d54-82be-b78efb372d07)  
(KB2675064)  
(Ważny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Expression Design z dodatkiem Service Pack 1
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Microsoft Expression Design z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=899c6860-6081-429b-971a-4d689444920f)  
(KB2667724)  
(Ważny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Expression Design 2
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Microsoft Expression Design 2](http://www.microsoft.com/downloads/details.aspx?familyid=2ca4fb5a-3ab4-410b-b42b-075eb1d70410)  
(KB2667725)  
(Ważny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Expression Design 3
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Microsoft Expression Design 3](http://www.microsoft.com/downloads/details.aspx?familyid=73b44e97-6dda-4e24-9758-e86a1de4c0c8)  
(KB2667727)  
(Ważny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Expression Design 4
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Microsoft Expression Design 4](http://www.microsoft.com/downloads/details.aspx?familyid=be56221e-4271-42dc-a6e4-ebf0290e4ad8)  
(KB2667730)  
(Ważny)
</td>
</tr>
</table>
 

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

-   [Nikolaos Bougalis](https://technet.microsoft.com/pl-PL/mailto:nikb@bougalis.net), za zgłoszenie problemu opisanego w biuletynie MS12-018
-   Khaled M. Salameh za zgłoszenie problemu opisanego w biuletynie MS12-019
-   Luigi Auriemma, współpracujący z oddziałem [Zero Day Initiative](http://www.zerodayinitiative.com/) firmy [TippingPoint](http://www.tippingpoint.com/), za zgłoszenie problemu opisanego w biuletynie MS12-020
-   Firma [Laplinker](http://www.laplinker.com) za zgłoszenie problemu opisanego w biuletynie MS12-021
-   Firma [Laplinker](http://www.laplinker.com) za zgłoszenie problemu opisanego w biuletynie MS12-022

#### Pomoc techniczna

-   Wymienione oprogramowanie zostało przetestowane w celu ustalenia, których wersji dotyczy problem. Dla pozostałych wersji upłynął okres pomocy technicznej. Aby zapoznać się z zasadami cyklu pomocy technicznej dotyczącymi używanej wersji oprogramowania, odwiedź [witrynę zasad cyklu pomocy technicznej firmy Microsoft](http://go.microsoft.com/fwlink/?linkid=21742).
-   Klienci mogą uzyskać pomoc techniczną w [Biurze Obsługi Klienta Microsoft](http://go.microsoft.com/fwlink/?linkid=21131) pod numerem 0 801 802 000 (opłata według stawek Twojego operatora) lub (0-22) 594 19 99 w godzinach od 9:00 do 17:00, od poniedziałku do piątku. Dodatkowe informacje dotyczące możliwości skorzystania z pomocy technicznej można znaleźć w witrynie [Pomoc i obsługa techniczna firmy Microsoft](http://support.microsoft.com/).
-   Klienci międzynarodowi mogą uzyskać pomoc w lokalnych przedstawicielstwach firmy Microsoft. Informacje o sposobie kontaktowania się z pomocą techniczną firmy Microsoft są dostępne w [międzynarodowej witrynie sieci Web pomocy i obsługi technicznej](http://go.microsoft.com/fwlink/?linkid=21155).

#### Zrzeczenie odpowiedzialności

Informacje w bazie wiedzy Microsoft Knowledge Base są dostarczane „tak jak są” bez jakiejkolwiek gwarancji. Firma Microsoft odrzuca wszelkie gwarancje, wyraźne i dorozumiane, w tym gwarancje dotyczące wartości handlowej i przydatności do określonego celu. Firma Microsoft Corporation ani jej dostawcy w żadnym wypadku nie ponoszą odpowiedzialności za jakiekolwiek szkody, w tym bezpośrednie, pośrednie, przypadkowe, wynikowe, utratę zysków handlowych lub szkody specjalne, nawet jeżeli firmę Microsoft Corporation lub jej dostawców powiadomiono o możliwości zaistnienia takich szkód. W niektórych stanach wyłączenie lub ograniczenie odpowiedzialności za straty wynikowe lub przypadkowe, a więc i powyższe ograniczenia, nie mają zastosowania.

#### Wersje

-   Wersja 1.0 (13 marca 2012 r.): Opublikowane podsumowanie biuletynów zabezpieczeń.

*Built at 2014-04-18T01:50:00Z-07:00*
