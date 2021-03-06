---
TOCTitle: 'MS12-APR'
Title: 'Podsumowanie biuletynów zabezpieczeń firmy Microsoft za kwiecień 2012 r.'
ms:assetid: 'ms12-apr'
ms:contentKeyID: 61233133
ms:mtpsurl: 'https://technet.microsoft.com/pl-PL/library/ms12-apr(v=Security.10)'
---

Podsumowanie biuletynów zabezpieczeń firmy Microsoft za kwiecień 2012 r.
========================================================================

Opublikowano: 10 kwietnia 2012 | Zaktualizowano: 26 kwietnia 2012

**Wersja:** 2.0

Niniejsze podsumowanie biuletynów zabezpieczeń zawiera spis biuletynów za kwiecień 2012 r.

Z chwilą opublikowania biuletynów zabezpieczeń za kwiecień 2012 r. niniejsze podsumowanie biuletynów zastąpi powiadomienie o biuletynach zabezpieczeń wydane 5 kwietnia 2012 r. Aby uzyskać więcej informacji na temat usługi powiadamiania o biuletynach, zobacz [Powiadomienia o biuletynach zabezpieczeń firmy Microsoft (j. ang.)](http://go.microsoft.com/fwlink/?linkid=217213).

Aby dowiedzieć się, jak otrzymywać automatyczne powiadomienia o publikacji biuletynów zabezpieczeń firmy Microsoft, odwiedź stronę [Microsoft Technical Security Notifications](http://go.microsoft.com/fwlink/?linkid=21163).

11 kwietnia 2012 r. o godz. 11:00 czasu Pacyfiku (godz. 20:00 czasu środkowoeuropejskiego) firma Microsoft udostępni emisję internetową, w której znajdą się odpowiedzi na pytania klientów dotyczące tych biuletynów (USA i Kanada). [Zarejestruj się, aby zobaczyć emisję internetową dotyczącą biuletynów zabezpieczeń za kwiecień](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032499650). Po tym dniu emisja internetowa będzie dostępna na żądanie. Aby uzyskać więcej informacji, zobacz [Podsumowania biuletynów zabezpieczeń i emisje internetowe firmy Microsoft](http://go.microsoft.com/fwlink/?linkid=217214).

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=242739">MS12-023</a></td>
<td style="border:1px solid black;"><strong>Zbiorcza aktualizacja zabezpieczeń dla programu Internet Explorer (2675157)</strong><br />
<br />
Niniejsza aktualizacja zabezpieczeń usuwa pięć luk w zabezpieczeniach programu Internet Explorer, które zostały zgłoszone przez użytkowników. Najpoważniejsze z tych luk umożliwiają zdalne wykonanie kodu, jeśli użytkownik wyświetli specjalnie spreparowaną stronę sieci Web przy użyciu programu Internet Explorer. Osoba atakująca, której uda się wykorzystać jedną z tych luk, może uzyskać takie same uprawnienia, jak bieżący użytkownik. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Krytyczny</a><br />
Zdalne wykonanie kodu</td>
<td style="border:1px solid black;">Wymaga ponownego uruchomienia komputera</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=238623">MS12-024</a></td>
<td style="border:1px solid black;"><strong>Luka w zabezpieczeniach systemu Windows umożliwia zdalne wykonanie kodu (2653956)</strong><br />
<br />
Ta aktualizacja zabezpieczeń usuwa lukę w zabezpieczeniach systemu Microsoft Windows. Luka w zabezpieczeniach może pozwolić na zdalne wykonanie kodu, jeśli użytkownik bądź aplikacja uruchomi lub zainstaluje specjalnie spreparowany, podpisany przenośny plik wykonywalny (PE) w zagrożonym systemie.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Krytyczny</a><br />
Zdalne wykonanie kodu</td>
<td style="border:1px solid black;">Wymaga ponownego uruchomienia komputera</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=242032">MS12-025</a></td>
<td style="border:1px solid black;"><strong>Luka w zabezpieczeniach systemu .NET Framework umożliwia zdalne</strong> <strong>wykonanie kodu (2671605)</strong><br />
<br />
Niniejsza aktualizacja zabezpieczeń usuwa jedną zgłoszoną przez użytkowników lukę w zabezpieczeniach systemu Microsoft .NET Framework. Luka w zabezpieczeniach umożliwia zdalne wykonanie kodu w systemie klienta, jeśli użytkownik wyświetli specjalnie spreparowaną stronę sieci Web w przeglądarce obsługującej aplikacje przeglądarki XAML (XBAP). Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi. Omawiana luka umożliwia także zdalne wykonanie kodu w systemach serwerowych z działającym programem IIS, jeśli dany serwer zezwala na przetwarzanie stron ASP.NET, a osobie atakującej uda się przekazać na ten serwer specjalnie spreparowaną stronę ASP.NET i uruchomić ją, tak jak mogłoby to wyglądać w scenariuszu z wykorzystaniem hostingu w sieci Web. Omawiana luka może też zostać wykorzystana przez aplikacje Windows .NET do obejścia ograniczeń zabezpieczeń dostępu kodu (CAS). Osoba atakująca za pośrednictwem sieci Web, która chce wykorzystać tę lukę, może udostępniać witrynę zawierającą odpowiednią stronę sieci Web. Dodatkowo, witryny sieci Web, które akceptują lub udostępniają zawartość wprowadzoną przez użytkownika lub reklamy, jak również witryny, do których się włamano, mogą zawierać specjalnie spreparowane treści mogące wykorzystać lukę w zabezpieczeniach. Jednakże w żadnym przypadku osoba atakująca nie może zmusić użytkowników do odwiedzenia takich witryn. Musi przekonać użytkowników do odwiedzenia takiej witryny, najczęściej zachęcając do kliknięcia łącza w wiadomości e-mail lub wiadomości błyskawicznej, które przekieruje ich do witryny osoby atakującej.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Krytyczny</a><br />
Zdalne wykonanie kodu</td>
<td style="border:1px solid black;">Może wymagać ponownego uruchomienia</td>
<td style="border:1px solid black;">Microsoft Windows, Microsoft .NET Framework</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=246275">MS12-027</a></td>
<td style="border:1px solid black;"><strong>Luka w zabezpieczeniach formantów standardowych systemu Windows umożliwia zdalne wykonanie kodu (2664258)</strong><br />
<br />
Ta aktualizacja zabezpieczeń ma na celu usunięcie luki w zabezpieczeniach formantów standardowych systemu Windows, która została zgłoszona przez użytkowników. Luka ta może pozwolić na zdalne wykonanie kodu, jeśli użytkownik odwiedzi witrynę sieci Web zawierającą specjalnie spreparowaną zawartość, która została stworzona z myślą o wykorzystaniu omawianej luki. Jednakże w żadnym przypadku osoba atakująca nie może zmusić użytkowników do odwiedzenia takiej witryny. Musi przekonać użytkowników do odwiedzenia takiej witryny, najczęściej zachęcając do kliknięcia łącza w wiadomości e-mail lub wiadomości błyskawicznej, które przekieruje ich do witryny osoby atakującej. Złośliwy plik może zostać również wysłany w załączniku wiadomości e-mail, ale w celu wykorzystania luki osoba atakująca musi nakłonić użytkownika do otwarcia takiego załącznika.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Krytyczny</a><br />
Zdalne wykonanie kodu</td>
<td style="border:1px solid black;">Może wymagać ponownego uruchomienia</td>
<td style="border:1px solid black;">Microsoft Office,<br />
Microsoft SQL Server,<br />
Oprogramowanie serwerów firmy Microsoft,<br />
Narzędzia firmy Microsoft dla deweloperów</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=238519">MS12-026</a></td>
<td style="border:1px solid black;"><strong>Luki w zabezpieczeniach programu Forefront Unified Access Gateway (UAG) umożliwiają ujawnienie informacji (2663860)</strong><br />
<br />
Ta aktualizacja zabezpieczeń usuwa dwie luki w zabezpieczeniach programu Microsoft Forefront Unified Access Gateway (UAG), które zostały zgłoszone przez użytkowników. Bardziej poważna z tych luk może pozwolić na ujawnienie informacji, jeśli osoba atakująca wyśle do serwera UAG specjalnie spreparowaną kwerendę.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Ważny</a><br />
Ujawnienie informacji</td>
<td style="border:1px solid black;">Może wymagać ponownego uruchomienia</td>
<td style="border:1px solid black;">Microsoft Forefront United Access Gateway</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=232498">MS12-028</a></td>
<td style="border:1px solid black;"><strong>Luka w zabezpieczeniach pakietu Microsoft Office umożliwia zdalne wykonanie kodu (2639185)</strong><br />
<br />
Ta aktualizacja zabezpieczeń usuwa lukę w zabezpieczeniach pakietu Microsoft Office i programu Microsoft Works, która została zgłoszona przez użytkowników. Luka ta może pozwolić na zdalne wykonanie kodu, jeśli użytkownik otworzy specjalnie spreparowany plik pakietu Works. Osoba atakująca, której uda się wykorzystać tę lukę, może uzyskać takie same uprawnienia, jak bieżący użytkownik. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi.</td>
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
  
| Identyfikator biuletynu                                   | Nazwa luki w zabezpieczeniach                                                                  | CVE ID                                                                           | Ocena możliwości wykorzystania luki w najnowszej wersji programu                                            | Ocena możliwości wykorzystania luki w poprzedniej wersji programu                                      | Ocena możliwości wykorzystania luki w celu wytworzenia sytuacji typu „odmowa usługi” | Najważniejsze uwagi                                                                                                                       |  
|-----------------------------------------------------------|------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------|  
| [MS12-023](http://go.microsoft.com/fwlink/?linkid=242739) | Luka w zabezpieczeniach biblioteki JScript9 umożliwiająca zdalne wykonanie kodu                | [CVE-2012-0169](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0169) | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) — kod wykorzystujący lukę mało prawdopodobny | Brak zagrożenia                                                                                        | Tymczasowy                                                                           | (Brak)                                                                                                                                    |  
| [MS12-023](http://go.microsoft.com/fwlink/?linkid=242739) | Luka w zabezpieczeniach funkcji OnReadyStateChange umożliwiająca zdalne wykonanie kodu         | [CVE-2012-0170](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0170) | Brak zagrożenia                                                                                             | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny kod wykorzystujący lukę | Tymczasowy                                                                           | (Brak)                                                                                                                                    |  
| [MS12-023](http://go.microsoft.com/fwlink/?linkid=242739) | Luka w zabezpieczeniach funkcji SelectAll umożliwiająca zdalne wykonanie kodu                  | [CVE-2012-0171](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0171) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny kod wykorzystujący lukę      | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny kod wykorzystujący lukę | Tymczasowy                                                                           | (Brak)                                                                                                                                    |  
| [MS12-023](http://go.microsoft.com/fwlink/?linkid=242739) | Luka w zabezpieczeniach stylów VML umożliwiająca zdalne wykonanie kodu                         | [CVE-2012-0172](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0172) | Brak zagrożenia                                                                                             | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny kod wykorzystujący lukę | Tymczasowy                                                                           | (Brak)                                                                                                                                    |  
| [MS12-024](http://go.microsoft.com/fwlink/?linkid=238623) | Luka w zabezpieczeniach procedury sprawdzania poprawności podpisu funkcji WinVerifyTrust       | [CVE-2012-0151](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0151) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny kod wykorzystujący lukę      | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny kod wykorzystujący lukę | Nie dotyczy                                                                          | (Brak)                                                                                                                                    |  
| [MS12-025](http://go.microsoft.com/fwlink/?linkid=242032) | Luka w zabezpieczeniach systemu .NET Framework związana ze sprawdzaniem poprawności parametrów | [CVE-2012-0163](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0163) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny kod wykorzystujący lukę      | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny kod wykorzystujący lukę | Nie dotyczy                                                                          | (Brak)                                                                                                                                    |  
| [MS12-026](http://go.microsoft.com/fwlink/?linkid=238519) | Luka w zabezpieczeniach związana z niefiltrowanym dostępem do domyślnej witryny programu UAG   | [CVE-2012-0147](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0147) | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) — kod wykorzystujący lukę mało prawdopodobny | Brak zagrożenia                                                                                        | Nie dotyczy                                                                          | Ta luka może doprowadzić do ujawnienia informacji.                                                                                        |  
| [MS12-027](http://go.microsoft.com/fwlink/?linkid=246275) | Luka w zabezpieczeniach pliku MSCOMCTL.OCX umożliwiająca zdalne wykonanie kodu                 | [CVE-2012-0158](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0158) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny kod wykorzystujący lukę      | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny kod wykorzystujący lukę | Nie dotyczy                                                                          | Firma Microsoft zna niewielką liczbę przypadków prób ataków wykorzystujących tę lukę.                                                     |  
| [MS12-028](http://go.microsoft.com/fwlink/?linkid=232498) | Luka w zabezpieczeniach konwertera plików WPS pakietu Office związana z przepełnieniem stosu   | [CVE-2012-0177](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0177) | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) — kod wykorzystujący lukę mało prawdopodobny | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny kod wykorzystujący lukę | Nie dotyczy                                                                          | Pakiet Microsoft Office 2007 z dodatkiem Service Pack 3 oraz wszystkie obsługiwane wersje pakietu Microsoft Office 2010 nie są zagrożone. |
  
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
<th colspan="4">
Windows XP  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS12-023**](http://go.microsoft.com/fwlink/?linkid=242739)
</td>
<td style="border:1px solid black;">
[**MS12-024**](http://go.microsoft.com/fwlink/?linkid=238623)
</td>
<td style="border:1px solid black;">
[**MS12-025**](http://go.microsoft.com/fwlink/?linkid=242032)
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP z dodatkiem Service Pack 3
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=2a490c62-16c4-402a-b2d9-3e8cfb5bcebd)  
(KB2675157)  
(Krytyczny)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=81b28dd9-87aa-46cc-94c6-2da39d0298db)  
(KB2675157)  
(Krytyczny)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=74ce0e29-046b-4ac3-89a1-b292a177972f)  
(KB2675157)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows XP z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=575afd20-cee4-4fa9-b781-9f8dfdd41ebe)  
(KB2653956)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.0 z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=1cfeae57-d4e9-4fff-8956-523e7b71453c)  
(KB2656378)  
(tylko Media Center Edition 2005 i Tablet PC Edition 2005)  
(Krytyczny)  
[Microsoft .NET Framework 1.1 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c376fbdc-2289-47b6-950b-4e668cd3a390)  
(KB2656370)  
(Krytyczny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c1338821-d8b2-4513-aa35-087323188509)  
(KB2656369)  
(Krytyczny)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Krytyczny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=a1b7be43-a32e-456b-8df0-c26cdf187682)  
(KB2675157)  
(Krytyczny)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=29ec7b06-c7aa-4149-bb2c-25af7d38a6a9)  
(KB2675157)  
(Krytyczny)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=646c6352-4d99-413a-a75b-71289b5d2b25)  
(KB2675157)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=adc31695-1be6-4976-869c-007df8ac8508)  
(KB2653956)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c376fbdc-2289-47b6-950b-4e668cd3a390)  
(KB2656370)  
(Krytyczny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c1338821-d8b2-4513-aa35-087323188509)  
(KB2656369)  
(Krytyczny)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Krytyczny)
</td>
</tr>
<tr>
<th colspan="4">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS12-023**](http://go.microsoft.com/fwlink/?linkid=242739)
</td>
<td style="border:1px solid black;">
[**MS12-024**](http://go.microsoft.com/fwlink/?linkid=238623)
</td>
<td style="border:1px solid black;">
[**MS12-025**](http://go.microsoft.com/fwlink/?linkid=242032)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Zbiorczy** **wskaźnik ważności**
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=020e0d68-dd1c-4297-b565-fcc6dcf5f280)  
(KB2675157)  
(Umiarkowany)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=17b0c139-2709-424d-9d17-827af468e858)  
(KB2675157)  
(Umiarkowany)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=3289a80a-d1b1-4494-bede-03d0be579acf)  
(KB2675157)  
(Umiarkowany)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f79c8940-ca31-4ff7-924e-847f5eef7864)  
(KB2653956)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ffd26218-e149-44ea-a0b9-f2a1315fce9e)  
(KB2656376)  
(Krytyczny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c1338821-d8b2-4513-aa35-087323188509)  
(KB2656369)  
(Krytyczny)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Krytyczny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=295292d3-01a3-4574-b994-8cdbcf5a0d2e)  
(KB2675157)  
(Umiarkowany)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=04656a93-e958-4764-afe8-27c476855506)  
(KB2675157)  
(Umiarkowany)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=dff4fb63-b319-49ed-8a9d-6b15e43d5bfd)  
(KB2675157)  
(Umiarkowany)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=03ebf111-1e7b-4dc2-b84f-a26c6b5f0d58)  
(KB2653956)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c376fbdc-2289-47b6-950b-4e668cd3a390)  
(KB2656370)  
(Krytyczny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c1338821-d8b2-4513-aa35-087323188509)  
(KB2656369)  
(Krytyczny)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Krytyczny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=09011393-c7d5-4225-9b8e-5a234d4dbcd1)  
(KB2675157)  
(Umiarkowany)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=a5ef0147-595e-43b5-819f-73780fcef10d)  
(KB2675157)  
(Umiarkowany)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=734ff97a-7d72-4bfe-9557-7fac91902f8e)  
(KB2653956)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c376fbdc-2289-47b6-950b-4e668cd3a390)  
(KB2656370)  
(Krytyczny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c1338821-d8b2-4513-aa35-087323188509)  
(KB2656369)  
(Krytyczny)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Krytyczny)
</td>
</tr>
<tr>
<th colspan="4">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS12-023**](http://go.microsoft.com/fwlink/?linkid=242739)
</td>
<td style="border:1px solid black;">
[**MS12-024**](http://go.microsoft.com/fwlink/?linkid=238623)
</td>
<td style="border:1px solid black;">
[**MS12-025**](http://go.microsoft.com/fwlink/?linkid=242032)
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=f598cad1-4d1a-40ce-a016-bb58778d5dc0)  
(KB2675157)  
(Krytyczny)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=44284277-06a7-405d-9187-8f50a042604d)  
(KB2675157)  
(Krytyczny)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=51088164-13b7-4216-90f1-20c92c8b8ca9)  
(KB2675157)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Vista z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c7683919-6d46-4b3e-aa98-1bef20141835)  
(KB2653956)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c376fbdc-2289-47b6-950b-4e668cd3a390)  
(KB2656370)  
(Krytyczny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8e1c10a1-9cb2-4815-8aa6-e401ced5df80)  
(KB2656374)  
(Krytyczny)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Krytyczny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=2717a997-2066-4a83-ae9b-4611a0851101)  
(KB2675157)  
(Krytyczny)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=19684033-ddeb-464f-9a22-f580a9c19f8e)  
(KB2675157)  
(Krytyczny)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=bbb99aee-aadd-4ec7-9e27-91cb8d90803e)  
(KB2675157)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4d9f8a6e-17bd-4ed3-8bc7-d5e3b11ca12a)  
(KB2653956)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c376fbdc-2289-47b6-950b-4e668cd3a390)  
(KB2656370)  
(Krytyczny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8e1c10a1-9cb2-4815-8aa6-e401ced5df80)  
(KB2656374)  
(Krytyczny)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Krytyczny)
</td>
</tr>
<tr>
<th colspan="4">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS12-023**](http://go.microsoft.com/fwlink/?linkid=242739)
</td>
<td style="border:1px solid black;">
[**MS12-024**](http://go.microsoft.com/fwlink/?linkid=238623)
</td>
<td style="border:1px solid black;">
[**MS12-025**](http://go.microsoft.com/fwlink/?linkid=242032)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Zbiorczy wskaźnik ważności**
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 z dodatkiem Service Pack 2 dla systemów 32-bitowych
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=3e361edd-234b-4053-aa49-278b9fde4d5c)\*\*  
(KB2675157)  
(Umiarkowany)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=6eb6781e-7b38-4679-afbc-4e3bb5747fd8)\*\*  
(KB2675157)  
(Umiarkowany)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=d34d7981-ed63-460d-95e4-e6da1ac41d2f)\*\*  
(KB2675157)  
(Umiarkowany)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów 32-bitowych z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c36c20f7-a742-4151-b8f2-85ef80479d06)\*  
(KB2653956)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c376fbdc-2289-47b6-950b-4e668cd3a390)  
(KB2656370)  
(Krytyczny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8e1c10a1-9cb2-4815-8aa6-e401ced5df80)  
(KB2656374)  
(Krytyczny)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Krytyczny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem x64
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=60b76a3c-4530-4101-931f-45df621e1eed)\*\*  
(KB2675157)  
(Umiarkowany)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=fd657467-a45c-4354-b947-3a3cceb9b690)\*\*  
(KB2675157)  
(Umiarkowany)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=c9d773e9-6a2e-45db-8f30-7da0082d909c)\*\*  
(KB2675157)  
(Umiarkowany)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem x64 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=330cea47-221d-439e-b106-58a146fc28ee)\*  
(KB2653956)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c376fbdc-2289-47b6-950b-4e668cd3a390)  
(KB2656370)  
(Krytyczny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8e1c10a1-9cb2-4815-8aa6-e401ced5df80)  
(KB2656374)  
(Krytyczny)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Krytyczny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem Itanium
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=3235216f-497f-4934-81b8-1eb9929e98c9)  
(KB2675157)  
(Umiarkowany)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=1ec74522-ec1e-4b3c-bfeb-6a505cc4f11a)  
(KB2653956)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c376fbdc-2289-47b6-950b-4e668cd3a390)  
(KB2656370)  
(Krytyczny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8e1c10a1-9cb2-4815-8aa6-e401ced5df80)  
(KB2656374)  
(Krytyczny)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Krytyczny)
</td>
</tr>
<tr>
<th colspan="4">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS12-023**](http://go.microsoft.com/fwlink/?linkid=242739)
</td>
<td style="border:1px solid black;">
[**MS12-024**](http://go.microsoft.com/fwlink/?linkid=238623)
</td>
<td style="border:1px solid black;">
[**MS12-025**](http://go.microsoft.com/fwlink/?linkid=242032)
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 dla systemów 32-bitowych
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=9a58ca0b-fad7-418e-80ae-ca478168f887)  
(KB2675157)  
(Krytyczny)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=e6724be3-ff4b-4dea-95f3-0b13998b6758)  
(KB2675157)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows 7 dla systemów 32-bitowych](http://www.microsoft.com/downloads/details.aspx?familyid=ac183b66-0247-4ae5-bda0-e8d0070917c8)  
(KB2653956)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=c3f521a9-4dc8-46b7-a7f2-696b8759b398)  
(KB2656372)  
(Krytyczny)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Krytyczny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 z dodatkiem Service Pack 1 dla systemów 32-bitowych
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=9a58ca0b-fad7-418e-80ae-ca478168f887)  
(KB2675157)  
(Krytyczny)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=e6724be3-ff4b-4dea-95f3-0b13998b6758)  
(KB2675157)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows 7 z dodatkiem Service Pack 1 dla systemów 32-bitowych](http://www.microsoft.com/downloads/details.aspx?familyid=ac183b66-0247-4ae5-bda0-e8d0070917c8)  
(KB2653956)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=efccca8d-1371-4cda-96ab-ceef735742e2)  
(KB2656373)  
(Krytyczny)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Krytyczny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 dla systemów z procesorem x64
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=7215f707-c536-4d81-ad66-e7bff592e400)  
(KB2675157)  
(Krytyczny)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=0ff822d0-074a-409c-9174-8100618c6171)  
(KB2675157)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows 7 dla systemów z procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=27226e64-266f-499e-8c57-866593fc3430)  
(KB2653956)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=c3f521a9-4dc8-46b7-a7f2-696b8759b398)  
(KB2656372)  
(Krytyczny)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Krytyczny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 z dodatkiem Service Pack 1 dla systemów opartych na procesorach x64
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=7215f707-c536-4d81-ad66-e7bff592e400)  
(KB2675157)  
(Krytyczny)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=0ff822d0-074a-409c-9174-8100618c6171)  
(KB2675157)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows 7 z dodatkiem Service Pack 1 dla systemów opartych na procesorach x64](http://www.microsoft.com/downloads/details.aspx?familyid=27226e64-266f-499e-8c57-866593fc3430)  
(KB2653956)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=efccca8d-1371-4cda-96ab-ceef735742e2)  
(KB2656373)  
(Krytyczny)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Krytyczny)
</td>
</tr>
<tr>
<th colspan="4">
System Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS12-023**](http://go.microsoft.com/fwlink/?linkid=242739)
</td>
<td style="border:1px solid black;">
[**MS12-024**](http://go.microsoft.com/fwlink/?linkid=238623)
</td>
<td style="border:1px solid black;">
[**MS12-025**](http://go.microsoft.com/fwlink/?linkid=242032)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Zbiorczy wskaźnik ważności**
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 dla systemów opartych na procesorach x64
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=237d94e6-b9b9-4177-81fa-a67df2806b0e)\*\*  
(KB2675157)  
(Umiarkowany)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=d002bfe4-10e9-46d3-a460-06d112201ca5)\*\*  
(KB2675157)  
(Umiarkowany)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach x64](http://www.microsoft.com/downloads/details.aspx?familyid=54db1495-31bb-4435-a442-74e484630b8a)\*  
(KB2653956)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=c3f521a9-4dc8-46b7-a7f2-696b8759b398)\*  
(KB2656372)  
(Krytyczny)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Krytyczny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 z dodatkiem Service Pack 1 dla systemów opartych na procesorach x64
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=237d94e6-b9b9-4177-81fa-a67df2806b0e)\*\*  
(KB2675157)  
(Umiarkowany)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=d002bfe4-10e9-46d3-a460-06d112201ca5)\*\*  
(KB2675157)  
(Umiarkowany)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach x64 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=54db1495-31bb-4435-a442-74e484630b8a)\*  
(KB2653956)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=efccca8d-1371-4cda-96ab-ceef735742e2)\*  
(KB2656373)  
(Krytyczny)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)\*<sup>[1]</sup>
(KB2656368)  
(Krytyczny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 dla systemów opartych na procesorach Itanium
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=7bdba902-0a6e-451e-a29b-6d0a03ff5664)  
(KB2675157)  
(Umiarkowany)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=9a4115bf-028b-4dcc-8995-d3341fdf42f2)  
(KB2653956)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=c3f521a9-4dc8-46b7-a7f2-696b8759b398)  
(KB2656372)  
(Krytyczny)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Krytyczny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 z dodatkiem Service Pack 1 dla systemów opartych na procesorach Itanium
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=7bdba902-0a6e-451e-a29b-6d0a03ff5664)  
(KB2675157)  
(Umiarkowany)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 z dodatkiem Service Pack 1 dla systemów opartych na procesorach Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=9a4115bf-028b-4dcc-8995-d3341fdf42f2)  
(KB2653956)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=efccca8d-1371-4cda-96ab-ceef735742e2)  
(KB2656373)  
(Krytyczny)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Krytyczny)
</td>
</tr>
</table>
 
