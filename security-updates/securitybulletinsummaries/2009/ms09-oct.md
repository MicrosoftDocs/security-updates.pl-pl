---
TOCTitle: 'MS09-OCT'
Title: 'Podsumowanie biuletynów zabezpieczeń firmy Microsoft za październik 2009 r.'
ms:assetid: 'ms09-oct'
ms:contentKeyID: 61233106
ms:mtpsurl: 'https://technet.microsoft.com/pl-PL/library/ms09-oct(v=Security.10)'
---

Security Bulletin Summary

Podsumowanie biuletynów zabezpieczeń firmy Microsoft za październik 2009 r.
===========================================================================

Opublikowano: 13 października 2009 | Zaktualizowano: 22 czerwca 2010

**Wersja:** 4.2

Niniejsze podsumowanie biuletynów zabezpieczeń zawiera spis biuletynów za październik 2009 r.

Z chwilą opublikowania biuletynów za październik 2009 r. niniejsze podsumowanie biuletynów zastępuje powiadomienie o biuletynach zabezpieczeń wydane 8 października 2009 r. Aby uzyskać więcej informacji na temat usługi powiadamiania o biuletynach, zobacz [Powiadomienia o biuletynach zabezpieczeń firmy Microsoft (jęz. ang.)](http://technet.microsoft.com/security/bulletin/advance).

Aby dowiedzieć się, jak otrzymywać automatyczne powiadomienia o publikacji biuletynów zabezpieczeń firmy Microsoft, odwiedź stronę [Microsoft Technical Security Notifications](http://go.microsoft.com/fwlink/?linkid=21163).

14 października 2009 r. o godz. 11:00 czasu Pacyfiku (godz. 20:00 czasu środkowoeuropejskiego) firma Microsoft udostępni emisję internetową, w której znajdą się odpowiedzi na pytania klientów dotyczące tych biuletynów (USA i Kanada). [Zarejestruj się, aby zobaczyć emisję internetową dotyczącą biuletynów zabezpieczeń za październik](http://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032407488&culture=en-us). Po tym dniu emisja internetowa będzie dostępna na żądanie. Aby uzyskać więcej informacji, zobacz [Podsumowania biuletynów zabezpieczeń i emisje internetowe firmy Microsoft](http://technet.microsoft.com/security/bulletin/summary).

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=163970">MS09-050</a></td>
<td style="border:1px solid black;"><strong>Luki w zabezpieczeniach protokołu SMBv2 umożliwiają zdalne wykonanie kodu (975517)</strong><br />
<br />
Niniejsza aktualizacja zabezpieczeń usuwa jedną lukę zgłoszoną przez organizacje publiczne oraz dwie luki zgłoszone przez użytkowników. Luki te znajdują się w protokole SMBv2 (Server Message Block Version 2). Najpoważniejsza z tych luk umożliwia zdalne wykonanie kodu, gdy osoba atakująca wyśle specjalnie spreparowany pakiet SMB do komputera z uruchomioną usługą Serwer. Sprawdzone metody działania stosowane w zaporach oraz standardowe domyślne konfiguracje zapór mogą pomóc w ochronie sieci przed atakami spoza przedsiębiorstwa. Zgodnie ze standardowymi zasadami działania zaleca się, aby w systemach połączonych z Internetem była otwarta jak najmniejsza liczba portów.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Krytyczny</a><br />
Zdalne wykonanie kodu</td>
<td style="border:1px solid black;">Wymaga ponownego uruchomienia komputera</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=125438">MS09-051</a></td>
<td style="border:1px solid black;"><strong>Luki w zabezpieczeniach programu Microsoft Windows Media Runtime umożliwiają zdalne wykonanie kodu (975682)</strong><br />
<br />
Ta aktualizacja zabezpieczeń usuwa dwie luki w zabezpieczeniach programu Windows Media Runtime, które zostały zgłoszone przez użytkowników. Luki umożliwiają zdalne wykonanie kodu, gdy użytkownik otworzy specjalnie spreparowany plik multimedialny lub odbierze specjalnie spreparowany strumień danych z witryny sieci Web lub dowolnej aplikacji dostarczającej treści z sieci Web. Osoba atakująca, której uda się wykorzystać te luki, może uzyskać takie same uprawnienia, jak użytkownik lokalny. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Krytyczny</a><br />
Zdalne wykonanie kodu</td>
<td style="border:1px solid black;">Może wymagać ponownego uruchomienia</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=163913">MS09-052</a></td>
<td style="border:1px solid black;"><strong>Luka w zabezpieczeniach programu Windows Media Player potencjalnie umożliwia zdalne wykonanie kodu (974112)</strong><br />
<br />
Niniejsza aktualizacja zabezpieczeń usuwa zgłoszoną przez użytkowników lukę w zabezpieczeniach programu Windows Media Player. Luka umożliwia zdalne wykonanie kodu, gdy specjalnie spreparowany plik ASF zostanie odtworzony przy użyciu programu Windows Media Player 6.4. Osoba atakująca, której uda się wykorzystać tę lukę, może uzyskać takie same uprawnienia, jak użytkownik lokalny. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Krytyczny</a><br />
Zdalne wykonanie kodu</td>
<td style="border:1px solid black;">Może wymagać ponownego uruchomienia</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=163979">MS09-054</a></td>
<td style="border:1px solid black;"><strong>Zbiorcza aktualizacja zabezpieczeń dla programu Internet Explorer (974455)</strong><br />
<br />
Ta aktualizacja zabezpieczeń usuwa trzy luki w zabezpieczeniach programu Internet Explorer zgłoszone przez użytkowników i jedną lukę w zabezpieczeniach programu Internet Explorer zgłoszoną przez organizacje publiczne. Luki te mogą pozwolić na zdalne wykonanie kodu, jeśli użytkownik wyświetli specjalnie spreparowaną stronę sieci Web przy użyciu programu Internet Explorer. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi. Tę aktualizację zabezpieczeń powinni również zastosować użytkownicy programu Firefox, którzy korzystają z dodatku plug-in Windows Presentation Foundation (WPF) i nie wyłączyli go. Więcej informacji na temat tego problemu można znaleźć w sekcji Często zadawane pytania dotyczące luki w zabezpieczeniach związanej z obsługą składników HTML - CVE-2009-2529.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Krytyczny</a><br />
Zdalne wykonanie kodu</td>
<td style="border:1px solid black;">Wymaga ponownego uruchomienia komputera</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms09-055">MS09-055</a></td>
<td style="border:1px solid black;"><strong>Zbiorcza aktualizacja zabezpieczeń bitów „zabicia” dla formantów ActiveX (973525)</strong><br />
<br />
Ta aktualizacja zabezpieczeń usuwa zgłoszoną przez użytkowników lukę dotyczącą wielu formantów ActiveX, która jest aktualnie wykorzystywana. Luka dotycząca formantów ActiveX skompilowanych przy użyciu wersji biblioteki Microsoft Active Template Library (ATL), której dotyczy luka, umożliwia zdalne wykonanie kodu, gdy użytkownik wyświetli specjalnie spreparowaną stronę sieci Web w programie Internet Explorer, uruchamiającą formant ActiveX. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Krytyczny</a><br />
Zdalne wykonanie kodu</td>
<td style="border:1px solid black;">Może wymagać ponownego uruchomienia</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=160633">MS09-060</a></td>
<td style="border:1px solid black;"><strong>Luki w zabezpieczeniach formantów ActiveX skompilowanych przy użyciu biblioteki Microsoft Active Template Library (ATL) umożliwiają zdalne wykonanie kodu (973965)</strong><br />
<br />
Ta aktualizacja zabezpieczeń usuwa kilka zgłoszonych przez użytkowników luk w zabezpieczeniach formantów ActiveX dla pakietu Microsoft Office, które zostały skompilowane przy użyciu wersji biblioteki Microsoft Active Template Library (ATL) zawierającej luki. Luki te umożliwiają zdalne wykonanie kodu, jeśli użytkownik załaduje specjalnie spreparowany składnik lub formant. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Krytyczny</a><br />
Zdalne wykonanie kodu</td>
<td style="border:1px solid black;">Może wymagać ponownego uruchomienia</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=160527">MS09-061</a></td>
<td style="border:1px solid black;"><strong>Luki w zabezpieczeniach aparatu plików wykonywalnych języka wspólnego systemu Microsoft .NET umożliwiają zdalne wykonanie kodu (974378)</strong><br />
<br />
Niniejsza aktualizacja zabezpieczeń usuwa trzy luki w zabezpieczeniach programów Microsoft .NET Framework i Microsoft Silverlight, które zostały zgłoszone przez użytkowników. Luki te mogą pozwolić na zdalne wykonanie kodu w systemie klienta, jeśli użytkownik wyświetli specjalnie spreparowaną stronę sieci Web przy użyciu przeglądarki sieci Web, która umożliwia uruchamianie aplikacji przeglądarki XAML (XBAP) lub aplikacji Silverlight, lub jeśli osobie atakującej uda się przekonać użytkownika do uruchomienia specjalnie spreparowanej aplikacji Microsoft .NET. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi. Omawiane luki umożliwiają także zdalne wykonanie kodu w systemach serwerowych z działającym programem IIS, jeśli dany serwer zezwala na przetwarzanie stron ASP.NET, a osobie atakującej uda się przekazać na ten serwer specjalnie spreparowaną stronę ASP.NET i uruchomić ją, tak jak mogłoby to wyglądać w scenariuszu z wykorzystaniem hostingu w sieci Web. Niezłośliwe aplikacje Microsoft .NET, Silverlight i XBAP oraz strony ASP.NET nie są narażone na wykorzystanie w związku z omawianą luką.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Krytyczny</a><br />
Zdalne wykonanie kodu</td>
<td style="border:1px solid black;">Może wymagać ponownego uruchomienia</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Microsoft .NET Framework,<br />
Microsoft Silverlight</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=161342">MS09-062</a></td>
<td style="border:1px solid black;"><strong>Luki w zabezpieczeniach interfejsu GDI+ umożliwiają zdalne wykonanie kodu (957488)</strong><br />
<br />
Ta aktualizacja zabezpieczeń usuwa kilka luk w zabezpieczeniach interfejsu Microsoft Windows GDI+, które zostały zgłoszone przez użytkowników. Luki te umożliwiają zdalne wykonanie kodu, jeśli użytkownik wyświetli specjalnie spreparowany plik obrazu przy użyciu oprogramowania dotkniętego problemem, lub jeśli przejdzie do witryny sieci Web zawierającej specjalnie spreparowaną zawartość. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Krytyczny</a><br />
Zdalne wykonanie kodu</td>
<td style="border:1px solid black;">Może wymagać ponownego uruchomienia</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer,<br />
Microsoft .NET Framework,<br />
Microsoft Office,<br />
Microsoft SQL Server,<br />
Narzędzia firmy Microsoft dla deweloperów,<br />
Microsoft Forefront</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=164004">MS09-053</a></td>
<td style="border:1px solid black;"><strong>Luki w zabezpieczeniach usługi FTP dla Internet Information Services umożliwiają zdalne wykonanie kodu (975254)</strong><br />
<br />
Niniejsza aktualizacja zabezpieczeń usuwa dwie luki w zabezpieczeniach usługi FTP w programach Microsoft Internet Information Services (IIS) 5.0, Microsoft Internet Information Services (IIS) 5.1, Microsoft Internet Information Services (IIS) 6.0 i Microsoft Internet Information Services (IIS) 7.0 zgłoszone przez organizacje publiczne. W przypadku programu IIS 7.0 luka dotyczy tylko usługi FTP 6.0. Luki umożliwiają zdalne wykonanie kodu w systemach z usługą FTP uruchomioną w programie IIS 5.0 albo atak typu „odmowa usługi” w systemach z usługą FTP uruchomioną w programie IIS 5.0, IIS 5.1, IIS 6.0 lub IIS 7.0.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Ważny</a><br />
Zdalne wykonanie kodu</td>
<td style="border:1px solid black;">Może wymagać ponownego uruchomienia</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=163830">MS09-056</a></td>
<td style="border:1px solid black;"><strong>Luki w zabezpieczeniach interfejsu Windows CryptoAPI mogą umożliwiać fałszowanie (974571)</strong><br />
<br />
Niniejsza aktualizacja zabezpieczeń usuwa dwie luki w zabezpieczeniach systemu Microsoft Windows, które zostały zgłoszone przez organizację publiczną. Luki te mogą umożliwiać fałszowanie, jeśli osoba atakująca uzyska dostęp do certyfikatu wykorzystywanego do uwierzytelniania przez użytkownika końcowego.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Ważny</a><br />
Fałszowanie</td>
<td style="border:1px solid black;">Wymaga ponownego uruchomienia komputera</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=163832">MS09-057</a></td>
<td style="border:1px solid black;"><strong>Luka usługi indeksowania umożliwia zdalne wykonanie kodu (969059)</strong><br />
<br />
Ta aktualizacja zabezpieczeń usuwa lukę w zabezpieczeniach systemu Microsoft Windows. Luka ta może pozwolić na zdalne wykonanie kodu, jeśli osoba atakująca udostępni w sieci odpowiednio spreparowaną witrynę internetową, która uruchomi usługę indeksowania poprzez odwołanie do jej składnika ActiveX. Wywołanie to może zawierać szkodliwy adres URL i spowodować wykorzystanie luki, zapewniając osobie atakującej dostęp do systemu klienta z uprawnieniami użytkownika przeglądającego witrynę internetową. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Ważny</a><br />
Zdalne wykonanie kodu</td>
<td style="border:1px solid black;">Wymaga ponownego uruchomienia komputera</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=162442">MS09-058</a></td>
<td style="border:1px solid black;"><strong>Luki w zabezpieczeniach jądra systemu Windows umożliwiają podniesienie poziomu uprawnień (971486)</strong><br />
<br />
Ta aktualizacja zabezpieczeń usuwa kilka luk w zabezpieczeniach jądra systemu Windows, które zostały zgłoszone przez użytkowników. Najpoważniejsza z luk może umożliwić podniesienie uprawnień, jeśli osoba atakująca zaloguje się do systemu i uruchomi specjalnie spreparowaną aplikację. Osoba atakująca musi dysponować prawidłowymi poświadczeniami logowania oraz być w stanie zalogować się lokalnie, aby wykorzystać jedną z tych luk. Nie jest możliwe wykorzystanie luk w sposób zdalny ani przez użytkowników anonimowych.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Ważny</a><br />
Podniesienie uprawnień</td>
<td style="border:1px solid black;">Wymaga ponownego uruchomienia komputera</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=163843">MS09-059</a></td>
<td style="border:1px solid black;"><strong>Luka w zabezpieczeniach usługi LSASS (Local Security Authority Subsystem Service) umożliwia przeprowadzenie ataku typu „odmowa usługi” (975467)</strong><br />
<br />
Ta aktualizacja zabezpieczeń usuwa lukę w zabezpieczeniach systemu Microsoft Windows. Luka umożliwia przeprowadzenie ataku typu „odmowa usługi”, jeśli osoba atakująca podczas procesu uwierzytelniania NTLM wysłała złośliwie spreparowany pakiet.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Ważny</a><br />
Odmowa usługi</td>
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
  
| Identyfikator biuletynu                                             | Tytuł biuletynu                                                                                                                                                                 | CVE ID                                                                           | Ocena wskaźnika możliwości wykorzystania luki                                                                              | Najważniejsze uwagi                                                                                                                                                                                                                                                                                                                                                                                                                            |  
|---------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| [MS09-050](http://go.microsoft.com/fwlink/?linkid=163970)           | Luki w zabezpieczeniach protokołu SMBv2 umożliwiają zdalne wykonanie kodu (975517)                                                                                              | [CVE-2009-2526](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2526) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - działający kod wykorzystujący lukę mało prawdopodobny | Ta luka powoduje ograniczoną awarię typu odmowa usługi.                                                                                                                                                                                                                                                                                                                                                                                        |  
| [MS09-050](http://go.microsoft.com/fwlink/?linkid=163970)           | Luki w zabezpieczeniach protokołu SMBv2 umożliwiają zdalne wykonanie kodu (975517)                                                                                              | [CVE-2009-2532](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2532) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny spójny kod wykorzystujący lukę          | (Brak)                                                                                                                                                                                                                                                                                                                                                                                                                                         |  
| [MS09-050](http://go.microsoft.com/fwlink/?linkid=163970)           | Luki w zabezpieczeniach protokołu SMBv2 umożliwiają zdalne wykonanie kodu (975517)                                                                                              | [CVE-2009-3103](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-3103) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny spójny kod wykorzystujący lukę          | Kod wykorzystujący tę lukę został ogłoszony publicznie.                                                                                                                                                                                                                                                                                                                                                                                        |  
| [MS09-051](http://go.microsoft.com/fwlink/?linkid=125438)           | Luki w zabezpieczeniach programu Windows Media Runtime umożliwiają zdalne wykonanie kodu (975682)                                                                               | [CVE-2009-0555](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0555) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny spójny kod wykorzystujący lukę          | (Brak)                                                                                                                                                                                                                                                                                                                                                                                                                                         |  
| [MS09-051](http://go.microsoft.com/fwlink/?linkid=125438)           | Luki w zabezpieczeniach programu Windows Media Runtime umożliwiają zdalne wykonanie kodu (975682)                                                                               | [CVE-2009-2525](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2525) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny niespójny kod wykorzystujący lukę       | (Brak)                                                                                                                                                                                                                                                                                                                                                                                                                                         |  
| [MS09-052](http://go.microsoft.com/fwlink/?linkid=163913)           | Luka w zabezpieczeniach programu Windows Media Player umożliwia zdalne wykonanie kodu (974112)                                                                                  | [CVE-2009-2527](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2527) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny spójny kod wykorzystujący lukę          | (Brak)                                                                                                                                                                                                                                                                                                                                                                                                                                         |  
| [MS09-053](http://go.microsoft.com/fwlink/?linkid=164004)           | Luki w zabezpieczeniach usługi FTP dla programu Internet Information Services umożliwiają zdalne wykonanie kodu (975254)                                                        | [CVE-2009-2521](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2521) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - działający kod wykorzystujący lukę mało prawdopodobny | Ta luka powoduje awarię typu odmowa usługi. Kod wykorzystujący tę lukę został ogłoszony publicznie.                                                                                                                                                                                                                                                                                                                                            |  
| [MS09-053](http://go.microsoft.com/fwlink/?linkid=164004)           | Luki w zabezpieczeniach usługi FTP dla programu Internet Information Services umożliwiają zdalne wykonanie kodu (975254)                                                        | [CVE-2009-3023](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-3023) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny spójny kod wykorzystujący lukę          | Kod wykorzystujący tę lukę został ogłoszony publicznie.                                                                                                                                                                                                                                                                                                                                                                                        |  
| [MS09-054](http://go.microsoft.com/fwlink/?linkid=163979)           | Zbiorcza aktualizacja zabezpieczeń dla programu Internet Explorer (974455)                                                                                                      | [CVE-2009-1547](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1547) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny niespójny kod wykorzystujący lukę       | (Brak)                                                                                                                                                                                                                                                                                                                                                                                                                                         |  
| [MS09-054](http://go.microsoft.com/fwlink/?linkid=163979)           | Zbiorcza aktualizacja zabezpieczeń dla programu Internet Explorer (974455)                                                                                                      | [CVE-2009-2529](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2529) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny spójny kod wykorzystujący lukę          | (Brak)                                                                                                                                                                                                                                                                                                                                                                                                                                         |  
| [MS09-054](http://go.microsoft.com/fwlink/?linkid=163979)           | Zbiorcza aktualizacja zabezpieczeń dla programu Internet Explorer (974455)                                                                                                      | [CVE-2009-2530](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2530) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny niespójny kod wykorzystujący lukę       | W systemach Microsoft Windows 2000 brak zabezpieczeń stosu podwyższa wskaźnik możliwości wykorzystania luki do [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny spójny kod wykorzystujący lukę.                                                                                                                                                                                                              |  
| [MS09-054](http://go.microsoft.com/fwlink/?linkid=163979)           | Zbiorcza aktualizacja zabezpieczeń dla programu Internet Explorer (974455)                                                                                                      | [CVE-2009-2531](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2531) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny niespójny kod wykorzystujący lukę       |                                                                                                                                                                                                                                                                                                                                                                                                                                                |  
| [MS09-055](http://technet.microsoft.com/security/bulletin/ms09-055) | Zbiorcza aktualizacja zabezpieczeń bitów „zabicia” dla formantów ActiveX (973525)                                                                                               | [CVE-2009-2493](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2493) | Brak                                                                                                                       | (Tej luce w zabezpieczeniach nadano już ocenę wskaźnika możliwości wykorzystania luki w [podsumowaniu biuletynów za lipiec](http://technet.microsoft.com/security/bulletin/ms09-jul). Wynika to z faktu, że luka ta została po raz pierwszy omówiona w biuletynie [MS09-035](http://go.microsoft.com/fwlink/?linkid=158131)). Zobacz także ten sam numer CVE w biuletynie [MS09-060](http://go.microsoft.com/fwlink/?linkid=160633).           |  
| [MS09-056](http://go.microsoft.com/fwlink/?linkid=163830)           | Luki w zabezpieczeniach składnika Windows CryptoAPI umożliwiają fałszowanie (974571)                                                                                            | [CVE-2009-2510](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2510) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - działający kod wykorzystujący lukę mało prawdopodobny | Jest to luka w zabezpieczeniach związana z fałszowaniem.                                                                                                                                                                                                                                                                                                                                                                                       |  
| [MS09-056](http://go.microsoft.com/fwlink/?linkid=163830)           | Luki w zabezpieczeniach składnika Windows CryptoAPI umożliwiają fałszowanie (974571)                                                                                            | [CVE-2009-2511](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2511) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - działający kod wykorzystujący lukę mało prawdopodobny | Jest to luka w zabezpieczeniach związana z fałszowaniem.                                                                                                                                                                                                                                                                                                                                                                                       |  
| [MS09-057](http://go.microsoft.com/fwlink/?linkid=163832)           | Luka w usłudze indeksowania umożliwia zdalne wykonanie kodu (969059)                                                                                                            | [CVE-2009-2507](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2507) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny niespójny kod wykorzystujący lukę       | (Brak)                                                                                                                                                                                                                                                                                                                                                                                                                                         |  
| [MS09-058](http://go.microsoft.com/fwlink/?linkid=162442)           | Luki w jądrze systemu Windows umożliwiają podniesienie uprawnień (971486)                                                                                                       | [CVE-2009-2515](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2515) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny niespójny kod wykorzystujący lukę       | (Brak)                                                                                                                                                                                                                                                                                                                                                                                                                                         |  
| [MS09-058](http://go.microsoft.com/fwlink/?linkid=162442)           | Luki w jądrze systemu Windows umożliwiają podniesienie uprawnień (971486)                                                                                                       | [CVE-2009-2516](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2516) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - działający kod wykorzystujący lukę mało prawdopodobny | Ta luka doprowadza do sytuacji typu „odmowa usługi”, jeśli zostanie wykorzystana przy użyciu udziału sieciowego oraz do sytuacji umożliwiającej podniesienie poziomu uprawnień, jeśli zostanie wykorzystana w celu zaatakowania systemu lokalnego.                                                                                                                                                                                             |  
| [MS09-058](http://go.microsoft.com/fwlink/?linkid=162442)           | Luki w jądrze systemu Windows umożliwiają podniesienie uprawnień (971486)                                                                                                       | [CVE-2009-2517](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2517) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - działający kod wykorzystujący lukę mało prawdopodobny | Ta luka powoduje awarię typu odmowa usługi.                                                                                                                                                                                                                                                                                                                                                                                                    |  
| [MS09-059](http://go.microsoft.com/fwlink/?linkid=163843)           | Luka w zabezpieczeniach usługi LSASS (Local Security Authority Subsystem Service) umożliwia przeprowadzenie ataku typu „odmowa usługi” (975467)                                 | [CVE-2009-2524](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2524) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - działający kod wykorzystujący lukę mało prawdopodobny | Ta luka powoduje ograniczoną awarię typu odmowa usługi.                                                                                                                                                                                                                                                                                                                                                                                        |  
| [MS09-060](http://go.microsoft.com/fwlink/?linkid=160633)           | Luki w zabezpieczeniach formantów ActiveX z biblioteki Active Template Library (ATL) firmy Microsoft dla pakietu Microsoft Office mogą umożliwić zdalne wykonanie kodu (973965) | [CVE-2009-0901](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0901) | Brak                                                                                                                       | (Tej luce w zabezpieczeniach nadano już ocenę wskaźnika możliwości wykorzystania luki w [podsumowaniu biuletynów za lipiec](http://technet.microsoft.com/security/bulletin/ms09-jul). Wynika to z faktu, że luka ta została po raz pierwszy omówiona w biuletynie [MS09-035](http://go.microsoft.com/fwlink/?linkid=158131)).                                                                                                                  |  
| [MS09-060](http://go.microsoft.com/fwlink/?linkid=160633)           | Luki w zabezpieczeniach formantów ActiveX z biblioteki Active Template Library (ATL) firmy Microsoft dla pakietu Microsoft Office mogą umożliwić zdalne wykonanie kodu (973965) | [CVE-2009-2493](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2493) | Brak                                                                                                                       | (Tej luce w zabezpieczeniach nadano już ocenę wskaźnika możliwości wykorzystania luki w [podsumowaniu biuletynów za lipiec](http://technet.microsoft.com/security/bulletin/ms09-jul). Wynika to z faktu, że luka ta została po raz pierwszy omówiona w biuletynie [MS09-035](http://go.microsoft.com/fwlink/?linkid=158131)). Zobacz także ten sam numer CVE w biuletynie [MS09-055](http://technet.microsoft.com/security/bulletin/ms09-055). |  
| [MS09-060](http://go.microsoft.com/fwlink/?linkid=160633)           | Luki w zabezpieczeniach formantów ActiveX z biblioteki Active Template Library (ATL) firmy Microsoft dla pakietu Microsoft Office mogą umożliwić zdalne wykonanie kodu (973965) | [CVE-2009-2495](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2495) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - działający kod wykorzystujący lukę mało prawdopodobny | Ta luka może doprowadzić do ujawnienia informacji.                                                                                                                                                                                                                                                                                                                                                                                             |  
| [MS09-061](http://go.microsoft.com/fwlink/?linkid=160527)           | Luki w zabezpieczeniach aparatu plików wykonywalnych języka wspólnego Microsoft .NET mogą umożliwić zdalne wykonanie kodu (974378)                                              | [CVE-2009-0090](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0090) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny spójny kod wykorzystujący lukę          | (Brak)                                                                                                                                                                                                                                                                                                                                                                                                                                         |  
| [MS09-061](http://go.microsoft.com/fwlink/?linkid=160527)           | Luki w zabezpieczeniach aparatu plików wykonywalnych języka wspólnego Microsoft .NET mogą umożliwić zdalne wykonanie kodu (974378)                                              | [CVE-2009-0091](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0091) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny spójny kod wykorzystujący lukę          | (Brak)                                                                                                                                                                                                                                                                                                                                                                                                                                         |  
| [MS09-061](http://go.microsoft.com/fwlink/?linkid=160527)           | Luki w zabezpieczeniach aparatu plików wykonywalnych języka wspólnego Microsoft .NET mogą umożliwić zdalne wykonanie kodu (974378)                                              | [CVE-2009-2497](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2497) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny spójny kod wykorzystujący lukę          | Istnieje ryzyko ataków z Internetu.                                                                                                                                                                                                                                                                                                                                                                                                            |  
| [MS09-062](http://go.microsoft.com/fwlink/?linkid=161342)           | Luki w zabezpieczeniach interfejsu GDI+ umożliwiają zdalne wykonanie kodu (957488)                                                                                              | [CVE-2009-2500](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2500) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny niespójny kod wykorzystujący lukę       | (Brak)                                                                                                                                                                                                                                                                                                                                                                                                                                         |  
| [MS09-062](http://go.microsoft.com/fwlink/?linkid=161342)           | Luki w zabezpieczeniach interfejsu GDI+ umożliwiają zdalne wykonanie kodu (957488)                                                                                              | [CVE-2009-2501](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2501) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny niespójny kod wykorzystujący lukę       | (Brak)                                                                                                                                                                                                                                                                                                                                                                                                                                         |  
| [MS09-062](http://go.microsoft.com/fwlink/?linkid=161342)           | Luki w zabezpieczeniach interfejsu GDI+ umożliwiają zdalne wykonanie kodu (957488)                                                                                              | [CVE-2009-2502](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2502) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny niespójny kod wykorzystujący lukę       | (Brak)                                                                                                                                                                                                                                                                                                                                                                                                                                         |  
| [MS09-062](http://go.microsoft.com/fwlink/?linkid=161342)           | Luki w zabezpieczeniach interfejsu GDI+ umożliwiają zdalne wykonanie kodu (957488)                                                                                              | [CVE-2009-2503](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2503) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny spójny kod wykorzystujący lukę          | (Brak)                                                                                                                                                                                                                                                                                                                                                                                                                                         |  
| [MS09-062](http://go.microsoft.com/fwlink/?linkid=161342)           | Luki w zabezpieczeniach interfejsu GDI+ umożliwiają zdalne wykonanie kodu (957488)                                                                                              | [CVE-2009-2504](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2504) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny niespójny kod wykorzystujący lukę       | (Brak)                                                                                                                                                                                                                                                                                                                                                                                                                                         |  
| [MS09-062](http://go.microsoft.com/fwlink/?linkid=161342)           | Luki w zabezpieczeniach interfejsu GDI+ umożliwiają zdalne wykonanie kodu (957488)                                                                                              | [CVE-2009-2518](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2518) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny niespójny kod wykorzystujący lukę       | (Brak)                                                                                                                                                                                                                                                                                                                                                                                                                                         |  
| [MS09-062](http://go.microsoft.com/fwlink/?linkid=161342)           | Luki w zabezpieczeniach interfejsu GDI+ umożliwiają zdalne wykonanie kodu (957488)                                                                                              | [CVE-2009-2528](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2528) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny spójny kod wykorzystujący lukę          | (Brak)                                                                                                                                                                                                                                                                                                                                                                                                                                         |  
| [MS09-062](http://go.microsoft.com/fwlink/?linkid=161342)           | Luki w zabezpieczeniach interfejsu GDI+ umożliwiają zdalne wykonanie kodu (957488)                                                                                              | [CVE-2009-3126](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-3126) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny niespójny kod wykorzystujący lukę       | (Brak)                                                                                                                                                                                                                                                                                                                                                                                                                                         |
  
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
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="13">
Microsoft Windows 2000  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS09-050**](http://go.microsoft.com/fwlink/?linkid=163970)
</td>
<td style="border:1px solid black;">
[**MS09-051**](http://go.microsoft.com/fwlink/?linkid=125438)
</td>
<td style="border:1px solid black;">
[**MS09-052**](http://go.microsoft.com/fwlink/?linkid=163913)
</td>
<td style="border:1px solid black;">
[**MS09-054**](http://go.microsoft.com/fwlink/?linkid=163979)
</td>
<td style="border:1px solid black;">
[**MS09-055**](http://technet.microsoft.com/security/bulletin/ms09-055)
</td>
<td style="border:1px solid black;">
[**MS09-061**](http://go.microsoft.com/fwlink/?linkid=160527)
</td>
<td style="border:1px solid black;">
[**MS09-062**](http://go.microsoft.com/fwlink/?linkid=161342)
</td>
<td style="border:1px solid black;">
[**MS09-053**](http://go.microsoft.com/fwlink/?linkid=164004)
</td>
<td style="border:1px solid black;">
[**MS09-056**](http://go.microsoft.com/fwlink/?linkid=163830)
</td>
<td style="border:1px solid black;">
[**MS09-057**](http://go.microsoft.com/fwlink/?linkid=163832)
</td>
<td style="border:1px solid black;">
[**MS09-058**](http://go.microsoft.com/fwlink/?linkid=162442)
</td>
<td style="border:1px solid black;">
[**MS09-059**](http://go.microsoft.com/fwlink/?linkid=163843)
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
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Brak**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 z dodatkiem Service Pack 4
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Koder-dekoder głosu DirectShow WMA](http://www.microsoft.com/downloads/details.aspx?familyid=4fe0dff5-04d9-4409-8d1d-52419537126b)  
(KB969878)  
(Krytyczny)  
[Dekoder Windows Media Audio Voice](http://www.microsoft.com/downloads/details.aspx?familyid=8f850a82-61f9-447b-a0aa-a2c192cc5d2e)  
(KB954155)  
(Krytyczny)  
[Menedżer kompresji audio](http://www.microsoft.com/downloads/details.aspx?familyid=6dfd5405-cabe-4bd7-9330-b6bde1d99194)  
(KB975025)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft Windows Media Player 6.4](http://www.microsoft.com/downloads/details.aspx?familyid=13035ef7-7e47-487c-8b7c-7795d33ce7de)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 5.01 z dodatkiem Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=26515c7b-d7a6-4405-96b5-a518dcb39d38)  
(Krytyczny)  
[Microsoft Internet Explorer 6 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=8154ba37-0fbc-4d31-9d6e-0b21586ad65a)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 z dodatkiem Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=edfea805-9544-4dc0-a52c-d7594205657b)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f) (KB953297)  
(Krytyczny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d4a328b5-5470-46b0-86c7-cfe0e6a3ea01) (KB953300)  
(Krytyczny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=491874d4-5eea-4545-9b7d-3861857c862e) (KB974417)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=f3fef608-dafb-4b37-a65a-9cc4ae8e2c4c)  
(KB958869)  
(Krytyczny)  
[Microsoft .NET Framework 1.1 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ecf78619-80fa-417d-852b-1b5b2cf574e2)  
(KB971108)  
(Ważny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=3e534aa8-29c2-4379-9f57-931a6ff47418)  
(KB971110)  
(Ważny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e6f5e730-85cc-4c08-a50d-c456b1e9f5bc)  
(KB971111)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 z dodatkiem Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=7fecd367-aaff-458b-91bc-8925c8e57528)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 z dodatkiem Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=52b9198d-b65f-467a-a5ab-141e23d64a86)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 z dodatkiem Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=b34d94b5-b828-4e16-a636-04344c60d945)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 z dodatkiem Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=bdfa6583-28a2-4d6b-91d2-157a8518b664)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr>
<th colspan="13">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS09-050**](http://go.microsoft.com/fwlink/?linkid=163970)
</td>
<td style="border:1px solid black;">
[**MS09-051**](http://go.microsoft.com/fwlink/?linkid=125438)
</td>
<td style="border:1px solid black;">
[**MS09-052**](http://go.microsoft.com/fwlink/?linkid=163913)
</td>
<td style="border:1px solid black;">
[**MS09-054**](http://go.microsoft.com/fwlink/?linkid=163979)
</td>
<td style="border:1px solid black;">
[**MS09-055**](http://technet.microsoft.com/security/bulletin/ms09-055)
</td>
<td style="border:1px solid black;">
[**MS09-061**](http://go.microsoft.com/fwlink/?linkid=160527)
</td>
<td style="border:1px solid black;">
[**MS09-062**](http://go.microsoft.com/fwlink/?linkid=161342)
</td>
<td style="border:1px solid black;">
[**MS09-053**](http://go.microsoft.com/fwlink/?linkid=164004)
</td>
<td style="border:1px solid black;">
[**MS09-056**](http://go.microsoft.com/fwlink/?linkid=163830)
</td>
<td style="border:1px solid black;">
[**MS09-057**](http://go.microsoft.com/fwlink/?linkid=163832)
</td>
<td style="border:1px solid black;">
[**MS09-058**](http://go.microsoft.com/fwlink/?linkid=162442)
</td>
<td style="border:1px solid black;">
[**MS09-059**](http://go.microsoft.com/fwlink/?linkid=163843)
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
Windows XP z dodatkiem Service Pack 2 i Windows XP z dodatkiem Service Pack 3
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Koder-dekoder głosu DirectShow WMA](http://www.microsoft.com/downloads/details.aspx?familyid=4fe0dff5-04d9-4409-8d1d-52419537126b)  
(KB969878)  
(Krytyczny)  
[Dekoder Windows Media Audio Voice](http://www.microsoft.com/downloads/details.aspx?familyid=4516c219-e357-485e-a52b-23dcb8ee49d8)  
(KB954155)  
(Krytyczny)  
(tylko system Windows XP z dodatkiem Service Pack 2)  
[Dekoder Windows Media Audio Voice](http://www.microsoft.com/downloads/details.aspx?familyid=746d3440-5a6a-421e-9286-7b534a1dfe54)  
(KB954155)  
(Krytyczny)  
(tylko system Windows XP z dodatkiem Service Pack 3)  
[Menedżer kompresji audio](http://www.microsoft.com/downloads/details.aspx?familyid=6ecc7129-8caa-4daf-a8e2-8f3536225fb3)  
(KB975025)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft Windows Media Player 6.4](http://www.microsoft.com/downloads/details.aspx?familyid=b2efe1ac-d8d7-41bb-b87d-fc5e22afef0f)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=9aacf890-afb4-46a7-a13f-dd9fe3c0ca4a)  
(Krytyczny)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=dc166dc6-577f-4d8d-94df-dd963233dd85)  
(Krytyczny)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=8799159d-df69-49f6-9db5-49147690ce0c)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows XP z dodatkiem Service Pack 2 i Windows XP z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=171d43d3-669c-4923-b266-e47591833c05)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.0 z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=1bc56c26-1c7c-47e3-94f4-37af7e00392c)  
(KB953295)  
(Krytyczny)  
(tylko Tablet PC Edition 2005 i Media Center Edition 2005)  
[Microsoft .NET Framework 1.1 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f) (KB953297)  
(Krytyczny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 1 i Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=d4a328b5-5470-46b0-86c7-cfe0e6a3ea01) (KB953300)  
(Krytyczny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2 i Microsoft .NET Framework 3.5 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=491874d4-5eea-4545-9b7d-3861857c862e) (KB974417)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows XP z dodatkiem Service Pack 2 i Windows XP z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=e2acde20-a6d3-4135-b6eb-1214f743d474)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows XP z dodatkiem Service Pack 2 i Windows XP z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=2ae0bdd4-f8b2-420a-b1ac-d2cdaa87c828)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows XP z dodatkiem Service Pack 2 i Windows XP z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=9c5ab624-e37b-418a-a919-d8f652b15679)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows XP z dodatkiem Service Pack 2 i Windows XP z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=768fd74e-0a2f-4353-ac22-65d0d6321739)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows XP z dodatkiem Service Pack 2 i Windows XP z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=cece4c55-0756-4357-9d2d-6709e8426068)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows XP z dodatkiem Service Pack 2 i Windows XP z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=e997ea40-668e-40df-bd50-0ca53437b375)<sup>[1]</sup>
(Ważny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Koder-dekoder głosu DirectShow WMA](http://www.microsoft.com/downloads/details.aspx?familyid=c116ae9d-e416-4b7d-be75-4b4b2ebcc33a)  
(KB969878)  
(Krytyczny)  
[Dekoder Windows Media Audio Voice](http://www.microsoft.com/downloads/details.aspx?familyid=4729de51-8fd8-46c6-b4ad-9c9f25202684)  
(KB954155)  
(Krytyczny)  
[Dekoder Windows Media Audio Voice](http://www.microsoft.com/downloads/details.aspx?familyid=fe0d51b2-345e-4eb7-a036-d8c3f6a683d2) w zestawie Windows Media Format SDK 9.5 x64 Edition  
(KB954155)  
(Krytyczny)  
[Dekoder Windows Media Audio Voice](http://www.microsoft.com/downloads/details.aspx?familyid=a866a490-6d3a-4ecd-acf4-770312ba2fd6) w zestawie Windows Media Format SDK 11  
(KB954155)  
(Krytyczny)  
[Menedżer kompresji audio](http://www.microsoft.com/downloads/details.aspx?familyid=46daf7c7-1cd3-4f47-9c7a-d5eb6ea7327b)  
(KB975025)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft Windows Media Player 6.4](http://www.microsoft.com/downloads/details.aspx?familyid=a9e7dfd8-7ba1-4f14-8e60-92ef00d91467)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=89a2cf2a-a7a2-4d4b-aa6f-24dde288d500)  
(Krytyczny)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=bd54e595-25f2-4839-a838-2a0f809bde2b)  
(Krytyczny)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=77b18fc2-e769-47c6-8e72-916716a49e58)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c08623bf-94bc-4c50-8c10-f50fb8448a0b)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f) (KB953297)  
(Krytyczny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 1 i Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=d4a328b5-5470-46b0-86c7-cfe0e6a3ea01) (KB953300)  
(Krytyczny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2 i Microsoft .NET Framework 3.5 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=491874d4-5eea-4545-9b7d-3861857c862e) (KB974417)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ad92503a-8c91-4d73-98b0-942d7961637d)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=819dd2d1-cad5-4784-9baf-185d8a76df5d)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ad29696d-4611-4a12-9dfa-74fa6866b759)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=270ec100-5ba1-4f8c-aa36-105d30ad57bf)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5459b7d4-1fab-4a04-ab9d-b8323505c1e2)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=17008892-7950-44c4-850d-002c8d73495f)<sup>[1]</sup>
(Ważny)
</td>
</tr>
<tr>
<th colspan="13">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS09-050**](http://go.microsoft.com/fwlink/?linkid=163970)
</td>
<td style="border:1px solid black;">
[**MS09-051**](http://go.microsoft.com/fwlink/?linkid=125438)
</td>
<td style="border:1px solid black;">
[**MS09-052**](http://go.microsoft.com/fwlink/?linkid=163913)
</td>
<td style="border:1px solid black;">
[**MS09-054**](http://go.microsoft.com/fwlink/?linkid=163979)
</td>
<td style="border:1px solid black;">
[**MS09-055**](http://technet.microsoft.com/security/bulletin/ms09-055)
</td>
<td style="border:1px solid black;">
[**MS09-061**](http://go.microsoft.com/fwlink/?linkid=160527)
</td>
<td style="border:1px solid black;">
[**MS09-062**](http://go.microsoft.com/fwlink/?linkid=161342)
</td>
<td style="border:1px solid black;">
[**MS09-053**](http://go.microsoft.com/fwlink/?linkid=164004)
</td>
<td style="border:1px solid black;">
[**MS09-056**](http://go.microsoft.com/fwlink/?linkid=163830)
</td>
<td style="border:1px solid black;">
[**MS09-057**](http://go.microsoft.com/fwlink/?linkid=163832)
</td>
<td style="border:1px solid black;">
[**MS09-058**](http://go.microsoft.com/fwlink/?linkid=162442)
</td>
<td style="border:1px solid black;">
[**MS09-059**](http://go.microsoft.com/fwlink/?linkid=163843)
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
[**Krytyczny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Krytyczny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Krytyczny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Umiarkowany**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
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
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Koder-dekoder głosu DirectShow WMA](http://www.microsoft.com/downloads/details.aspx?familyid=4fe0dff5-04d9-4409-8d1d-52419537126b)  
(KB969878)  
(Krytyczny)  
[Dekoder Windows Media Audio Voice](http://www.microsoft.com/downloads/details.aspx?familyid=00b3cb86-c9eb-4fbe-987e-2b0d94271d87)  
(KB954155)  
(Krytyczny)  
[Menedżer kompresji audio](http://www.microsoft.com/downloads/details.aspx?familyid=ab1803ff-2371-487f-a7b6-95747c46ba4e)  
(KB975025)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft Windows Media Player 6.4](http://www.microsoft.com/downloads/details.aspx?familyid=5f82d01c-573e-425e-b9f2-86a54f377b19)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=8101625d-ee93-46e5-aec2-3bdbf2d86472)  
(Krytyczny)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=4647bcf1-69fb-4ad6-9e03-7bc22d8a914b)  
(Krytyczny)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=9eae7eca-1a6f-4397-a6e2-7dda6b9d5276)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f3249c99-82e4-45dc-a254-28e647e822c8)  
(Umiarkowany)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d1b4a58b-f0b1-4400-a6e6-0255b0513bd1) (KB953298)  
(Ważny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 1 i Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=d4a328b5-5470-46b0-86c7-cfe0e6a3ea01) (KB953300)  
(Ważny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2 i Microsoft .NET Framework 3.5 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=491874d4-5eea-4545-9b7d-3861857c862e) (KB974417)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=414466a4-39a0-476d-9a43-ae7674cbd6a0)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=48256ea3-b433-4e84-9019-22300069cfc1)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d170cef9-f5d2-4fcd-997b-e778ad5a6797)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=78072164-84d1-44da-8ede-2a9d212d47a9)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1e3f3842-f8fd-4969-a2cf-706db38d7580)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9dff4662-7771-4bdc-87ec-7899d79b3a55)<sup>[1]</sup>
(Ważny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Koder-dekoder głosu DirectShow WMA](http://www.microsoft.com/downloads/details.aspx?familyid=c116ae9d-e416-4b7d-be75-4b4b2ebcc33a)  
(KB969878)  
(Krytyczny)  
[Dekoder Windows Media Audio Voice](http://www.microsoft.com/downloads/details.aspx?familyid=13ba4839-7fa9-4bbb-95f6-3fafb6c49f20)  
(KB954155)  
(Krytyczny)  
[Dekoder Windows Media Audio Voice](http://www.microsoft.com/downloads/details.aspx?familyid=fe0d51b2-345e-4eb7-a036-d8c3f6a683d2) w zestawie Windows Media Format SDK 9.5 x64 Edition  
(KB954155)  
(Krytyczny)  
[Menedżer kompresji audio](http://www.microsoft.com/downloads/details.aspx?familyid=46daf7c7-1cd3-4f47-9c7a-d5eb6ea7327b)  
(KB975025)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft Windows Media Player 6.4](http://www.microsoft.com/downloads/details.aspx?familyid=65e9036e-2e1b-40ff-a84b-c507107bcce8)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=2f966053-01eb-4a23-a9d5-71deac2498ea)  
(Krytyczny)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=e7d77bd9-8317-42f3-9ad1-a0b8bfa65b53)  
(Krytyczny)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=708a549d-11fd-43bf-a6e1-309e3205d59d)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1ad3f7b3-58d5-4507-ae20-a265e47cee9c)  
(Umiarkowany)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f) (KB953297)  
(Ważny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 1 i Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=d4a328b5-5470-46b0-86c7-cfe0e6a3ea01) (KB953300)  
(Ważny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2 i Microsoft .NET Framework 3.5 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=491874d4-5eea-4545-9b7d-3861857c862e) (KB974417)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=eb95e8d9-6ef5-4526-99d2-507e50de049b)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=61bded07-201e-4815-ac1e-468bf907e063)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d170cef9-f5d2-4fcd-997b-e778ad5a6797)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8aa1f97d-ad53-4450-bb93-4a147dd10a87)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=95286b8d-4b53-4e6c-af59-e9e18fad3559)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8df7a2d9-2f97-4f18-84e8-415a1632cf09)<sup>[1]</sup>
(Ważny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium
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
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=79a1a94d-3b47-47e9-9476-2f591c3f6a59)  
(Krytyczny)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=07e66c09-2cd7-47ba-bf87-d3da602184b4)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=575e75d9-e348-4fbb-9eaa-43240e4d715e)  
(Umiarkowany)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f) (KB953297)  
(Ważny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 1 i Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=d4a328b5-5470-46b0-86c7-cfe0e6a3ea01) (KB953300)  
(Ważny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2 i Microsoft .NET Framework 3.5 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=491874d4-5eea-4545-9b7d-3861857c862e) (KB974417)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=a678ceb9-a37a-4c29-8bd1-f209922990e5)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=b99d4d9b-e0cc-4a8c-ad99-6a53958b37c8)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=2ede1eb9-7f5f-411d-bbc3-5db46d80e0bb)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=fb5678b9-5ef1-42db-902e-c9ea02880e0a)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=faef714b-5f46-47f2-bea7-881df05a1bc0)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=83c77015-7f96-4c0d-bd56-60aef90ea2f8)<sup>[1]</sup>
(Ważny)
</td>
</tr>
<tr>
<th colspan="13">
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS09-050**](http://go.microsoft.com/fwlink/?linkid=163970)
</td>
<td style="border:1px solid black;">
[**MS09-051**](http://go.microsoft.com/fwlink/?linkid=125438)
</td>
<td style="border:1px solid black;">
[**MS09-052**](http://go.microsoft.com/fwlink/?linkid=163913)
</td>
<td style="border:1px solid black;">
[**MS09-054**](http://go.microsoft.com/fwlink/?linkid=163979)
</td>
<td style="border:1px solid black;">
[**MS09-055**](http://technet.microsoft.com/security/bulletin/ms09-055)
</td>
<td style="border:1px solid black;">
[**MS09-061**](http://go.microsoft.com/fwlink/?linkid=160527)
</td>
<td style="border:1px solid black;">
[**MS09-062**](http://go.microsoft.com/fwlink/?linkid=161342)
</td>
<td style="border:1px solid black;">
[**MS09-053**](http://go.microsoft.com/fwlink/?linkid=164004)
</td>
<td style="border:1px solid black;">
[**MS09-056**](http://go.microsoft.com/fwlink/?linkid=163830)
</td>
<td style="border:1px solid black;">
[**MS09-057**](http://go.microsoft.com/fwlink/?linkid=163832)
</td>
<td style="border:1px solid black;">
[**MS09-058**](http://go.microsoft.com/fwlink/?linkid=162442)
</td>
<td style="border:1px solid black;">
[**MS09-059**](http://go.microsoft.com/fwlink/?linkid=163843)
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
<td style="border:1px solid black;">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista z dodatkiem Service Pack 1 i Windows Vista z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=29842c0c-8930-4b5f-83c6-1a718974b63f)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Dekoder Windows Media Audio Voice](http://www.microsoft.com/downloads/details.aspx?familyid=f17ee0ea-f1e2-49f4-9f90-60296246ddfe)  
(KB954155)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=f6995616-2a84-4c26-9599-26f1314873ed)  
(Krytyczny)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=e8f6014f-950b-4e11-a105-51d298069f1a)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista z dodatkiem Service Pack 1 i Windows Vista z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7313c03b-8844-4086-a0cc-43dfdb3ca48c)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f) (KB953297)  
(Krytyczny)  
[Microsoft .NET Framework 2.0](http://www.microsoft.com/downloads/details.aspx?familyid=6f99521e-86b3-4083-9132-e5ac06d40b63) (KB974468)  
(Krytyczny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 1 i Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=3cf329c6-6d3d-41eb-bb72-8ba241df0882) (KB974292)  
(Krytyczny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2 i Microsoft .NET Framework 3.5 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7438eb1e-6e86-4aa1-b1f4-f71a7699d233) (KB974467)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Vista i Windows Vista z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=19aa01f3-026d-4264-85f8-216d0597969b)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista z dodatkiem Service Pack 1 i Windows Vista z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=bb96eb1c-66a2-4276-9773-eea22179bcd4)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista z dodatkiem Service Pack 1 i Windows Vista z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8b5a9a95-9439-40c8-acef-000b919daa04)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Vista i Windows Vista z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=acf6f3e6-282e-4f05-9060-8d0ebb874b97)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista z dodatkiem Service Pack 1 i Windows Vista z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=04ae306b-0d0d-4767-ab54-cc11aec477ed)  
(Ważny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista z dodatkiem Service Pack 1
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f) (KB953297)  
(Krytyczny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=30e5410d-0942-4964-9037-52330488efda) (KB974291)  
(Krytyczny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2 i Microsoft .NET Framework 3.5 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=72fe9066-2397-439d-82fb-2b7f9d2bcce8) (KB974469)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f) (KB953297)  
(Krytyczny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=614a92ee-0512-4ccc-b6b8-32ebcec8e6a4) (KB974470)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Vista z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=acf6f3e6-282e-4f05-9060-8d0ebb874b97)  
(Umiarkowany)
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition z dodatkiem Service Pack 1 i Windows Vista x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=62ed5d0a-5ca6-4942-80c9-7808b14cb6b5)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Dekoder Windows Media Audio Voice](http://www.microsoft.com/downloads/details.aspx?familyid=26905f12-92c7-4d45-99e7-227f03d2cb82)  
(KB954155)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=b3de5236-afdd-436e-8648-5382d564cc99)  
(Krytyczny)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=85978f28-5fc0-481b-9b03-2021c785889b)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition z dodatkiem Service Pack 1 i Windows Vista x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7216bcb1-ff16-402b-ad1b-1500d46d0157)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f) (KB953297)  
(Krytyczny)  
[Microsoft .NET Framework 2.0](http://www.microsoft.com/downloads/details.aspx?familyid=6f99521e-86b3-4083-9132-e5ac06d40b63) (KB974468)  
(Krytyczny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 1 i Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=3cf329c6-6d3d-41eb-bb72-8ba241df0882) (KB974292)  
(Krytyczny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2 i Microsoft .NET Framework 3.5 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7438eb1e-6e86-4aa1-b1f4-f71a7699d233) (KB974467)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition i Windows Vista x64 Edition z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=8f5f0c1d-1dd6-47fa-aef2-d3c96c8fc06e)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition z dodatkiem Service Pack 1 i Windows Vista x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=bce096c8-833b-45c8-99cd-1280f0744f2f)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition z dodatkiem Service Pack 1 i Windows Vista x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4a60f789-1a4a-49a8-8d13-fda989ed40be)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition i Windows Vista x64 Edition z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=13a3fe0b-e300-4568-aa08-d586ab8d5434)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition z dodatkiem Service Pack 1 i Windows Vista x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=58c995ca-f308-4e07-8e60-2e542384d95d)  
(Ważny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition z dodatkiem Service Pack 1
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f) (KB953297)  
(Krytyczny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=30e5410d-0942-4964-9037-52330488efda) (KB974291)  
(Krytyczny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2 i Microsoft .NET Framework 3.5 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=72fe9066-2397-439d-82fb-2b7f9d2bcce8) (KB974469)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f) (KB953297)  
(Krytyczny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=614a92ee-0512-4ccc-b6b8-32ebcec8e6a4) (KB974470)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=13a3fe0b-e300-4568-aa08-d586ab8d5434)  
(Umiarkowany)
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
</tr>
<tr>
<th colspan="13">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS09-050**](http://go.microsoft.com/fwlink/?linkid=163970)
</td>
<td style="border:1px solid black;">
[**MS09-051**](http://go.microsoft.com/fwlink/?linkid=125438)
</td>
<td style="border:1px solid black;">
[**MS09-052**](http://go.microsoft.com/fwlink/?linkid=163913)
</td>
<td style="border:1px solid black;">
[**MS09-054**](http://go.microsoft.com/fwlink/?linkid=163979)
</td>
<td style="border:1px solid black;">
[**MS09-055**](http://technet.microsoft.com/security/bulletin/ms09-055)
</td>
<td style="border:1px solid black;">
[**MS09-061**](http://go.microsoft.com/fwlink/?linkid=160527)
</td>
<td style="border:1px solid black;">
[**MS09-062**](http://go.microsoft.com/fwlink/?linkid=161342)
</td>
<td style="border:1px solid black;">
[**MS09-053**](http://go.microsoft.com/fwlink/?linkid=164004)
</td>
<td style="border:1px solid black;">
[**MS09-056**](http://go.microsoft.com/fwlink/?linkid=163830)
</td>
<td style="border:1px solid black;">
[**MS09-057**](http://go.microsoft.com/fwlink/?linkid=163832)
</td>
<td style="border:1px solid black;">
[**MS09-058**](http://go.microsoft.com/fwlink/?linkid=162442)
</td>
<td style="border:1px solid black;">
[**MS09-059**](http://go.microsoft.com/fwlink/?linkid=163843)
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
<td style="border:1px solid black;">
[**Krytyczny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Niski**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
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
[Windows Server 2008 dla systemów 32-bitowych i Windows Server 2008 z dodatkiem Service Pack 2 dla systemów 32-bitowych\*](http://www.microsoft.com/downloads/details.aspx?familyid=ff6bfcf3-76c9-4c45-b57d-22f94458dd6e)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Dekoder głosu Windows Media Audio](http://www.microsoft.com/downloads/details.aspx?familyid=2eaa9857-a147-4f31-9bf4-b9e2cf4c15c3)\*\*  
(KB954155)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=72dd580e-eb53-41da-a5c0-a392ad388bfc)\*\*  
(Krytyczny)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=1baf7e96-ba3e-47e7-8ea3-eb092e653a39)\*\*  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów 32-bitowych i Windows Server 2008 z dodatkiem Service Pack 2 dla systemów 32-bitowych](http://www.microsoft.com/downloads/details.aspx?familyid=51eb56fa-8204-45f3-86d7-6d03a2c8d78d)\*\*  
(Niski)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f)\*\*  
(KB953297)  
(Ważny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=30e5410d-0942-4964-9037-52330488efda)\*\*  
(KB974291)  
(Ważny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2 i Microsoft .NET Framework 3.5 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=72fe9066-2397-439d-82fb-2b7f9d2bcce8)\*\*  
(KB974469)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów 32-bitowych](http://www.microsoft.com/downloads/details.aspx?familyid=fd1694af-8873-43aa-9243-91f7cde452b7)\*\*  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów 32-bitowych i Windows Server 2008 z dodatkiem Service Pack 2 dla systemów 32-bitowych\*](http://www.microsoft.com/downloads/details.aspx?familyid=d9c5039f-d0cf-4d84-850f-f2f7701dcb79)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów 32-bitowych i Windows Server 2008 z dodatkiem Service Pack 2 dla systemów 32-bitowych\*](http://www.microsoft.com/downloads/details.aspx?familyid=f9b487af-fe73-42a8-b240-d59c4321f95b)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów 32-bitowych\*](http://www.microsoft.com/downloads/details.aspx?familyid=71aec6f6-a36b-465e-8885-b094dfd30423)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów 32-bitowych i Windows Server 2008 z dodatkiem Service Pack 2 dla systemów 32-bitowych\*](http://www.microsoft.com/downloads/details.aspx?familyid=f2f617c2-f149-4e9b-bfdd-08ed0f3f99db)  
(Ważny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 z dodatkiem Service Pack 2 dla systemów 32-bitowych
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f)\*\*  
(KB953297)  
(Ważny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=614a92ee-0512-4ccc-b6b8-32ebcec8e6a4)\*\*  
(KB974470)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów 32-bitowych z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=71aec6f6-a36b-465e-8885-b094dfd30423)\*  
(Umiarkowany)
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 dla systemów opartych na procesorach X64
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem x64 i Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem x64\*](http://www.microsoft.com/downloads/details.aspx?familyid=aff6f9c7-4a72-48f2-b750-204d796c7daa)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Dekoder głosu Windows Media Audio](http://www.microsoft.com/downloads/details.aspx?familyid=70aabba3-53d6-4b52-be83-6d3f3869ecbd)\*\*  
(KB954155)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=0111d741-bda4-4a50-a12b-d3337ff4441d)\*\*  
(Krytyczny)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=7a4b755b-7fa0-43aa-8862-c1d0c7d94c2c)\*\*  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem x64 i Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=131b047a-ae93-4a99-83e5-71d5a79e96ea)\*\*  
(Niski)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f)\*\*  
(KB953297)  
(Ważny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=30e5410d-0942-4964-9037-52330488efda)\*\*  
(KB974291)  
(Ważny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2 i Microsoft .NET Framework 3.5 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=72fe9066-2397-439d-82fb-2b7f9d2bcce8)\*\*  
(KB974469)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów opartych na procesorach x64](http://www.microsoft.com/downloads/details.aspx?familyid=41bc4cdb-273a-4a6e-80d9-c8ce20e32da9)\*\*  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem x64 i Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem x64\*](http://www.microsoft.com/downloads/details.aspx?familyid=db969ddc-708e-42b7-9956-6c27bf346bbb)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem x64 i Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem x64\*](http://www.microsoft.com/downloads/details.aspx?familyid=0d8a2a3e-d7d4-47fb-8364-16fce28e4d38)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów opartych na procesorach X64](http://www.microsoft.com/downloads/details.aspx?familyid=88f4189f-71fe-404a-869e-3f76692acf94)\*  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem x64 i Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem x64\*](http://www.microsoft.com/downloads/details.aspx?familyid=deb84cb8-2ba3-47e3-9185-2bbc5b0a7e18)  
(Ważny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem x64
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f)\*\*  
(KB953297)  
(Ważny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=614a92ee-0512-4ccc-b6b8-32ebcec8e6a4)\*\*  
(KB974470)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem x64 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=88f4189f-71fe-404a-869e-3f76692acf94)\*  
(Umiarkowany)
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 dla systemów z procesorem Itanium
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem Itanium i Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=7b70108b-7f59-4898-ab4e-76be990de878)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=e81f30b7-ef05-4488-b62a-d330e17129cf)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem Itanium i Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=3d16c5bf-ee5c-4220-9755-5cb92eac2aae)  
(Niski)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f)  
(KB953297)  
(Ważny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=30e5410d-0942-4964-9037-52330488efda)  
(KB974291)  
(Ważny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2 oraz Microsoft .NET Framework 3.5 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=72fe9066-2397-439d-82fb-2b7f9d2bcce8)  
(KB974469)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=a4f42085-1cb9-4b8d-a931-85be71fdf06d)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem Itanium i Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=a221451a-cb4e-4a43-a225-4b1e86e87525)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem Itanium i Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=8962f0b6-f346-4e88-9d83-4d15b699dd9d)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=3e0f0b1c-ca5d-43fc-9770-73396a5f191c)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem Itanium i Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=4aac0e3e-9b49-4a4a-ab17-707ff03b4d9b)  
(Ważny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem Itanium
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f)  
(KB953297)  
(Ważny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=614a92ee-0512-4ccc-b6b8-32ebcec8e6a4)  
(KB974470)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=3e0f0b1c-ca5d-43fc-9770-73396a5f191c)  
(Umiarkowany)
</td>
<td style="border:1px solid black;">
Analogicznie jak wyżej
</td>
</tr>
<tr>
<th colspan="13">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS09-050**](http://go.microsoft.com/fwlink/?linkid=163970)
</td>
<td style="border:1px solid black;">
[**MS09-051**](http://go.microsoft.com/fwlink/?linkid=125438)
</td>
<td style="border:1px solid black;">
[**MS09-052**](http://go.microsoft.com/fwlink/?linkid=163913)
</td>
<td style="border:1px solid black;">
[**MS09-054**](http://go.microsoft.com/fwlink/?linkid=163979)
</td>
<td style="border:1px solid black;">
[**MS09-055**](http://technet.microsoft.com/security/bulletin/ms09-055)
</td>
<td style="border:1px solid black;">
[**MS09-061**](http://go.microsoft.com/fwlink/?linkid=160527)
</td>
<td style="border:1px solid black;">
[**MS09-062**](http://go.microsoft.com/fwlink/?linkid=161342)
</td>
<td style="border:1px solid black;">
[**MS09-053**](http://go.microsoft.com/fwlink/?linkid=164004)
</td>
<td style="border:1px solid black;">
[**MS09-056**](http://go.microsoft.com/fwlink/?linkid=163830)
</td>
<td style="border:1px solid black;">
[**MS09-057**](http://go.microsoft.com/fwlink/?linkid=163832)
</td>
<td style="border:1px solid black;">
[**MS09-058**](http://go.microsoft.com/fwlink/?linkid=162442)
</td>
<td style="border:1px solid black;">
[**MS09-059**](http://go.microsoft.com/fwlink/?linkid=163843)
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
<td style="border:1px solid black;">
Brak
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 dla systemów 32-bitowych
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
<td style="border:1px solid black;">
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=89d1fb78-68cd-48dd-afc2-15a79ebe9fde)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows 7 dla systemów 32-bitowych](http://www.microsoft.com/downloads/details.aspx?familyid=b64bcc14-38a7-45b9-8f85-acc573777506)  
(Ważny)
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
<td style="border:1px solid black;">
[Windows 7 dla systemów 32-bitowych](http://www.microsoft.com/downloads/details.aspx?familyid=ad6f06d5-27db-445d-a8b2-c42adc90afc0)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows 7 dla systemów 32-bitowych](http://www.microsoft.com/downloads/details.aspx?familyid=35b85783-90df-4f67-a3cb-02351432133e)  
(Ważny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 dla systemów z procesorem x64
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
<td style="border:1px solid black;">
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=10d9f7ac-65f4-437c-91cc-171632c69b0e)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows 7 dla systemów z procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=809e29f3-ec68-4a2b-b04e-11759dd16001)  
(Ważny)
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
<td style="border:1px solid black;">
[Windows 7 dla systemów z procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=70cd0270-77e9-492a-82d9-798364640c10)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows 7 dla systemów z procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=97010f2c-6c10-4fda-84fd-6c8749968db5)  
(Ważny)
</td>
</tr>
<tr>
<th colspan="13">
System Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS09-050**](http://go.microsoft.com/fwlink/?linkid=163970)
</td>
<td style="border:1px solid black;">
[**MS09-051**](http://go.microsoft.com/fwlink/?linkid=125438)
</td>
<td style="border:1px solid black;">
[**MS09-052**](http://go.microsoft.com/fwlink/?linkid=163913)
</td>
<td style="border:1px solid black;">
[**MS09-054**](http://go.microsoft.com/fwlink/?linkid=163979)
</td>
<td style="border:1px solid black;">
[**MS09-055**](http://technet.microsoft.com/security/bulletin/ms09-055)
</td>
<td style="border:1px solid black;">
[**MS09-061**](http://go.microsoft.com/fwlink/?linkid=160527)
</td>
<td style="border:1px solid black;">
[**MS09-062**](http://go.microsoft.com/fwlink/?linkid=161342)
</td>
<td style="border:1px solid black;">
[**MS09-053**](http://go.microsoft.com/fwlink/?linkid=164004)
</td>
<td style="border:1px solid black;">
[**MS09-056**](http://go.microsoft.com/fwlink/?linkid=163830)
</td>
<td style="border:1px solid black;">
[**MS09-057**](http://go.microsoft.com/fwlink/?linkid=163832)
</td>
<td style="border:1px solid black;">
[**MS09-058**](http://go.microsoft.com/fwlink/?linkid=162442)
</td>
<td style="border:1px solid black;">
[**MS09-059**](http://go.microsoft.com/fwlink/?linkid=163843)
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
<td style="border:1px solid black;">
Brak
</td>
<td style="border:1px solid black;">
[**Krytyczny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Niski**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Brak
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
Windows Server 2008 R2 dla systemów opartych na procesorach x64
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
<td style="border:1px solid black;">
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=f50307d6-7869-4996-9ff7-23f87d08994b)\*\*  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach x64](http://www.microsoft.com/downloads/details.aspx?familyid=bcd2b944-6852-48f2-820b-cce7d195e391)\*\*  
(Niski)
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
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach x64](http://www.microsoft.com/downloads/details.aspx?familyid=ce78c019-ec08-4ec6-abec-334f5ec5cb76)\*  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach x64](http://www.microsoft.com/downloads/details.aspx?familyid=597ac3a7-e02d-49a5-9b8e-d097e867acea)\*  
(Ważny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 dla systemów opartych na procesorach Itanium
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
<td style="border:1px solid black;">
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=9b6a28ae-b3f2-42b0-8209-e3950ec37abb)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=85e76e55-3766-4ffe-9a18-8655de935b7c)  
(Niski)
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
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=6442a77a-3c0d-4beb-b2d2-2885376c2135)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=abc94857-37d8-4bb8-ad9e-46e687fca40e)  
(Ważny)
</td>
</tr>
</table>
 
**Uwagi dotyczące systemu Windows Server 2008 i Windows Server 2008 R2**

**\*Luka w zabezpieczeniach dotyczy instalacji Server Core.** Ta aktualizacja ma zastosowanie, z takim samym wskaźnikiem ważności, w przypadku obsługiwanych wersji systemu Windows Server 2008 lub Windows Server 2008 R2, niezależnie od tego, czy zostały zainstalowane przy użyciu opcji instalacji Server Core. Aby uzyskać więcej informacji na temat tej opcji instalacji, zobacz artykuły MSDN, [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx) (j. ang.) i [Server Core for Windows Server 2008 R2](http://msdn.microsoft.com/en-us/library/ee391631(vs.85).aspx) (j. ang.). Należy pamiętać, że opcja instalacji Server Core nie dotyczy niektórych wersji systemu Windows Server 2008 i Windows Server 2008 R2. Zobacz [Porównanie opcji instalacji Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Luka w zabezpieczeniach nie dotyczy instalacji Server Core.** Luki usuwane przez tę aktualizację zabezpieczeń nie dotyczą obsługiwanych wersji systemu Windows Server 2008 ani Windows Server 2008 R2, jeżeli systemy te zostały zainstalowane przy użyciu opcji instalacji Server Core. Aby uzyskać więcej informacji na temat tej opcji instalacji, zobacz artykuły MSDN, [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx) (j. ang.) i [Server Core for Windows Server 2008 R2](http://msdn.microsoft.com/en-us/library/ee391631(vs.85).aspx) (j. ang.). Należy pamiętać, że opcja instalacji Server Core nie dotyczy niektórych wersji systemu Windows Server 2008 i Windows Server 2008 R2. Zobacz [Porównanie opcji instalacji Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**Uwaga dotycząca biuletynu MS09-061**

Zobacz także pozostałe kategorie oprogramowania w sekcji **Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki**, aby uzyskać więcej plików aktualizacji w ramach tego samego identyfikatora biuletynu. Ten biuletyn obejmuje więcej niż jedną kategorię oprogramowania.

**Uwagi dotyczące biuletynu MS09-062**

Zobacz także pozostałe kategorie oprogramowania w sekcji **Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki**, aby uzyskać więcej plików aktualizacji w ramach tego samego identyfikatora biuletynu. Ten biuletyn obejmuje więcej niż jedną kategorię oprogramowania.

**Uwaga dotycząca biuletynu MS09-059**

<sup>[1]</sup>Luka dotyczy tego systemu operacyjnego jedynie w przypadku, gdy zainstalowano w nim aktualizację KB968389 związaną z rozszerzoną ochroną uwierzytelniania (zobacz [Poradnik zabezpieczeń firmy Microsoft 973811](http://technet.microsoft.com/security/advisory/973811)). Więcej informacji można znaleźć we wpisie w sekcji Często zadawane pytania dotyczące tej aktualizacji zabezpieczeń w biuletynie [MS09-059](http://go.microsoft.com/fwlink/?linkid=163843).

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
Pakiety Microsoft Office, systemy i ich składniki
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS09-060**](http://go.microsoft.com/fwlink/?linkid=160633)
</td>
<td style="border:1px solid black;">
[**MS09-062**](http://go.microsoft.com/fwlink/?linkid=161342)
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
Microsoft Office XP
</td>
<td style="border:1px solid black;">
[Microsoft Outlook 2002 z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=04878c2c-eb97-426f-be08-89036a6799db)  
(KB973702)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft Office XP z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=b4ac7fbe-dd19-4940-a576-89a6b7ed602d)<sup>[2]</sup>
(KB974811)  
(Ważny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2003
</td>
<td style="border:1px solid black;">
[Microsoft Office Outlook 2003 z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=79e2b2e8-d5e8-4014-b489-720af2b5083d)  
(KB973705)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2003 z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=48752ab4-5928-476d-a8bc-e998d188b1f7)<sup>[3]</sup>
(KB972580)  
(Ważny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Pakiet Microsoft Office 2007
</td>
<td style="border:1px solid black;">
[Microsoft Office Outlook 2007 z dodatkiem Service Pack 1 i Microsoft Office Outlook 2007 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d39234a3-c62c-44ba-a626-3179a183ca09)  
(KB972363)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Pakiet Microsoft Office System 2007 z dodatkiem Service Pack 1 i pakiet Microsoft Office System 2007 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=98d7c4ab-f8ca-4806-a609-453fb29b02ec)\[4\]  
(KB972581)  
(Ważny)
</td>
</tr>
<tr>
<th colspan="3">
Inne programy pakietu Microsoft Office
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS09-060**](http://go.microsoft.com/fwlink/?linkid=160633)
</td>
<td style="border:1px solid black;">
[**MS09-062**](http://go.microsoft.com/fwlink/?linkid=161342)
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visio
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Microsoft Visio 2002 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=920ee70b-c5c1-47b5-8f33-938ffe14eea4)  
(KB975365)  
(Ważny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Visio Viewer
</td>
<td style="border:1px solid black;">
Podgląd programu Microsoft Visio 2002<sup>[1]</sup>
(Krytyczny)  
Microsoft Office Visio 2003 Viewer<sup>[1]</sup>
(Krytyczny)  
[Microsoft Office Visio Viewer 2007 z dodatkiem Service Pack 1 i Microsoft Office Visio Viewer 2007 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d20004c5-dd01-459e-8120-5f127e20c085)  
(KB973709)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft Office Visio Viewer 2007 z dodatkiem Service Pack 1 i Microsoft Office Visio Viewer 2007 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=98d7c4ab-f8ca-4806-a609-453fb29b02ec)\[4\]  
(KB972581)  
(Ważny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Project
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Microsoft Office Project 2002 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=b4ac7fbe-dd19-4940-a576-89a6b7ed602d)<sup>[2]</sup>
(KB974811)  
(Ważny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Word Viewer, Microsoft Office Excel Viewer i Microsoft PowerPoint Viewer
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Przeglądarka programu Microsoft Word 2003 z dodatkiem Service Pack 3 i Przeglądarka programu Microsoft Office Excel 2003 z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=48752ab4-5928-476d-a8bc-e998d188b1f7)<sup>[3]</sup>
(KB972580)  
(Ważny)  
[Przeglądarka programu Microsoft Office Excel z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=98d7c4ab-f8ca-4806-a609-453fb29b02ec)\[4\]  
(KB972581)  
(Ważny)  
[Podgląd programu PowerPoint 2007 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=98d7c4ab-f8ca-4806-a609-453fb29b02ec)\[4\]  
(KB972581)  
(Ważny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Pakiet zgodności formatu plików pakietu Microsoft Office dla programów Word, Excel i PowerPoint 2007
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Pakiet zgodności formatu plików pakietu Microsoft Office dla programów Word, Excel i PowerPoint 2007 z dodatkiem Service Pack 1 i Pakiet zgodności formatu plików pakietu Microsoft Office dla programów Word, Excel i PowerPoint 2007 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=98d7c4ab-f8ca-4806-a609-453fb29b02ec)\[4\]  
(KB972581)  
Ważny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Works
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Microsoft Works 8.5](http://www.microsoft.com/downloads/details.aspx?familyid=6f96de9a-62d8-428f-9567-51d55c129be6)  
(KB973636)  
(Ważny)
</td>
</tr>
</table>
 
**Uwagi dotyczące biuletynu MS09-060**

<sup>[1]</sup>Firma Microsoft zaleca, aby użytkownicy programów Microsoft Visio Viewer 2002 oraz Microsoft Visio Viewer 2003 dokonali aktualizacji do programu Microsoft Office Visio Viewer 2007 Service Pack 2.

**Uwagi dotyczące biuletynu MS09-062**

<sup>[2]</sup>Te aktualizacje są identyczne.

<sup>[3]</sup>Te aktualizacje są identyczne.

\[4\]Te aktualizacje są identyczne.

Zobacz także pozostałe kategorie oprogramowania w sekcji **Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki**, aby uzyskać więcej plików aktualizacji w ramach tego samego identyfikatora biuletynu. Ten biuletyn obejmuje więcej niż jedną kategorię oprogramowania.

#### Oprogramowanie serwerów firmy Microsoft

 
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
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
[**MS09-062**](http://go.microsoft.com/fwlink/?linkid=161342)
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
SQL Server 2000 Reporting Services z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
Aktualizacja GDR  
Nie dotyczy  
Aktualizacja QFE:  
[SQL Server 2000 Reporting Services z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=33554f96-5af7-4683-a537-9db293b67b8d)  
(KB970899)  
(Krytyczny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
SQL Server 2005 z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
Aktualizacja GDR:  
[SQL Server 2005 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d971a262-1dfb-498c-a4f3-59fdc1b85d23)<sup>[1]</sup>
(KB970895)  
(Krytyczny)  
Aktualizacja QFE:  
[SQL Server 2005 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=76d3d653-e9a0-48bc-afae-d3553f7b9235)<sup>[1]</sup>
(KB970896)  
(Krytyczny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
SQL Server 2005 x64 Edition z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
Aktualizacja GDR:  
[SQL Server 2005 x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d971a262-1dfb-498c-a4f3-59fdc1b85d23)<sup>[1]</sup>
(KB970895)  
(Krytyczny)  
Aktualizacja QFE:  
[SQL Server 2005 x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=76d3d653-e9a0-48bc-afae-d3553f7b9235)<sup>[1]</sup>
(KB970896)  
(Krytyczny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
SQL Server 2005 dla systemów z procesorem Itanium z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
Aktualizacja GDR:  
[SQL Server 2005 dla systemów z procesorem Itanium z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d971a262-1dfb-498c-a4f3-59fdc1b85d23)<sup>[1]</sup>
(KB970895)  
(Krytyczny)  
Aktualizacja QFE:  
[SQL Server 2005 dla systemów z procesorem Itanium z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=76d3d653-e9a0-48bc-afae-d3553f7b9235)<sup>[1]</sup>
(KB970896)  
(Krytyczny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
SQL Server 2005 z dodatkiem Service Pack 3
</td>
<td style="border:1px solid black;">
Aktualizacja GDR  
[SQL Server 2005 z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=0d878f4b-71e8-4170-9a14-1bce684811ce)<sup>[2]</sup>
(KB970892)  
(Krytyczny)  
Aktualizacja QFE:  
[SQL Server 2005 z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=e6f307c1-8b21-406e-9c6f-b1a3a1e9a98f)<sup>[2]</sup>
(KB970894)  
(Krytyczny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
SQL Server 2005 x64 Edition z dodatkiem Service Pack 3
</td>
<td style="border:1px solid black;">
Aktualizacja GDR:  
[SQL Server 2005 x64 Edition z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=0d878f4b-71e8-4170-9a14-1bce684811ce)<sup>[2]</sup>
(KB970892)  
(Krytyczny)  
Aktualizacja QFE:  
[SQL Server 2005 x64 Edition z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=e6f307c1-8b21-406e-9c6f-b1a3a1e9a98f)<sup>[2]</sup>
(KB970894)  
(Krytyczny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
SQL Server 2005 dla systemów z procesorem Itanium z dodatkiem Service Pack 3
</td>
<td style="border:1px solid black;">
Aktualizacja GDR:  
[SQL Server 2005 dla systemów z procesorem Itanium z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=0d878f4b-71e8-4170-9a14-1bce684811ce)<sup>[2]</sup>
(KB970892)  
(Krytyczny)  
Aktualizacja QFE:  
[SQL Server 2005 dla systemów z procesorem Itanium z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=e6f307c1-8b21-406e-9c6f-b1a3a1e9a98f)<sup>[2]</sup>
(KB970894)  
(Krytyczny)
</td>
</tr>
</table>
 
**Uwaga dotycząca biuletynu MS09-062**

<sup>[1]</sup>Użytkownicy programu SQL Server 2005 z dodatkiem Service Pack 2, korzystający z usług Reporting Services za pomocą programu SharePoint, muszą również zainstalować [Dodatek Reporting Services dla programu Microsoft SQL Server 2005 dla dodatku Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=%20f4d4d0ae-e5d4-4ed1-8d78-7137578161ce&displaylang=en) z witryny Centrum pobierania Microsoft.

<sup>[2]</sup>Użytkownicy programu SQL Server 2005 z dodatkiem Service Pack 3, korzystający z usług Reporting Services za pomocą programu SharePoint, muszą również zainstalować [Dodatek Reporting Services dla programu Microsoft SQL Server 2005 dla dodatku Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=%20648766ac-2a35-4238-a3f4-c26d7077f2a9&displaylang=en) z witryny Centrum pobierania Microsoft.

Zobacz także pozostałe kategorie oprogramowania w sekcji **Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki**, aby uzyskać więcej plików aktualizacji w ramach tego samego identyfikatora biuletynu. Ten biuletyn obejmuje więcej niż jedną kategorię oprogramowania.

#### Narzędzia i oprogramowanie firmy Microsoft dla deweloperów

 
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
Microsoft Silverlight
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS09-061**](http://go.microsoft.com/fwlink/?linkid=160527)
</td>
<td style="border:1px solid black;">
[**MS09-062**](http://go.microsoft.com/fwlink/?linkid=161342)
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
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Silverlight
</td>
<td style="border:1px solid black;">
[Microsoft Silverlight 2](http://www.microsoft.com/silverlight/get-started/install/default.aspx)<sup>[1]</sup> na komputerach Macintosh  
(KB970363)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Silverlight
</td>
<td style="border:1px solid black;">
[Microsoft Silverlight 2](http://www.microsoft.com/silverlight/get-started/install/default.aspx)<sup>[1]</sup> we wszystkich wersjach klientów systemu Microsoft Windows  
(KB970363)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Silverlight
</td>
<td style="border:1px solid black;">
[Microsoft Silverlight 2](http://www.microsoft.com/silverlight/get-started/install/default.aspx)<sup>[1]</sup> we wszystkich wersjach serwerów systemu Microsoft Windows\*\*  
(KB970363)  
(Umiarkowany)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr>
<th colspan="3">
Microsoft Visual Studio
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS09-061**](http://go.microsoft.com/fwlink/?linkid=160527)
</td>
<td style="border:1px solid black;">
[**MS09-062**](http://go.microsoft.com/fwlink/?linkid=161342)
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
Brak
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual Studio .NET 2003 z dodatkiem Service Pack 1
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio .NET 2003 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=9e3b52d3-b211-4d62-891c-ae8f2e4ffc6c)  
(KB971022)  
(Brak wskaźnika ważności<sup>[2]</sup>)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visual Studio 2005 z dodatkiem Service Pack 1
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio 2005 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=e186aeed-e9d7-4a02-84b3-bbed116ca060)  
(KB971023)  
(Brak wskaźnika ważności<sup>[2]</sup>)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual Studio 2008
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio 2008](http://www.microsoft.com/downloads/details.aspx?familyid=4fa10c93-ce20-43df-a725-ef4c77353747)  
(KB972221)  
(Brak wskaźnika ważności<sup>[2]</sup>)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visual Studio 2008 z dodatkiem Service Pack 1
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio 2008 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=b904dee8-8a26-43f8-8ca9-86ad12cfdb52)  
(KB972222)  
(Brak wskaźnika ważności<sup>[2]</sup>)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual FoxPro 8.0 z dodatkiem Service Pack 1 zainstalowany w systemie Microsoft Windows 2000 z dodatkiem Service Pack 4  
(KB971104)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Microsoft Visual FoxPro 8.0 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=e5d0d515-4b36-4025-bc6f-1c5cdf09e1af)  
zainstalowany w systemie Microsoft Windows 2000 z dodatkiem Service Pack 4  
(KB971104)  
(Brak wskaźnika ważności<sup>[2]</sup>)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visual FoxPro 9.0 z dodatkiem Service Pack 2 zainstalowany w systemie Microsoft Windows 2000 z dodatkiem Service Pack 4  
(KB971105)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Microsoft Visual FoxPro 9.0 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2a930f56-59ac-49a6-830f-bfae7c540ec7)  
zainstalowany w systemie Microsoft Windows 2000 z dodatkiem Service Pack 4  
(KB971105)  
(Brak wskaźnika ważności<sup>[2]</sup>)
</td>
</tr>
<tr>
<th colspan="3">
Microsoft Report Viewer
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS09-061**](http://go.microsoft.com/fwlink/?linkid=160527)
</td>
<td style="border:1px solid black;">
[**MS09-062**](http://go.microsoft.com/fwlink/?linkid=161342)
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
[**Krytyczny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Pakiet redystrybucyjny narzędzia Microsoft Report Viewer 2005 z dodatkiem Service Pack 1
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Pakiet redystrybucyjny narzędzia Microsoft Report Viewer 2005 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=0dfaf300-2b53-4678-a779-0d805ddfe538)  
(KB971117)  
(Krytyczny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Pakiet redystrybucyjny narzędzia Microsoft Report Viewer 2008
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Pakiet redystrybucyjny narzędzia Microsoft Report Viewer 2008](http://www.microsoft.com/downloads/details.aspx?familyid=42ed040f-cf94-4754-b0b3-c8016fbcbe22)  
(KB971118)  
(Krytyczny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Pakiet redystrybucyjny narzędzia Microsoft Report Viewer 2008 z dodatkiem Service Pack 1
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Pakiet redystrybucyjny Microsoft Report Viewer 2008 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6aaa74bd-a46e-4478-b4e1-2063d18d2d42)  
(KB971119)  
(Krytyczny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Zestaw SDK platformy Microsoft do dystrybucji: GDI+
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Zestaw SDK platformy Microsoft do dystrybucji: GDI+](http://www.microsoft.com/downloads/details.aspx?familyid=6a63ab9c-df12-4d41-933c-be590feaa05a)  
(KB975337)  
(Brak wskaźnika ważności<sup>[2]</sup>)
</td>
</tr>
</table>
 
**Uwagi dotyczące biuletynu MS09-061**

<sup>[1]</sup>Ta aktualizacja uaktualnia program Microsoft Silverlight 2 do wersji Microsoft Silverlight 3, dzięki czemu zostaje usunięta luka opisana w biuletynie.

**\*\*Luka w zabezpieczeniach nie dotyczy instalacji Server Core.** Luki usuwane przez tę aktualizację zabezpieczeń nie dotyczą obsługiwanych wersji systemu Windows Server 2008 ani Windows Server 2008 R2, jeżeli systemy te zostały zainstalowane przy użyciu opcji instalacji Server Core. Aby uzyskać więcej informacji na temat tej opcji instalacji, zobacz artykuły MSDN, [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx) (j. ang.) i [Server Core for Windows Server 2008 R2](http://msdn.microsoft.com/en-us/library/ee391631(vs.85).aspx) (j. ang.). Należy pamiętać, że opcja instalacji Server Core nie dotyczy niektórych wersji systemu Windows Server 2008 i Windows Server 2008 R2. Zobacz [Porównanie opcji instalacji Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

Zobacz także pozostałe kategorie oprogramowania w sekcji **Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki**, aby uzyskać więcej plików aktualizacji w ramach tego samego identyfikatora biuletynu. Ten biuletyn obejmuje więcej niż jedną kategorię oprogramowania.

**Uwagi dotyczące biuletynu MS09-062**

<sup>[2]</sup>Do tej aktualizacji nie stosuje się wskaźników ważności, ponieważ firma Microsoft nie znalazła kierunków ataku dla luk omówionych w niniejszym biuletynie, odnoszących się do wspomnianego oprogramowania. Niniejsza aktualizacja zabezpieczeń jest jednak oferowana programistom korzystającym z tego oprogramowania, tak aby mogli oni samodzielnie publikować zaktualizowane wersje swoich aplikacji.

Zobacz także pozostałe kategorie oprogramowania w sekcji **Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki**, aby uzyskać więcej plików aktualizacji w ramach tego samego identyfikatora biuletynu. Ten biuletyn obejmuje więcej niż jedną kategorię oprogramowania.

#### Oprogramowanie zabezpieczające firmy Microsoft

 
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="2">
Microsoft Forefront Security
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS09-062**](http://go.microsoft.com/fwlink/?linkid=161342)
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
Microsoft Forefront Client Security 1.0
</td>
<td style="border:1px solid black;">
[Microsoft Forefront Client Security 1.0](http://www.microsoft.com/downloads/details.aspx?familyid=c0ce624c-8df3-4223-8a7a-5cba4ac334a8)  
zainstalowany w systemie Microsoft Windows 2000 z dodatkiem Service Pack 4  
(KB975962)  
(Ważny)
</td>
</tr>
</table>
 
**Uwaga dotycząca biuletynu MS09-062**

Zobacz także pozostałe kategorie oprogramowania w sekcji **Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki**, aby uzyskać więcej plików aktualizacji w ramach tego samego identyfikatora biuletynu. Ten biuletyn obejmuje więcej niż jedną kategorię oprogramowania.

Narzędzia wykrywania i wdrażania oraz wskazówki
-----------------------------------------------

<span></span>
**Centrum zabezpieczeń**

Zarządzanie oprogramowaniem oraz aktualizacjami zabezpieczeń, które należy zainstalować na serwerach oraz komputerach stacjonarnych i przenośnych w organizacji. Więcej informacji można znaleźć w [Centrum TechNet Update Management Center](http://go.microsoft.com/fwlink/?linkid=69903). Witryna [TechNet Security Center](http://go.microsoft.com/fwlink/?linkid=21171) zawiera dodatkowe informacje na temat zabezpieczeń w produktach firmy Microsoft. Użytkownicy mogą także uzyskać dostęp do tych informacji w witrynie [Bezpieczeństwo w domu](http://go.microsoft.com/fwlink/?linkid=85102), klikając łącze „Najnowsze aktualizacje zabezpieczeń”.

Aktualizacje zabezpieczeń dostępne są w witrynach [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747) i [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130). Aktualizacje zabezpieczeń są także dostępne w witrynie [Centrum pobierania Microsoft](http://go.microsoft.com/fwlink/?linkid=21129). Najłatwiej je znaleźć, wyszukując wyrażenie „aktualizacja zabezpieczeń”.

Aktualizacje zabezpieczeń można także pobierać z [Wykazu usługi Microsoft Update](http://go.microsoft.com/fwlink/?linkid=96155). Wykaz usługi Microsoft Update zawiera katalog zawartości z możliwością przeszukiwania, który udostępniany jest poprzez usługi Windows Update i Microsoft Update i obejmuje aktualizacje zabezpieczeń, sterowniki i dodatki Service Pack. Wyszukiwanie przy użyciu numeru biuletynu zabezpieczeń (np. „MS07-036”) pozwala dodać do koszyka wszystkie odpowiednie aktualizacje (w tym różne wersje językowe aktualizacji) i pobrać pliki do wybranego folderu. Więcej informacji na temat Wykazu usługi Microsoft Update można znaleźć w [Często zadawanych pytaniach dotyczących Wykazu usługi Microsoft Update](http://go.microsoft.com/fwlink/?linkid=97900).

**Uwaga** Dnia 1 sierpnia 2009 r. firma Microsoft zakończyła świadczenie pomocy technicznej dla usługi Office Update oraz narzędzia Office Update Inventory Tool. Aby w dalszym ciągu otrzymywać najnowsze aktualizacje dla produktów Microsoft Office, skorzystaj z witryny [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747). Aby uzyskać więcej informacji, zobacz artykuł [Informacje o witrynie Microsoft Office Update: Często zadawane pytania](http://office.microsoft.com/en-us/downloads/fx010402221033.aspx).

**Porady dotyczące wykrywania i wdrażania**

Firma Microsoft udziela porad dotyczących wykrywania i wdrażania aktualizacji zabezpieczeń. Porady takie zawierają zalecenia i informacje ułatwiające specjalistom IT poznanie obsługi różnych narzędzi do wykrywania i wdrażania aktualizacji zabezpieczeń. Więcej informacji na ten temat można znaleźć w [artykule 961747 bazy wiedzy Microsoft Knowledge Base](http://support.microsoft.com/kb/961747).

**Narzędzie Microsoft Baseline Security Analyzer (MBSA)**

Narzędzie Microsoft Baseline Security Analyzer umożliwia administratorom skanowanie lokalnych i zdalnych systemów w poszukiwaniu brakujących aktualizacji zabezpieczeń oraz typowych błędów konfiguracji zabezpieczeń. Więcej informacji na temat narzędzia MBSA można znaleźć w witrynie sieci Web[Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134).

**Windows Server Update Services**

Korzystając z programu Windows Server Update Services (WSUS), administratorzy mogą szybko i niezawodnie wdrożyć najnowsze aktualizacje krytyczne i aktualizacje zabezpieczeń przeznaczonych dla systemu operacyjnego Windows 2000 i nowszych, pakietu Office XP i nowszych, programu Exchange Server 2003 oraz SQL Server 2000 w systemie operacyjnym Windows 2000 i nowszych.

Więcej informacji na temat sposobu wdrażania tej aktualizacji zabezpieczeń za pomocą programu Windows Server Update Services można znaleźć w [witrynie sieci Web programu Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=50120).

**Program Systems Management Server**

Program Systems Management Server (SMS) jest przeznaczonym dla przedsiębiorstw i w znacznym stopniu konfigurowalnym rozwiązaniem służącym do zarządzania aktualizacjami. Program SMS umożliwia administratorom znalezienie komputerów z systemem Windows, na których należy zainstalować aktualizację zabezpieczeń, a także przeprowadzić kontrolowane wdrożenie tych aktualizacji w całym przedsiębiorstwie, w minimalnym stopniu zakłócając przy tym pracę użytkowników końcowych. Dostępne jest kolejne wydanie programu SMS, System Center Configuration Manager 2007. Zapoznaj się także z zawartością witryny [System Center Configuration Manager 2007](http://technet.microsoft.com/en-us/library/bb735860.aspx). Więcej informacji na temat możliwości wykorzystania przez administratorów programu SMS 2003 do wdrażania aktualizacji zabezpieczeń można znaleźć w [witrynie sieci Web zarządzania poprawkami zabezpieczeń programu SMS 2003](http://go.microsoft.com/fwlink/?linkid=22939). Użytkownicy programu SMS 2.0 mogą także skorzystać z narzędzia Security Update Inventory Tool (SUIT) ułatwiającego wdrożenie aktualizacji zabezpieczeń. Więcej informacji na temat programu SMS można znaleźć w witrynie sieci Web [Microsoft Systems Management Server](http://go.microsoft.com/fwlink/?linkid=21158).

**Uwaga** Program SMS zapewnia obsługę rozwiązań zawartych w biuletynach zabezpieczeń dzięki narzędziu Microsoft Baseline Security Analyzer. Narzędzia te mogą nie wykrywać wszystkich aktualizacji oprogramowania. W takich przypadkach administratorzy mogą wykorzystywać dostępne w programie SMS funkcje zarządzania zasobami do przyporządkowania poszczególnych aktualizacji określonym systemom. Aby uzyskać więcej informacji dotyczących tej procedury, zobacz [Wdrażanie aktualizacji oprogramowania za pomocą funkcji Software Distribution programu SMS](http://go.microsoft.com/fwlink/?linkid=33341). Niektóre aktualizacje oprogramowania wymagają od użytkownika uprawnień administratora po ponownym uruchomieniu systemu. Do zainstalowania tych aktualizacji administratorzy mogą użyć narzędzia Elevated Rights Deployment Tool (dostępnego w dodatkach [SMS 2003 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=33387) oraz [SMS 2.0 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=21161)).

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

-   [Matthieu Suiche](http://www.msuiche.net/) z instytutu [Netherlands Forensics Institute](http://www.nederlandsforensischinstituut.nl/) za zgłoszenie problemu opisanego w biuletynie MS09-050
-   Ivan Fratric z firmy [Zero Day Initiative](http://www.zerodayinitiative.com/) i Jun Xie z firmy [McAfee Avert Labs](http://www.avertlabs.com/) za zgłoszenie problemu opisanego w biuletynie MS09-051
-   Vinay Anantharaman z firmy [Adobe Systems, Inc.](http://www.adobe.com/) za zgłoszenie problemu opisanego w biuletynie MS09-051
-   Yamata Li z firmy [Palo Alto Networks](http://www.paloaltonetworks.com/) za zgłoszenie problemu opisanego w biuletynie MS09-052
-   SkyLined z firmy [Google Inc.](http://www.google.com/) za zgłoszenie problemu opisanego w biuletynie MS09-054
-   Mark Dowd z firmy [IBM ISS X-Force](http://www.iss.net/) za zgłoszenie problemu opisanego w biuletynie MS09-054
-   [TippingPoint](http://www.tippingpoint.com/) i [Zero Day Initiative](http://www.zerodayinitiative.com/) za zgłoszenie problemu opisanego w biuletynie MS09-054
-   Sam Thomas [(eshu.co.uk](http://www.tippingpoint.com/)), współpracownikowi firm [TippingPoint](http://www.zerodayinitiative.com/) i Zero Day Initiative, za zgłoszenie problemu opisanego w biuletynie MS09-054
-   Ian Wright i Jean-Luc Giraud z firmy [Citrix](http://www.citrix.com/) za współpracę z firmą Microsoft przy rozwiązywaniu problemu opisanego w biuletynie MS09-056
-   Danowi Kaminsky z firmy [IOActive](http://www.ioactive.com/) za zgłoszenie dwóch problemów opisanych w biuletynie MS09-056
-   Yamata Li z firmy [Palo Alto Networks](http://www.paloaltonetworks.com/) za zgłoszenie problemu opisanego w biuletynie MS09-057
-   Tavis Ormandy i Neel Mehta z firmy [Google Inc.](http://www.google.com/) za zgłoszenie dwóch problemów opisanych w biuletynie MS09-058
-   Firmie [NSFocus Security Team](http://www.nsfocus.com/) za zgłoszenie problemu opisanego w biuletynie MS09-058.
-   Davidowi Dewey z firmy [IBM ISS X-Force](http://www.iss.net/) za zgłoszenie problemu opisanego w biuletynie MS09-060
-   Ryanowi Smith z firmy [VeriSign iDefense Labs](http://labs.idefense.com/) za zgłoszenie dwóch problemów opisanych w biuletynie MS09-060
-   [Pavel Minaev](http://int19h.org/) za zgłoszenie problemu opisanego w biuletynie MS09-061
-   Jeroenowi Frijters z firmy [Sumatra](http://www.sumatra.nl/) za zgłoszenie problemu opisanego w biuletynie MS09-061.
-   Yamata Li z firmy [Palo Alto Networks](http://www.paloaltonetworks.com/) za zgłoszenie problemu opisanego w biuletynie MS09-062
-   Thomasowi Garnier z firmy [SkyRecon](http://www.skyrecon.com/) za zgłoszenie problemu opisanego w biuletynie MS09-062
-   Wushi z firmy [VeriSign iDefense Labs](http://labs.idefense.com/) za zgłoszenie problemu opisanego w biuletynie MS09-062
-   Ivanowi Fratric z firmy [Zero Day Initiative](http://www.zerodayinitiative.com/) za zgłoszenie problemu opisanego w biuletynie MS09-062
-   Tavis Ormandy z firmy [Google Inc.](http://www.google.com/) za zgłoszenie dwóch problemów opisanych w biuletynie MS09-062
-   Carlo Di Dato (alias shinnai) za zgłoszenie problemu opisanego w biuletynie MS09-062
-   Marsu Pilami z firmy [VeriSign iDefense Labs](http://labs.idefense.com/) za zgłoszenie problemu opisanego w biuletynie MS09-062
-   Carsten H. Eiram z firmy [Secunia](http://secunia.com/) za zgłoszenie problemu opisanego w biuletynie MS09-062

#### Pomoc techniczna

-   Wymienione oprogramowanie zostało przetestowane w celu ustalenia, których wersji dotyczy problem. Dla pozostałych wersji upłynął okres pomocy technicznej. Aby zapoznać się z zasadami cyklu pomocy technicznej dotyczącymi używanej wersji oprogramowania, odwiedź [witrynę zasad cyklu pomocy technicznej firmy Microsoft](http://go.microsoft.com/fwlink/?linkid=21742).
-   Klienci mogą uzyskać pomoc techniczną w [Biurze Obsługi Klienta Microsoft](http://go.microsoft.com/fwlink/?linkid=21131) pod numerem 0 801 802 000 (Opłata według stawek Twojego operatora) lub (0-22) 594 19 99 w godzinach od 9:00 do 17:00, od poniedziałku do piątku. Połączenia z działem pomocy technicznej związane z aktualizacjami zabezpieczeń są bezpłatne. Dodatkowe informacje dotyczące możliwości skorzystania z pomocy technicznej można znaleźć w witrynie [Pomoc i obsługa techniczna firmy Microsoft](http://support.microsoft.com/).
-   Klienci międzynarodowi mogą uzyskać pomoc w lokalnych przedstawicielstwach firmy Microsoft. Pomoc techniczna związana z aktualizacjami zabezpieczeń jest bezpłatna. Informacje o sposobie kontaktowania się z pomocą techniczną firmy Microsoft są dostępne w [międzynarodowej witrynie sieci Web pomocy i obsługi technicznej](http://go.microsoft.com/fwlink/?linkid=21155).

#### Zrzeczenie odpowiedzialności

Informacje w bazie wiedzy Microsoft Knowledge Base są dostarczane „tak jak są” bez jakiejkolwiek gwarancji. Firma Microsoft odrzuca wszelkie gwarancje, wyraźne i dorozumiane, w tym gwarancje dotyczące wartości handlowej i przydatności do określonego celu. Firma Microsoft Corporation ani jej dostawcy w żadnym wypadku nie ponoszą odpowiedzialności za jakiekolwiek szkody, w tym bezpośrednie, pośrednie, przypadkowe, wynikowe, utratę zysków handlowych lub szkody specjalne, nawet jeżeli firmę Microsoft Corporation lub jej dostawców powiadomiono o możliwości zaistnienia takich szkód. W niektórych stanach wyłączenie lub ograniczenie odpowiedzialności za straty wynikowe lub przypadkowe, a więc i powyższe ograniczenia, nie mają zastosowania.

#### Wersje

-   Wersja 1.0 (13 października 2009 r.): Opublikowane podsumowanie biuletynów zabezpieczeń.
-   Wersja 1.1 (14 października 2009 r.): Poprawiono łącze pobierania dodatku Service Pack2 dla systemu Windows XP x64 Edition w biuletynie MS09-055.
-   Wersja 1.2 (18 października 2009 r.): Zaktualizowano sekcję „Streszczenie” dla biuletynu MS09-054 w celu przekazania wskazówek użytkownikom programu Firefox.
-   Wersja 2.0 (28 października 2009 r.): W tabeli „Programy, których dotyczy problem” dodano programy Microsoft Office Visio Viewer 2007, Microsoft Office Visio Viewer 2007 z dodatkiem Service Pack 1 i Microsoft Office Visio Viewer 2007 z dodatkiem Service Pack 2, których dotyczył biuletyn MS09-062. Dodano również uwagi do biuletynu MS09-062 przeznaczone dla użytkowników programu SQL Server 2005, korzystających z usług Reporting Services za pomocą programu SharePoint.
-   Wersja 3.0 (2 listopada 2009 r.): Biuletyn zmieniono, aby poinformować o udostępnieniu poprawki do aktualizacji MS09-054 rozwiązującej problemy ze zgodnością aplikacji. Klienci, którzy zainstalowali już tę aktualizację, mogą zainstalować poprawkę z artykułu 976749 bazy wiedzy Microsoft Knowledge Base.
-   Wersja 3.1 (4 listopada 2009 r.): Usunięto błędne odwołania do pierwszej wersji programu Microsoft Office Visio Viewer 2007, jako oprogramowania, którego dotyczy problem, w biuletynach MS09-060 i MS09-062.
-   Wersja 4.0 (10 listopada 2009 r.): Biuletyn zaktualizowano w celu poinformowania o ponownym wydaniu w biuletynie MS09-051 aktualizacji dla programu Menedżer kompresji audio w systemie Microsoft Windows 2000 z dodatkiem Service Pack 4 usuwającej problem z wykrywaniem. Zmiana objęła tylko wykrywanie. Nie wprowadzono żadnych zmian do plików binarnych. Klienci, którym udało się zaktualizować swoje systemy, nie muszą instalować tej aktualizacji.
-   Wersja 4.1 (12 stycznia 2010 r.): Usunięto Microsoft Expression Web, Microsoft Expression Web 2, Microsoft Office Groove 2007 i Microsoft Office Groove 2007 z dodatkiem Service Pack 1 z listy oprogramowania, którego dotyczy problem omówiony w biuletynie MS09-062.
-   Wersja 4.2 (22 czerwca 2010 r.): Z biuletynu MS09-061 usunięto program .NET Framework 1.1 z dodatkiem Service Pack 1 jako składnik systemów Windows 7 i Windows Server 2008 R2, którego dotyczy luka.

*Built at 2014-04-18T01:50:00Z-07:00*
