---
TOCTitle: 'MS11-NOV'
Title: 'Podsumowanie biuletynów zabezpieczeń firmy Microsoft za listopad 2011 r.'
ms:assetid: 'ms11-nov'
ms:contentKeyID: 61233129
ms:mtpsurl: 'https://technet.microsoft.com/pl-PL/library/ms11-nov(v=Security.10)'
---
Podsumowanie biuletynów zabezpieczeń firmy Microsoft za listopad 2011 r.
========================================================================

Opublikowano: 8 listopada 2011

**Wersja:** 1.0

Niniejsze podsumowanie biuletynów zabezpieczeń zawiera spis biuletynów za listopad 2011 r.

Z chwilą opublikowania biuletynów zabezpieczeń za listopad 2011 r. niniejsze podsumowanie biuletynów zastąpi powiadomienie o biuletynach zabezpieczeń wydane 3 listopada 2011 r. Aby uzyskać więcej informacji na temat usługi powiadamiania o biuletynach, zobacz [Powiadomienia o biuletynach zabezpieczeń firmy Microsoft (j. ang.)](http://go.microsoft.com/fwlink/?linkid=217213).

Aby dowiedzieć się, jak otrzymywać automatyczne powiadomienia o publikacji biuletynów zabezpieczeń firmy Microsoft, odwiedź stronę [Microsoft Technical Security Notifications](http://go.microsoft.com/fwlink/?linkid=21163).

9 listopada 2011 r. o godz. 11:00 czasu Pacyfiku (godz. 20:00 czasu środkowoeuropejskiego) firma Microsoft udostępni emisję internetową, w której znajdą się odpowiedzi na pytania klientów dotyczące tych biuletynów (USA i Kanada). [Zarejestruj się, aby zobaczyć emisję internetową dotyczącą biuletynów zabezpieczeń za listopad](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032487958). Po tym dniu emisja internetowa będzie dostępna na żądanie. Aby uzyskać więcej informacji, zobacz [Podsumowania biuletynów zabezpieczeń i emisje internetowe firmy Microsoft](http://go.microsoft.com/fwlink/?linkid=217214).

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=229071">MS11-083</a></td>
<td style="border:1px solid black;"><strong>Luka w zabezpieczeniach protokołu TCP/IP może pozwolić na zdalne wykonanie kodu (2588516)</strong><br />
<br />
Ta aktualizacja zabezpieczeń usuwa lukę w zabezpieczeniach systemu Microsoft Windows. Omawiana luka może pozwolić na zdalne wykonanie kodu, jeśli osoba atakująca będzie wysyłać do zamkniętego portu w systemie docelowym ciągły strumień specjalnie spreparowanych pakietów UDP.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Krytyczny</a><br />
Zdalne wykonanie kodu</td>
<td style="border:1px solid black;">Wymaga ponownego uruchomienia komputera</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=229638">MS11-085</a></td>
<td style="border:1px solid black;"><strong>Luka w zabezpieczeniach programów Poczta systemu Windows i Obszar spotkań w systemie Windows umożliwia zdalne wykonanie kodu (2620704)</strong><br />
<br />
Ta aktualizacja zabezpieczeń usuwa lukę w zabezpieczeniach systemu Microsoft Windows. Luka ta umożliwia zdalne wykonanie kodu, gdy użytkownik otworzy prawidłowy plik (na przykład plik .eml lub .wcinv), który znajduje się w tym samym katalogu sieciowym, co specjalnie spreparowany plik biblioteki dołączanej dynamicznie (DLL). Następnie, podczas otwierania poprawnego pliku program Poczta systemu Windows lub Obszar spotkań w systemie Windows może podjąć próbę załadowania pliku DLL i uruchomienia zawartego w nim kodu. Aby atak mógł się powieść, użytkownik musi odwiedzić niezaufaną zdalną lokalizację systemu plików lub udział WebDAV i z takiej otworzyć lokalizacji prawidłowy plik (na przykład plik .eml lub .wcinv), który następnie zostanie załadowany przez aplikację zagrożoną przez omawianą lukę.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Ważny</a><br />
Zdalne wykonanie kodu</td>
<td style="border:1px solid black;">Może wymagać ponownego uruchomienia</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=229253">MS11-086</a></td>
<td style="border:1px solid black;"><strong>Luka w zabezpieczeniach usługi Active Directory może pozwolić na podniesienie uprawnień (2630837)</strong><br />
<br />
Ta aktualizacja zabezpieczeń pozwala usunąć zgłoszoną przez użytkowników lukę w zabezpieczeniach usługi Active Directory, trybu aplikacji usługi Active Directory (ADAM) oraz usługi Active Directory Lightweight Directory Service (AD LDS). Omawiana luka w zabezpieczeniach może pozwolić na podniesienie uprawnień, jeśli usługa Active Directory jest skonfigurowana do korzystania z protokołu LDAP over SSL (LDAPS), a osoba atakująca zdobędzie odwołany certyfikat powiązany z prawidłowym kontem domeny i wykorzysta ten certyfikat do uwierzytelnienia się w domenie usługi Active Directory. Usługa Active Directory domyślnie nie jest skonfigurowana do korzystania z protokołu LDAP over SSL.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Ważny</a><br />
Podniesienie uprawnień</td>
<td style="border:1px solid black;">Wymaga ponownego uruchomienia komputera</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=229245">MS11-084</a></td>
<td style="border:1px solid black;"><strong>Luka w zabezpieczeniach sterowników trybu jądra systemu Windows umożliwia przeprowadzenie ataku typu „odmowa usługi” (2617657)</strong><br />
<br />
Ta aktualizacja zabezpieczeń usuwa lukę w zabezpieczeniach systemu Microsoft Windows. Luka ta umożliwia przeprowadzenie ataku typu „odmowa usługi”, jeśli użytkownik otworzy otrzymany w załączniku poczty e-mail specjalnie spreparowany plik czcionki TrueType lub przejdzie do udziału sieciowego lub lokalizacji WebDAV, gdzie znajduje się taki plik czcionki TrueType. Aby atak mógł się powieść, użytkownik musi odwiedzić niezaufaną zdalną lokalizację systemu plików lub udział WebDAV, w których znajduje się specjalnie spreparowany plik czcionki TrueType, lub otworzyć taki plik otrzymany w załączniku poczty e-mail. Jednakże w żadnym przypadku osoba atakująca nie może zmusić użytkownika do wykonania tych działań. Musi natomiast przekonać go do ich wykonania, zazwyczaj przez kliknięcie łącza znajdującego się w wiadomości e-mail lub wiadomości błyskawicznej.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Umiarkowany</a><br />
Odmowa usługi</td>
<td style="border:1px solid black;">Wymaga ponownego uruchomienia komputera</td>
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
  
| Identyfikator biuletynu                                   | Nazwa luki w zabezpieczeniach                                                                          | CVE ID                                                                           | Ocena możliwości wykorzystania luki w celu wykonania kodu w najnowszej wersji programu                           | Ocena możliwości wykorzystania luki w celu wykonania kodu w starszych wersjach programu                          | Ocena możliwości wykorzystania luki w celu wytworzenia sytuacji typu „odmowa usługi” | Najważniejsze uwagi |  
|-----------------------------------------------------------|--------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------|---------------------|  
| [MS11-083](http://go.microsoft.com/fwlink/?linkid=229071) | Luka w zabezpieczeniach związana z przepełnieniem licznika odwołań                                     | [CVE-2011-2013](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-2013) | [2](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny niespójny kod wykorzystujący lukę | [2](http://technet.microsoft.com/en-us/security/cc998259.aspx) — prawdopodobny niespójny kod wykorzystujący lukę | Stałe                                                                                | (Brak)              |  
| [MS11-085](http://go.microsoft.com/fwlink/?linkid=229638) | Luka w zabezpieczeniach programu Poczta systemu Windows związana z niebezpiecznym ładowaniem bibliotek | [CVE-2011-2016](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-2016) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Prawdopodobny spójny kod wykorzystujący lukę    | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Prawdopodobny spójny kod wykorzystujący lukę    | Nie dotyczy                                                                          | (Brak)              |  
| [MS11-086](http://go.microsoft.com/fwlink/?linkid=229253) | Luka w zabezpieczeniach związana z obejściem uwierzytelniania protokołu LDAPS                          | [CVE-2011-2014](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-2014) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Prawdopodobny spójny kod wykorzystujący lukę    | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Prawdopodobny spójny kod wykorzystujący lukę    | Nie dotyczy                                                                          | (Brak)              |
  
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
<th style="border:1px solid black;" >
</th>
</tr>
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
[**MS11-083**](http://go.microsoft.com/fwlink/?linkid=229071)
</td>
<td style="border:1px solid black;">
[**MS11-085**](http://go.microsoft.com/fwlink/?linkid=229638)
</td>
<td style="border:1px solid black;" colspan="2">
[**MS11-086**](http://go.microsoft.com/fwlink/?linkid=229253)
</td>
<td style="border:1px solid black;" colspan="2">
[**MS11-084**](http://go.microsoft.com/fwlink/?linkid=229245)
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
Brak
</td>
<td style="border:1px solid black;" colspan="2">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;" colspan="2">
Brak
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP z dodatkiem Service Pack 3
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;" colspan="2">
[Tryb aplikacji usługi Active Directory (ADAM)](http://www.microsoft.com/downloads/details.aspx?familyid=8c7c21c5-677d-4a5d-8f2b-8ca7691b6b00)  
(KB2616310)  
(Ważny)
</td>
<td style="border:1px solid black;" colspan="2">
Nie dotyczy
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;" colspan="2">
[Tryb aplikacji usługi Active Directory (ADAM)](http://www.microsoft.com/downloads/details.aspx?familyid=989cca2d-cce1-4f52-b50e-43152693f240)  
(KB2616310)  
(Ważny)
</td>
<td style="border:1px solid black;" colspan="2">
Nie dotyczy
</td>
</tr>
<tr>
<th colspan="7">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS11-083**](http://go.microsoft.com/fwlink/?linkid=229071)
</td>
<td style="border:1px solid black;">
[**MS11-085**](http://go.microsoft.com/fwlink/?linkid=229638)
</td>
<td style="border:1px solid black;" colspan="2">
[**MS11-086**](http://go.microsoft.com/fwlink/?linkid=229253)
</td>
<td style="border:1px solid black;" colspan="2">
[**MS11-084**](http://go.microsoft.com/fwlink/?linkid=229245)
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
Brak
</td>
<td style="border:1px solid black;" colspan="2">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;" colspan="2">
Brak
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;" colspan="2">
[Active Directory](http://www.microsoft.com/downloads/details.aspx?familyid=08b27ce7-c32e-41e4-ad04-481c5eab17a7)  
(KB2601626)  
(Ważny)  
[Tryb aplikacji usługi Active Directory (ADAM)](http://www.microsoft.com/downloads/details.aspx?familyid=f116824e-ea48-422d-b284-c9ffa7604bf5)  
(KB2616310)  
(Ważny)
</td>
<td style="border:1px solid black;" colspan="2">
Nie dotyczy
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;" colspan="2">
[Active Directory](http://www.microsoft.com/downloads/details.aspx?familyid=de5a74f2-2cc8-4677-b495-3a40fe3d6b9e)  
(KB2601626)  
(Ważny)  
[Tryb aplikacji usługi Active Directory (ADAM)](http://www.microsoft.com/downloads/details.aspx?familyid=1af1b734-62c7-4e08-91c8-90b6d026da84)  
(KB2616310)  
(Ważny)
</td>
<td style="border:1px solid black;" colspan="2">
Nie dotyczy
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;" colspan="2">
[Active Directory](http://www.microsoft.com/downloads/details.aspx?familyid=6168bc67-3d59-450f-bd8a-02d61dabe16b)  
(KB2601626)  
(Ważny)
</td>
<td style="border:1px solid black;" colspan="2">
Nie dotyczy
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
[**MS11-083**](http://go.microsoft.com/fwlink/?linkid=229071)
</td>
<td style="border:1px solid black;">
[**MS11-085**](http://go.microsoft.com/fwlink/?linkid=229638)
</td>
<td style="border:1px solid black;" colspan="2">
[**MS11-086**](http://go.microsoft.com/fwlink/?linkid=229253)
</td>
<td style="border:1px solid black;" colspan="2">
[**MS11-084**](http://go.microsoft.com/fwlink/?linkid=229245)
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
<td style="border:1px solid black;" colspan="2">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;" colspan="2">
Brak
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fc3fe87c-2493-431d-a904-dec9310f6042)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Vista z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e08266d8-fffa-40bf-b8f6-10a65ee27524)  
(Ważny)
</td>
<td style="border:1px solid black;" colspan="2">
[Usługa Active Directory Lightweight Directory Service (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=2bd602cf-ae0d-4790-a5d0-6133fd7d01a0)  
(KB2601626)  
(Ważny)
</td>
<td style="border:1px solid black;" colspan="2">
Nie dotyczy
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=042c1a8f-834d-4eed-8a59-9e030ccc6d39)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4f2365ed-d50e-44d9-b859-1ec54d3b4d38)  
(Ważny)
</td>
<td style="border:1px solid black;" colspan="2">
[Usługa Active Directory Lightweight Directory Service (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=783521ad-5c50-4194-a582-4e5a1c9999e7)  
(KB2601626)  
(Ważny)
</td>
<td style="border:1px solid black;" colspan="2">
Nie dotyczy
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
[**MS11-083**](http://go.microsoft.com/fwlink/?linkid=229071)
</td>
<td style="border:1px solid black;">
[**MS11-085**](http://go.microsoft.com/fwlink/?linkid=229638)
</td>
<td style="border:1px solid black;" colspan="2">
[**MS11-086**](http://go.microsoft.com/fwlink/?linkid=229253)
</td>
<td style="border:1px solid black;" colspan="2">
[**MS11-084**](http://go.microsoft.com/fwlink/?linkid=229245)
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
<td style="border:1px solid black;" colspan="2">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;" colspan="2">
Brak
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 z dodatkiem Service Pack 2 dla systemów 32-bitowych
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów 32-bitowych z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=79382bf2-d2cb-42ea-92dc-64f949353521)\*  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów 32-bitowych z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f82dc413-668c-4ca8-a8c8-db74f05346bc)\*\*  
(Umiarkowany)
</td>
<td style="border:1px solid black;" colspan="2">
[Usługa Active Directory i usługa Active Directory Lightweight Directory Service (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=b5688923-3914-4f6c-8bc9-036fb4870cc6)\*  
(KB2601626)  
(Ważny)
</td>
<td style="border:1px solid black;" colspan="2">
Nie dotyczy
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem x64
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem x64 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=71ff3a89-d7ad-4dda-9e59-fab54b21bd5d)\*  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=06ad5637-56a1-4478-aaa0-063e877503c9)\*\*  
(Umiarkowany)
</td>
<td style="border:1px solid black;" colspan="2">
[Usługa Active Directory i usługa Active Directory Lightweight Directory Service (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=51f47181-08f6-4de1-80e5-253355675965)\*  
(KB2601626)  
(Ważny)
</td>
<td style="border:1px solid black;" colspan="2">
Nie dotyczy
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem Itanium
</td>
<td style="border:1px solid black;">
[Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=b1c0cb05-c284-49b1-ae4f-92813fdf520f)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=2de5de74-e643-4045-9c22-ff95b0dbcafc)  
(Umiarkowany)
</td>
<td style="border:1px solid black;" colspan="2">
Nie dotyczy
</td>
<td style="border:1px solid black;" colspan="2">
Nie dotyczy
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
[**MS11-083**](http://go.microsoft.com/fwlink/?linkid=229071)
</td>
<td style="border:1px solid black;">
[**MS11-085**](http://go.microsoft.com/fwlink/?linkid=229638)
</td>
<td style="border:1px solid black;" colspan="2">
[**MS11-086**](http://go.microsoft.com/fwlink/?linkid=229253)
</td>
<td style="border:1px solid black;" colspan="2">
[**MS11-084**](http://go.microsoft.com/fwlink/?linkid=229245)
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
[**Niski**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;" colspan="2">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;" colspan="2">
[**Umiarkowany**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 dla systemów 32-bitowych i Windows 7 z dodatkiem Service Pack 1 dla systemów 32-bitowych
</td>
<td style="border:1px solid black;">
[Windows 7 dla systemów 32-bitowych i Windows 7 z dodatkiem Service Pack 1 dla systemów 32-bitowych](http://www.microsoft.com/downloads/details.aspx?familyid=4ddb4c2a-bada-49b0-ad78-e07e7e11ced7)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows 7 dla systemów 32-bitowych i Windows 7 z dodatkiem Service Pack 1 dla systemów 32-bitowych](http://www.microsoft.com/downloads/details.aspx?familyid=2307fa93-8e45-4841-a5a9-7e89960712f9)  
(Niski)
</td>
<td style="border:1px solid black;" colspan="2">
[Usługa Active Directory Lightweight Directory Service (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=b06f9f55-e3b2-4705-83d0-1b9f5de9d378)  
(KB2601626)  
(Ważny)
</td>
<td style="border:1px solid black;" colspan="2">
[Windows 7 dla systemów 32-bitowych i Windows 7 z dodatkiem Service Pack 1 dla systemów 32-bitowych](http://www.microsoft.com/downloads/details.aspx?familyid=156c1bd9-55bc-482c-874b-61998d1ef153)  
(Umiarkowany)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 dla systemów opartych na procesorach x64 i Windows 7 z dodatkiem Service Pack 1 dla systemów opartych na procesorach x64
</td>
<td style="border:1px solid black;">
[Windows 7 dla systemów opartych na procesorach x64 i Windows 7 z dodatkiem Service Pack 1 dla systemów opartych na procesorach x64](http://www.microsoft.com/downloads/details.aspx?familyid=05eef5d7-acf6-46e4-abfc-dc83f0a7cae5)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows 7 dla systemów opartych na procesorach x64 i Windows 7 z dodatkiem Service Pack 1 dla systemów opartych na procesorach x64](http://www.microsoft.com/downloads/details.aspx?familyid=62603d18-1b21-400c-8eba-202193182960)  
(Niski)
</td>
<td style="border:1px solid black;" colspan="2">
[Usługa Active Directory Lightweight Directory Service (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=790f1d99-96a5-438d-b433-895b692912ce)  
(KB2601626)  
(Ważny)
</td>
<td style="border:1px solid black;" colspan="2">
[Windows 7 dla systemów opartych na procesorach x64 i Windows 7 z dodatkiem Service Pack 1 dla systemów opartych na procesorach x64](http://www.microsoft.com/downloads/details.aspx?familyid=5c7db930-5495-43f0-928c-d586ac9e80d0)  
(Umiarkowany)
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
[**MS11-083**](http://go.microsoft.com/fwlink/?linkid=229071)
</td>
<td style="border:1px solid black;">
[**MS11-085**](http://go.microsoft.com/fwlink/?linkid=229638)
</td>
<td style="border:1px solid black;" colspan="2">
[**MS11-086**](http://go.microsoft.com/fwlink/?linkid=229253)
</td>
<td style="border:1px solid black;" colspan="2">
[**MS11-084**](http://go.microsoft.com/fwlink/?linkid=229245)
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
[**Niski**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;" colspan="2">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;" colspan="2">
[**Umiarkowany**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 dla systemów opartych na procesorach x64 i Windows Server 2008 R2 z dodatkiem Service Pack 1 dla systemów opartych na procesorach x64
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach x64 i Windows Server 2008 R2 z dodatkiem Service Pack 1 dla systemów opartych na procesorach x64](http://www.microsoft.com/downloads/details.aspx?familyid=3f9f74a6-e984-4aab-837c-ef7286e7305f)\*  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach x64 i Windows Server 2008 R2 z dodatkiem Service Pack 1 dla systemów opartych na procesorach x64](http://www.microsoft.com/downloads/details.aspx?familyid=c9cf6a22-f9ab-427a-9b16-33c60baaabb5)\*\*  
(Niski)
</td>
<td style="border:1px solid black;" colspan="2">
[Usługa Active Directory i usługa Active Directory Lightweight Directory Service (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=cc1e99af-fc67-400b-a82c-171f8c4d1ac9)\*  
(KB2601626)  
(Ważny)
</td>
<td style="border:1px solid black;" colspan="2">
[Windows Server 2008 R2 dla systemów opartych na procesorach x64 i Windows Server 2008 R2 z dodatkiem Service Pack 1 dla systemów opartych na procesorach x64](http://www.microsoft.com/downloads/details.aspx?familyid=5d810dae-5c52-4155-b5c2-163d27be6e78)\*\*\*  
(Umiarkowany)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 dla systemów opartych na procesorach Itanium i Windows Server 2008 R2 z dodatkiem Service Pack 1 dla systemów opartych na procesorach Itanium
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach Itanium i Windows Server 2008 R2 z dodatkiem Service Pack 1 dla systemów opartych na procesorach Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=b20bfcbd-a515-4074-b56e-b82539fe5bad)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach Itanium i Windows Server 2008 R2 z dodatkiem Service Pack 1 dla systemów opartych na procesorach Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=012777f5-51f2-4944-91af-a9c79b8081a1)  
(Niski)
</td>
<td style="border:1px solid black;" colspan="2">
Nie dotyczy
</td>
<td style="border:1px solid black;" colspan="2">
[Windows Server 2008 R2 dla systemów opartych na procesorach Itanium i Windows Server 2008 R2 z dodatkiem Service Pack 1 dla systemów opartych na procesorach Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=395819e2-1028-44b7-ace4-ca754b1a7543)  
(Umiarkowany)
</td>
</tr>
</table>
 
**Uwagidotyczące systemu Windows Server 2008 i Windows Server 2008 R2**

**\*Luka w zabezpieczeniach dotyczy instalacji Server Core.** Ta aktualizacja ma zastosowanie, z takim samym wskaźnikiem ważności, w przypadku obsługiwanych wersji systemu Windows Server 2008 lub Windows Server 2008 R2, niezależnie od tego, czy zostały zainstalowane przy użyciu opcji instalacji Server Core. Więcej informacji na temat tej opcji instalacji można znaleźć w artykułach TechNet, [Managing a Server Core Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) i [Servicing a Server Core Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) (jęz. ang.). Należy pamiętać, że opcja instalacji Server Core nie dotyczy niektórych wersji systemu Windows Server 2008 i Windows Server 2008 R2. Zobacz [Porównanie opcji instalacji Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Luka w zabezpieczeniach nie dotyczy instalacji Server Core.** Luki usuwane przez tę aktualizację zabezpieczeń nie dotyczą obsługiwanych wersji systemu Windows Server 2008 ani Windows Server 2008 R2, jeżeli systemy te zostały zainstalowane przy użyciu opcji instalacji Server Core. Więcej informacji na temat tej opcji instalacji można znaleźć w artykułach TechNet, [Managing a Server Core Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) i [Servicing a Server Core Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) (jęz. ang.). Należy pamiętać, że opcja instalacji Server Core nie dotyczy niektórych wersji systemu Windows Server 2008 i Windows Server 2008 R2. Zobacz [Porównanie opcji instalacji Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*\*Luka w zabezpieczeniach nie dotyczy instalacji Server Core.** Luka usuwana przez tę aktualizację zabezpieczeń nie dotyczy obsługiwanych wersji systemu Windows Server 2008 lub Windows Server 2008 R2, jeśli zostały one zainstalowane przy użyciu opcji instalacji Server Core, mimo że na komputerze mogą znajdować się pliki, których dotyczy omawiana luka. Aktualizacja ta będzie jednak w dalszym ciągu oferowana użytkownikom posiadającym pliki podlegające luce, ponieważ zaktualizowane pliki są nowsze (mają wyższe numery wersji) niż pliki znajdujące się obecnie w systemie. Więcej informacji na temat tej opcji instalacji można znaleźć w artykułach TechNet, [Managing a Server Core Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) i [Servicing a Server Core Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) (jęz. ang.). Należy pamiętać, że opcja instalacji Server Core nie dotyczy niektórych wersji systemu Windows Server 2008 i Windows Server 2008 R2. Zobacz [Porównanie opcji instalacji Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

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

**Narzędzie Microsoft Baseline Security Analyzer (MBSA)**

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

-   Will Dorman z firmy [CERT/CC](http://www.cert.org/), za zgłoszenie problemu opisanego w biuletynie MS11-084
-   Ivan Sanchez z EvilCode, za zgłoszenie problemu opisanego w biuletynie MS11-085
-   Xavier Lassoie i Sébastien Godard z Autosécurité, za zgłoszenie problemu opisanego w biuletynie MS11-086

#### Pomoc techniczna

-   Wymienione oprogramowanie zostało przetestowane w celu ustalenia, których wersji dotyczy problem. Dla pozostałych wersji upłynął okres pomocy technicznej. Aby zapoznać się z zasadami cyklu pomocy technicznej dotyczącymi używanej wersji oprogramowania, odwiedź [witrynę zasad cyklu pomocy technicznej firmy Microsoft](http://go.microsoft.com/fwlink/?linkid=21742).
-   Klienci mogą uzyskać pomoc techniczną w [Biurze Obsługi Klienta Microsoft](http://go.microsoft.com/fwlink/?linkid=21131) pod numerem 0 801 802 000 (opłata według stawek Twojego operatora) lub (0-22) 594 19 99 w godzinach od 9:00 do 17:00, od poniedziałku do piątku. Połączenia z działem pomocy technicznej związane z aktualizacjami zabezpieczeń są bezpłatne. Dodatkowe informacje dotyczące możliwości skorzystania z pomocy technicznej można znaleźć w witrynie [Pomoc i obsługa techniczna firmy Microsoft](http://support.microsoft.com/).
-   Klienci międzynarodowi mogą uzyskać pomoc w lokalnych przedstawicielstwach firmy Microsoft. Pomoc techniczna związana z aktualizacjami zabezpieczeń jest bezpłatna. Informacje o sposobie kontaktowania się z pomocą techniczną firmy Microsoft są dostępne w [międzynarodowej witrynie sieci Web pomocy i obsługi technicznej](http://go.microsoft.com/fwlink/?linkid=21155).

#### Zrzeczenie odpowiedzialności

Informacje w bazie wiedzy Microsoft Knowledge Base są dostarczane „tak jak są” bez jakiejkolwiek gwarancji. Firma Microsoft odrzuca wszelkie gwarancje, wyraźne i dorozumiane, w tym gwarancje dotyczące wartości handlowej i przydatności do określonego celu. Firma Microsoft Corporation ani jej dostawcy w żadnym wypadku nie ponoszą odpowiedzialności za jakiekolwiek szkody, w tym bezpośrednie, pośrednie, przypadkowe, wynikowe, utratę zysków handlowych lub szkody specjalne, nawet jeżeli firmę Microsoft Corporation lub jej dostawców powiadomiono o możliwości zaistnienia takich szkód. W niektórych stanach wyłączenie lub ograniczenie odpowiedzialności za straty wynikowe lub przypadkowe, a więc i powyższe ograniczenia, nie mają zastosowania.

#### Wersje

-   Wersja 1.0 (8 listopada 2011 r.): Opublikowane podsumowanie biuletynów zabezpieczeń.

*Built at 2014-04-18T01:50:00Z-07:00*