**Uwagi dotyczące systemu Windows Server 2008 i Windows Server 2008 R2**

**\*Luka w zabezpieczeniach dotyczy instalacji Server Core.** Ta aktualizacja ma zastosowanie, z takim samym wskaźnikiem ważności, w przypadku obsługiwanych wersji systemu Windows Server 2008 lub Windows Server 2008 R2, niezależnie od tego, czy zostały zainstalowane przy użyciu opcji instalacji Server Core. Więcej informacji na temat tej opcji instalacji można znaleźć w artykułach TechNet, [Managing a Server Core Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) i [Servicing a Server Core Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) (jęz. ang.). Należy pamiętać, że opcja instalacji Server Core nie dotyczy niektórych wersji systemu Windows Server 2008 i Windows Server 2008 R2. Zobacz [Porównanie opcji instalacji Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Luka w zabezpieczeniach nie dotyczy instalacji Server Core.** Luki usuwane przez tę aktualizację zabezpieczeń nie dotyczą obsługiwanych wersji systemu Windows Server 2008 ani Windows Server 2008 R2, jeżeli systemy te zostały zainstalowane przy użyciu opcji instalacji Server Core. Więcej informacji na temat tej opcji instalacji można znaleźć w artykułach TechNet, [Managing a Server Core Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) i [Servicing a Server Core Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) (jęz. ang.). Należy pamiętać, że opcja instalacji Server Core nie dotyczy niektórych wersji systemu Windows Server 2008 i Windows Server 2008 R2. Zobacz [Porównanie opcji instalacji Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**Uwaga** **dotycząca biuletynu** **MS12-025**

<sup>[1]</sup>**Dotyczy systemu .NET Framework 4 i .NET Framework 4 Client Profile.** Pakiety redystrybucyjne systemu .NET Framework w wersji 4 są dostępne w dwóch profilach: .NET Framework 4 i .NET Framework 4 Client Profile. Aplikacja .NET Framework 4 Client Profile jest składnikiem systemu .NET Framework 4. Luka, do której odnosi się ta aktualizacja zabezpieczeń, dotyczy zarówno wersji .NET Framework 4, jak i .NET Framework 4 Client Profile. Więcej informacji znajduje się w artykule MSDN [Instalowanie systemu .NET Framework](http://msdn.microsoft.com/en-us/library/5a4x27ek.aspx) (j. ang.).

#### Pakiety i oprogramowanie Microsoft Office

 
<table style="border:1px solid black;">
<tr>
<th colspan="3">
Pakiety Microsoft Office i ich składniki
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS12-027**](http://go.microsoft.com/fwlink/?linkid=246275)
</td>
<td style="border:1px solid black;">
[**MS12-028**](http://go.microsoft.com/fwlink/?linkid=232498)
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
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2003 z dodatkiem Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office 2003 z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=d0d34b4f-4bcd-4df7-8ebc-87367e889959)  
(formanty standardowe systemu Windows)  
(KB2597112)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2007 z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Office 2007 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)  
(formanty standardowe systemu Windows)  
(KB2598041)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2007 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fbf24cc6-89e1-48dd-bb83-23eed30195e1)  
(KB2596871)  
(Ważny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2007 z dodatkiem Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office 2007 z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)  
(formanty standardowe systemu Windows)  
(KB2598041)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2010 (wersje 32-bitowe)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2010 (wersje 32-bitowe)](http://www.microsoft.com/downloads/details.aspx?familyid=23c9d7bf-c9e0-4e01-8b66-da542332a28b)  
(formanty standardowe systemu Windows)  
(KB2598039)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2010 z dodatkiem Service Pack 1 (wersje 32-bitowe)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2010 z dodatkiem Service Pack 1 (wersje 32-bitowe)](http://www.microsoft.com/downloads/details.aspx?familyid=23c9d7bf-c9e0-4e01-8b66-da542332a28b)  
(formanty standardowe systemu Windows)  
(KB2598039)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr>
<th colspan="3">
Składniki Microsoft Office Web Components
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS12-027**](http://go.microsoft.com/fwlink/?linkid=246275)
</td>
<td style="border:1px solid black;">
[**MS12-028**](http://go.microsoft.com/fwlink/?linkid=232498)
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Składniki Microsoft Office 2003 Web Components z dodatkiem Service Pack 3
</td>
<td style="border:1px solid black;">
[Składniki Microsoft Office 2003 Web Components z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=d0d34b4f-4bcd-4df7-8ebc-87367e889959)  
(formanty standardowe systemu Windows)  
(KB2597112)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr>
<th colspan="3">
Inne programy pakietu Microsoft Office
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS12-027**](http://go.microsoft.com/fwlink/?linkid=246275)
</td>
<td style="border:1px solid black;">
[**MS12-028**](http://go.microsoft.com/fwlink/?linkid=232498)
</td>
</tr>
<tr class="alternateRow">
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
<tr>
<td style="border:1px solid black;">
Microsoft Works 9
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Microsoft Works 9](http://www.microsoft.com/downloads/details.aspx?familyid=94e17a66-cf09-4314-89ec-53deadabfa66)  
(KB2680317)  
(Ważny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Works 6–9 File Converter
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Microsoft Works 6–9 File Converter](http://www.microsoft.com/downloads/details.aspx?familyid=4605f684-6314-4758-adeb-2a8810dfc8d1)  
(KB2680326)  
(Ważny)
</td>
</tr>
</table>
 
**Uwaga dotycząca biuletynu MS12-027**

Zobacz także pozostałe kategorie oprogramowania w sekcji **Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki**, aby uzyskać więcej plików aktualizacji w ramach tego samego identyfikatora biuletynu. Ten biuletyn obejmuje więcej niż jedną kategorię oprogramowania.

#### Oprogramowanie serwerów firmy Microsoft

 
<table style="border:1px solid black;">
<tr>
<th colspan="2">
Microsoft SQL Server
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS12-027**](http://go.microsoft.com/fwlink/?linkid=246275)
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
Microsoft SQL Server 2000 z dodatkiem Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2000 Analysis Services z dodatkiem Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=198f1819-818b-4b2e-a424-4a45729746eb)  
(KB983807)  
(Krytyczny)  
Aktualizacja GDR:  
[Microsoft SQL Server 2000 z dodatkiem Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=2a9d97e8-79e0-4997-88fe-1224707e1b37)  
(KB983808)  
(Krytyczny)  
Aktualizacja QFE:  
[Microsoft SQL Server 2000 z dodatkiem Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=8d0cac2f-f227-4e00-9454-4df62be86407)  
(KB983809)  
(Krytyczny)
</td>
</tr>
<tr>
<th colspan="2">
Składniki serwera Microsoft SQL Server
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft SQL Server 2005 dla systemów 32-bitowych z dodatkiem Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2005 dla systemów 32-bitowych z dodatkiem Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=d0d34b4f-4bcd-4df7-8ebc-87367e889959)<sup>[1]</sup>
(formanty standardowe systemu Windows)  
(KB2597112)  
(Krytyczny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SQL Server 2005 dla systemów z procesorem Itanium z dodatkiem Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2005 dla systemów z procesorem Itanium z dodatkiem Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=d0d34b4f-4bcd-4df7-8ebc-87367e889959)<sup>[1]</sup>
(formanty standardowe systemu Windows)  
(KB2597112)  
(Krytyczny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft SQL Server 2005 dla systemów z procesorem x64 z dodatkiem Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2005 dla systemów z procesorem x64 z dodatkiem Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=d0d34b4f-4bcd-4df7-8ebc-87367e889959)<sup>[1]</sup>
(formanty standardowe systemu Windows)  
(KB2597112)  
(Krytyczny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SQL Server 2005 Express Edition with Advanced Services z dodatkiem Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2005 Express Edition with Advanced Services z dodatkiem Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=d0d34b4f-4bcd-4df7-8ebc-87367e889959)<sup>[1]</sup>
(formanty standardowe systemu Windows)  
(KB2597112)  
(Krytyczny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft SQL Server 2008 dla systemów 32-bitowych z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2008 dla systemów 32-bitowych z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(formanty standardowe systemu Windows)  
(KB2598041)  
(Krytyczny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SQL Server 2008 dla systemów 32-bitowych z dodatkiem Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2008 dla systemów 32-bitowych z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(formanty standardowe systemu Windows)  
(KB2598041)  
(Krytyczny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft SQL Server 2008 dla systemów z procesorem x64 z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2008 dla systemów z procesorem x64 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(formanty standardowe systemu Windows)  
(KB2598041)  
(Krytyczny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SQL Server 2008 dla systemów z procesorem x64 z dodatkiem Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2008 dla systemów z procesorem x64 z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(formanty standardowe systemu Windows)  
(KB2598041)  
(Krytyczny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft SQL Server 2008 dla systemów z procesorem Itanium z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2008 dla systemów z procesorem Itanium z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(formanty standardowe systemu Windows)  
(KB2598041)  
(Krytyczny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SQL Server 2008 dla systemów z procesorem Itanium z dodatkiem Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2008 dla systemów z procesorem Itanium z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(formanty standardowe systemu Windows)  
(KB2598041)  
(Krytyczny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft SQL Server 2008 R2 dla systemów 32-bitowych
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2008 R2 dla systemów 32-bitowych](http://www.microsoft.com/downloads/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(formanty standardowe systemu Windows)  
(KB2598041)  
(Krytyczny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SQL Server 2008 R2 dla systemów 32-bitowych z dodatkiem Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2008 R2 dla systemów 32-bitowych z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(formanty standardowe systemu Windows)  
(KB2598041)  
(Krytyczny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft SQL Server 2008 R2 dla systemów z procesorem x64
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2008 R2 dla systemów z procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(formanty standardowe systemu Windows)  
(KB2598041)  
(Krytyczny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SQL Server 2008 R2 dla systemów z procesorem x64 z dodatkiem Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2008 R2 dla systemów z procesorem x64 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(formanty standardowe systemu Windows)  
(KB2598041)  
(Krytyczny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft SQL Server 2008 R2 dla systemów z procesorem Itanium
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2008 R2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(formanty standardowe systemu Windows)  
(KB2598041)  
(Krytyczny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SQL Server 2008 R2 dla systemów z procesorem Itanium z dodatkiem Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2008 R2 dla systemów z procesorem Itanium z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(formanty standardowe systemu Windows)  
(KB2598041)  
(Krytyczny)
</td>
</tr>
</table>
 
**Uwagidotyczące biuletynu** **MS12-027**

<sup>[1]</sup>Ta aktualizacja jest taka sama, jak aktualizacja KB2597112 dla pakietu Microsoft Office 2003

<sup>[2]</sup>Ta aktualizacja jest taka sama, jak aktualizacja KB2598041 dla pakietu Microsoft Office 2007

Zobacz także pozostałe kategorie oprogramowania w sekcji **Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki**, aby uzyskać więcej plików aktualizacji w ramach tego samego identyfikatora biuletynu. Ten biuletyn obejmuje więcej niż jedną kategorię oprogramowania.

 
<table style="border:1px solid black;">
<tr>
<th colspan="2">
Microsoft BizTalk Server
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS12-027**](http://go.microsoft.com/fwlink/?linkid=246275)
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
Microsoft BizTalk Server 2002 z dodatkiem Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft BizTalk Server 2002 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d90b78d2-551b-499b-9bd2-85b40646dbc7)  
(KB2645025)  
(Krytyczny)
</td>
</tr>
<tr>
<th colspan="2">
Microsoft Commerce Server
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS12-027**](http://go.microsoft.com/fwlink/?linkid=246275)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Zbiorczy wskaźnik ważności**
</td>
<td style="border:1px solid black;">
[**Krytyczny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Commerce Server 2002 z dodatkiem Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft Commerce Server 2002 z dodatkiem Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=35de8833-50ae-482d-aa07-497bf68fb38e)  
(KB2658674)  
(Krytyczny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Commerce Server 2007 z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Commerce Server 2007 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3f04fb90-8f11-4392-a4bc-800903091f04)  
(KB2658677)  
(Krytyczny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Commerce Server 2009
</td>
<td style="border:1px solid black;">
[Microsoft Commerce Server 2009](http://www.microsoft.com/downloads/details.aspx?familyid=a8998b6b-e9a4-457e-a34f-0458dda81f2f)  
(KB2655547)  
(Krytyczny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Commerce Server 2009 R2
</td>
<td style="border:1px solid black;">
[Microsoft Commerce Server 2009 R2](http://www.microsoft.com/downloads/details.aspx?familyid=e9221811-8913-412b-ae04-21a55ce7c4c5)  
(KB2658676)  
(Krytyczny)
</td>
</tr>
</table>
 
**Uwaga dotycząca biuletynu MS12-027**

Zobacz także pozostałe kategorie oprogramowania w sekcji **Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki**, aby uzyskać więcej plików aktualizacji w ramach tego samego identyfikatora biuletynu. Ten biuletyn obejmuje więcej niż jedną kategorię oprogramowania.

#### Narzędzia i oprogramowanie firmy Microsoft dla deweloperów

 
<table style="border:1px solid black;">
<tr>
<th colspan="2">
Microsoft Visual FoxPro
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS12-027**](http://go.microsoft.com/fwlink/?linkid=246275)
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
Microsoft Visual FoxPro 8.0 z dodatkiem Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Visual FoxPro 8.0 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=3a7ff474-f1e0-4c86-9555-64e8e7357890)  
(KB2647488)  
(Krytyczny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual FoxPro 9.0 z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Visual FoxPro 9.0 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=53c0132e-7724-4e94-abe9-e79b76ce35d7)  
(KB2647490)  
(Krytyczny)
</td>
</tr>
<tr>
<th colspan="2">
Visual Basic
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS12-027**](http://go.microsoft.com/fwlink/?linkid=246275)
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
Visual Basic 6.0 Runtime
</td>
<td style="border:1px solid black;">
[Visual Basic 6.0 Runtime](http://www.microsoft.com/downloads/details.aspx?familyid=0afe933a-1e62-45c4-910c-ea94b203df5a)  
(KB2641426)  
(Krytyczny)
</td>
</tr>
</table>
 
**Uwaga dotycząca biuletynu MS12-027**

Zobacz także pozostałe kategorie oprogramowania w sekcji **Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki**, aby uzyskać więcej plików aktualizacji w ramach tego samego identyfikatora biuletynu. Ten biuletyn obejmuje więcej niż jedną kategorię oprogramowania.

#### Program Microsoft Remote Access

 
<table style="border:1px solid black;">
<tr>
<th colspan="2">
Program Microsoft Forefront Unified Access Gateway
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS12-026**](http://go.microsoft.com/fwlink/?linkid=238519)
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
Program Microsoft Forefront Unified Access Gateway
</td>
<td style="border:1px solid black;">
[Microsoft Forefront Unified Access Gateway 2010 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d4b4ecc4-8bc6-43d0-b872-93673e0d9a6f)<sup>[1]</sup>
(KB2649261)  
(Ważny)  
[Microsoft Forefront Unified Access Gateway 2010 z dodatkiem Service Pack 1 Update 1](http://www.microsoft.com/downloads/details.aspx?familyid=e0f9acab-bfb8-4758-b60d-64e68a84fba0)<sup>[1]</sup>
(KB2649262)  
(Ważny)
</td>
</tr>
</table>
 
**Uwaga** **dotycząca biuletynu** **MS12-026**

<sup>[1]</sup>Ta aktualizacja jest dostępna tylko w witrynie Centrum pobierania Microsoft.

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

-   linx2008 z firmy [AISec](http://www.aisec.cn/), za zgłoszenie problemu opisanego w biuletynie MS12-023
-   Roel Spilker z firmy [TOPdesk](http://www.topdesk.com), za zgłoszenie problemu opisanego w biuletynie MS12-023
-   Jose Antonio Vazquez Gonzalez, we współpracy z [VeriSign iDefense Labs](http://labs.idefense.com), za zgłoszenie problemu opisanego w biuletynie MS12-023
-   Anonimowy analityk współpracujący z oddziałem [Zero Day Initiative](http://www.zerodayinitiative.com/) firmy [TippingPoint](http://www.tippingpoint.com), za zgłoszenie problemu opisanego w biuletynie MS12-023
-   Anonimowy analityk współpracujący z oddziałem [Zero Day Initiative](http://www.zerodayinitiative.com/) firmy [TippingPoint](http://www.tippingpoint.com), za zgłoszenie problemu opisanego w biuletynie MS12-023
-   Masato Kinugawa, za współpracę z firmą Microsoft przy wprowadzaniu kompleksowych zmian zabezpieczeń zawartych w biuletynie MS12-023
-   Robert Zacek i Igor Glucksmann z firmy [Avast Software](http://www.avast.com/), za zgłoszenie problemu opisanego w biuletynie MS12-024
-   Witalij Toropow, we współpracy z firmą [VeriSign iDefense Labs](http://labs.idefense.com/), za zgłoszenie problemu opisanego w biuletynie MS12-025
-   Shaun Colley z firmy [IOActive, Ltd.](http://ioactive.co.uk/), za zgłoszenie problemu opisanego w biuletynie MS12-028

#### Pomoc techniczna

-   Wymienione oprogramowanie zostało przetestowane w celu ustalenia, których wersji dotyczy problem. Dla pozostałych wersji upłynął okres pomocy technicznej. Aby zapoznać się z zasadami cyklu pomocy technicznej dotyczącymi używanej wersji oprogramowania, odwiedź [witrynę zasad cyklu pomocy technicznej firmy Microsoft](http://go.microsoft.com/fwlink/?linkid=21742).
-   Rozwiązania zabezpieczeń dla specjalistów IT: [Centrum zabezpieczeń TechNet — obsługa techniczna i rozwiązywanie problemów](http://technet.microsoft.com/security/bb980617.aspx)
-   Zabezpiecz swój komputer z systemem Windows przed wirusami i złośliwym oprogramowaniem: [Virus Solution i centrum zabezpieczeń](http://support.microsoft.com/contactus/cu_sc_virsec_master)
-   Lokalna pomoc techniczna dla twojego kraju: [Międzynarodowa pomoc techniczna](http://support.microsoft.com/common/international.aspx)

#### Zrzeczenie odpowiedzialności

Informacje w bazie wiedzy Microsoft Knowledge Base są dostarczane „tak jak są” bez jakiejkolwiek gwarancji. Firma Microsoft odrzuca wszelkie gwarancje, wyraźne i dorozumiane, w tym gwarancje dotyczące wartości handlowej i przydatności do określonego celu. Firma Microsoft Corporation ani jej dostawcy w żadnym wypadku nie ponoszą odpowiedzialności za jakiekolwiek szkody, w tym bezpośrednie, pośrednie, przypadkowe, wynikowe, utratę zysków handlowych lub szkody specjalne, nawet jeżeli firmę Microsoft Corporation lub jej dostawców powiadomiono o możliwości zaistnienia takich szkód. W niektórych stanach wyłączenie lub ograniczenie odpowiedzialności za straty wynikowe lub przypadkowe, a więc i powyższe ograniczenia, nie mają zastosowania.

#### Wersje

-   Wersja 1.0 (10 kwietnia 2012 r.): Opublikowane podsumowanie biuletynów zabezpieczeń.
-   Wersja 2.0 (26 kwietnia 2012 r.): W biuletynie MS12-027 do sekcji „Programy, których dotyczy problem”, dodano program SQL Server 2008 R2 z dodatkiem Service Pack 1. Wyjaśniono też, że aktualizacja ma zastosowanie do wszystkich instalacji programu Microsoft SQL Server 2000 Analysis Services z dodatkiem Service Pack 4, ponieważ rozróżnienie na aktualizacje QFE i GDR nie ma zastosowania do tego produktu. Zmiany te mają charakter wyłącznie informacyjny. Nie wprowadzono żadnych zmian do plików aktualizacji zabezpieczeń ani logiki wykrywania. Ponieważ te aktualizacje były oferowane poprawnie od chwili pierwszej publikacji, klienci, którzy je wdrożyli, nie muszą podejmować żadnych działań.

*Built at 2014-04-18T01:50:00Z-07:00*
