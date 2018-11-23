---
TOCTitle: 'MS09-MAR'
Title: 'Podsumowanie biuletynów zabezpieczeń firmy Microsoft za marzec 2009 r.'
ms:assetid: 'ms09-mar'
ms:contentKeyID: 61233103
ms:mtpsurl: 'https://technet.microsoft.com/pl-PL/library/ms09-mar(v=Security.10)'
---

Podsumowanie biuletynów zabezpieczeń firmy Microsoft za marzec 2009 r.
======================================================================

Opublikowano: 10 marca 2009 | Zaktualizowano: 11 marca 2009

**Wersja:** 1.1

Niniejsze podsumowanie biuletynów zabezpieczeń zawiera spis biuletynów za marzec 2009 r.

Z chwilą opublikowania biuletynów za marzec 2009 r. niniejsze podsumowanie biuletynów zastępuje powiadomienie o biuletynach zabezpieczeń wydane 5 marca 2009 r. Aby uzyskać więcej informacji na temat usługi powiadamiania o biuletynach, zobacz [Powiadomienia o biuletynach zabezpieczeń firmy Microsoft (j. ang.)](http://technet.microsoft.com/security/bulletin/advance).

Aby dowiedzieć się, jak otrzymywać automatyczne powiadomienia o publikacji biuletynów zabezpieczeń firmy Microsoft, odwiedź stronę [Microsoft Technical Security Notifications](http://go.microsoft.com/fwlink/?linkid=21163).

11 marca 2009 r. o godz. 11:00 czasu Pacyfiku (godz. 20:00 czasu środkowoeuropejskiego) firma Microsoft udostępni emisję internetową, w której znajdą się odpowiedzi na pytania klientów dotyczące tych biuletynów (USA i Kanada). Zarejestruj się, aby zobaczyć [emisję internetową dotyczącą biuletynów zabezpieczeń za marzec](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032395124). Po tym dniu emisja internetowa będzie dostępna na żądanie. Aby uzyskać więcej informacji, zobacz [Podsumowania biuletynów zabezpieczeń i emisje internetowe firmy Microsoft](http://technet.microsoft.com/security/bulletin/summary).

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
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms09-006">MS09-006</a></td>
<td style="border:1px solid black;"><strong>Luki w zabezpieczeniach jądra systemu Windows umożliwiają zdalne wykonanie kodu (958690)</strong><br />
<br />
Ta aktualizacja zabezpieczeń usuwa kilka luk w zabezpieczeniach jądra systemu Windows, które zostały zgłoszone przez użytkowników. Najpoważniejsza z tych luk może umożliwiać zdalne wykonanie kodu, jeśli użytkownik wyświetli specjalnie spreparowany plik obrazu EMF lub WMF z systemu, którego dotyczy problem.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Krytyczny</a><br />
Zdalne wykonanie kodu</td>
<td style="border:1px solid black;">Wymaga ponownego uruchomienia komputera</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms09-007">MS09-007</a></td>
<td style="border:1px solid black;"><strong>Luka w zabezpieczeniach SChannel może pozwolić na fałszowanie (960225)</strong><br />
<br />
Ta aktualizacja zabezpieczeń usuwa zgłoszoną przez użytkowników lukę w pakiecie zabezpieczeń bezpiecznego kanału (Schannel) w systemie Windows. Luka może umożliwiać fałszowanie, jeśli osoba atakująca uzyska dostęp do certyfikatu wykorzystywanego do uwierzytelniania przez użytkownika końcowego. Luka dotyczy użytkowników tylko wtedy, gdy osoba atakująca innymi drogami uzyska składnik klucza publicznego certyfikatu służącego do uwierzytelniania.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Ważny</a><br />
Fałszowanie</td>
<td style="border:1px solid black;">Wymaga ponownego uruchomienia komputera</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms09-008">MS09-008</a></td>
<td style="border:1px solid black;"><strong>Luki w zabezpieczeniach serwerów DNS i WINS umożliwiają fałszowanie (962238)</strong><br />
<br />
Ta aktualizacja zabezpieczeń usuwa dwie luki w zabezpieczeniach serwera DNS i serwera WINS systemu Windows, które zostały zgłoszone przez użytkowników, oraz dwie luki w zabezpieczeniach, które zostały zgłoszone przez organizację publiczną. Luki te umożliwiają zdalnej osobie atakującej przekierowanie ruchu sieciowego, który jest przeznaczony dla systemów w Internecie, do systemów tej osoby.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Ważny</a><br />
Fałszowanie</td>
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
  
| Identyfikator biuletynu                                             | Tytuł biuletynu                                                                          | CVE ID                                                                           | Ocena wskaźnika możliwości wykorzystania luki                                                                              | Najważniejsze uwagi                                                                                                                                                                      |  
|---------------------------------------------------------------------|------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| [MS09-006](http://technet.microsoft.com/security/bulletin/ms09-006) | Luki w zabezpieczeniach jądra systemu Windows umożliwiają zdalne wykonanie kodu (958690) | [CVE-2009-0081](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0081) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - działający kod wykorzystujący lukę mało prawdopodobny | Bardziej prawdopodobna jest konsekwentna odmowa usługi niż niezawodne, funkcjonalne wykonanie kodu                                                                                       |  
| [MS09-006](http://technet.microsoft.com/security/bulletin/ms09-006) | Luki w zabezpieczeniach jądra systemu Windows umożliwiają zdalne wykonanie kodu (958690) | [CVE-2009-0082](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0082) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny niespójny kod wykorzystujący lukę       | Bardziej prawdopodobna jest konsekwentna odmowa usługi niż niezawodne, funkcjonalne wykonanie kodu                                                                                       |  
| [MS09-006](http://technet.microsoft.com/security/bulletin/ms09-006) | Luki w zabezpieczeniach jądra systemu Windows umożliwiają zdalne wykonanie kodu (958690) | [CVE-2009-0083](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0083) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - działający kod wykorzystujący lukę mało prawdopodobny | Zagrożenie lokalne występuje jedynie w postaci konsekwentnej odmowy usługi lub ujawnienia informacji, które są bardziej prawdopodobne niż niezawodne, funkcjonalne wykonanie kodu        |  
| [MS09-007](http://technet.microsoft.com/security/bulletin/ms09-007) | Luka w zabezpieczeniach SChannel może pozwolić na fałszowanie (960225)                   | [CVE-2009-0085](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0085) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny niespójny kod wykorzystujący lukę       | Wymagania dotyczące niezawodnego wykorzystania są wysokie, natomiast liczba potencjalnych scenariuszy obejmujących klientów - niska                                                      |  
| [MS09-008](http://technet.microsoft.com/security/bulletin/ms09-008) | Luki w zabezpieczeniach serwerów DNS i WINS umożliwiają fałszowanie (962238)             | [CVE-2009-0093](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0093) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny niespójny kod wykorzystujący lukę       | Spójny kod koncepcyjny udowadniający możliwość fałszowania jest prawdopodobny, ale działający kod wykorzystujący lukę skutkujący wykonaniem kodu złośliwego jest wysoce nieprawdopodobny |  
| [MS09-008](http://technet.microsoft.com/security/bulletin/ms09-008) | Luki w zabezpieczeniach serwerów DNS i WINS umożliwiają fałszowanie (962238)             | [CVE-2009-0094](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0094) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny niespójny kod wykorzystujący lukę       | Spójny kod koncepcyjny udowadniający możliwość fałszowania jest prawdopodobny, ale działający kod wykorzystujący lukę skutkujący wykonaniem kodu złośliwego jest wysoce nieprawdopodobny |  
| [MS09-008](http://technet.microsoft.com/security/bulletin/ms09-008) | Luki w zabezpieczeniach serwerów DNS i WINS umożliwiają fałszowanie (962238)             | [CVE-2009-0233](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0233) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny niespójny kod wykorzystujący lukę       | Spójny kod koncepcyjny udowadniający możliwość fałszowania jest prawdopodobny, ale działający kod wykorzystujący lukę skutkujący wykonaniem kodu złośliwego jest wysoce nieprawdopodobny |  
| [MS09-008](http://technet.microsoft.com/security/bulletin/ms09-008) | Luki w zabezpieczeniach serwerów DNS i WINS umożliwiają fałszowanie (962238)             | [CVE-2009-0234](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0234) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny niespójny kod wykorzystujący lukę       | Spójny kod koncepcyjny udowadniający możliwość fałszowania jest prawdopodobny, ale działający kod wykorzystujący lukę skutkujący wykonaniem kodu złośliwego jest wysoce nieprawdopodobny |
  
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
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="4">
Microsoft Windows 2000  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS09-006**](http://technet.microsoft.com/security/bulletin/ms09-006)
</td>
<td style="border:1px solid black;">
[**MS09-007**](http://technet.microsoft.com/security/bulletin/ms09-007)
</td>
<td style="border:1px solid black;">
[**MS09-008**](http://technet.microsoft.com/security/bulletin/ms09-008)
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
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 z dodatkiem Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 z dodatkiem Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=98bb7d40-89a0-470a-8eb7-06f15072a635)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 z dodatkiem Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=bf7065bc-c183-4a78-8d46-72fe7385c07c)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Serwer DNS w systemie Microsoft Windows 2000 Server z dodatkiem Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=110354f7-5ece-4c4d-b563-3adba6ac0116)  
(961063)  
(Ważny)  
[Serwer WINS w systemie Microsoft Windows 2000 Server z dodatkiem Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=4319abb3-1ea2-466a-a815-c0b3b86b4462)  
(961064)  
(Ważny)
</td>
</tr>
<tr>
<th colspan="4">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS09-006**](http://technet.microsoft.com/security/bulletin/ms09-006)
</td>
<td style="border:1px solid black;">
[**MS09-007**](http://technet.microsoft.com/security/bulletin/ms09-007)
</td>
<td style="border:1px solid black;">
[**MS09-008**](http://technet.microsoft.com/security/bulletin/ms09-008)
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP z dodatkiem Service Pack 2 i Windows XP z dodatkiem Service Pack 3
</td>
<td style="border:1px solid black;">
[Windows XP z dodatkiem Service Pack 2 i Windows XP z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=e09641ba-6cbe-4095-82b5-703d3a7dc33b)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows XP z dodatkiem Service Pack 2 i Windows XP z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=942d87f6-3cb1-4d36-a70a-70d9c34488f3)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition oraz Microsoft Windows XP Professional x64 Edition z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition oraz Windows XP Professional x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d0d704c6-48c2-4907-b6c3-2455d7cf21c8)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition oraz Windows XP Professional x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6d02306e-9e2e-4ae8-bd21-8a2c1a229472)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr>
<th colspan="4">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS09-006**](http://technet.microsoft.com/security/bulletin/ms09-006)
</td>
<td style="border:1px solid black;">
[**MS09-007**](http://technet.microsoft.com/security/bulletin/ms09-007)
</td>
<td style="border:1px solid black;">
[**MS09-008**](http://technet.microsoft.com/security/bulletin/ms09-008)
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 z dodatkiem Service Pack 1 i Windows Server 2003 z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem Service Pack 1 i Windows Server 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f5cfb8da-e7cc-4183-8631-507c2a406500)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem Service Pack 1 i Windows Server 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0b3f6fdd-276e-4267-99d8-8f00d91ad6a2)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Serwer DNS w systemie Windows Server 2003 z dodatkiem Service Pack 1 i Windows Server 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6cc42c9e-c34e-4577-8b23-9e07e2369878)  
(961063)  
(Ważny)  
[Serwer WINS w systemie Windows Server 2003 z dodatkiem Service Pack 1 i Windows Server 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=049e5db5-7315-4188-99fd-4a54833e6bf2)  
(961064)  
(Ważny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition i Windows Server 2003 x64 Edition z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition i Windows Server 2003 x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ecf75c70-8489-41ad-9759-3a07e13957be)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition i Windows Server 2003 x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ce98ff55-f565-469d-bbd2-32b681faf908)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Serwer DNS w systemie Windows Server 2003 x64 Edition i Windows Server 2003 x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b1f81fd2-0099-4450-8543-0459561d22d0)  
(961063)  
(Ważny)  
[Serwer WINS w systemie Windows Server 2003 x64 Edition i Windows Server 2003 x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4a393c63-eff5-4c8c-9c3f-33ce45c32428)  
(961064)  
(Ważny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Systemy operacyjne Windows Server 2003 z dodatkiem SP1 dla systemów z procesorem Itanium oraz Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem SP1 dla systemów z procesorem Itanium oraz Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=04be3d7e-7dda-4dca-887a-e7a8156ede1c)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem SP1 dla systemów z procesorem Itanium oraz Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=5ca3c72c-cadb-4b0a-b3a3-fb81d0bfd7b3)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Serwer DNS w systemie Windows Server 2003 z dodatkiem SP1 dla systemów z procesorem Itanium i Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=d3ed7d9a-d652-4bd0-aecc-5a415bec6c59)  
(961063)  
(Ważny)  
[Serwer WINS w systemie Windows Server 2003 z dodatkiem SP1 dla systemów z procesorem Itanium i Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=37e3a75e-0a5d-4df0-881f-cdb87efa4dcf)  
(961064)  
(Ważny)
</td>
</tr>
<tr>
<th colspan="4">
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS09-006**](http://technet.microsoft.com/security/bulletin/ms09-006)
</td>
<td style="border:1px solid black;">
[**MS09-007**](http://technet.microsoft.com/security/bulletin/ms09-007)
</td>
<td style="border:1px solid black;">
[**MS09-008**](http://technet.microsoft.com/security/bulletin/ms09-008)
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
Brak
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista i Windows Vista z dodatkiem Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Vista i Windows Vista z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=4b1aaaba-f355-4265-83c0-50b901856ced)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Vista i Windows Vista z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=21086a04-402a-4940-8358-7fa63508102b)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition i Windows Vista x64 Edition z dodatkiem Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition i Windows Vista x64 Edition z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=0fcac480-d6db-4a94-8c7d-b7319282cf56)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition i Windows Vista x64 Edition z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c75a2ea9-b42f-457b-be09-5c8fa0339388)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr>
<th colspan="4">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS09-006**](http://technet.microsoft.com/security/bulletin/ms09-006)
</td>
<td style="border:1px solid black;">
[**MS09-007**](http://technet.microsoft.com/security/bulletin/ms09-007)
</td>
<td style="border:1px solid black;">
[**MS09-008**](http://technet.microsoft.com/security/bulletin/ms09-008)
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 dla systemów 32-bitowych
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów 32-bitowych\*](http://www.microsoft.com/downloads/details.aspx?familyid=38851df2-4fb5-4d28-9d15-181c260cf8cf)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów 32-bitowych\*](http://www.microsoft.com/downloads/details.aspx?familyid=47b361ce-624b-466c-b5c5-8703f6532615)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Serwer DNS w systemie Windows Server 2008 dla systemów 32-bitowych\*](http://www.microsoft.com/downloads/details.aspx?familyid=92e89882-d656-4b61-a05c-3afb44895f08)  
(961063)  
(Ważny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 dla systemów opartych na procesorach X64
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów opartych na procesorach X64](http://www.microsoft.com/downloads/details.aspx?familyid=ec15acc4-3e0f-4414-9383-61c122ff1382)\*  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów opartych na procesorach X64](http://www.microsoft.com/downloads/details.aspx?familyid=5c81ac45-60e6-4121-ab6b-d3b3179aacc4)\*  
(Ważny)
</td>
<td style="border:1px solid black;">
[Serwer DNS w systemie Windows Server 2008 dla systemów opartych na procesorach x64\*](http://www.microsoft.com/downloads/details.aspx?familyid=be068d06-5939-4ad8-8191-e85931ed610f)  
(961063)  
(Ważny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 dla systemów z procesorem Itanium
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=eead6f93-10fd-4492-8137-481d9876a5fe)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=bf8f5a86-1757-4f9b-b632-d4aa7005a9f8)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
</table>
 
**Uwagi dotyczące systemu Windows Server 2008**

**\*Luka w zabezpieczeniach dotyczy instalacji Server Core systemu operacyjnego Windows Server 2008.** W przypadku obsługiwanych wersji systemu Windows Server 2008 ta aktualizacja ma zastosowanie, z takim samym wskaźnikiem ważności, niezależnie od tego, czy system Windows Server 2008 został zainstalowany przy użyciu opcji instalacji Server Core. Aby uzyskać więcej informacji na temat tej opcji instalacji, zobacz [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Należy pamiętać, że opcja instalacji Server Core nie dotyczy niektórych wersji systemu Windows Server 2008; zobacz [Porównanie opcji instalacji Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

Narzędzia wykrywania i wdrażania oraz wskazówki
-----------------------------------------------

<span></span>
**Centrum zabezpieczeń**

Zarządzanie oprogramowaniem oraz aktualizacjami zabezpieczeń, które należy zainstalować na serwerach oraz komputerach stacjonarnych i przenośnych w organizacji. Więcej informacji można znaleźć w [Centrum TechNet Update Management Center](http://go.microsoft.com/fwlink/?linkid=69903). Witryna [TechNet Security Center](http://go.microsoft.com/fwlink/?linkid=21171) zawiera dodatkowe informacje na temat zabezpieczeń w produktach firmy Microsoft. Użytkownicy mogą także uzyskać dostęp do tych informacji w witrynie [Bezpieczeństwo w domu](http://go.microsoft.com/fwlink/?linkid=85102), klikając łącze „Najnowsze aktualizacje zabezpieczeń”.

Aktualizacje zabezpieczeń dostępne są w witrynach [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747), [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130) i [Office Update](http://go.microsoft.com/fwlink/?linkid=21135). Aktualizacje zabezpieczeń są także dostępne w witrynie [Microsoft Download Center](http://go.microsoft.com/fwlink/?linkid=21129). Najłatwiej je znaleźć, wyszukując wyrażenie „aktualizacja zabezpieczeń”.

Aktualizacje zabezpieczeń można także pobierać z [Wykazu usługi Microsoft Update](http://go.microsoft.com/fwlink/?linkid=96155). Wykaz usługi Microsoft Update zawiera katalog zawartości z możliwością przeszukiwania, który udostępniany jest poprzez usługi Windows Update i Microsoft Update i obejmuje aktualizacje zabezpieczeń, sterowniki i dodatki Service Pack. Wyszukiwanie przy użyciu numeru biuletynu zabezpieczeń (np. „MS07-036”) pozwala dodać do koszyka wszystkie odpowiednie aktualizacje (w tym różne wersje językowe aktualizacji) i pobrać pliki do wybranego folderu. Więcej informacji na temat Wykazu usługi Microsoft Update można znaleźć w [Często zadawanych pytaniach dotyczących Wykazu usługi Microsoft Update](http://go.microsoft.com/fwlink/?linkid=97900).

**Porady dotyczące wykrywania i wdrażania**

Firma Microsoft opublikowała porady dotyczące wykrywania i wdrażania, odnoszące się do aktualizacji zabezpieczeń udostępnionych w tym miesiącu. Porady te będą również pomocne dla informatyków, wyjaśniając, jak mogą oni wdrażać aktualizacje za pomocą różnych narzędzi, takich jak Windows Update, Microsoft Update, Office Update, Microsoft Baseline Security Analyzer (MBSA), Office Detection Tool, Microsoft Systems Management Server (SMS) i Extended Security Update Inventory Tool (ESUIT). Więcej informacji na ten temat można znaleźć w [artykule 910723 bazy wiedzy Microsoft Knowledge Base](http://support.microsoft.com/kb/910723).

**Narzędzie Microsoft Baseline Security Analyzer (MBSA)**

Narzędzie Microsoft Baseline Security Analyzer umożliwia administratorom skanowanie lokalnych i zdalnych systemów w poszukiwaniu brakujących aktualizacji zabezpieczeń oraz typowych błędów konfiguracji zabezpieczeń. Więcej informacji na temat narzędzia MBSA można znaleźć w witrynie sieci Web[Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134).

**Windows Server Update Services**

Korzystając z programu Windows Server Update Services (WSUS), administratorzy mogą szybko i niezawodnie wdrożyć najnowsze aktualizacje krytyczne i aktualizacje zabezpieczeń przeznaczonych dla systemu operacyjnego Windows 2000 i nowszych, pakietu Office XP i nowszych, programu Exchange Server 2003 oraz SQL Server 2000 w systemie operacyjnym Windows 2000 i nowszych.

Więcej informacji na temat sposobu wdrażania tej aktualizacji zabezpieczeń za pomocą programu Windows Server Update Services można znaleźć w [witrynie sieci Web programu Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=50120).

**Program Systems Management Server**

Program Systems Management Server (SMS) jest przeznaczonym dla przedsiębiorstw i w znacznym stopniu konfigurowalnym rozwiązaniem służącym do zarządzania aktualizacjami. Program SMS umożliwia administratorom znalezienie komputerów z systemem Windows, na których należy zainstalować aktualizację zabezpieczeń, a także przeprowadzić kontrolowane wdrożenie tych aktualizacji w całym przedsiębiorstwie, w minimalnym stopniu zakłócając przy tym pracę użytkowników końcowych. Dostępne jest kolejne wydanie programu SMS, System Center Configuration Manager 2007. Zapoznaj się także z zawartością witryny [System Center Configuration Manager 2007](http://technet.microsoft.com/en-us/library/bb735860.aspx). Więcej informacji na temat możliwości wykorzystania przez administratorów programu SMS 2003 do wdrażania aktualizacji zabezpieczeń można znaleźć w [witrynie sieci Web zarządzania poprawkami zabezpieczeń programu SMS 2003](http://go.microsoft.com/fwlink/?linkid=22939). Użytkownicy programu SMS 2.0 mogą także skorzystać z dodatku [Software Updates Services Feature Pack](http://go.microsoft.com/fwlink/?linkid=33340) ułatwiającego wdrożenie aktualizacji zabezpieczeń. Więcej informacji na temat programu SMS można znaleźć w witrynie sieci Web [Microsoft Systems Management Server](http://go.microsoft.com/fwlink/?linkid=21158).

**Uwaga** Program SMS zapewnia obsługę rozwiązań zawartych w biuletynach zabezpieczeń dzięki narzędziom Microsoft Baseline Security Analyzer oraz Microsoft Office Detection Tool. Narzędzia te mogą nie wykrywać wszystkich aktualizacji oprogramowania. W takich przypadkach administratorzy mogą wykorzystywać dostępne w programie SMS funkcje zarządzania zasobami do przyporządkowania poszczególnych aktualizacji określonym systemom. Aby uzyskać więcej informacji dotyczących tej procedury, zobacz [Wdrażanie aktualizacji oprogramowania za pomocą funkcji Software Distribution programu SMS](http://go.microsoft.com/fwlink/?linkid=33341). Niektóre aktualizacje oprogramowania wymagają od użytkownika uprawnień administratora po ponownym uruchomieniu systemu. Do zainstalowania tych aktualizacji administratorzy mogą użyć narzędzia Elevated Rights Deployment Tool (dostępnego w dodatkach [SMS 2003 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=33387) oraz [SMS 2.0 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=21161)).

**Tester zgodności aktualizacji i zestaw narzędzi do sprawdzania zgodności aplikacji**

Często aktualizacje zapisują informacje w tych samych plikach i ustawieniach rejestru niezbędnych do działania określonych aplikacji użytkownika. Może to prowadzić do niezgodności i wydłużyć czas wdrażania aktualizacji zabezpieczeń. Dzięki składnikom narzędzia [Tester zgodności aplikacji](http://technet2.microsoft.com/windowsvista/en/library/4279e239-37a4-44aa-aec5-4e70fe39f9de1033.mspx?mfr=true) znajdującego się w [Zestawie narzędzi do sprawdzania zgodności aplikacji 5.0](http://www.microsoft.com/downloads/details.aspx?familyid=24da89e9-b581-47b0-b45e-492dd6da2971&displaylang=en) można usprawnić proces testowania i sprawdzania poprawności aktualizacji systemu Windows.

W Zestawie narzędzi do sprawdzania zgodności aplikacji znajdują się niezbędne narzędzia i dokumentacja, które umożliwiają ocenę zgodności aplikacji przed wdrożeniem systemu Microsoft Windows Vista, aktualizacji dla systemu Windows, aktualizacji zabezpieczeń firmy Microsoft lub nowej wersji programu Windows Internet Explorer w środowisku użytkownika, oraz ograniczenie problemów ze zgodnością aplikacji.

### Inne informacje:

#### Narzędzie Microsoft Windows do usuwania złośliwego oprogramowania

Firma Microsoft opublikowała zaktualizowaną wersję narzędzia Microsoft Windows Malicious Software Removal Tool, która dostępna jest w witrynach sieci Web Windows Update i Microsoft Update, poprzez usługi Windows Server Update Services i w witrynie Microsoft Download Center.

#### Aktualizacje o wysokim priorytecie niezwiązane z zabezpieczeniami, dostępne w witrynach MU, WU oraz usługach WSUS

Aby uzyskać informacje na temat publikacji niezwiązanych z zabezpieczeniami, dostępnych w witrynach Windows Update i Microsoft Update, zobacz:

-   [Artykuł 894199 bazy wiedzy Microsoft Knowledge Base](http://support.microsoft.com/kb/894199): Opis zmian zawartości Usług aktualizacji oprogramowania i usług Windows Server Update Services. Zawiera wszystkie treści dotyczące systemu Windows.
-   [Nowe, zmienione i opublikowane aktualizacje dla produktów firmy Microsoft innych niż Microsoft Windows](http://technet.microsoft.com/en-us/wsus/bb466214.aspx).

#### Microsoft Active Protections Program (MAPP)

W celu zwiększenia poziomu bezpieczeństwa swoich klientów firma Microsoft dostarcza informacje na temat luk w zabezpieczeniach największym dostawcom oprogramowania zabezpieczającego przed publikacją comiesięcznej aktualizacji zabezpieczeń. Dzięki informacjom dotyczącym luk w zabezpieczeniach dostawcy oprogramowania zabezpieczającego mogą zaoferować swoim klientom zaktualizowane poprawki za pośrednictwem programów lub urządzeń zabezpieczających np. programów antywirusowych, sieciowych systemów wykrywania włamań lub hostowych systemów zapobiegania włamaniom. Aby sprawdzić, czy dostawcy oprogramowania zabezpieczającego zapewniają aktywną ochronę, odwiedź witryny poszczególnych partnerów programu, których listę znaleźć można w sekcji [Microsoft Active Protections Program (MAPP) Partners](http://www.microsoft.com/security/msrc/mapp/partners.mspx).

#### Strategie i społeczność związane z zabezpieczeniami

**Strategie zarządzania aktualizacjami**

Na stronie [Security Guidance for Update Management](http://go.microsoft.com/fwlink/?linkid=21168) (Wskazówki z zakresu bezpieczeństwa dotyczące zarządzania aktualizacjami) znajdują się dodatkowe informacje o zalecanych przez firmę Microsoft najlepszych sposobach stosowania aktualizacji zabezpieczeń.

**Uzyskiwanie innych aktualizacji zabezpieczeń**

Aktualizacje dotyczące innych problemów związanych z zabezpieczeniami można uzyskać w następujących lokalizacjach:

-   Aktualizacje zabezpieczeń są dostępne w witrynie [Microsoft Download Center](http://go.microsoft.com/fwlink/?linkid=21129). Najłatwiej je znaleźć, wyszukując wyrażenie „aktualizacja zabezpieczeń”.
-   Aktualizacje dla poszczególnych platform są dostępne w [witrynie sieci Web Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747).
-   Aktualizacje zabezpieczeń dostępne w tym miesiącu w witrynie Windows Update można otrzymać w witrynie Microsoft Download Center w postaci plików obrazu dysku CD zawierającego zabezpieczenia i aktualizacje krytyczne. Więcej informacji na ten temat można znaleźć w [artykule 913086 bazy wiedzy Microsoft Knowledge Base](http://support.microsoft.com/kb/913086).

**Społeczność IT Pro Security Community**

Dowiedz się, jak poprawić bezpieczeństwo i zoptymalizować infrastrukturę informatyczną oraz weź udział w dyskusjach dotyczących zabezpieczeń wraz z innymi specjalistami branży IT, odwiedzając witrynę sieci Web społeczności [IT Pro Security Community](http://go.microsoft.com/fwlink/?linkid=21164) (jęz. ang.).

#### Podziękowania

Firma Microsoft [dziękuje](http://go.microsoft.com/fwlink/?linkid=21127) wymienionym poniżej organizacjom i osobom za współpracę w dziedzinie ochrony klientów:

-   Helmut Buhler (<http://home.arcor.de/clipboarder/>) za zgłoszenie problemu opisanego w biuletynie MS09-006
-   Thomas Garnier z firmy [SkyRecon](http://www.skyrecon.com/), za zgłoszenie problemu opisanego w biuletynie MS09-006
-   [Secretaria da Fazenda do Estado do Rio Grande do Sul](http://www.sefaz.rs.gov.br/) za zgłoszenie problemu opisanego w biuletynie MS09-007
-   [Cia de Processamento de Dados do Estado do Rio Grande do Sul](http://www.procergs.rs.gov.br/) za zgłoszenie problemu opisanego w biuletynie MS09-007
-   Kevin Day, za współpracę przy rozwiązywaniu dwóch problemów opisanych w biuletynie MS09-008
-   Dave Dagon z ośrodka [Georgia Tech Information Security Center](http://www.gtisc.gatech.edu/), za współpracę z firmą Microsoft przy rozwiązywaniu dwóch problemów opisanych w biuletynie MS09-008

#### Pomoc techniczna

-   Wymienione oprogramowanie zostało przetestowane w celu ustalenia, których wersji dotyczy problem. Dla pozostałych wersji upłynął okres pomocy technicznej. Aby zapoznać się z zasadami cyklu pomocy technicznej dotyczącymi używanej wersji oprogramowania, odwiedź [witrynę zasad cyklu pomocy technicznej firmy Microsoft](http://go.microsoft.com/fwlink/?linkid=21742).
-   Klienci mogą uzyskać pomoc techniczną w [Biurze Obsługi Klienta Microsoft](http://go.microsoft.com/fwlink/?linkid=21131) pod numerem 0 801 802 000 (Opłata według stawek Twojego operatora) lub (0-22) 594 19 99 w godzinach od 9:00 do 17:00, od poniedziałku do piątku. Połączenia z działem pomocy technicznej związane z aktualizacjami zabezpieczeń są bezpłatne.
-   Klienci międzynarodowi mogą uzyskać pomoc w lokalnych przedstawicielstwach firmy Microsoft. Pomoc techniczna związana z aktualizacjami zabezpieczeń jest bezpłatna. Informacje o sposobie kontaktowania się z pomocą techniczną firmy Microsoft są dostępne w [międzynarodowej witrynie sieci Web pomocy i obsługi technicznej](http://go.microsoft.com/fwlink/?linkid=21155).

#### Zrzeczenie odpowiedzialności

Informacje w bazie wiedzy Microsoft Knowledge Base są dostarczane „tak jak są” bez jakiejkolwiek gwarancji. Firma Microsoft odrzuca wszelkie gwarancje, wyraźne i dorozumiane, w tym gwarancje dotyczące wartości handlowej i przydatności do określonego celu. Firma Microsoft Corporation ani jej dostawcy w żadnym wypadku nie ponoszą odpowiedzialności za jakiekolwiek szkody, w tym bezpośrednie, pośrednie, przypadkowe, wynikowe, utratę zysków handlowych lub szkody specjalne, nawet jeżeli firmę Microsoft Corporation lub jej dostawców powiadomiono o możliwości zaistnienia takich szkód. W niektórych stanach wyłączenie lub ograniczenie odpowiedzialności za straty wynikowe lub przypadkowe, a więc i powyższe ograniczenia, nie mają zastosowania.

#### Wersje

-   Wersja 1.0 (10 marca 2009 r.): Opublikowane podsumowanie biuletynów zabezpieczeń.
-   Wersja 1.1 (11 marca 2009 r.): Zaktualizowano informacje o osobie, która znalazła lukę opisaną w biuletynie MS09-008.

*Built at 2014-04-18T01:50:00Z-07:00*
