---
TOCTitle: 'MS10-NOV'
Title: 'Podsumowanie biuletynów zabezpieczeń firmy Microsoft za listopad 2010 r.'
ms:assetid: 'ms10-nov'
ms:contentKeyID: 61233117
ms:mtpsurl: 'https://technet.microsoft.com/pl-PL/library/ms10-nov(v=Security.10)'
---
Podsumowanie biuletynów zabezpieczeń firmy Microsoft za listopad 2010 r.
========================================================================

Opublikowano: 9 listopada 2010 | Zaktualizowano: 13 kwietnia 2011

**Wersja:** 2.1

Niniejsze podsumowanie biuletynów zabezpieczeń zawiera spis biuletynów za listopad 2010 r.

Z chwilą opublikowania biuletynów za listopad 2010 r. niniejsze podsumowanie biuletynów zastępuje powiadomienie o biuletynach zabezpieczeń wydane 4 listopada 2010 r. Aby uzyskać więcej informacji na temat usługi powiadamiania o biuletynach, zobacz [Powiadomienia o biuletynach zabezpieczeń firmy Microsoft (j. ang.)](http://technet.microsoft.com/security/bulletin/advance).

Aby dowiedzieć się, jak otrzymywać automatyczne powiadomienia o publikacji biuletynów zabezpieczeń firmy Microsoft, odwiedź stronę [Microsoft Technical Security Notifications](http://go.microsoft.com/fwlink/?linkid=21163).

10 listopada 2010 r. o godz. 11:00 czasu Pacyfiku (godz. 20:00 czasu środkowoeuropejskiego) firma Microsoft udostępni emisję internetową, w której znajdą się odpowiedzi na pytania klientów dotyczące tych biuletynów (USA i Kanada). [Zarejestruj się, aby zobaczyć emisję internetową dotyczącą biuletynów zabezpieczeń za listopad](https://msevents.microsoft.com/cui/webcasteventdetails.aspx?culture=en-us&eventid=1032454441). Po tym dniu emisja internetowa będzie dostępna na żądanie. Aby uzyskać więcej informacji, zobacz [Podsumowania biuletynów zabezpieczeń i emisje internetowe firmy Microsoft](http://technet.microsoft.com/security/bulletin/summary).

Firma Microsoft udostępnia także informacje, dzięki którym klienci mogą ustalić priorytety dla aktualizacji zabezpieczeń w związku z niezwiązanymi z zabezpieczeniami aktualizacjami o wysokim priorytecie, które publikowane są w tym samym dniu, co comiesięczne aktualizacje zabezpieczeń. Zapoznaj się z sekcją **Inne informacje**.

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=203241">MS10-087</a></td>
<td style="border:1px solid black;"><strong>Luki w zabezpieczeniach pakietu Microsoft Office umożliwiają zdalne wykonanie kodu (2423930)</strong><br />
<br />
Niniejsza aktualizacja zabezpieczeń usuwa jedną lukę zgłoszoną przez organizacje publiczne oraz pięć luk zgłoszonych przez użytkowników, istniejących w pakiecie Microsoft Office. Najpoważniejsza z tych luk umożliwia zdalne wykonanie kodu, jeśli użytkownik otworzy specjalnie spreparowaną wiadomość e-mail w formacie RTF lub wyświetli jej podgląd. Osoba atakująca, której uda się wykorzystać jedną z tych luk, może uzyskać takie same uprawnienia, jak użytkownik lokalny. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Krytyczny</a><br />
Zdalne wykonanie kodu</td>
<td style="border:1px solid black;">Może wymagać ponownego uruchomienia</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=198186">MS10-088</a></td>
<td style="border:1px solid black;"><strong>Luki w zabezpieczeniach programu Microsoft PowerPoint umożliwiają zdalne wykonanie kodu (2293386)</strong><br />
<br />
Ta aktualizacja zabezpieczeń usuwa dwie zgłoszone przez użytkowników luki w zabezpieczeniach pakietu Microsoft Office, które umożliwiają zdalne wykonanie kodu, gdy użytkownik otworzy specjalnie spreparowany plik programu PowerPoint. Osoba atakująca, której uda się wykorzystać jedną z tych luk, może uzyskać pełną kontrolę nad zagrożonym systemem. Osoba taka mogłaby wówczas instalować programy, przeglądać, zmieniać i usuwać dane oraz tworzyć nowe konta z pełnymi uprawnieniami. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Ważny</a><br />
Zdalne wykonanie kodu</td>
<td style="border:1px solid black;">Może wymagać ponownego uruchomienia</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=199536">MS10-089</a></td>
<td style="border:1px solid black;"><strong>Luki w zabezpieczeniach programu Forefront UAG mogą pozwolić na podniesienie poziomu uprawnień (2316074)</strong><br />
<br />
Ta aktualizacja zabezpieczeń usuwa cztery luki w zabezpieczeniach programu Forefront UAG, które zostały zgłoszone przez użytkowników. Najpoważniejsza z tych luk może umożliwić podniesienie uprawnień, jeśli użytkownik odwiedzi witrynę sieci Web, której dotyczy problem, korzystając ze specjalnie spreparowanego adresu URL. Intruz nie może jednak w żaden sposób zmusić użytkowników do odwiedzenia takiej witryny. Musi natomiast przekonać użytkowników do odwiedzenia tej witryny, najczęściej zachęcając do kliknięcia łącza w wiadomości e-mail lub wiadomości błyskawicznej, które przekieruje użytkowników do witryny osoby atakującej.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Ważny</a><br />
Podniesienie uprawnień</td>
<td style="border:1px solid black;">Może wymagać ponownego uruchomienia</td>
<td style="border:1px solid black;">Microsoft Forefront United Access Gateway</td>
</tr>
</tbody>
</table>
  
Wskaźnik możliwości wykorzystania luki  
--------------------------------------
  
<span></span>
Poniższa tabela przedstawia ocenę możliwości wykorzystania luk dla każdej luki opisywanej w tym miesiącu. Luki są wymienione według malejącego poziomu oceny możliwości wykorzystania, a nie według identyfikatora CVE. Uwzględniono wyłącznie te luki, które w biuletynach mają nadany wskaźnik ważności „krytyczny” lub „ważny”.
  
**W jaki sposób korzystać z tej tabeli?**
  
Tabela ta pozwala sprawdzić prawdopodobieństwo, że w ciągu 30 dni od wydania biuletynu zabezpieczeń dla każdej z aktualizacji zabezpieczeń, których zainstalowanie może być potrzebne, opublikowany zostanie działający kod wykorzystujący lukę w zabezpieczeniach. Aby ustalić priorytety wdrażania, zapoznaj się z dostępnymi poniżej ocenami, rozpatrując je w kontekście posiadanej konfiguracji. Więcej informacji na temat znaczenia tych ocen oraz sposobu ich wyznaczania można znaleźć na stronie sieci Web [Microsoft Exploitability Index](http://technet.microsoft.com/en-us/security/cc998259.aspx).
  
| Identyfikator biuletynu                                   | Nazwa luki w zabezpieczeniach                                                                                            | CVE ID                                                                           | Ocena wskaźnika możliwości wykorzystania luki                                                                              | Najważniejsze uwagi                                                                                  |  
|-----------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------|  
| [MS10-088](http://go.microsoft.com/fwlink/?linkid=198186) | Luka w zabezpieczeniach programu PowerPoint związana z przepełnieniem buforu analizy                                     | [CVE-2010-2572](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2572) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny spójny kod wykorzystujący lukę          | (Brak)                                                                                               |  
| [MS10-089](http://go.microsoft.com/fwlink/?linkid=199536) | Luka w zabezpieczeniach programu UAG związana ze skryptami krzyżowymi umożliwia podniesienie uprawnień                   | [CVE-2010-2733](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2733) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny spójny kod wykorzystujący lukę          | (Brak)                                                                                               |  
| [MS10-089](http://go.microsoft.com/fwlink/?linkid=199536) | Luka w zabezpieczeniach programu Forefront UAG związana z problemem ze skryptami krzyżowymi w witrynie UAG Mobile Portal | [CVE-2010-2734](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2734) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny spójny kod wykorzystujący lukę          | (Brak)                                                                                               |  
| [MS10-087](http://go.microsoft.com/fwlink/?linkid=203241) | Luka w zabezpieczeniach formatu RTF związana z przepełnieniem buforu stosu                                               | [CVE-2010-3333](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3333) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny spójny kod wykorzystujący lukę          | (Brak)                                                                                               |  
| [MS10-087](http://go.microsoft.com/fwlink/?linkid=203241) | Luka w zabezpieczeniach rekordów rysunków obiektów Office Art                                                            | [CVE-2010-3334](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3334) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny spójny kod wykorzystujący lukę          | (Brak)                                                                                               |  
| [MS10-087](http://go.microsoft.com/fwlink/?linkid=203241) | Luka w zabezpieczeniach rysunków związana z obsługą wyjątków                                                             | [CVE-2010-3335](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3335) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny spójny kod wykorzystujący lukę          | (Brak)                                                                                               |  
| [MS10-087](http://go.microsoft.com/fwlink/?linkid=203241) | Luka w zabezpieczeniach związana z niebezpiecznym ładowaniem bibliotek                                                   | [CVE-2010-3337](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3337) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny spójny kod wykorzystujący lukę          | **Informacje o tej luce są znane publicznie**                                                        |  
| [MS10-089](http://go.microsoft.com/fwlink/?linkid=199536) | Luka dotycząca skryptów krzyżowych na stronie Signurl.asp                                                                | [CVE-2010-3936](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3936) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny spójny kod wykorzystujący lukę          | (Brak)                                                                                               |  
| [MS10-087](http://go.microsoft.com/fwlink/?linkid=203241) | Luka w zabezpieczeniach programu PowerPoint związana z niedopełnieniem liczby całkowitej i powodująca uszkodzenie stosu  | [CVE-2010-2573](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2573) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobnie niespójny kod wykorzystujący lukę      | Luce tej jest również poświęcony biuletyn [MS10-088](http://go.microsoft.com/fwlink/?linkid=198186). |  
| [MS10-088](http://go.microsoft.com/fwlink/?linkid=198186) | Luka w zabezpieczeniach programu PowerPoint związana z niedopełnieniem liczby całkowitej i powodująca uszkodzenie stosu  | [CVE-2010-2573](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2573) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobnie niespójny kod wykorzystujący lukę      | Luce tej jest również poświęcony biuletyn [MS10-087](http://go.microsoft.com/fwlink/?linkid=203241). |  
| [MS10-087](http://go.microsoft.com/fwlink/?linkid=203241) | Luka w zabezpieczeniach programu antywirusowego związana z odczytem dużej wartości identyfikatora SPID MSO               | [CVE-2010-3336](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3336) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobnie niespójny kod wykorzystujący lukę      | (Brak)                                                                                               |  
| [MS10-089](http://go.microsoft.com/fwlink/?linkid=199536) | Luka w zabezpieczeniach procedury przekierowania programu UAG związana z fałszowaniem                                    | [CVE-2010-2732](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2732) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) — działający kod wykorzystujący lukę mało prawdopodobny | Jest to tylko luka w zabezpieczeniach związana z fałszowaniem.                                       |
  
Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki  
---------------------------------------------------------------------------------
  
<span></span>
Poniższe tabele wymieniają biuletyny według najważniejszych kategorii programów i wskaźnika ważności.
  
**Jak korzystać z tych tabel?**
  
Tabele te pozwalają odczytać informacje o aktualizacjach zabezpieczeń, których zainstalowanie może być konieczne. Należy zapoznać się z informacjami dotyczącymi każdego wymienionego programu lub składnika oprogramowania w celu sprawdzenia, czy aktualizacje zabezpieczeń odnoszą się do danej instalacji. Jeśli program lub składnik znajduje się na liście, dostępne jest łącze prowadzące do aktualizacji oprogramowania i podana jest informacja o wskaźniku ważności tej aktualizacji.
  
**Uwaga** Konieczne może być zainstalowanie kilku aktualizacji zabezpieczeń dotyczących jednej luki. Przejrzyj całą kolumnę dla każdego wymienionego identyfikatora biuletynu, aby sprawdzić, jakie aktualizacje musisz zainstalować, w oparciu o programy bądź składniki zainstalowane w systemie.
  
#### Pakiety i oprogramowanie Office

 
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
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
[**MS10-087**](http://go.microsoft.com/fwlink/?linkid=203241)
</td>
<td style="border:1px solid black;">
[**MS10-088**](http://go.microsoft.com/fwlink/?linkid=198186)
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
Microsoft Office XP z dodatkiem Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office XP z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=f32648e3-2fb5-472c-932f-360e5d3c0931)  
(KB2289169)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Microsoft Office PowerPoint 2002 z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=3efbf9f6-734a-46ac-8f92-87b6ec819bfa)  
(KB2413272)  
(Ważny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2003 z dodatkiem Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office 2003 z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=07a6cf76-2cea-4c54-b66d-50e9eed108ac)  
(KB2289187)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Microsoft PowerPoint 2003 z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=108286d4-fb68-40d6-a7b1-64b3a4eb87ee)  
(KB2413304)  
(Ważny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2007 z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Office 2007 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=be0c5878-60c0-4700-8836-50d369b51d04)  
(KB2289158)  
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
[Microsoft Office 2010 (wersje 32-bitowe)](http://www.microsoft.com/downloads/details.aspx?familyid=0b308508-0e1e-4e90-b2b8-7e32bfc5dbf4)  
(KB2289161)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2010 (wersje 64-bitowe)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2010 (wersje 64-bitowe)](http://www.microsoft.com/downloads/details.aspx?familyid=534c6a2a-e7c6-4adf-8b81-e009a2b5fff4)  
(KB2289161)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr>
<th colspan="3">
Microsoft Office dla komputerów Macintosh
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS10-087**](http://go.microsoft.com/fwlink/?linkid=203241)
</td>
<td style="border:1px solid black;">
[**MS10-088**](http://go.microsoft.com/fwlink/?linkid=198186)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Zbiorczy wskaźnik ważności**
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
Microsoft Office 2004 dla komputerów Macintosh
</td>
<td style="border:1px solid black;">
Pakiet Microsoft Office 2004 dla komputerów Macintosh<sup>[1]</sup>
(Ważny)
</td>
<td style="border:1px solid black;">
Pakiet Microsoft Office 2004 dla komputerów Macintosh<sup>[1]</sup>
(Ważny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2008 dla komputerów Macintosh
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 dla komputerów Macintosh](http://www.microsoft.com/downloads/details.aspx?familyid=ad1b1984-b2b2-49b3-a1dd-385b77d9248a)  
(KB2476512)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2011 dla komputerów Macintosh
</td>
<td style="border:1px solid black;">
[Microsoft Office 2011 dla komputerów Macintosh](http://www.microsoft.com/downloads/details.aspx?familyid=8bd6ca3b-8004-4e8d-a09d-220dcbbce799)  
(KB2454823)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Open XML File Format Converter for Mac
</td>
<td style="border:1px solid black;">
[Open XML File Format Converter dla komputerów Macintosh](http://www.microsoft.com/downloads/details.aspx?familyid=b846d255-a7d4-4a2c-a084-d434c29fe676)  
(KB2476511)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr>
<th colspan="3">
Inne programy pakietu Office
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS10-087**](http://go.microsoft.com/fwlink/?linkid=203241)
</td>
<td style="border:1px solid black;">
[**MS10-088**](http://go.microsoft.com/fwlink/?linkid=198186)
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
Podgląd programu Microsoft PowerPoint
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Podgląd programu Microsoft PowerPoint 2007 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=df826b79-7398-45de-943c-6f6f0af1b4e3)  
(KB2413381)  
(Ważny)
</td>
</tr>
</table>
 
**Uwaga dotycząca biuletynu MS10-087**

<sup>[1]</sup>\]Aktualizacja zabezpieczeń dla pakietu Microsoft Office 2004 dla komputerów Macintosh (KB2505924) jest dostępna od 12 kwietnia 2011 r. Szczegółowe informacje zawiera biuletyn.

**Uwaga dotycząca biuletynu MS10-088**

<sup>[1]</sup>\]Aktualizacja zabezpieczeń dla pakietu Microsoft Office 2004 dla komputerów Macintosh (KB2505924) jest dostępna od 12 kwietnia 2011 r. Szczegółowe informacje zawiera biuletyn.

#### Program Microsoft Remote Access

 
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
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
[**MS10-089**](http://go.microsoft.com/fwlink/?linkid=199536)
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
[Forefront Unified Access Gateway 2010](http://www.microsoft.com/downloads/details.aspx?familyid=5f2ee08e-e289-47db-bd3f-7b9cfc1eb985)<sup>[1]</sup>
(KB2433585)  
(Ważny)  
[Forefront Unified Access Gateway 2010 Update 1](http://www.microsoft.com/downloads/details.aspx?familyid=db0b70c8-1fa5-4d92-9888-3500c7566b19)<sup>[1]</sup>
(KB2433584)  
(Ważny)  
[Forefront Unified Access Gateway 2010 Update 2](http://www.microsoft.com/downloads/details.aspx?familyid=4e3ee07a-771c-46ee-959f-82389bab67d7)<sup>[1]</sup>
(KB2418933)  
(Ważny)
</td>
</tr>
</table>
 
**Uwaga dotycząca biuletynu MS10-089**

<sup>[1]</sup>Ta aktualizacja jest dostępna tylko w witrynie Centrum pobierania Microsoft.

Narzędzia wykrywania i wdrażania oraz wskazówki
-----------------------------------------------

<span></span>
**Centrum zabezpieczeń**

Zarządzanie oprogramowaniem oraz aktualizacjami zabezpieczeń, które należy zainstalować na serwerach oraz komputerach stacjonarnych i przenośnych w organizacji. Więcej informacji można znaleźć w [Centrum TechNet Update Management Center](http://go.microsoft.com/fwlink/?linkid=69903). Witryna [TechNet Security Center](http://go.microsoft.com/fwlink/?linkid=21171) zawiera dodatkowe informacje na temat zabezpieczeń w produktach firmy Microsoft. Użytkownicy mogą także uzyskać dostęp do tych informacji w witrynie [Bezpieczeństwo w domu](http://go.microsoft.com/fwlink/?linkid=85102), klikając łącze „Najnowsze aktualizacje zabezpieczeń”.

Aktualizacje zabezpieczeń dostępne są w witrynach [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747) i [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130). Aktualizacje zabezpieczeń są także dostępne w witrynie [Centrum pobierania Microsoft](http://go.microsoft.com/fwlink/?linkid=21129). Najłatwiej je znaleźć, wyszukując wyrażenie „aktualizacja zabezpieczeń”.

Aktualizacje zabezpieczeń można także pobierać z [Wykazu usługi Microsoft Update](http://go.microsoft.com/fwlink/?linkid=96155). Wykaz usługi Microsoft Update zawiera katalog zawartości z możliwością przeszukiwania, który udostępniany jest poprzez usługi Windows Update i Microsoft Update i obejmuje aktualizacje zabezpieczeń, sterowniki i dodatki Service Pack. Wyszukiwanie przy użyciu numeru biuletynu zabezpieczeń (np. „MS07-036”) pozwala dodać do koszyka wszystkie odpowiednie aktualizacje (w tym różne wersje językowe aktualizacji) i pobrać pliki do wybranego folderu. Więcej informacji na temat Wykazu usługi Microsoft Update można znaleźć w [Często zadawanych pytaniach dotyczących Wykazu usługi Microsoft Update](http://go.microsoft.com/fwlink/?linkid=97900).

**Porady dotyczące wykrywania i wdrażania**

Firma Microsoft udziela porad dotyczących wykrywania i wdrażania aktualizacji zabezpieczeń. Porady takie zawierają zalecenia i informacje ułatwiające specjalistom IT poznanie obsługi różnych narzędzi do wykrywania i wdrażania aktualizacji zabezpieczeń. Więcej informacji na ten temat można znaleźć w [artykule 961747 bazy wiedzy Microsoft Knowledge Base](http://support.microsoft.com/kb/961747).

**Narzędzie Microsoft Baseline Security Analyzer**

Narzędzie Microsoft Baseline Security Analyzer umożliwia administratorom skanowanie lokalnych i zdalnych systemów w poszukiwaniu brakujących aktualizacji zabezpieczeń oraz typowych błędów konfiguracji zabezpieczeń. Więcej informacji na temat narzędzia MBSA można znaleźć w witrynie sieci Web[Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134).

**Windows Server Update Services**

Korzystając z programu Windows Server Update Services (WSUS), administratorzy mogą szybko i niezawodnie wdrożyć najnowsze aktualizacje krytyczne i aktualizacje zabezpieczeń przeznaczone dla systemów operacyjnych Microsoft Windows 2000 i nowszych, pakietów Office XP i nowszych, programu Exchange Server 2003 oraz SQL Server 2000 w systemach operacyjnych Microsoft Windows 2000 i nowszych.

Więcej informacji na temat sposobu wdrażania tej aktualizacji zabezpieczeń za pomocą programu Windows Server Update Services można znaleźć w [witrynie sieci Web programu Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=50120).

**Program Systems Management Server**

Program Systems Management Server (SMS) jest przeznaczonym dla przedsiębiorstw i w znacznym stopniu konfigurowalnym rozwiązaniem służącym do zarządzania aktualizacjami. Program SMS umożliwia administratorom znalezienie komputerów z systemem Windows, na których należy zainstalować aktualizację zabezpieczeń, a także przeprowadzić kontrolowane wdrożenie tych aktualizacji w całym przedsiębiorstwie, w minimalnym stopniu zakłócając przy tym pracę użytkowników końcowych. Dostępne jest kolejne wydanie programu SMS, System Center Configuration Manager 2007. Zapoznaj się także z zawartością witryny [System Center Configuration Manager 2007](http://technet.microsoft.com/en-us/library/bb735860.aspx). Więcej informacji na temat możliwości wykorzystania przez administratorów programu SMS 2003 do wdrażania aktualizacji zabezpieczeń można znaleźć w [witrynie sieci Web zarządzania poprawkami zabezpieczeń programu SMS 2003](http://go.microsoft.com/fwlink/?linkid=22939). Użytkownicy programu SMS 2.0 mogą także skorzystać z narzędzia Security Update Inventory Tool (SUIT) ułatwiającego wdrożenie aktualizacji zabezpieczeń. Więcej informacji na temat programu SMS można znaleźć w witrynie sieci Web [Microsoft Systems Management Server](http://go.microsoft.com/fwlink/?linkid=21158).

**Uwaga** Program SMS zapewnia obsługę rozwiązań zawartych w biuletynach zabezpieczeń dzięki narzędziu Microsoft Baseline Security Analyzer. Narzędzia te mogą nie wykrywać wszystkich aktualizacji oprogramowania. W takich przypadkach administratorzy mogą wykorzystywać dostępne w programie SMS funkcje zarządzania zasobami do przyporządkowania poszczególnych aktualizacji określonym systemom. Aby uzyskać więcej informacji dotyczących tej procedury, zobacz [Wdrażanie aktualizacji oprogramowania za pomocą funkcji Software Distribution programu SMS](http://go.microsoft.com/fwlink/?linkid=33341). Niektóre aktualizacje oprogramowania wymagają od użytkownika uprawnień administratora po ponownym uruchomieniu systemu. Do zainstalowania tych aktualizacji administratorzy mogą użyć narzędzia Elevated Rights Deployment Tool (dostępnego w dodatku [SMS 2.0 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=21161)).

**Tester zgodności aktualizacji i zestaw narzędzi do sprawdzania zgodności aplikacji**

Często aktualizacje zapisują informacje w tych samych plikach i ustawieniach rejestru niezbędnych do działania określonych aplikacji użytkownika. Może to prowadzić do niezgodności i wydłużyć czas wdrażania aktualizacji zabezpieczeń. Dzięki składnikom narzędzia [Tester zgodności aplikacji](http://technet2.microsoft.com/windowsvista/en/library/4279e239-37a4-44aa-aec5-4e70fe39f9de1033.mspx?mfr=true) znajdującego się w [Zestawie narzędzi do sprawdzania zgodności aplikacji](http://www.microsoft.com/downloads/details.aspx?familyid=24da89e9-b581-47b0-b45e-492dd6da2971&displaylang=en) można usprawnić proces testowania i sprawdzania poprawności aktualizacji systemu Windows.

W Zestawie narzędzi do sprawdzania zgodności aplikacji znajdują się niezbędne narzędzia i dokumentacja, które umożliwiają ocenę zgodności aplikacji przed wdrożeniem systemu Microsoft Windows Vista, aktualizacji dla systemu Windows, aktualizacji zabezpieczeń firmy Microsoft lub nowej wersji programu Windows Internet Explorer w środowisku użytkownika, oraz ograniczenie problemów ze zgodnością aplikacji.

### Inne informacje:

#### Narzędzie Microsoft Windows do usuwania złośliwego oprogramowania

Firma Microsoft opublikowała zaktualizowaną wersję narzędzia Microsoft Windows Malicious Software Removal Tool, która dostępna jest w witrynach sieci Web Windows Update i Microsoft Update, poprzez usługi Windows Server Update Services i w witrynie Centrum pobierania Microsoft.

#### Aktualizacje o wysokim priorytecie niezwiązane z zabezpieczeniami, dostępne w witrynach MU, WU oraz usługach WSUS

Aby uzyskać informacje na temat publikacji niezwiązanych z zabezpieczeniami, dostępnych w witrynach Windows Update i Microsoft Update, zobacz:

-   [Artykuł 894199 bazy wiedzy Microsoft Knowledge Base](http://support.microsoft.com/kb/894199): Opis zmian zawartości Usług aktualizacji oprogramowania i usług Windows Server Update Services. Zawiera wszystkie treści dotyczące systemu Windows.
-   [Aktualizacje z poprzednich miesięcy dla usług Windows Server Update Services](http://technet.microsoft.com/en-us/wsus/bb456965.aspx). Wyświetla nowe, zmienione i opublikowane ponownie aktualizacje dla produktów firmy Microsoft innych niż Microsoft Windows.

#### Microsoft Active Protections Program (MAPP)

W celu zwiększenia poziomu bezpieczeństwa swoich klientów firma Microsoft dostarcza informacje na temat luk w zabezpieczeniach największym dostawcom oprogramowania zabezpieczającego przed publikacją comiesięcznej aktualizacji zabezpieczeń. Dzięki informacjom dotyczącym luk w zabezpieczeniach dostawcy oprogramowania zabezpieczającego mogą zaoferować swoim klientom zaktualizowane poprawki za pośrednictwem programów lub urządzeń zabezpieczających np. programów antywirusowych, sieciowych systemów wykrywania włamań lub hostowych systemów zapobiegania włamaniom. Aby sprawdzić, czy dostawcy oprogramowania zabezpieczającego zapewniają aktywną ochronę, odwiedź witryny poszczególnych partnerów programu, których listę znaleźć można w sekcji [Microsoft Active Protections Program (MAPP) Partners](http://www.microsoft.com/security/msrc/mapp/partners.mspx).

#### Strategie i społeczność związane z zabezpieczeniami

**Strategie zarządzania aktualizacjami**

Na stronie [Security Guidance for Update Management](http://go.microsoft.com/fwlink/?linkid=21168) (Wskazówki z zakresu bezpieczeństwa dotyczące zarządzania aktualizacjami) znajdują się dodatkowe informacje o zalecanych przez firmę Microsoft najlepszych sposobach stosowania aktualizacji zabezpieczeń.

**Uzyskiwanie innych aktualizacji zabezpieczeń**

Aktualizacje dotyczące innych problemów związanych z zabezpieczeniami można uzyskać w następujących lokalizacjach:

-   Aktualizacje zabezpieczeń są dostępne w witrynie [Centrum pobierania Microsoft](http://go.microsoft.com/fwlink/?linkid=21129). Najłatwiej je znaleźć, wyszukując wyrażenie „aktualizacja zabezpieczeń”.
-   Aktualizacje dla poszczególnych platform są dostępne w [witrynie sieci Web Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747).
-   Aktualizacje zabezpieczeń dostępne w tym miesiącu w witrynie Windows Update można otrzymać w witrynie Centrum pobierania Microsoft w postaci plików obrazu dysku CD zawierającego zabezpieczenia i aktualizacje krytyczne. Więcej informacji na ten temat można znaleźć w [artykule 913086 bazy wiedzy Microsoft Knowledge Base](http://support.microsoft.com/kb/913086).

**Społeczność IT Pro Security Community**

Dowiedz się, jak poprawić bezpieczeństwo i zoptymalizować infrastrukturę informatyczną oraz weź udział w dyskusjach dotyczących zabezpieczeń wraz z innymi specjalistami branży IT, odwiedzając witrynę sieci Web społeczności [IT Pro Security Community](http://go.microsoft.com/fwlink/?linkid=21164) (jęz. ang.).

#### Podziękowania

Firma Microsoft [dziękuje](http://go.microsoft.com/fwlink/?linkid=21127) wymienionym poniżej organizacjom i osobom za współpracę w dziedzinie ochrony klientów:

-   Anonimowy analityk współpracujący z [TippingPoint's](http://www.tippingpoint.com/) [Zero Day Initiative](http://www.zerodayinitiative.com/), za zgłoszenie problemu opisanego w biuletynie MS10-087
-   [team509](http://www.team509.com/), we współpracy z firmą [Verisign iDefense Labs](http://labs.idefense.com/), za zgłoszenie problemu opisanego w biuletynie MS10-087
-   Dyon Balding z firmy [Secunia](http://secunia.com/), za zgłoszenie problemu opisanego w biuletynie MS10-087
-   Will Dorman z firmy [CERT Coordination Center](http://www.cert.org/), za zgłoszenie problemu opisanego w biuletynie MS10-087
-   [TippingPoint's](http://www.tippingpoint.com/) [Zero Day Initiative](http://www.zerodayinitiative.com/), za zgłoszenie problemu opisanego w biuletynie MS10-087
-   Chaouki Bekrar z firmy [VUPEN Vulnerability Research Team](http://www.vupen.com/), za zgłoszenie problemu opisanego w biuletynie MS10-087
-   Haifei Li z [FortiGuard Labs firmy Fortinet](http://www.fortiguard.com/), za zgłoszenie problemu opisanego w biuletynie MS10-087
-   Simon Raner z firmy [ACROS Security](http://www.acrossecurity.com), za zgłoszenie problemu opisanego w biuletynie MS10-087
-   Alin Rad Pop z firmy [Secunia Research](http://secunia.com/), za zgłoszenie problemu opisanego w biuletynie MS10-088
-   Anonimowy analityk współpracujący z [TippingPoint's](http://www.tippingpoint.com/) [Zero Day Initiative](http://www.zerodayinitiative.com/), za zgłoszenie problemu opisanego w biuletynie MS10-088
-   Eyal Gruner z firmy [BugSec](http://www.bugsec.com/) za współpracę przy rozwiązywaniu trzech problemów opisanych w biuletynie MS10-089

#### Pomoc techniczna

-   Wymienione oprogramowanie zostało przetestowane w celu ustalenia, których wersji dotyczy problem. Dla pozostałych wersji upłynął okres pomocy technicznej. Aby zapoznać się z zasadami cyklu pomocy technicznej dotyczącymi używanej wersji oprogramowania, odwiedź [witrynę zasad cyklu pomocy technicznej firmy Microsoft](http://go.microsoft.com/fwlink/?linkid=21742).
-   Klienci mogą uzyskać pomoc techniczną w [Biurze Obsługi Klienta Microsoft](http://go.microsoft.com/fwlink/?linkid=21131) pod numerem 0 801 802 000 (opłata według stawek Twojego operatora) lub (0-22) 594 19 99 w godzinach od 9:00 do 17:00, od poniedziałku do piątku. Połączenia z działem pomocy technicznej związane z aktualizacjami zabezpieczeń są bezpłatne. Dodatkowe informacje dotyczące możliwości skorzystania z pomocy technicznej można znaleźć w witrynie [Pomoc i obsługa techniczna firmy Microsoft](http://support.microsoft.com/).
-   Klienci międzynarodowi mogą uzyskać pomoc w lokalnych przedstawicielstwach firmy Microsoft. Pomoc techniczna związana z aktualizacjami zabezpieczeń jest bezpłatna. Informacje o sposobie kontaktowania się z pomocą techniczną firmy Microsoft są dostępne w [międzynarodowej witrynie sieci Web pomocy i obsługi technicznej](http://go.microsoft.com/fwlink/?linkid=21155).

#### Zrzeczenie odpowiedzialności

Informacje w bazie wiedzy Microsoft Knowledge Base są dostarczane „tak jak są” bez jakiejkolwiek gwarancji. Firma Microsoft odrzuca wszelkie gwarancje, wyraźne i dorozumiane, w tym gwarancje dotyczące wartości handlowej i przydatności do określonego celu. Firma Microsoft Corporation ani jej dostawcy w żadnym wypadku nie ponoszą odpowiedzialności za jakiekolwiek szkody, w tym bezpośrednie, pośrednie, przypadkowe, wynikowe, utratę zysków handlowych lub szkody specjalne, nawet jeżeli firmę Microsoft Corporation lub jej dostawców powiadomiono o możliwości zaistnienia takich szkód. W niektórych stanach wyłączenie lub ograniczenie odpowiedzialności za straty wynikowe lub przypadkowe, a więc i powyższe ograniczenia, nie mają zastosowania.

#### Wersje

-   Wersja 1.0 (9 listopada 2010 r.): Opublikowane podsumowanie biuletynów zabezpieczeń.
-   Wersja 1.1 (9 listopada 2010 r.): W odniesieniu do biuletynu MS10-088 poprawiono nazwę wersji, której dotyczy problem, z „Podgląd programu Microsoft PowerPoint” na „Podgląd programu Microsoft PowerPoint 2007 z dodatkiem Service Pack 2”. Zmiana ta ma wyłącznie charakter informacyjny. Klienci, którym udało się zaktualizować swoje systemy, włącznie z klientami z włączoną funkcję automatycznych aktualizacji, nie muszą podejmować żadnej czynności. Klienci, którzy nie zainstalowali wcześniej tej aktualizacji, mogą dokonać ponownej oceny, czy ich systemy wymagają aktualizacji, opierając się na poprawionej tabeli programów, których dotyczy problem.
-   Wersja 1.2 (17 listopada 2010 r.): W biuletynie MS10-087 poprawiono Wskaźnik możliwości wykorzystania luki, aby dodać lukę CVE-2010-2573 do wykazu luk, których dotyczy ta aktualizacja. Zmiana ta ma wyłącznie charakter informacyjny.
-   Wersja 2.0 (15 grudnia 2010 r.): Niniejsze podsumowanie biuletynów zaktualizowano w celu poinformowania o dostępności aktualizacji zabezpieczeń dla pakietu Microsoft Office 2008 dla komputerów Macintosh (KB2476512) i programu Open XML File Format Converter dla komputerów Macintosh (KB2476511), usuwających luki w zabezpieczeniach opisane w biuletynie MS10-087. Firma Microsoft zaleca użytkownikom tych programów jak najszybszą instalację tych aktualizacji.
-   Wersja 2.1 (13 kwietnia 2011 r.): Zaktualizowano ten biuletyn, aby poinformować o dostępności aktualizacji zabezpieczeń dla pakietu Microsoft Office 2004 dla komputerów Macintosh (KB2505924). Aby uzyskać szczegółowe informacje, zobacz biuletyny MS10-087 i MS10-088.

*Built at 2014-04-18T01:50:00Z-07:00*
