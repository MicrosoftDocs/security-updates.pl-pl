---
TOCTitle: 'MS12-JAN'
Title: 'Podsumowanie biuletynów zabezpieczeń firmy Microsoft za styczeń 2012 r.'
ms:assetid: 'ms12-jan'
ms:contentKeyID: 61233135
ms:mtpsurl: 'https://technet.microsoft.com/pl-PL/library/ms12-jan(v=Security.10)'
---
Podsumowanie biuletynów zabezpieczeń firmy Microsoft za styczeń 2012 r.
=======================================================================

Opublikowano: 10 stycznia 2012 | Zaktualizowano: 27 stycznia 2012

**Wersja:** 2.1

Niniejsze podsumowanie biuletynów zabezpieczeń zawiera spis biuletynów za styczeń 2012 r.

Z chwilą opublikowania biuletynów zabezpieczeń za styczeń 2012 r. niniejsze podsumowanie biuletynów zastąpi powiadomienie o biuletynach zabezpieczeń wydane 5 stycznia 2012 r. Aby uzyskać więcej informacji na temat usługi powiadamiania o biuletynach, zobacz [Powiadomienia o biuletynach zabezpieczeń firmy Microsoft (j. ang.)](http://go.microsoft.com/fwlink/?linkid=217213).

Aby dowiedzieć się, jak otrzymywać automatyczne powiadomienia o publikacji biuletynów zabezpieczeń firmy Microsoft, odwiedź stronę [Microsoft Technical Security Notifications](http://go.microsoft.com/fwlink/?linkid=21163).

11 stycznia 2012 r. o godz. 11:00 czasu Pacyfiku (godz. 20:00 czasu środkowoeuropejskiego) firma Microsoft udostępni emisję internetową, w której znajdą się odpowiedzi na pytania klientów dotyczące tych biuletynów (USA i Kanada). [Zarejestruj się, aby zobaczyć emisję internetową dotyczącą biuletynów zabezpieczeń za styczeń](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032499498). Po tym dniu emisja internetowa będzie dostępna na żądanie. Aby uzyskać więcej informacji, zobacz [Podsumowania biuletynów zabezpieczeń i emisje internetowe firmy Microsoft](http://go.microsoft.com/fwlink/?linkid=217214).

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=227487">MS12-004</a></td>
<td style="border:1px solid black;"><strong>Luki w zabezpieczeniach formatu Windows Media umożliwiają zdalne wykonanie kodu (2636391)</strong><br />
<br />
Ta aktualizacja zabezpieczeń usuwa dwie luki w zabezpieczeniach systemu Windows, które zostały zgłoszone przez użytkowników. Luki te mogą umożliwić zdalne wykonanie kodu, jeśli użytkownik otworzy specjalnie spreparowany plik multimedialny. Osoba atakująca, której uda się wykorzystać luki, może uzyskać takie same prawa użytkownika jak użytkownik lokalny. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Krytyczny</a><br />
Zdalne wykonanie kodu</td>
<td style="border:1px solid black;">Wymaga ponownego uruchomienia komputera</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=235999">MS12-001</a></td>
<td style="border:1px solid black;"><strong>Luka w zabezpieczeniach jądra systemu Windows może pozwolić na obejście funkcji zabezpieczeń (2644615)</strong><br />
<br />
Ta aktualizacja zabezpieczeń usuwa lukę w zabezpieczeniach systemu Microsoft Windows. Luka w zabezpieczeniach może pozwolić osobie atakującej na obejście funkcji zabezpieczeń SafeSEH w aplikacji. Osoba atakująca może następnie użyć innych luk, aby wykorzystać strukturalną procedurę obsługi wyjątków do uruchomienia dowolnego kodu. Omawiana luka może zostać wykorzystana tylko przy użyciu aplikacji skompilowanych przy użyciu oprogramowania Microsoft Visual C++ .NET 2003.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Ważny</a><br />
Obejście funkcji zabezpieczeń</td>
<td style="border:1px solid black;">Wymaga ponownego uruchomienia komputera</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=229637">MS12-002</a></td>
<td style="border:1px solid black;"><strong>Luka w zabezpieczeniach programu Pakowarka obiektów systemu Windows umożliwia zdalne wykonanie kodu (2603381)</strong><br />
<br />
Ta aktualizacja zabezpieczeń usuwa lukę w zabezpieczeniach systemu Microsoft Windows. Luka ta umożliwia zdalne wykonanie kodu, gdy użytkownik otworzy prawidłowy plik z osadzonym spakowanym obiektem, który znajduje się w tym samym katalogu sieciowym, co specjalnie spreparowany plik wykonywalny. Osoba atakująca, której uda się wykorzystać tę lukę, może uzyskać takie same uprawnienia, jak zalogowany użytkownik. Osoba taka mogłaby wówczas instalować programy, przeglądać, zmieniać i usuwać dane oraz tworzyć nowe konta z pełnymi uprawnieniami. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Ważny</a><br />
Zdalne wykonanie kodu</td>
<td style="border:1px solid black;">Może wymagać ponownego uruchomienia</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=235400">MS12-003</a></td>
<td style="border:1px solid black;"><strong>Luka w zabezpieczeniach Podsystemu wykonawczego serwera klienta w systemie Windows umożliwia podniesienie uprawnień (2646524)</strong><br />
<br />
Ta aktualizacja zabezpieczeń usuwa lukę w zabezpieczeniach systemu Microsoft Windows zgłoszoną przez użytkowników. Niniejsza aktualizacja zabezpieczeń ma wskaźnik ważności „ważny” dla wszystkich obsługiwanych wersji systemów Windows XP, Windows Server 2003, Windows Vista i Windows Server 2008. Omawiana luka nie dotyczy żadnej z obsługiwanych wersji systemów Windows 7 ani Windows Server 2008 R2.<br />
<br />
Luka ta może umożliwić podniesienie uprawnień, jeśli osoba atakująca zaloguje się do zagrożonego systemu i uruchomi specjalnie spreparowaną aplikację. Osoba atakująca może wówczas przejąć pełną kontrolę nad zagrożonym systemem i instalować programy; wyświetlać, zmieniać i usuwać dane; lub tworzyć nowe konta z pełnymi prawami użytkownika. Omawianą lukę można wykorzystać wyłącznie w systemach z chińskimi, japońskimi lub koreańskimi ustawieniami regionalnymi.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Ważny</a><br />
Podniesienie uprawnień</td>
<td style="border:1px solid black;">Wymaga ponownego uruchomienia komputera</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=230777">MS12-005</a></td>
<td style="border:1px solid black;"><strong>Luka w zabezpieczeniach systemu Microsoft Windows może pozwolić na zdalne wykonanie kodu (2584146)</strong><br />
<br />
Ta aktualizacja zabezpieczeń usuwa lukę w zabezpieczeniach systemu Microsoft Windows. Luka w zabezpieczeniach może umożliwić zdalne wykonanie kodu, jeśli użytkownik otworzy specjalnie spreparowany plik pakietu Microsoft Office zawierający złośliwą osadzoną aplikację ClickOnce. Osoba atakująca, której uda się wykorzystać tę lukę, może uzyskać takie same uprawnienia, jak użytkownik lokalny. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Ważny</a><br />
Zdalne wykonanie kodu</td>
<td style="border:1px solid black;">Może wymagać ponownego uruchomienia</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=232510">MS12-006</a></td>
<td style="border:1px solid black;"><strong>Luka w zabezpieczeniach protokołu SSL/TLS umożliwia ujawnienie informacji (2643584)</strong><br />
<br />
Ta aktualizacja zabezpieczeń usuwa lukę w zabezpieczeniach protokołów SSL 3.0 i TLS 1.0, która została zgłoszona przez organizację publiczną. Luka ta dotyczy samego protokołu i nie jest właściwa dla systemu operacyjnego Windows. Omawiana luka może pozwolić na ujawnienie informacji, jeśli osoba atakująca przechwyci zaszyfrowany ruch przesyłany z systemu podlegającego luce. Luka nie dotyczy protokołów TLS 1.1, TLS 1.2 ani żadnych pakietów szyfrów, w których nie jest wykorzystywany tryb CBC.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Ważny</a><br />
Ujawnienie informacji</td>
<td style="border:1px solid black;">Wymaga ponownego uruchomienia komputera</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=227561">MS12-007</a></td>
<td style="border:1px solid black;"><strong>Luka w zabezpieczeniach biblioteki</strong> <strong>AntiXSS</strong> <strong>może pozwolić na ujawnienie informacji (2607664)</strong><br />
<br />
Ta aktualizacja zabezpieczeń usuwa jedną lukę w zabezpieczeniach biblioteki AntiXSS (Microsoft Anti-Cross Site Scripting) zgłoszoną przez użytkowników. Luka ta może pozwolić na ujawnienie informacji w przypadku, gdy osoba atakująca przekaże do witryny sieci Web złośliwy skrypt za pomocą funkcji oczyszczania biblioteki AntiXSS. Konsekwencje ujawnienia informacji zależą od ich charakteru. Należy zauważyć, że ta luka nie pozwala osobie atakującej na wykonanie kodu ani bezpośrednie podniesienie poziomu jej praw użytkownika, może jednak zostać wykorzystana do uzyskania informacji przydatnych do dalszego naruszenia integralności zagrożonego systemu. Omawiana luka zagraża tylko witrynom, które korzystają z modułu oczyszczania biblioteki AntiXSS.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Ważny</a><br />
Ujawnienie informacji</td>
<td style="border:1px solid black;">Może wymagać ponownego uruchomienia</td>
<td style="border:1px solid black;">Narzędzia i oprogramowanie firmy Microsoft dla deweloperów</td>
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
  
| Identyfikator biuletynu                                   | Nazwa luki w zabezpieczeniach                                                                                    | CVE ID                                                                           | Ocena możliwości wykorzystania luki w najnowszej wersji programu                                            | Ocena możliwości wykorzystania luki w poprzedniej wersji programu                                           | Ocena możliwości wykorzystania luki w celu wytworzenia sytuacji typu „odmowa usługi” | Najważniejsze uwagi                                                                                                            |  
|-----------------------------------------------------------|------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------|  
| [MS12-001](http://go.microsoft.com/fwlink/?linkid=235999) | Luka w zabezpieczeniach związana z obejściem funkcji SafeSEH jądra systemu Windows                               | [CVE-2012-0001](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0001) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny kod wykorzystujący lukę      | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny kod wykorzystujący lukę      | Nie dotyczy                                                                          | Jest to luka związana z obejściem zabezpieczeń.                                                                                |  
| [MS12-002](http://go.microsoft.com/fwlink/?linkid=229637) | Luka w zabezpieczeniach programu Pakowarka obiektów związana z niebezpiecznym uruchamianiem plików wykonywalnych | [CVE-2012-0009](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0009) | Brak zagrożenia                                                                                             | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny kod wykorzystujący lukę      | Nie dotyczy                                                                          | (Brak)                                                                                                                         |  
| [MS12-003](http://go.microsoft.com/fwlink/?linkid=235400) | Luka w zabezpieczeniach podsystemu CSRSS umożliwiająca podniesienie poziomu uprawnień                            | [CVE-2012-0005](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0005) | Brak zagrożenia                                                                                             | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny kod wykorzystujący lukę      | Stałe                                                                                | (Brak)                                                                                                                         |  
| [MS12-004](http://go.microsoft.com/fwlink/?linkid=227487) | Luka w zabezpieczeniach obsługi plików MIDI umożliwiająca zdalne wykonanie kodu                                  | [CVE-2012-0003](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0003) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny kod wykorzystujący lukę      | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny kod wykorzystujący lukę      | Nie dotyczy                                                                          | (Brak)                                                                                                                         |  
| [MS12-004](http://go.microsoft.com/fwlink/?linkid=227487) | Luka w zabezpieczeniach programu DirectShow umożliwiająca zdalne wykonanie kodu                                  | [CVE-2012-0004](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0004) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny kod wykorzystujący lukę      | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny kod wykorzystujący lukę      | Nie dotyczy                                                                          | (Brak)                                                                                                                         |  
| [MS12-005](http://go.microsoft.com/fwlink/?linkid=230777) | Luka w zabezpieczeniach związana z wykonywaniem zestawów                                                         | [CVE-2012-0013](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0013) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny kod wykorzystujący lukę      | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny kod wykorzystujący lukę      | Nie dotyczy                                                                          | (Brak)                                                                                                                         |  
| [MS12-006](http://go.microsoft.com/fwlink/?linkid=232510) | Luka w zabezpieczeniach protokołów SSL i TLS                                                                     | [CVE-2011-3389](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-3389) | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) — kod wykorzystujący lukę mało prawdopodobny | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) — kod wykorzystujący lukę mało prawdopodobny | Nie dotyczy                                                                          | Ta luka może doprowadzić do ujawnienia informacji i została ujawniona publicznie z ograniczeniem ilości podawanych szczegółów. |  
| [MS12-007](http://go.microsoft.com/fwlink/?linkid=227561) | Luka w zabezpieczeniach związana z obejściem biblioteki AntiXSS                                                  | [CVE-2012-0007](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0007) | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) — kod wykorzystujący lukę mało prawdopodobny | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) — kod wykorzystujący lukę mało prawdopodobny | Nie dotyczy                                                                          | Ta luka może doprowadzić do ujawnienia informacji.                                                                             |
  
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
<th colspan="7">
Windows XP  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS12-004**](http://go.microsoft.com/fwlink/?linkid=227487)
</td>
<td style="border:1px solid black;">
[**MS12-001**](http://go.microsoft.com/fwlink/?linkid=235999)
</td>
<td style="border:1px solid black;">
[**MS12-002**](http://go.microsoft.com/fwlink/?linkid=229637)
</td>
<td style="border:1px solid black;">
[**MS12-003**](http://go.microsoft.com/fwlink/?linkid=235400)
</td>
<td style="border:1px solid black;">
[**MS12-005**](http://go.microsoft.com/fwlink/?linkid=230777)
</td>
<td style="border:1px solid black;">
[**MS12-006**](http://go.microsoft.com/fwlink/?linkid=232510)
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
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
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
[Biblioteka multimediów systemu Windows](http://www.microsoft.com/downloads/details.aspx?familyid=a142f7ba-4268-4453-a8eb-470213c028ac)  
(KB2598479)  
(Krytyczny)  
[Biblioteka multimediów systemu Windows](http://www.microsoft.com/downloads/details.aspx?familyid=89b23d72-410f-4133-9c14-24eb01e5a732)  
(KB2628259)  
(tylko Windows XP Media Center Edition 2005 z dodatkiem Service Pack 3)  
(Krytyczny)  
[DirectShow](http://www.microsoft.com/downloads/details.aspx?familyid=4b168ee8-eb15-4c2c-afb0-e63d62b4a6dc)  
(KB2631813)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows XP z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=feaeda8c-84ee-47be-8c68-736f0e5b1fc7)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows XP z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=cfc38dc2-c4c7-4a44-8e5a-b98bb9bc0396)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows XP z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=1bcb1d1e-9261-4a36-9256-90d3df9bd4fb)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows XP z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=fb0360b1-254c-4ecb-a36a-807cabfec1ab)  
(KB2585542)  
(Ważny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Biblioteka multimediów systemu Windows](http://www.microsoft.com/downloads/details.aspx?familyid=0928d720-ae88-40d6-b76f-636d67da8526)  
(KB2598479)  
(Krytyczny)  
[DirectShow](http://www.microsoft.com/downloads/details.aspx?familyid=13d74cc6-8d8e-45ea-8cdc-c15782f6626b)  
(KB2631813)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=46386269-6e37-4710-bfef-cedfe60d881c)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=211827f2-fe6a-4e16-a90c-0cc3b60a722d)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3956db98-88d9-49fc-be51-247b40bfc272)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2c687796-4c41-4d17-b738-511d2fbfc126)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=afe6b34d-21b1-4dfa-afa6-2c5c2a678e9e)  
(KB2585542)  
(Ważny)  
[Windows XP Professional x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=986f1156-0190-48c2-9f39-29cacb91f0f9)  
(KB2638806)  
(Ważny)
</td>
</tr>
<tr>
<th colspan="7">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator** **biuletynu**
</td>
<td style="border:1px solid black;">
[**MS12-004**](http://go.microsoft.com/fwlink/?linkid=227487)
</td>
<td style="border:1px solid black;">
[**MS12-001**](http://go.microsoft.com/fwlink/?linkid=235999)
</td>
<td style="border:1px solid black;">
[**MS12-002**](http://go.microsoft.com/fwlink/?linkid=229637)
</td>
<td style="border:1px solid black;">
[**MS12-003**](http://go.microsoft.com/fwlink/?linkid=235400)
</td>
<td style="border:1px solid black;">
[**MS12-005**](http://go.microsoft.com/fwlink/?linkid=230777)
</td>
<td style="border:1px solid black;">
[**MS12-006**](http://go.microsoft.com/fwlink/?linkid=232510)
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
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Biblioteka multimediów systemu Windows](http://www.microsoft.com/downloads/details.aspx?familyid=3c266dfb-630d-4f32-b2ca-63955279b6a9)  
(KB2598479)  
(Krytyczny)  
[DirectShow](http://www.microsoft.com/downloads/details.aspx?familyid=89ae6ed0-537f-421c-b755-ef28691abd88)  
(KB2631813)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9cdfc0fe-8f43-4e13-8a1f-2b48ff9ff472)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b8e46267-7988-4fbe-ae94-68b6fdb2e7d9)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=39f5f8fb-ee4d-4b7a-9cd7-3d1e9c8abd8c)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2c39be84-1eab-4794-b3ed-e529643aca21)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e2c503a5-3f15-4a77-9a05-9ea0fbaf4503)  
(KB2585542)  
(Ważny)  
[Windows Server 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c23e7604-d489-4836-8b54-3b2b3d6a365c)  
(KB2638806)  
(Ważny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Biblioteka multimediów systemu Windows](http://www.microsoft.com/downloads/details.aspx?familyid=8dd1c882-4ed1-4e47-a017-7d162bd94194)  
(KB2598479)  
(Krytyczny)  
[DirectShow](http://www.microsoft.com/downloads/details.aspx?familyid=08be569c-e9d1-4fc5-8670-ebe9da0a2072)  
(KB2631813)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4e5783aa-6847-404c-9b75-621fa14ebbb8)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5975b01e-139b-4b9d-a0d5-a87a279bfea1)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e27d85f8-a285-4e95-85a0-0868286cc2b9)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3cf29dfd-239e-4707-92e6-952133c1c1c2)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2ad34496-40af-40cb-9f85-5d3c31543211)  
(KB2585542)  
(Ważny)  
[Windows Server 2003 x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2f36e991-4e1a-4b8c-8cfb-e7f20d97cf0b)  
(KB2638806)  
(Ważny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium
</td>
<td style="border:1px solid black;">
[Biblioteka multimediów systemu Windows](http://www.microsoft.com/downloads/details.aspx?familyid=3a9b09d6-7060-47ab-9f76-c3c5acb024e6)  
(KB2598479)  
(Krytyczny)  
[DirectShow](http://www.microsoft.com/downloads/details.aspx?familyid=3401ac20-3701-471f-9757-097a9402d761)  
(KB2631813)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=cdf8208c-d55b-428f-bdd3-26e291dfb08d)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=26079c35-4b96-42fc-ad47-138be25a6bf0)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=b69bd01d-9925-4ff1-bfeb-b4473631578c)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=623c1c7d-6902-4876-9614-1b6e1ef80831)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=56deb935-9226-49f8-b705-edb3d662d8aa)  
(KB2585542)  
(Ważny)  
[Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=2d72cf5a-cca7-4341-b862-017e3f34a3c9)  
(KB2638806)  
(Ważny)
</td>
</tr>
<tr>
<th colspan="7">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS12-004**](http://go.microsoft.com/fwlink/?linkid=227487)
</td>
<td style="border:1px solid black;">
[**MS12-001**](http://go.microsoft.com/fwlink/?linkid=235999)
</td>
<td style="border:1px solid black;">
[**MS12-002**](http://go.microsoft.com/fwlink/?linkid=229637)
</td>
<td style="border:1px solid black;">
[**MS12-003**](http://go.microsoft.com/fwlink/?linkid=235400)
</td>
<td style="border:1px solid black;">
[**MS12-005**](http://go.microsoft.com/fwlink/?linkid=230777)
</td>
<td style="border:1px solid black;">
[**MS12-006**](http://go.microsoft.com/fwlink/?linkid=232510)
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
Brak
</td>
<td style="border:1px solid black;">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Biblioteka multimediów systemu Windows](http://www.microsoft.com/downloads/details.aspx?familyid=99d9b9fc-ed37-4a32-a20d-6604a1b9c4ca)  
(KB2598479)  
(Krytyczny)  
[Pakiet Windows Media Center TV Pack dla systemu Windows Vista (wersje 32-bitowe)](http://www.microsoft.com/downloads/details.aspx?familyid=f345e093-336d-4464-b7f8-a14398b62ebf)<sup>[1]</sup>
(KB2628642)  
(Ważny)  
[DirectShow](http://www.microsoft.com/downloads/details.aspx?familyid=4818059a-52ad-4c2e-9605-4e0f5d9da5ba)  
(KB2631813)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Vista z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=44eeb0a2-ae17-4971-8a7e-e25b260c582c)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Vista z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=73682d4b-3179-4488-8ba9-94ed68c4896b)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Vista z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=038970b6-aeec-4e18-8dfe-887b260a7c87)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Vista z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f9269bd6-8c4f-476e-8481-fc0de52a22e6)  
(KB2585542)  
(Ważny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Biblioteka multimediów systemu Windows](http://www.microsoft.com/downloads/details.aspx?familyid=44aa8d91-2b30-4191-8965-8aee2b860d50)  
(KB2598479)  
(Krytyczny)  
[Pakiet Windows Media Center TV Pack dla systemu Windows Vista (wersje 64-bitowe)](http://www.microsoft.com/downloads/details.aspx?familyid=559d028f-9810-4c50-b65d-f567cbb15427)<sup>[1]</sup>
(KB2628642)  
(Ważny)  
[DirectShow](http://www.microsoft.com/downloads/details.aspx?familyid=13cc2519-860d-4c64-b7f8-8f9c0bdaefcf)  
(KB2631813)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=79ceba86-59a1-4138-a5de-8df20ad81b02)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b5c33025-13d9-43d2-a415-a8a4d683a821)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=23abeb12-f2fe-43fd-9c4a-4d3d244832f8)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0403c753-d4fa-4e3d-a61b-7f816f5c352b)  
(KB2585542)  
(Ważny)
</td>
</tr>
<tr>
<th colspan="7">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS12-004**](http://go.microsoft.com/fwlink/?linkid=227487)
</td>
<td style="border:1px solid black;">
[**MS12-001**](http://go.microsoft.com/fwlink/?linkid=235999)
</td>
<td style="border:1px solid black;">
[**MS12-002**](http://go.microsoft.com/fwlink/?linkid=229637)
</td>
<td style="border:1px solid black;">
[**MS12-003**](http://go.microsoft.com/fwlink/?linkid=235400)
</td>
<td style="border:1px solid black;">
[**MS12-005**](http://go.microsoft.com/fwlink/?linkid=230777)
</td>
<td style="border:1px solid black;">
[**MS12-006**](http://go.microsoft.com/fwlink/?linkid=232510)
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
Brak
</td>
<td style="border:1px solid black;">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 z dodatkiem Service Pack 2 dla systemów 32-bitowych
</td>
<td style="border:1px solid black;">
[Biblioteka multimediów systemu Windows](http://www.microsoft.com/downloads/details.aspx?familyid=787e6285-3ba5-4aae-9d8d-e3c1eca3b35d)\*  
(KB2598479)  
(Krytyczny)  
[DirectShow](http://www.microsoft.com/downloads/details.aspx?familyid=92df13c1-fdf6-4602-acb2-e634a1bcd9da)\*\*  
(KB2631813)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów 32-bitowych z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5ab87c6c-5802-4454-bce4-12501e5b816d)\*  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów 32-bitowych z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fbf119cf-a8ed-4266-a673-442149992f7c)\*  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów 32-bitowych z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d089d9cb-382c-4e64-94c5-69b9864010b1)\*\*  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów 32-bitowych z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2fe2f398-433f-4338-a273-813185b43ea8)\*  
(KB2585542)  
(Ważny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem x64
</td>
<td style="border:1px solid black;">
[Biblioteka multimediów systemu Windows](http://www.microsoft.com/downloads/details.aspx?familyid=9eff12b2-70a4-452b-b6bc-0d83f2edcf6c)\*  
(KB2598479)  
(Krytyczny)  
[DirectShow](http://www.microsoft.com/downloads/details.aspx?familyid=7ff10d7f-26a6-403a-a4b7-7aff55e2fa16)\*\*  
(KB2631813)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem x64 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=726ff17e-ac90-4832-91e7-46f71ad2f868)\*  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem x64 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e8e68f89-27f4-4142-94ca-58f086a98157)\*  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=1ac8a368-4298-4c1d-9cfd-924d6df563af)\*\*  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem x64 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f54ac30d-8e41-4df9-bd43-db6742a24d4c)\*  
(KB2585542)  
(Ważny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem Itanium
</td>
<td style="border:1px solid black;">
[Biblioteka multimediów systemu Windows](http://www.microsoft.com/downloads/details.aspx?familyid=4e2edb23-7f4e-4fe4-848c-1d744e0dce9f)  
(KB2598479)  
(Krytyczny)  
[DirectShow](http://www.microsoft.com/downloads/details.aspx?familyid=5e0394c9-3de4-46f6-ae7f-18d5a555532e)  
(KB2631813)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=ba2c3d57-1bdd-44f2-9233-86c7ea6f0ddb)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=fc6491e8-6c3e-43a1-bc56-16c9a2fd2749)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=3e08b242-2516-4cf6-b38e-35ec2b8b788d)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=3979db3b-4961-4df8-84a4-1f26672b127c)  
(KB2585542)  
(Ważny)
</td>
</tr>
<tr>
<th colspan="7">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS12-004**](http://go.microsoft.com/fwlink/?linkid=227487)
</td>
<td style="border:1px solid black;">
[**MS12-001**](http://go.microsoft.com/fwlink/?linkid=235999)
</td>
<td style="border:1px solid black;">
[**MS12-002**](http://go.microsoft.com/fwlink/?linkid=229637)
</td>
<td style="border:1px solid black;">
[**MS12-003**](http://go.microsoft.com/fwlink/?linkid=235400)
</td>
<td style="border:1px solid black;">
[**MS12-005**](http://go.microsoft.com/fwlink/?linkid=230777)
</td>
<td style="border:1px solid black;">
[**MS12-006**](http://go.microsoft.com/fwlink/?linkid=232510)
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
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Brak
</td>
<td style="border:1px solid black;">
Brak
</td>
<td style="border:1px solid black;">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 dla systemów 32-bitowych i Windows 7 z dodatkiem Service Pack 1 dla systemów 32-bitowych
</td>
<td style="border:1px solid black;">
[DirectShow](http://www.microsoft.com/downloads/details.aspx?familyid=d736daf8-db6d-485f-b0cb-7f2d8c86f9a2)  
(KB2631813)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows 7 dla systemów 32-bitowych i Windows 7 z dodatkiem Service Pack 1 dla systemów 32-bitowych](http://www.microsoft.com/downloads/details.aspx?familyid=0ee22036-b7f4-40f5-8f40-a77e8faf48b2)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows 7 dla systemów 32-bitowych i Windows 7 z dodatkiem Service Pack 1 dla systemów 32-bitowych](http://www.microsoft.com/downloads/details.aspx?familyid=7422605b-7a02-4161-b7f8-92b3ccffef64)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows 7 dla systemów 32-bitowych i Windows 7 z dodatkiem Service Pack 1 dla systemów 32-bitowych](http://www.microsoft.com/downloads/details.aspx?familyid=0f433f2c-c61d-461d-af9c-0145af4b72ab)  
(KB2585542)  
(Ważny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 dla systemów opartych na procesorach x64 i Windows 7 z dodatkiem Service Pack 1 dla systemów opartych na procesorach x64
</td>
<td style="border:1px solid black;">
[DirectShow](http://www.microsoft.com/downloads/details.aspx?familyid=21b37775-3e7b-462d-8234-7c47d52daef9)  
(KB2631813)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows 7 dla systemów opartych na procesorach x64 i Windows 7 z dodatkiem Service Pack 1 dla systemów opartych na procesorach x64](http://www.microsoft.com/downloads/details.aspx?familyid=7444e20c-9821-4c91-9779-2728c537dd6a)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows 7 dla systemów opartych na procesorach x64 i Windows 7 z dodatkiem Service Pack 1 dla systemów opartych na procesorach x64](http://www.microsoft.com/downloads/details.aspx?familyid=4ba46bc7-af7a-445a-84f2-b0c13674409b)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows 7 dla systemów opartych na procesorach x64 i Windows 7 z dodatkiem Service Pack 1 dla systemów opartych na procesorach x64](http://www.microsoft.com/downloads/details.aspx?familyid=0839fec0-b6a7-4e47-9da3-2caef44a7df4)  
(KB2585542)  
(Ważny)
</td>
</tr>
<tr>
<th colspan="7">
System Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS12-004**](http://go.microsoft.com/fwlink/?linkid=227487)
</td>
<td style="border:1px solid black;">
[**MS12-001**](http://go.microsoft.com/fwlink/?linkid=235999)
</td>
<td style="border:1px solid black;">
[**MS12-002**](http://go.microsoft.com/fwlink/?linkid=229637)
</td>
<td style="border:1px solid black;">
[**MS12-003**](http://go.microsoft.com/fwlink/?linkid=235400)
</td>
<td style="border:1px solid black;">
[**MS12-005**](http://go.microsoft.com/fwlink/?linkid=230777)
</td>
<td style="border:1px solid black;">
[**MS12-006**](http://go.microsoft.com/fwlink/?linkid=232510)
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
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Brak
</td>
<td style="border:1px solid black;">
Brak
</td>
<td style="border:1px solid black;">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 dla systemów opartych na procesorach x64 i Windows Server 2008 R2 z dodatkiem Service Pack 1 dla systemów opartych na procesorach x64
</td>
<td style="border:1px solid black;">
[DirectShow](http://www.microsoft.com/downloads/details.aspx?familyid=355c980d-ec2e-4b2d-a7d4-2e3dbd3a0dde)\*\*  
(KB2631813)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach x64 i Windows Server 2008 R2 z dodatkiem Service Pack 1 dla systemów opartych na procesorach x64](http://www.microsoft.com/downloads/details.aspx?familyid=4c73a16d-e9fa-48de-9dca-a6360ce3d029)\*  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach x64 i Windows Server 2008 R2 z dodatkiem Service Pack 1 dla systemów opartych na procesorach x64](http://www.microsoft.com/downloads/details.aspx?familyid=db3a4814-a409-4def-944d-4eaa540b83b0)\*\*  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach x64 i Windows Server 2008 R2 z dodatkiem Service Pack 1 dla systemów opartych na procesorach x64](http://www.microsoft.com/downloads/details.aspx?familyid=34542a5a-88df-4a07-b1ed-d4c845502cd8)\*  
(KB2585542)  
(Ważny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 dla systemów opartych na procesorach Itanium i Windows Server 2008 R2 z dodatkiem Service Pack 1 dla systemów opartych na procesorach Itanium
</td>
<td style="border:1px solid black;">
[DirectShow](http://www.microsoft.com/downloads/details.aspx?familyid=d4b2389e-fd9f-47c7-9afd-4077f5632c21)  
(KB2631813)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach Itanium i Windows Server 2008 R2 z dodatkiem Service Pack 1 dla systemów opartych na procesorach Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=1cc14ee8-f035-4bfc-bf38-33c6b9a2e776)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach Itanium i Windows Server 2008 R2 z dodatkiem Service Pack 1 dla systemów opartych na procesorach Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=2101663a-ed3d-4850-b79a-16960ab56b45)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach Itanium i Windows Server 2008 R2 z dodatkiem Service Pack 1 dla systemów opartych na procesorach Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=fe661936-06e1-45d3-89f6-1093504496a7)  
(KB2585542)  
(Ważny)
</td>
</tr>
</table>
 
**Uwagi dotyczące systemu Windows Server 2008 i Windows Server 2008 R2**

**\*Luka w zabezpieczeniach dotyczy instalacji Server Core.** Ta aktualizacja ma zastosowanie, z takim samym wskaźnikiem ważności, w przypadku obsługiwanych wersji systemu Windows Server 2008 lub Windows Server 2008 R2, niezależnie od tego, czy zostały zainstalowane przy użyciu opcji instalacji Server Core. Więcej informacji na temat tej opcji instalacji można znaleźć w artykułach TechNet, [Managing a Server Core Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) i [Servicing a Server Core Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) (jęz. ang.). Należy pamiętać, że opcja instalacji Server Core nie dotyczy niektórych wersji systemu Windows Server 2008 i Windows Server 2008 R2. Zobacz [Porównanie opcji instalacji Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Luka w zabezpieczeniach nie dotyczy instalacji Server Core.** Luki usuwane przez tę aktualizację zabezpieczeń nie dotyczą obsługiwanych wersji systemu Windows Server 2008 ani Windows Server 2008 R2, jeżeli systemy te zostały zainstalowane przy użyciu opcji instalacji Server Core. Więcej informacji na temat tej opcji instalacji można znaleźć w artykułach TechNet, [Managing a Server Core Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) i [Servicing a Server Core Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) (jęz. ang.). Należy pamiętać, że opcja instalacji Server Core nie dotyczy niektórych wersji systemu Windows Server 2008 i Windows Server 2008 R2. Zobacz [Porównanie opcji instalacji Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**Uwaga dotycząca biuletynu MS12-004**

<sup>[1]</sup>Pakiet Windows Media Center TV Pack dla systemu Windows Vista jest dostępny tylko jako składnik opcjonalny w instalacjach OEM systemu Windows Vista w wersjach Home Premium i Ultimate. Klienci, którzy zainstalowali ten opcjonalny składnik, powinni zainstalować wszystkie aktualizacje dostępne dla posiadanej wersji systemu Windows Vista. Zgodnie z najlepszymi rozwiązaniami firma Microsoft zaleca zainstalowanie odpowiednich aktualizacji systemu operacyjnego (KB2598479 i KB2631813) przed instalacją aktualizacji pakietu Windows Media Center TV Pack (KB2628642).

#### Narzędzia i oprogramowanie firmy Microsoft dla deweloperów

 
<table style="border:1px solid black;">
<tr>
<th colspan="2">
Biblioteka AntiXSS firmy Microsoft
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS12-007**](http://go.microsoft.com/fwlink/?linkid=227561)
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
Biblioteka AntiXSS w wersjach 3.x i 4.0 firmy MIcrosoft
</td>
<td style="border:1px solid black;">
[Biblioteka AntiXSS w wersjach 3.x i 4.0 firmy MIcrosoft](http://www.microsoft.com/downloads/details.aspx?familyid=b3ef05ce-70fe-4f25-9aee-cb7a42a53d11)<sup>[1]</sup><sup>[2]</sup>
</td>
</tr>
</table>
 
**Uwaga dotycząca biuletynu MS12-007**

<sup>[1]</sup>Ten plik do pobrania uaktualnia bibliotekę AntiXSS (Anti-Cross Site Scripting) firmy Microsoft do nowszej wersji, która nie jest zagrożona przez omawianą lukę.

<sup>[2]</sup>To uaktualnienie jest dostępne tylko w witrynie Centrum pobierania Microsoft.

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

W Zestawie narzędzi do sprawdzania zgodności aplikacji znajdują się niezbędne narzędzia i dokumentacja, które umożliwiają ocenę zgodności aplikacji przed wdrożeniem systemu Microsoft Windows Vista, aktualizacji dla systemu Windows, aktualizacji zabezpieczeń firmy Microsoft lub nowej wersji programu Windows Internet Explorer w środowisku użytkownika, oraz ograniczenie problemów ze zgodnością aplikacji.

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

-   Joshua J. Drake z firmy [Accuvant LABS](http://www.accuvant.com/), za zgłoszenie problemu opisanego w biuletynie MS12-001
-   Parvez Anwar, we współpracy z firmą [Secunia Research](http://secunia.com/), za zgłoszenie problemu opisanego w biuletynie MS12-002
-   Kang Wu z firmy [Shenzhen Jowto Research Dep](http://www.jowto.com), za zgłoszenie problemu opisanego w biuletynie MS12-003
-   Shane Garrett z [IBM Security System's X-Force Research](http://xforce.iss.net/), za zgłoszenie problemu opisanego w biuletynie MS12-004
-   Neel Mehta z firmy [Google Inc.](http://www.google.com/), za zgłoszenie problemu opisanego w biuletynie MS12-004
-   Yorick Koster, współpracownik programu [SecuriTeam Secure Disclosure firmy Beyond Security](http://www.beyondsecurity.com/ssd.html), za zgłoszenie problemu opisanego w biuletynie MS12-005
-   Adi Cohen z firmy [IBM Rational Application Security](http://blog.watchfire.com/), za zgłoszenie problemu opisanego w biuletynie MS12-007

#### Pomoc techniczna

-   Wymienione oprogramowanie zostało przetestowane w celu ustalenia, których wersji dotyczy problem. Dla pozostałych wersji upłynął okres pomocy technicznej. Aby zapoznać się z zasadami cyklu pomocy technicznej dotyczącymi używanej wersji oprogramowania, odwiedź [witrynę zasad cyklu pomocy technicznej firmy Microsoft](http://go.microsoft.com/fwlink/?linkid=21742).
-   Klienci mogą uzyskać pomoc techniczną w [Biurze Obsługi Klienta Microsoft](http://go.microsoft.com/fwlink/?linkid=21131) pod numerem 0 801 802 000 (opłata według stawek Twojego operatora) lub (0-22) 594 19 99 w godzinach od 9:00 do 17:00, od poniedziałku do piątku. Połączenia z działem pomocy technicznej związane z aktualizacjami zabezpieczeń są bezpłatne. Dodatkowe informacje dotyczące możliwości skorzystania z pomocy technicznej można znaleźć w witrynie [Pomoc i obsługa techniczna firmy Microsoft](http://support.microsoft.com/).
-   Klienci międzynarodowi mogą uzyskać pomoc w lokalnych przedstawicielstwach firmy Microsoft. Pomoc techniczna związana z aktualizacjami zabezpieczeń jest bezpłatna. Informacje o sposobie kontaktowania się z pomocą techniczną firmy Microsoft są dostępne w [międzynarodowej witrynie sieci Web pomocy i obsługi technicznej](http://go.microsoft.com/fwlink/?linkid=21155).

#### Zrzeczenie odpowiedzialności

Informacje w bazie wiedzy Microsoft Knowledge Base są dostarczane „tak jak są” bez jakiejkolwiek gwarancji. Firma Microsoft odrzuca wszelkie gwarancje, wyraźne i dorozumiane, w tym gwarancje dotyczące wartości handlowej i przydatności do określonego celu. Firma Microsoft Corporation ani jej dostawcy w żadnym wypadku nie ponoszą odpowiedzialności za jakiekolwiek szkody, w tym bezpośrednie, pośrednie, przypadkowe, wynikowe, utratę zysków handlowych lub szkody specjalne, nawet jeżeli firmę Microsoft Corporation lub jej dostawców powiadomiono o możliwości zaistnienia takich szkód. W niektórych stanach wyłączenie lub ograniczenie odpowiedzialności za straty wynikowe lub przypadkowe, a więc i powyższe ograniczenia, nie mają zastosowania.

#### Wersje

-   Wersja 1.0 (10 stycznia 2012 r.): Opublikowane podsumowanie biuletynów zabezpieczeń.
-   Wersja 2.0 (11 stycznia 2012 r.): W biuletynie MS12-003, w sekcji **Wskaźnik możliwości wykorzystania luki** dotyczącej luki CVE-2012-0005, skorygowano ocenę możliwości wykorzystania luki w odniesieniu do najnowszej wersji oprogramowania. W biuletynie MS12-007 wprowadzono poprawki związane z ogłoszeniem ponownej publikacji biuletynu. Aby uzyskać więcej informacji, zapoznaj się z biuletynem MS12-007.
-   Wersja 2.1 (27 stycznia 2012 r.): W biuletynie MS12-004 poprawiono zbiorczy wskaźnik ważności dla pakietu aktualizacji KB2631813 dla wszystkich obsługiwanych wersji systemu Windows XP, Windows Server 2003, Windows Vista i Windows Server 2008. Szczegółowe informacje można znaleźć w biuletynie MS12-004.

*Built at 2014-04-18T01:50:00Z-07:00*
