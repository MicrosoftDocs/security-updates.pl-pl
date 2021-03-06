---
TOCTitle: 'MS10-JAN'
Title: 'Podsumowanie biuletynów zabezpieczeń firmy Microsoft za styczeń 2010 r.'
ms:assetid: 'ms10-jan'
ms:contentKeyID: 61233112
ms:mtpsurl: 'https://technet.microsoft.com/pl-PL/library/ms10-jan(v=Security.10)'
---
Podsumowanie biuletynów zabezpieczeń firmy Microsoft za styczeń 2010 r.
=======================================================================

Opublikowano: 12 stycznia 2010 | Zaktualizowano: 21 stycznia 2010

**Wersja:** 2.0

Niniejsze podsumowanie biuletynów zabezpieczeń zawiera spis biuletynów za styczeń 2010 r.

Z chwilą opublikowania biuletynów za styczeń 2010 r. niniejsze podsumowanie biuletynów zastępuje powiadomienie o biuletynach zabezpieczeń wydane 20 stycznia 2010 r. Aby uzyskać więcej informacji na temat usługi powiadamiania o biuletynach, zobacz [Powiadomienia o biuletynach zabezpieczeń firmy Microsoft (jęz. ang.)](http://technet.microsoft.com/security/bulletin/advance).

Aby dowiedzieć się, jak otrzymywać automatyczne powiadomienia o publikacji biuletynów zabezpieczeń firmy Microsoft, odwiedź stronę [Microsoft Technical Security Notifications](http://go.microsoft.com/fwlink/?linkid=21163).

13 stycznia 2010 r. o godz. 11:00 czasu Pacyfiku (godz. 20:00 czasu środkowoeuropejskiego) firma Microsoft udostępni emisję internetową, w której znajdą się odpowiedzi na pytania klientów dotyczące tych biuletynów (USA i Kanada). [Zarejestruj się, aby zobaczyć emisję internetową dotyczącą biuletynów zabezpieczeń za styczeń](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032427677&eventcategory=4&culture=en-us&countrycode=us). Po tym dniu emisja internetowa będzie dostępna na żądanie. Aby uzyskać więcej informacji, zobacz [Podsumowania biuletynów zabezpieczeń i emisje internetowe firmy Microsoft](http://technet.microsoft.com/security/bulletin/summary).

W odniesieniu do pozaplanowych biuletynów zabezpieczeń, MS10-002, dodanych do wersji 2.0 niniejszego podsumowania biuletynów, 21 stycznia 2010 r. o godz. 13:00 czasu Pacyfiku (godz. 22:00 czasu środkowoeuropejskiego) firma Microsoft udostępni transmisję internetową, zawierającą odpowiedzi na pytania klientów dotyczące tych biuletynów (USA i Kanada). [Zarejestruj się teraz, by wziąć udział w transmisji internetowej 21 stycznia, 22:00](http://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032440627&culture=en-us). Po tym dniu emisja internetowa będzie dostępna na żądanie. Aby uzyskać więcej informacji, zobacz [Podsumowania biuletynów zabezpieczeń i emisje internetowe firmy Microsoft](http://technet.microsoft.com/security/bulletin/summary).

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=169348">MS10-001</a></td>
<td style="border:1px solid black;"><strong>Luka w zabezpieczeniach aparatu osadzonych czcionek OpenType umożliwia zdalne wykonanie kodu (972270)</strong><br />
<br />
Ta aktualizacja zabezpieczeń usuwa lukę w zabezpieczeniach systemu Microsoft Windows. Luka w zabezpieczeniach umożliwia zdalne wykonanie kodu, jeśli użytkownik wyświetli treść zawierającą specjalnie spreparowaną osadzoną czcionkę OpenType (EOT) w aplikacjach klienckich z obsługą czcionek EOT, takich jak Microsoft Internet Explorer, Microsoft Office PowerPoint lub Microsoft Office Word. Osoba atakująca, której uda się wykorzystać tę lukę, może uzyskać pełną kontrolę nad systemem, którego dotyczy luka. Osoba taka może wówczas instalować programy, przeglądać, zmieniać i usuwać dane oraz tworzyć nowe konta z pełnymi uprawnieniami. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Krytyczny</a><br />
Zdalne wykonanie kodu</td>
<td style="border:1px solid black;">Może wymagać ponownego uruchomienia</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=179104">MS10-002</a></td>
<td style="border:1px solid black;"><strong>Zbiorcza aktualizacja zabezpieczeń dla programu Internet Explorer (978207)</strong><br />
<br />
Ta aktualizacja zabezpieczeń usuwa siedem luk w zabezpieczeniach programu Internet Explorer zgłoszonych przez użytkowników i jedną lukę w zabezpieczeniach programu Internet Explorer zgłoszoną przez organizacje publiczne. Najpoważniejsza z tych luk umożliwia zdalne wykonanie kodu, jeśli użytkownik wyświetli specjalnie spreparowaną stronę sieci Web przy użyciu programu Internet Explorer. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Krytyczny</a><br />
Zdalne wykonanie kodu</td>
<td style="border:1px solid black;">Wymaga ponownego uruchomienia komputera</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
</tbody>
</table>
  
Wskaźnik możliwości wykorzystania luki  
--------------------------------------
  
<span></span>
Poniższa tabela przedstawia ocenę możliwości wykorzystania luk dla każdej luki opisywanej w tym miesiącu. Luki są wymienione wg identyfikatora biuletynu i identyfikatora CVE.
  
**W jaki sposób korzystać z tej tabeli?**
  
Tabela ta pozwala sprawdzić prawdopodobieństwo, że w ciągu 30 dni od wydania biuletynu zabezpieczeń dla każdej z aktualizacji zabezpieczeń, których zainstalowanie może być potrzebne, opublikowany zostanie działający kod wykorzystujący lukę w zabezpieczeniach. Aby ustalić priorytety wdrażania, zapoznaj się z dostępnymi poniżej ocenami, rozpatrując je w kontekście posiadanej konfiguracji. Więcej informacji na temat znaczenia tych ocen oraz sposobu ich wyznaczania można znaleźć na stronie sieci Web [Microsoft Exploitability Index](http://technet.microsoft.com/en-us/security/cc998259.aspx).
  
| Identyfikator biuletynu                                   | Nazwa luki w zabezpieczeniach                                                                                                 | CVE ID                                                                           | Ocena wskaźnika możliwości wykorzystania luki                                                                        | Najważniejsze uwagi                                                                                                                                                                                 |  
|-----------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| [MS10-001](http://go.microsoft.com/fwlink/?linkid=169348) | Luka w zabezpieczeniach związana z błędem liczby całkowitej czcionek skompresowanych Microtype Express w dekompresorze LZCOMP | [CVE-2010-0018](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0018) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny niespójny kod wykorzystujący lukę | Ta ocena wskaźnika możliwości wykorzystania luki dotyczy komputerów z systemem Microsoft Windows 2000. Wykorzystanie luki na komputerach z systemem Windows XP lub nowszym jest mało prawdopodobne. |  
| [MS10-002](http://go.microsoft.com/fwlink/?linkid=179104) | Luka związana z obsługą skryptów filtru XSS                                                                                   | [CVE-2009-4074](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-4074) | Brak                                                                                                                 | Nie jest możliwe wykonanie kodu przy użyciu tej luki.                                                                                                                                               |  
| [MS10-002](http://go.microsoft.com/fwlink/?linkid=179104) | Luka związana ze sprawdzaniem poprawności adresu URL                                                                          | [CVE-2010-0027](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0027) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny spójny kod wykorzystujący lukę    | (Brak)                                                                                                                                                                                              |  
| [MS10-002](http://go.microsoft.com/fwlink/?linkid=179104) | Luka w zabezpieczeniach związana z uszkodzeniem niezainicjowanej pamięci                                                      | [CVE-2010-0244](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0244) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny spójny kod wykorzystujący lukę    | (Brak)                                                                                                                                                                                              |  
| [MS10-002](http://go.microsoft.com/fwlink/?linkid=179104) | Luka w zabezpieczeniach związana z uszkodzeniem niezainicjowanej pamięci                                                      | [CVE-2010-0245](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0245) | Brak                                                                                                                 | Klienci, którzy zastosowali poprawkę [MS09-072](http://go.microsoft.com/fwlink/?linkid=169404), są chronieni. Przedstawiona luka jest blokowana przez zmiany wprowadzone w poprawce MS09-072.       |  
| [MS10-002](http://go.microsoft.com/fwlink/?linkid=179104) | Luka w zabezpieczeniach związana z uszkodzeniem niezainicjowanej pamięci                                                      | [CVE-2010-0246](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0246) | Brak                                                                                                                 | Klienci, którzy zastosowali poprawkę [MS09-072](http://go.microsoft.com/fwlink/?linkid=169404), są chronieni. Przedstawiona luka jest blokowana przez zmiany wprowadzone w poprawce MS09-072.       |  
| [MS10-002](http://go.microsoft.com/fwlink/?linkid=179104) | Luka w zabezpieczeniach związana z uszkodzeniem niezainicjowanej pamięci                                                      | [CVE-2010-0247](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0247) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny spójny kod wykorzystujący lukę    | (Brak)                                                                                                                                                                                              |  
| [MS10-002](http://go.microsoft.com/fwlink/?linkid=179104) | Luka w zabezpieczeniach związana z uszkodzeniem pamięci obiektu HTML                                                          | [CVE-2010-0248](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0248) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny niespójny kod wykorzystujący lukę | (Brak)                                                                                                                                                                                              |  
| [MS10-002](http://go.microsoft.com/fwlink/?linkid=179104) | Luka w zabezpieczeniach związana z uszkodzeniem pamięci obiektu HTML                                                          | [CVE-2010-0249](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0249) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny spójny kod wykorzystujący lukę    | **Ta luka w zabezpieczeniach jest aktualnie wykorzystywana w Internecie.**                                                                                                                          |
  
Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki  
---------------------------------------------------------------------------------
  
<span></span>
Poniższe tabele wymieniają biuletyny według najważniejszych kategorii programów i wskaźnika ważności.
  
**Jak korzystać z tych tabel?**
  
Tabele te pozwalają odczytać informacje o aktualizacjach zabezpieczeń, których zainstalowanie może być konieczne. Należy zapoznać się z informacjami dotyczącymi każdego wymienionego programu lub składnika oprogramowania w celu sprawdzenia, czy aktualizacje zabezpieczeń odnoszą się do danej instalacji. Jeśli program lub składnik znajduje się na liście, dostępne jest łącze prowadzące do aktualizacji oprogramowania i podana jest informacja o wskaźniku ważności tej aktualizacji.
  
**Uwaga** Konieczne może być zainstalowanie kilku aktualizacji zabezpieczeń dotyczących jednej luki. Przejrzyj całą kolumnę dla każdego wymienionego identyfikatora biuletynu, aby sprawdzić, jakie aktualizacje musisz zainstalować, w oparciu o programy bądź składniki zainstalowane w systemie.
  
#### System operacyjny Windows i jego składniki:

 
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
Microsoft Windows 2000  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS10-001**](http://go.microsoft.com/fwlink/?linkid=169348)
</td>
<td style="border:1px solid black;">
[**MS10-002**](http://go.microsoft.com/fwlink/?linkid=179104)
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
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 z dodatkiem Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 z dodatkiem Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=47f85cbd-282e-4c92-9809-68bba49e0a12)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Internet Explorer 5.01 z dodatkiem Service Pack 4 w systemie Microsoft Windows 2000 z dodatkiem Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=51e99e4f-1670-4b12-a9fe-e0ccf50cdabc)  
(Krytyczny)  
[Internet Explorer 6 z dodatkiem Service Pack 1 zainstalowany w systemie Microsoft Windows 2000 z dodatkiem Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=a38aa9d0-c3fe-4d41-8805-7d5370263c1b)  
(Krytyczny)
</td>
</tr>
<tr>
<th colspan="3">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS10-001**](http://go.microsoft.com/fwlink/?linkid=169348)
</td>
<td style="border:1px solid black;">
[**MS10-002**](http://go.microsoft.com/fwlink/?linkid=179104)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Zbiorczy wskaźnik ważności**
</td>
<td style="border:1px solid black;">
[**Niski**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Krytyczny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP z dodatkiem Service Pack 2 i Windows XP z dodatkiem Service Pack 3
</td>
<td style="border:1px solid black;">
[Windows XP z dodatkiem Service Pack 2 i Windows XP z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=793a6b3f-7660-40be-b7d5-7b0eec55e1cd)  
(Niski)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6 dla systemów Windows XP z dodatkiem Service Pack 2 i Windows XP z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=207eecad-6e84-48e6-ae18-6794a3618ee0)  
(Krytyczny)  
[Internet Explorer 7 dla systemów Windows XP z dodatkiem Service Pack 2 i Windows XP z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=3510c7d8-7e8f-479e-b6f9-5745a845664d)  
(Krytyczny)  
[Internet Explorer 8 dla systemów Windows XP z dodatkiem Service Pack 2 i Windows XP z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=7c2948fb-f486-4801-bc21-bbf40d5a78c2)  
(Krytyczny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=31609ce9-656a-4f7d-a501-709a31ca34c3)  
(Niski)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6 dla Windows XP Professional x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=eb2d8055-4d50-4f83-82b8-055c7b8f5422)  
(Krytyczny)  
[Internet Explorer 7 dla Windows XP Professional x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=cc5aea0b-e553-4f7f-a2cc-cba41bb87ae7)  
(Krytyczny)  
[Internet Explorer 8 dla Windows XP Professional x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=41b83fad-948b-4a9c-80ed-9c5a60bd35b4)  
(Krytyczny)
</td>
</tr>
<tr>
<th colspan="3">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS10-001**](http://go.microsoft.com/fwlink/?linkid=169348)
</td>
<td style="border:1px solid black;">
[**MS10-002**](http://go.microsoft.com/fwlink/?linkid=179104)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Zbiorczy wskaźnik ważności**
</td>
<td style="border:1px solid black;">
[**Niski**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Krytyczny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e1d6e338-dea9-458e-b35d-796e069d74d7)  
(Niski)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6 dla systemu Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fea91227-44ad-4549-8732-497a8ceff870)  
(Umiarkowany)  
[Internet Explorer 7 dla systemu Windows Server 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=14726445-3ff4-463c-9fc1-c9b758079aca)  
(Krytyczny)  
[Internet Explorer 8 dla systemu Windows Server 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7d480c87-2ca9-4505-a59d-a6d73d001fa5)  
(Krytyczny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ddbcf231-9fde-4dc2-ad04-a01b69d1a980)  
(Niski)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6 dla systemu Windows Server 2003 x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=633e63f4-605b-43c4-8a4b-2730312a1c72)  
(Umiarkowany)  
[Internet Explorer 7 dla systemu Windows Server 2003 x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c8742230-16d8-4b2f-bd3e-8834c759856b)  
(Krytyczny)  
[Internet Explorer 8 dla systemu Windows Server 2003 x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3e2e740b-8417-4758-8468-15221249ec71)  
(Krytyczny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=c71a13cf-7e2f-4b02-8684-1a4e4b46ddda)  
(Niski)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6 dla systemu Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=b9308d50-ca66-43ff-9dc5-d05c90baa764)  
(Umiarkowany)  
[Internet Explorer 7 dla systemu Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=5622f223-df9c-4a6a-bdf0-feebaf9920fd)  
(Krytyczny)
</td>
</tr>
<tr>
<th colspan="3">
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS10-001**](http://go.microsoft.com/fwlink/?linkid=169348)
</td>
<td style="border:1px solid black;">
[**MS10-002**](http://go.microsoft.com/fwlink/?linkid=179104)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Zbiorczy wskaźnik ważności**
</td>
<td style="border:1px solid black;">
[**Niski**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Krytyczny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista, Windows Vista z dodatkiem Service Pack 1 i Windows Vista z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista z dodatkiem Service Pack 1 i Windows Vista z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6387228c-eedc-4511-b3c6-8922606f4c84)  
(Niski)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7 w systemie Windows Vista, Windows Vista z dodatkiem Service Pack 1 i Windows Vista z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=92495551-dedd-43d4-bb3a-51028bc5c6d6)  
(Krytyczny)  
[Internet Explorer 8 w systemie Windows Vista, Windows Vista z dodatkiem Service Pack 1 i Windows Vista z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5e2cbd7d-f64f-49e5-a159-1965ebfe2a92)  
(Krytyczny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition, Windows Vista x64 Edition z dodatkiem Service Pack 1 i Windows Vista x64 Edition z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition z dodatkiem Service Pack 1 i Windows Vista x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7b4f5089-13b1-421b-a00b-22632bba4229)  
(Niski)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7 w systemie Windows Vista x64 Edition, Windows Vista x64 Edition z dodatkiem Service Pack 1 i Windows Vista x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3cb139b3-59f4-44ef-9911-4dd4e3b83e7d)  
(Krytyczny)  
[Internet Explorer 8 w systemie Windows Vista x64 Edition, Windows Vista x64 Edition z dodatkiem Service Pack 1 i Windows Vista x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b7a7e8e7-f4c5-459d-ab6c-05a192e1e3f9)  
(Krytyczny)
</td>
</tr>
<tr>
<th colspan="3">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS10-001**](http://go.microsoft.com/fwlink/?linkid=169348)
</td>
<td style="border:1px solid black;">
[**MS10-002**](http://go.microsoft.com/fwlink/?linkid=179104)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Zbiorczy wskaźnik ważności**
</td>
<td style="border:1px solid black;">
[**Niski**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Krytyczny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 dla systemów 32-bitowych i Windows Server 2008 z dodatkiem Service Pack 2 dla systemów 32-bitowych
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów 32-bitowych i Windows Server 2008 z dodatkiem Service Pack 2 dla systemów 32-bitowych](http://www.microsoft.com/downloads/details.aspx?familyid=e175c436-37e0-497f-8b7f-6cacaa25ad7c)\*\*  
(Niski)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7 w systemie Windows Server 2008 w wersji 32-bitowej oraz Windows Server 2008 dla systemów 32-bitowych z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8c4c91ec-1b2b-4176-bd77-45245b590329)\*\*  
(Krytyczny)  
[Internet Explorer 8 w systemie Windows Server 2008 w wersji 32-bitowej oraz Windows Server 2008 dla systemów 32-bitowych z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f5ce8582-af63-4870-bee3-0abeeefa1458)\*\*  
(Krytyczny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 dla systemów z procesorem x64 i Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem x64
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem x64 i Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=1b10a177-fd45-406f-8edc-b8d4b84881b7)\*\*  
(Niski)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7 w systemie Windows Server 2008 dla systemów z procesorem x64 oraz Windows Server 2008 dla systemów z procesorem x64 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4f9975b8-3f91-4116-9200-ef55ece75854)\*\*  
(Krytyczny)  
[Internet Explorer 8 w systemie Windows Server 2008 dla systemów z procesorem x64 oraz Windows Server 2008 dla systemów z procesorem x64 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=be11981c-d286-4e3c-94bf-d4e67a975d5a)\*\*  
(Krytyczny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 dla systemów z procesorem Itanium i Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem Itanium
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem Itanium i Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=e8bc9a24-a794-4827-a6bb-785c6b2189f4)  
(Niski)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7 w systemie Windows Server 2008 dla systemów z procesorem Itanium i Windows Server 2008 dla systemów z procesorem Itanium z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9395547f-b620-4cbd-9ff5-11b76cd73859)  
(Krytyczny)
</td>
</tr>
<tr>
<th colspan="3">
Windows 7
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS10-001**](http://go.microsoft.com/fwlink/?linkid=169348)
</td>
<td style="border:1px solid black;">
[**MS10-002**](http://go.microsoft.com/fwlink/?linkid=179104)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Zbiorczy wskaźnik ważności**
</td>
<td style="border:1px solid black;">
[**Niski**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Krytyczny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 dla systemów 32-bitowych
</td>
<td style="border:1px solid black;">
[Windows 7 dla systemów 32-bitowych](http://www.microsoft.com/downloads/details.aspx?familyid=75491ad0-40a6-4efb-9574-d82210f6d0da)  
(Niski)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8 w systemie Windows 7 dla systemów 32-bitowych](http://www.microsoft.com/downloads/details.aspx?familyid=278443c1-15dc-436b-893b-ffea6d29d16d)  
(Krytyczny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 dla systemów z procesorem x64
</td>
<td style="border:1px solid black;">
[Windows 7 dla systemów z procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=8a53f0e9-0616-440e-90f2-a12524e1bee4)  
(Niski)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8 w systemie Windows 7 dla systemów opartych na procesorach x64](http://www.microsoft.com/downloads/details.aspx?familyid=a584cd0f-2e05-4e36-8858-0ffead637162)  
(Krytyczny)
</td>
</tr>
<tr>
<th colspan="3">
System Windows Server 2008 R2
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS10-001**](http://go.microsoft.com/fwlink/?linkid=169348)
</td>
<td style="border:1px solid black;">
[**MS10-002**](http://go.microsoft.com/fwlink/?linkid=179104)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Zbiorczy wskaźnik ważności**
</td>
<td style="border:1px solid black;">
[**Niski**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Krytyczny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 dla systemów opartych na procesorach x64
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach x64](http://www.microsoft.com/downloads/details.aspx?familyid=308166e4-571b-4d6c-bd9f-3ed4afa4eafe)\*\*  
(Niski)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8 w systemie Windows Server 2008 R2 dla systemów opartych na procesorach x64](http://www.microsoft.com/downloads/details.aspx?familyid=d3386793-a594-4bc5-8308-28b561d43087)\*\*  
(Krytyczny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 dla systemów opartych na procesorach Itanium
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=1d0da42b-9755-4fd2-afd1-0d023d187133)  
(Niski)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8 w systemie Windows Server 2008 R2 dla systemów opartych na procesorach Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=9d137bab-8312-4240-af74-c65ba652fde0)  
(Krytyczny)
</td>
</tr>
</table>
 
**Uwagi dotyczące systemu Windows Server 2008 i Windows Server 2008 R2**

**\*\*Luka w zabezpieczeniach nie dotyczy instalacji Server Core.** Luki usuwane przez tę aktualizację zabezpieczeń nie dotyczą obsługiwanych wersji systemu Windows Server 2008 ani Windows Server 2008 R2, jeżeli systemy te zostały zainstalowane przy użyciu opcji instalacji Server Core. Aby uzyskać więcej informacji na temat tej opcji instalacji, zobacz artykuły MSDN, [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx) (j. ang.) i [Server Core for Windows Server 2008 R2](http://msdn.microsoft.com/en-us/library/ee391631(vs.85).aspx) (j. ang.). Należy pamiętać, że opcja instalacji Server Core nie dotyczy niektórych wersji systemu Windows Server 2008 i Windows Server 2008 R2. Zobacz [Porównanie opcji instalacji Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

Narzędzia wykrywania i wdrażania oraz wskazówki
-----------------------------------------------

<span></span>
**Centrum zabezpieczeń**

Zarządzanie oprogramowaniem oraz aktualizacjami zabezpieczeń, które należy zainstalować na serwerach oraz komputerach stacjonarnych i przenośnych w organizacji. Więcej informacji można znaleźć w [Centrum TechNet Update Management Center](http://go.microsoft.com/fwlink/?linkid=69903). Witryna [TechNet Security Center](http://go.microsoft.com/fwlink/?linkid=21171) zawiera dodatkowe informacje na temat zabezpieczeń w produktach firmy Microsoft. Użytkownicy mogą także uzyskać dostęp do tych informacji w witrynie [Bezpieczeństwo w domu](http://go.microsoft.com/fwlink/?linkid=85102), klikając łącze „Najnowsze aktualizacje zabezpieczeń”.

Aktualizacje zabezpieczeń dostępne są w witrynach [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747) i [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130). Aktualizacje zabezpieczeń są także dostępne w witrynie [Microsoft Download Center](http://go.microsoft.com/fwlink/?linkid=21129). Najłatwiej je znaleźć, wyszukując wyrażenie „aktualizacja zabezpieczeń”.

Aktualizacje zabezpieczeń można także pobierać z [Wykazu usługi Microsoft Update](http://go.microsoft.com/fwlink/?linkid=96155). Wykaz usługi Microsoft Update zawiera katalog zawartości z możliwością przeszukiwania, który udostępniany jest poprzez usługi Windows Update i Microsoft Update i obejmuje aktualizacje zabezpieczeń, sterowniki i dodatki Service Pack. Wyszukiwanie przy użyciu numeru biuletynu zabezpieczeń (np. „MS07-036”) pozwala dodać do koszyka wszystkie odpowiednie aktualizacje (w tym różne wersje językowe aktualizacji) i pobrać pliki do wybranego folderu. Więcej informacji na temat Wykazu usługi Microsoft Update można znaleźć w [Często zadawanych pytaniach dotyczących Wykazu usługi Microsoft Update](http://go.microsoft.com/fwlink/?linkid=97900).

**Uwaga** Dnia 1 sierpnia 2009 r. firma Microsoft zakończyła świadczenie pomocy technicznej dla usługi Office Update oraz narzędzia Office Update Inventory Tool. Aby w dalszym ciągu otrzymywać najnowsze aktualizacje dla produktów Microsoft Office, skorzystaj z witryny [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747). Aby uzyskać więcej informacji, zobacz artykuł [Informacje o witrynie Microsoft Office Update: Często zadawane pytania](http://office.microsoft.com/en-us/downloads/fx010402221033.aspx).

**Porady dotyczące wykrywania i wdrażania**

Firma Microsoft udziela porad dotyczących wykrywania i wdrażania aktualizacji zabezpieczeń. Porady takie zawierają zalecenia i informacje ułatwiające specjalistom IT poznanie obsługi różnych narzędzi do wykrywania i wdrażania aktualizacji zabezpieczeń. Więcej informacji na ten temat można znaleźć w [artykule 961747 bazy wiedzy Microsoft Knowledge Base](http://support.microsoft.com/kb/961747/pl).

**Narzędzie Microsoft Baseline Security Analyzer (MBSA)**

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

Firma Microsoft opublikowała zaktualizowaną wersję narzędzia Microsoft Windows Malicious Software Removal Tool, która dostępna jest w witrynach sieci Web Windows Update i Microsoft Update, poprzez usługi Windows Server Update Services i w witrynie Microsoft Download Center.

#### Aktualizacje o wysokim priorytecie niezwiązane z zabezpieczeniami, dostępne w witrynach MU, WU oraz usługach WSUS

Aby uzyskać informacje na temat publikacji niezwiązanych z zabezpieczeniami, dostępnych w witrynach Windows Update i Microsoft Update, zobacz:

-   [Artykuł 894199 bazy wiedzy Microsoft Knowledge Base](http://support.microsoft.com/kb/894199/pl): Opis zmian zawartości Usług aktualizacji oprogramowania i usług Windows Server Update Services. Zawiera wszystkie treści dotyczące systemu Windows.
-   [Aktualizacje z poprzednich miesięcy dla usług Windows Server Update Services](http://technet.microsoft.com/en-us/wsus/bb456965.aspx). Wyświetla nowe, zmienione i opublikowane ponownie aktualizacje dla produktów firmy Microsoft innych niż Microsoft Windows.

#### Microsoft Active Protections Program (MAPP)

W celu zwiększenia poziomu bezpieczeństwa swoich klientów firma Microsoft dostarcza informacje na temat luk w zabezpieczeniach największym dostawcom oprogramowania zabezpieczającego przed publikacją comiesięcznej aktualizacji zabezpieczeń. Dzięki informacjom dotyczącym luk w zabezpieczeniach dostawcy oprogramowania zabezpieczającego mogą zaoferować swoim klientom zaktualizowane poprawki za pośrednictwem programów lub urządzeń zabezpieczających np. programów antywirusowych, sieciowych systemów wykrywania włamań lub hostowych systemów zapobiegania włamaniom. Aby sprawdzić, czy dostawcy oprogramowania zabezpieczającego zapewniają aktywną ochronę, odwiedź witryny poszczególnych partnerów programu, których listę znaleźć można w sekcji [Microsoft Active Protections Program (MAPP) Partners](http://www.microsoft.com/security/msrc/mapp/partners.mspx).

#### Strategie i społeczność związane z zabezpieczeniami

**Strategie zarządzania aktualizacjami**

Na stronie [Security Guidance for Update Management](http://go.microsoft.com/fwlink/?linkid=21168) (Wskazówki z zakresu bezpieczeństwa dotyczące zarządzania aktualizacjami) znajdują się dodatkowe informacje o zalecanych przez firmę Microsoft najlepszych sposobach stosowania aktualizacji zabezpieczeń.

**Uzyskiwanie innych aktualizacji zabezpieczeń**

Aktualizacje dotyczące innych problemów związanych z zabezpieczeniami można uzyskać w następujących lokalizacjach:

-   Aktualizacje zabezpieczeń są dostępne w witrynie [Microsoft Download Center](http://go.microsoft.com/fwlink/?linkid=21129). Najłatwiej je znaleźć, wyszukując wyrażenie „aktualizacja zabezpieczeń”.
-   Aktualizacje dla poszczególnych platform są dostępne w [witrynie sieci Web Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747).
-   Aktualizacje zabezpieczeń dostępne w tym miesiącu w witrynie Windows Update można otrzymać w witrynie Microsoft Download Center w postaci plików obrazu dysku CD zawierającego zabezpieczenia i aktualizacje krytyczne. Więcej informacji na ten temat można znaleźć w [artykule 913086 bazy wiedzy Microsoft Knowledge Base](http://support.microsoft.com/kb/913086/pl).

**Społeczność IT Pro Security Community**

Dowiedz się, jak poprawić bezpieczeństwo i zoptymalizować infrastrukturę informatyczną oraz weź udział w dyskusjach dotyczących zabezpieczeń wraz z innymi specjalistami branży IT, odwiedzając witrynę sieci Web społeczności [IT Pro Security Community](http://go.microsoft.com/fwlink/?linkid=21164) (jęz. ang.).

#### Podziękowania

Firma Microsoft [dziękuje](http://go.microsoft.com/fwlink/?linkid=21127) wymienionym poniżej organizacjom i osobom za współpracę w dziedzinie ochrony klientów:

-   Tavis Ormandy z firmy [Google Inc.](http://www.google.com/) za zgłoszenie problemu opisanego w biuletynie MS10-001
-   [David Lindsay „thornmaker”](http://p42.us/) i [Eduardo A. Vela Nava „sirdarckcat”](http://www.sirdarckcat.net/) za zgłoszenie problemu opisanego w biuletynie MS10-002
-   Lostmon Lords za zgłoszenie problemu opisanego w biuletynie MS10-002
-   Brett Moore, we współpracy z firmami [TippingPoint](http://www.tippingpoint.com/) i [Zero Day Initiative](http://www.zerodayinitiative.com/), za zgłoszenie problemu opisanego w biuletynie MS10-002
-   Wushi z zespołu [team509](http://www.team509.com/), we współpracy z firmami [TippingPoint](http://www.tippingpoint.com/) i [Zero Day Initiative](http://www.zerodayinitiative.com/), za zgłoszenie problemu opisanego w biuletynie MS10-002
-   Sam Thomas (eshu.co.uk), współpracownik firm [TippingPoint](http://www.tippingpoint.com/) i [Zero Day Initiative](http://www.zerodayinitiative.com/), za zgłoszenie kilku problemów opisanych w biuletynie MS10-002
-   Haifei Li z zespołu [FortiGuard Global Security Research Team](http://www.fortiguardcenter.com/) firmy Fortinet, za zgłoszenie problemu opisanego w biuletynie MS10-002
-   Peter Vreugdenhil z firmy [Verisign iDefense Labs](http://labs.idefense.com/), przy współpracy z firmami [TippingPoint](http://www.tippingpoint.com/) i [Zero Day Initiative](http://www.zerodayinitiative.com/), za zgłoszenie problemu opisanego w biuletynie MS10-002
-   Meron Sellem z firmy [BugSec](http://www.bugsec.com/) za zgłoszenie problemu opisanego w biuletynie MS10-002

Firma Microsoft [dziękuje](http://go.microsoft.com/fwlink/?linkid=21127) wymienionym poniżej firmom za współpracę i podanie szczegółowych informacji na temat problemu opisanego w biuletynie MS10-002:

-   [Google Inc.](http://www.google.com/) i [MANDIANT](http://www.mandiant.com/)
-   [Adobe](http://www.adobe.com/)
-   [McAfee](http://www.mcafee.com/)
-   Francuski rząd CSIRT ([CERTA](http://www.certa.ssi.gouv.fr))

#### Pomoc techniczna

-   Wymienione oprogramowanie zostało przetestowane w celu ustalenia, których wersji dotyczy problem. Dla pozostałych wersji upłynął okres pomocy technicznej. Aby zapoznać się z zasadami cyklu pomocy technicznej dotyczącymi używanej wersji oprogramowania, odwiedź [witrynę zasad cyklu pomocy technicznej firmy Microsoft](http://go.microsoft.com/fwlink/?linkid=21742).
-   Klienci mogą uzyskać pomoc techniczną w [Biurze Obsługi Klienta Microsoft](http://go.microsoft.com/fwlink/?linkid=21131) pod numerem 0 801 802 000 (Opłata według stawek Twojego operatora) lub (0-22) 594 19 99 w godzinach od 9:00 do 17:00, od poniedziałku do piątku. Połączenia z działem pomocy technicznej związane z aktualizacjami zabezpieczeń są bezpłatne. Dodatkowe informacje dotyczące możliwości skorzystania z pomocy technicznej można znaleźć w witrynie [Pomoc i obsługa techniczna firmy Microsoft](http://support.microsoft.com/?ln=pl).
-   Klienci międzynarodowi mogą uzyskać pomoc w lokalnych przedstawicielstwach firmy Microsoft. Pomoc techniczna związana z aktualizacjami zabezpieczeń jest bezpłatna. Informacje o sposobie kontaktowania się z pomocą techniczną firmy Microsoft są dostępne w [międzynarodowej witrynie sieci Web pomocy i obsługi technicznej](http://go.microsoft.com/fwlink/?linkid=21155).

#### Zrzeczenie odpowiedzialności

Informacje w bazie wiedzy Microsoft Knowledge Base są dostarczane „tak jak są” bez jakiejkolwiek gwarancji. Firma Microsoft odrzuca wszelkie gwarancje, wyraźne i dorozumiane, w tym gwarancje dotyczące wartości handlowej i przydatności do określonego celu. Firma Microsoft Corporation ani jej dostawcy w żadnym wypadku nie ponoszą odpowiedzialności za jakiekolwiek szkody, w tym bezpośrednie, pośrednie, przypadkowe, wynikowe, utratę zysków handlowych lub szkody specjalne, nawet jeżeli firmę Microsoft Corporation lub jej dostawców powiadomiono o możliwości zaistnienia takich szkód. W niektórych stanach wyłączenie lub ograniczenie odpowiedzialności za straty wynikowe lub przypadkowe, a więc i powyższe ograniczenia, nie mają zastosowania.

#### Wersje

-   Wersja 1.0 (12 stycznia 2010 r.): Opublikowane podsumowanie biuletynów zabezpieczeń.
-   Wersja 2.0 (21 stycznia 2010 r.): Dodano Biuletyn zabezpieczeń firmy Microsoft **MS10-002, Zbiorcza aktualizacja zabezpieczeń dla programu Internet Explorer (978207).** Dodano także łącze do emisji internetowej, odnoszące się do tego opublikowanego poza cyklem standardowym biuletynu zabezpieczeń.

*Built at 2014-04-18T01:50:00Z-07:00*
