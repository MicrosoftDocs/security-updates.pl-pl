---
TOCTitle: 'MS10-AUG'
Title: 'Podsumowanie biuletynów zabezpieczeń firmy Microsoft za sierpień 2010 r.'
ms:assetid: 'ms10-aug'
ms:contentKeyID: 61233109
ms:mtpsurl: 'https://technet.microsoft.com/pl-PL/library/ms10-aug(v=Security.10)'
---
Podsumowanie biuletynów zabezpieczeń firmy Microsoft za sierpień 2010 r.
========================================================================

Opublikowano: 2 sierpnia 2010 | Zaktualizowano: 1 września 2010

**Wersja:** 2.1

Niniejsze podsumowanie biuletynów zabezpieczeń zawiera spis biuletynów za sierpień 2010 r.

Z chwilą opublikowania biuletynów za sierpień 2010 r. niniejsze podsumowanie biuletynów zastępuje powiadomienie o biuletynach zabezpieczeń wydane 5 sierpnia 2010 r. Aby uzyskać więcej informacji na temat usługi powiadamiania o biuletynach, zobacz [Powiadomienia o biuletynach zabezpieczeń firmy Microsoft](http://technet.microsoft.com/security/bulletin/advance).

Aby dowiedzieć się, jak otrzymywać automatyczne powiadomienia o publikacji biuletynów zabezpieczeń firmy Microsoft, odwiedź stronę [Microsoft Technical Security Notifications](http://go.microsoft.com/fwlink/?linkid=21163).

11 sierpnia 2010 r. o godz. 11:00 czasu Pacyfiku (godz. 20:00 czasu środkowoeuropejskiego) firma Microsoft udostępni emisję internetową, w której znajdą się odpowiedzi na pytania klientów dotyczące tych biuletynów (USA i Kanada). [Zarejestruj się, aby obejrzeć emisję internetową dotyczącą biuletynów zabezpieczeń za sierpień](https://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032454431&eventcategory=4&culture=en-us&countrycode=us). Po tym dniu emisja internetowa będzie dostępna na żądanie. Aby uzyskać więcej informacji, zobacz [Podsumowania biuletynów zabezpieczeń i emisje internetowe firmy Microsoft](http://technet.microsoft.com/security/bulletin/summary).

W przypadku opublikowanego poza cyklem standardowym biuletynu zabezpieczeń, [MS10-046](http://go.microsoft.com/fwlink/?linkid=197393), pierwotnie zapowiedzianego w wersji 1.0 niniejszego podsumowania biuletynów, firma Microsoft opublikowała odpowiednie powiadomienie o biuletynach zabezpieczeń dnia 30 lipca 2010 r. i udostępniła emisję internetową dotyczącą biuletynu dnia 2 sierpnia 2010 r. Emisja internetowa z dnia [2 sierpnia 2010 r.](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032456779&culture=en-us) jest dostępna na żądanie. Aby uzyskać więcej informacji, zobacz [Podsumowania biuletynów zabezpieczeń i emisje internetowe firmy Microsoft](http://technet.microsoft.com/security/bulletin/summary).

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=197393">MS10-046</a></td>
<td style="border:1px solid black;"><strong>Luka w zabezpieczeniach powłoki systemu Windows umożliwia zdalne wykonanie kodu (2286198)</strong><br />
<br />
Niniejsza aktualizacja zabezpieczeń ma na celu usunięcie zgłoszonej przez organizację publiczną luki w zabezpieczeniach powłoki systemu Windows. Luka ta może pozwalać na zdalne wykonanie kodu, jeżeli wyświetlony zostanie specjalnie spreparowany skrót. Osoba atakująca, której uda się wykorzystać tę lukę, może uzyskać takie same uprawnienia, jak użytkownik lokalny. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Krytyczny</a><br />
Zdalne wykonanie kodu</td>
<td style="border:1px solid black;">Wymaga ponownego uruchomienia komputera</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=197104">MS10-049</a></td>
<td style="border:1px solid black;"><strong>Luki w zabezpieczeniach protokołu SChannel umożliwiają zdalne wykonanie kodu (980436)</strong><br />
<br />
Ta aktualizacja zabezpieczeń usuwa dwie luki w pakiecie zabezpieczeń bezpiecznego kanału (SChannel) w systemie Windows, z których jedna została zgłoszona przez organizację publiczną, a druga przez użytkowników . Najpoważniejsza z tych luk umożliwia zdalne wykonanie kodu, jeśli użytkownik odwiedzi specjalnie spreparowaną witrynę sieci Web, której celem jest wykorzystanie tych luk w zabezpieczeniach za pośrednictwem przeglądarki sieci Web. Jednakże w żadnym przypadku osoba atakująca nie może zmusić użytkowników do odwiedzenia takich witryn. Musi natomiast przekonać użytkowników do odwiedzenia tej witryny, najczęściej zachęcając do kliknięcia łącza w wiadomości e-mail lub wiadomości błyskawicznej, które przekieruje użytkowników do witryny osoby atakującej.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Krytyczny</a><br />
Zdalne wykonanie kodu</td>
<td style="border:1px solid black;">Wymaga ponownego uruchomienia komputera</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=196268">MS10-051</a></td>
<td style="border:1px solid black;"><strong>Luka w zabezpieczeniach programu Microsoft XML Core Services umożliwia zdalne wykonanie kodu (2079403)</strong><br />
<br />
Niniejsza aktualizacja zabezpieczeń usuwa zgłoszoną przez użytkowników lukę w zabezpieczeniach programu Microsoft XML Core Services. Luka ta może pozwolić na zdalne wykonanie kodu, jeśli użytkownik wyświetli specjalnie spreparowaną stronę sieci Web przy użyciu programu Internet Explorer. Intruz nie może w żaden sposób zmusić użytkowników do odwiedzenia szkodliwych witryn. Musi natomiast przekonać użytkowników do odwiedzenia tej witryny, najczęściej zachęcając do kliknięcia łącza w wiadomości e-mail lub wiadomości błyskawicznej, które przekieruje użytkowników do witryny osoby atakującej.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Krytyczny</a><br />
Zdalne wykonanie kodu</td>
<td style="border:1px solid black;">Wymaga ponownego uruchomienia komputera</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=194432">MS10-052</a></td>
<td style="border:1px solid black;"><strong>Luka w zabezpieczeniach koderów-dekoderów formatu MPEG Layer-3 firmy Microsoft może umożliwić zdalne wykonanie kodu (2115168)</strong><br />
<br />
Niniejsza aktualizacja zabezpieczeń usuwa lukę w zabezpieczeniach kodera-dekodera audio formatu MPEG Layer-3 firmy Microsoft, która została zgłoszona przez użytkowników. Luka ta umożliwia zdalne wykonanie kodu, gdy użytkownik otworzy specjalnie spreparowany plik multimedialny lub odbierze specjalnie spreparowany strumień danych z witryny sieci Web lub dowolnej aplikacji dostarczającej treści z sieci Web. Osoba atakująca, której uda się wykorzystać tę lukę, może uzyskać takie same uprawnienia, jak użytkownik lokalny. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Krytyczny</a><br />
Zdalne wykonanie kodu</td>
<td style="border:1px solid black;">Może wymagać ponownego uruchomienia</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=196549">MS10-053</a></td>
<td style="border:1px solid black;"><strong>Zbiorcza aktualizacja zabezpieczeń dla programu Internet Explorer (2183461)</strong><br />
<br />
Niniejsza aktualizacja zabezpieczeń usuwa sześć luk w zabezpieczeniach programu Internet Explorer, które zostały zgłoszone przez użytkowników. Najpoważniejsze z tych luk umożliwiają zdalne wykonanie kodu, jeśli użytkownik wyświetli specjalnie spreparowaną stronę sieci Web przy użyciu programu Internet Explorer. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Krytyczny</a><br />
Zdalne wykonanie kodu</td>
<td style="border:1px solid black;">Wymaga ponownego uruchomienia komputera</td>
<td style="border:1px solid black;">Microsoft Windows, Internet Explorer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=190318">MS10-054</a></td>
<td style="border:1px solid black;"><strong>Luki w zabezpieczeniach serwera SMB umożliwiają zdalne wykonanie kodu (982214)</strong><br />
<br />
Ta aktualizacja zabezpieczeń usuwa kilka luk w zabezpieczeniach systemu Microsoft Windows, które zostały zgłoszone przez użytkowników. Najpoważniejsze z tych luk umożliwiają zdalne wykonanie kodu, jeśli osoba atakująca utworzy specjalnie spreparowany pakiet SMB i wyśle go do systemu, którego dotyczy problem. Stosowanie najlepszych rozwiązań dotyczących zapór oraz standardowych konfiguracji domyślnej zapory może uchronić sieci przed atakami mającymi wykorzystać omawiane luki, których źródło znajduje się poza granicami przedsiębiorstwa.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Krytyczny</a><br />
Zdalne wykonanie kodu</td>
<td style="border:1px solid black;">Wymaga ponownego uruchomienia komputera</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=194906">MS10-055</a></td>
<td style="border:1px solid black;"><strong>Luka w zabezpieczeniach kodera-dekodera Cinepak umożliwia zdalne wykonanie kodu (982665)</strong><br />
<br />
Ta aktualizacja zabezpieczeń usuwa lukę w zabezpieczeniach kodera-dekodera Cinepak, która została zgłoszona przez użytkowników. Luka ta umożliwia zdalne wykonanie kodu, gdy użytkownik otworzy specjalnie spreparowany plik multimedialny lub odbierze specjalnie spreparowany strumień danych z witryny sieci Web lub dowolnej aplikacji dostarczającej treści z sieci Web. Osoba atakująca, której uda się wykorzystać tę lukę, może uzyskać takie same uprawnienia, jak użytkownik lokalny. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Krytyczny</a><br />
Zdalne wykonanie kodu</td>
<td style="border:1px solid black;">Może wymagać ponownego uruchomienia</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=196938">MS10-056</a></td>
<td style="border:1px solid black;"><strong>Luki w zabezpieczeniach programu Microsoft Office Word umożliwiają zdalne wykonanie kodu (2269638)</strong><br />
<br />
Ta aktualizacja zabezpieczeń usuwa cztery luki w zabezpieczeniach pakietu Microsoft Office, które zostały zgłoszone przez użytkowników. Najpoważniejsze z tych luk umożliwiają zdalne wykonanie kodu, jeśli użytkownik otworzy specjalnie spreparowaną wiadomość e-mail w formacie RTF lub wyświetli jej podgląd. Osoba atakująca, której uda się wykorzystać jedną z tych luk, może uzyskać takie same uprawnienia, jak użytkownik lokalny. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Krytyczny</a><br />
Zdalne wykonanie kodu</td>
<td style="border:1px solid black;">Może wymagać ponownego uruchomienia</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=179830">MS10-060</a></td>
<td style="border:1px solid black;"><strong>Luki w zabezpieczeniach aparatu plików wykonywalnych języka wspólnego Microsoft .NET i w programie Microsoft Silverlight mogą umożliwić zdalne wykonanie kodu (2265906)</strong><br />
<br />
Niniejsza aktualizacja zabezpieczeń usuwa dwie luki w zabezpieczeniach programów Microsoft .NET Framework i Microsoft Silverlight, które zostały zgłoszone przez użytkowników. Luki te mogą pozwolić na zdalne wykonanie kodu w systemie klienta, jeśli użytkownik wyświetli specjalnie spreparowaną stronę sieci Web przy użyciu przeglądarki sieci Web, która umożliwia uruchamianie aplikacji przeglądarki XAML (XBAP) lub aplikacji Silverlight, lub jeśli osobie atakującej uda się przekonać użytkownika do uruchomienia specjalnie spreparowanej aplikacji Microsoft .NET. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi. Omawiane luki umożliwiają także zdalne wykonanie kodu w systemach serwerowych z działającym programem IIS, jeśli dany serwer zezwala na przetwarzanie stron ASP.NET, a osobie atakującej uda się przekazać na ten serwer specjalnie spreparowaną stronę ASP.NET i uruchomić ją, tak jak mogłoby to wyglądać w scenariuszu z wykorzystaniem hostingu w sieci Web.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Krytyczny</a><br />
Zdalne wykonanie kodu</td>
<td style="border:1px solid black;">Może wymagać ponownego uruchomienia</td>
<td style="border:1px solid black;">Microsoft Windows, Microsoft .NET Framework, Microsoft Silverlight</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=195812">MS10-047</a></td>
<td style="border:1px solid black;"><strong>Luki w zabezpieczeniach jądra systemu Windows umożliwiają podniesienie poziomu uprawnień (981852)</strong><br />
<br />
Ta aktualizacja zabezpieczeń usuwa kilka luk w zabezpieczeniach systemu Microsoft Windows, które zostały zgłoszone przez użytkowników. Najpoważniejsza z tych luk może umożliwić podniesienie uprawnień, jeśli osoba atakująca zaloguje się lokalnie i uruchomi specjalnie spreparowaną aplikację. Osoba atakująca musi dysponować prawidłowymi poświadczeniami logowania oraz być w stanie zalogować się lokalnie, aby wykorzystać możliwości stwarzane przez luki. Nie jest możliwe wykorzystanie luk w sposób zdalny ani przez użytkowników anonimowych.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Ważny</a><br />
Podniesienie uprawnień</td>
<td style="border:1px solid black;">Wymaga ponownego uruchomienia komputera</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=194552">MS10-048</a></td>
<td style="border:1px solid black;"><strong>Luki w zabezpieczeniach sterowników trybu jądra systemu Windows umożliwiają podniesienie uprawnień (2160329)</strong><br />
<br />
Niniejsza aktualizacja zabezpieczeń usuwa jedną lukę zgłoszoną przez organizacje publiczne oraz cztery luki zgłoszone przez użytkowników, istniejące w sterownikach trybu jądra systemu Windows. Najpoważniejsza z luk może umożliwić podniesienie uprawnień, jeśli osoba atakująca zaloguje się do systemu i uruchomi specjalnie spreparowaną aplikację. Osoba atakująca musi dysponować prawidłowymi poświadczeniami logowania oraz być w stanie zalogować się lokalnie, aby wykorzystać możliwości stwarzane przez lukę. Nie jest możliwe wykorzystanie luki w sposób zdalny lub przez użytkowników anonimowych.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Ważny</a><br />
Podniesienie uprawnień</td>
<td style="border:1px solid black;">Wymaga ponownego uruchomienia komputera</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=197103">MS10-050</a></td>
<td style="border:1px solid black;"><strong>Luka w zabezpieczeniach programu Windows Movie Maker umożliwia zdalne wykonanie kodu (981997)</strong><br />
<br />
Niniejsza aktualizacja zabezpieczeń usuwa zgłoszoną przez użytkowników lukę w zabezpieczeniach programu Windows Movie Maker. Luka ta umożliwia zdalne wykonanie kodu, gdy osoba atakująca wyśle specjalnie spreparowany plik programu Movie Maker i nakłoni użytkownika do jego otwarcia. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Ważny</a><br />
Zdalne wykonanie kodu</td>
<td style="border:1px solid black;">Może wymagać ponownego uruchomienia</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=196275">MS10-057</a></td>
<td style="border:1px solid black;"><strong>Luka w zabezpieczeniach programu Microsoft Office Excel umożliwia zdalne wykonanie kodu (2269707)</strong><br />
<br />
Ta krytyczna aktualizacja zabezpieczeń usuwa lukę w zabezpieczeniach pakietu Microsoft Office, która została zgłoszona przez użytkowników. Luka ta umożliwia zdalne wykonanie kodu, jeśli użytkownik otworzy specjalnie spreparowany plik programu Excel. Osoba atakująca, której uda się wykorzystać tę lukę, może uzyskać takie same uprawnienia, jak zalogowany użytkownik. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Ważny</a><br />
Zdalne wykonanie kodu</td>
<td style="border:1px solid black;">Może wymagać ponownego uruchomienia</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=194562">MS10-058</a></td>
<td style="border:1px solid black;"><strong>Luki w zabezpieczeniach protokołu TCP/IP umożliwiają podniesienie poziomu uprawnień (978886)</strong><br />
<br />
Ta aktualizacja zabezpieczeń usuwa dwie luki w zabezpieczeniach systemu Windows, które zostały zgłoszone przez użytkowników. Poważniejsza z tych luk umożliwia podniesienie uprawnień ze względu na błąd podczas przetwarzania danych z określonego buforu wejściowego. Osoba atakująca, której uda się zalogować do systemu docelowego, może wykorzystać tę lukę i uruchomić dowolny kod z uprawnieniami na poziomie systemu. Osoba taka może wówczas instalować programy, przeglądać, zmieniać i usuwać dane oraz tworzyć nowe konta z pełnymi uprawnieniami.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Ważny</a><br />
Podniesienie uprawnień</td>
<td style="border:1px solid black;">Wymaga ponownego uruchomienia komputera</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=196444">MS10-059</a></td>
<td style="border:1px solid black;"><strong>Luki w zabezpieczeniach funkcji śledzenia usług umożliwiają podniesienie poziomu uprawnień (982799)</strong><br />
<br />
Niniejsza aktualizacja zabezpieczeń usuwa dwie luki w zabezpieczeniach funkcji śledzenia dotyczącej usług, z których jedną zgłosiły organizacje publiczne, a drugą użytkownicy. Luki te mogą pozwalać na podniesienie uprawnień, jeśli osoba atakująca uruchomi specjalnie spreparowaną aplikację. Osoba atakująca musi dysponować prawidłowymi poświadczeniami logowania oraz być w stanie zalogować się lokalnie, aby wykorzystać możliwości stwarzane przez lukę. Nie jest możliwe wykorzystanie luki w sposób zdalny lub przez użytkowników anonimowych.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Ważny</a><br />
Podniesienie uprawnień</td>
<td style="border:1px solid black;">Może wymagać ponownego uruchomienia</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
</tbody>
</table>
  
Wskaźnik możliwości wykorzystania luki  
--------------------------------------
  
<span></span>
Poniższa tabela przedstawia ocenę możliwości wykorzystania luk dla każdej luki opisywanej w tym miesiącu. Luki są wymienione według malejącego poziomu oceny możliwości wykorzystania, a nie według identyfikatora CVE. Uwzględniono wyłącznie te luki, które w biuletynach mają nadany wskaźnik ważności „krytyczny” lub „ważny”.
  
**W jaki sposób korzystać z tej tabeli?**
  
Tabela ta pozwala sprawdzić prawdopodobieństwo, że w ciągu 30 dni od wydania biuletynu zabezpieczeń dla każdej z aktualizacji zabezpieczeń, których zainstalowanie może być potrzebne, opublikowany zostanie działający kod wykorzystujący lukę w zabezpieczeniach. Aby ustalić priorytety wdrażania, zapoznaj się z dostępnymi poniżej ocenami, rozpatrując je w kontekście posiadanej konfiguracji. Więcej informacji na temat znaczenia tych ocen oraz sposobu ich wyznaczania można znaleźć na stronie sieci Web [Microsoft Exploitability Index](http://technet.microsoft.com/en-us/security/cc998259.aspx).
  
| Identyfikator biuletynu                                   | Nazwa luki w zabezpieczeniach                                                                                                      | CVE ID                                                                           | Ocena wskaźnika możliwości wykorzystania luki                                                                              | Najważniejsze uwagi                                                                                                                                                                                |  
|-----------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| [MS10-060](http://go.microsoft.com/fwlink/?linkid=179830) | Luka w zabezpieczeniach programu Microsoft Silverlight związana z uszkodzeniem pamięci                                             | [CVE-2010-0019](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0019) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny spójny kod wykorzystujący lukę          | (Brak)                                                                                                                                                                                             |  
| [MS10-052](http://go.microsoft.com/fwlink/?linkid=194432) | Luka w zabezpieczeniach związana z przepełnieniem bufora dekodera audio MPEG Layer-3                                               | [CVE-2010-1882](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1882) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny spójny kod wykorzystujący lukę          | (Brak)                                                                                                                                                                                             |  
| [MS10-047](http://go.microsoft.com/fwlink/?linkid=195812) | Luka w zabezpieczeniach jądra systemu Windows związana z inicjacją danych                                                          | [CVE-2010-1888](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1888) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny spójny kod wykorzystujący lukę          | (Brak)                                                                                                                                                                                             |  
| [MS10-058](http://go.microsoft.com/fwlink/?linkid=194562) | Luka w zabezpieczeniach sieci systemu Windows związana z przepełnieniem liczby całkowitej                                          | [CVE-2010-1893](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1893) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny spójny kod wykorzystujący lukę          | (Brak)                                                                                                                                                                                             |  
| [MS10-048](http://go.microsoft.com/fwlink/?linkid=194552) | Luka w zabezpieczeniach sterownika Win32k związana z obsługą wyjątków                                                              | [CVE-2010-1894](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1894) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny spójny kod wykorzystujący lukę          | **Informacje o tej luce są znane publicznie.**                                                                                                                                                     |  
| [MS10-048](http://go.microsoft.com/fwlink/?linkid=194552) | Luka w zabezpieczeniach sterownika Win32k związana z przepełnieniem puli                                                           | [CVE-2010-1895](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1895) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny spójny kod wykorzystujący lukę          | (Brak)                                                                                                                                                                                             |  
| [MS10-048](http://go.microsoft.com/fwlink/?linkid=194552) | Luka w zabezpieczeniach sterownika Win32k związana ze sprawdzaniem poprawności danych wejściowych użytkownika                      | [CVE-2010-1896](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1896) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny spójny kod wykorzystujący lukę          | (Brak)                                                                                                                                                                                             |  
| [MS10-048](http://go.microsoft.com/fwlink/?linkid=194552) | Luka w zabezpieczeniach sterownika Win32k związana z tworzeniem okna                                                               | [CVE-2010-1897](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1897) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny spójny kod wykorzystujący lukę          | (Brak)                                                                                                                                                                                             |  
| [MS10-060](http://go.microsoft.com/fwlink/?linkid=179830) | Luka w zabezpieczeniach związana z wyznaczaniem metody wirtualnej w programie Microsoft Silverlight i Microsoft .NET Framework CLR | [CVE-2010-1898](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1898) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny spójny kod wykorzystujący lukę          | (Brak)                                                                                                                                                                                             |  
| [MS10-056](http://go.microsoft.com/fwlink/?linkid=196938) | Luka w zabezpieczeniach programu Word związana z analizą rekordów                                                                  | [CVE-2010-1900](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1900) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny spójny kod wykorzystujący lukę          | (Brak)                                                                                                                                                                                             |  
| [MS10-056](http://go.microsoft.com/fwlink/?linkid=196938) | Luka w zabezpieczeniach aparatu analizy formatu RTF programu Word związana z uszkodzeniem pamięci                                  | [CVE-2010-1901](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1901) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny spójny kod wykorzystujący lukę          | (Brak)                                                                                                                                                                                             |  
| [MS10-055](http://go.microsoft.com/fwlink/?linkid=194906) | Luka w zabezpieczeniach kodera-dekodera Cinepak związana z dekompresją plików                                                      | [CVE-2010-2553](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2553) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny spójny kod wykorzystujący lukę          | (Brak)                                                                                                                                                                                             |  
| [MS10-059](http://go.microsoft.com/fwlink/?linkid=196444) | Luka w zabezpieczeniach związana z uszkodzeniem pamięci funkcji śledzenia                                                          | [CVE-2010-2555](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2555) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny spójny kod wykorzystujący lukę          | (Brak)                                                                                                                                                                                             |  
| [MS10-053](http://go.microsoft.com/fwlink/?linkid=196549) | Luka w zabezpieczeniach związana z uszkodzeniem niezainicjowanej pamięci                                                           | [CVE-2010-2557](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2557) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny spójny kod wykorzystujący lukę          | Wykorzystanie tej luki jest bardziej prawdopodobne w programie Internet Explorer 6, ze względu na brak ograniczania w postaci funkcji zapobiegania wykonywaniu danych (Data Execution Prevention). |  
| [MS10-053](http://go.microsoft.com/fwlink/?linkid=196549) | Luka w zabezpieczeniach związana z uszkodzeniem pamięci usługi układu HTML                                                         | [CVE-2010-2560](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2560) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny spójny kod wykorzystujący lukę          | (Brak)                                                                                                                                                                                             |  
| [MS10-057](http://go.microsoft.com/fwlink/?linkid=196275) | Luka w zabezpieczeniach programu Excel związana z uszkodzeniem pamięci                                                             | [CVE-2010-2562](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2562) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny spójny kod wykorzystujący lukę          | (Brak)                                                                                                                                                                                             |  
| [MS10-050](http://go.microsoft.com/fwlink/?linkid=197103) | Luka w zabezpieczeniach związana z uszkodzeniem pamięci programu Movie Maker                                                       | [CVE-2010-2564](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2564) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny spójny kod wykorzystujący lukę          | (Brak)                                                                                                                                                                                             |  
| [MS10-046](http://go.microsoft.com/fwlink/?linkid=197393) | Luka w zabezpieczeniach związana z wczytywaniem ikony skrótu                                                                       | [CVE-2010-2568](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2568) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobny spójny kod wykorzystujący lukę          | **Ta luka w zabezpieczeniach jest aktualnie wykorzystywana w Internecie.**                                                                                                                         |  
| [MS10-047](http://go.microsoft.com/fwlink/?linkid=195812) | Luka w zabezpieczeniach jądra systemu Windows związana z podwójnym zwolnieniem                                                     | [CVE-2010-1889](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1889) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobnie niespójny kod wykorzystujący lukę      | (Brak)                                                                                                                                                                                             |  
| [MS10-056](http://go.microsoft.com/fwlink/?linkid=196938) | Luka w zabezpieczeniach programu Word związana z przepełnieniem buforu analizy formatu RTF                                         | [CVE-2010-1902](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1902) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobnie niespójny kod wykorzystujący lukę      | Systemy Windows Vista i Windows 7 są w mniejszym stopniu narażone na działanie tej luki, ze względu na dodatkowe mechanizmy ograniczenia zagrożeń związanych ze stosem.                            |  
| [MS10-056](http://go.microsoft.com/fwlink/?linkid=196938) | Luka w zabezpieczeniach programu Word związana z uszkodzeniem pamięci obiektów połączonych HTML                                    | [CVE-2010-1903](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1903) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobnie niespójny kod wykorzystujący lukę      | (Brak)                                                                                                                                                                                             |  
| [MS10-054](http://go.microsoft.com/fwlink/?linkid=190318) | Luka w zabezpieczeniach protokołu SMB związana z przepełnieniem puli                                                               | [CVE-2010-2550](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2550) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobnie niespójny kod wykorzystujący lukę      | Bardziej prawdopodobnym efektem wykorzystania luki jest odmowa usługi niż wykonanie kodu.                                                                                                          |  
| [MS10-053](http://go.microsoft.com/fwlink/?linkid=196549) | Luka w zabezpieczeniach związana z uszkodzeniem niezainicjowanej pamięci                                                           | [CVE-2010-2556](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2556) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobnie niespójny kod wykorzystujący lukę      | (Brak)                                                                                                                                                                                             |  
| [MS10-053](http://go.microsoft.com/fwlink/?linkid=196549) | Luka w zabezpieczeniach powodująca uszkodzenie pamięci związane z sytuacją wyścigu                                                 | [CVE-2010-2558](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2558) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobnie niespójny kod wykorzystujący lukę      | (Brak)                                                                                                                                                                                             |  
| [MS10-053](http://go.microsoft.com/fwlink/?linkid=196549) | Luka w zabezpieczeniach związana z uszkodzeniem niezainicjowanej pamięci                                                           | [CVE-2010-2559](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2559) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobnie niespójny kod wykorzystujący lukę      | (Brak)                                                                                                                                                                                             |  
| [MS10-051](http://go.microsoft.com/fwlink/?linkid=196268) | Luka w zabezpieczeniach związana z uszkodzeniem pamięci podczas obsługi odpowiedzi Msxml2.XMLHTTP.3.0                              | [CVE-2010-2561](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2561) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobnie niespójny kod wykorzystujący lukę      | (Brak)                                                                                                                                                                                             |  
| [MS10-049](http://go.microsoft.com/fwlink/?linkid=197104) | Luka w zabezpieczeniach związana z nieprawidłowo utworzonym żądaniem certyfikatu SChannel i umożliwiająca zdalne wykonanie kodu    | [CVE-2010-2566](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2566) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - prawdopodobnie niespójny kod wykorzystujący lukę      | Prawdopodobnym skutkiem wykorzystania tej luki jest odmowa usługi. Zdalne wykonanie kodu jest mało prawdopodobne.                                                                                  |  
| [MS10-049](http://go.microsoft.com/fwlink/?linkid=197104) | Luka w zabezpieczeniach dotycząca renegocjacji TLS/SSL                                                                             | [CVE-2009-3555](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-3555) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - działający kod wykorzystujący lukę mało prawdopodobny | Jest to luka w zabezpieczeniach związana z fałszowaniem. Została ona opisana w [Poradniku zabezpieczeń firmy Microsoft 977377](http://technet.microsoft.com/security/advisory/977377).             |  
| [MS10-053](http://go.microsoft.com/fwlink/?linkid=196549) | Luka w zabezpieczeniach międzydomenowych związana z procedurą obsługi zdarzeń                                                      | [CVE-2010-1258](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1258) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - działający kod wykorzystujący lukę mało prawdopodobny | Ta luka może doprowadzić do ujawnienia informacji.                                                                                                                                                 |  
| [MS10-058](http://go.microsoft.com/fwlink/?linkid=194562) | Luka w zabezpieczeniach protokołu IPv6 związana z uszkodzeniem pamięci                                                             | [CVE-2010-1892](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-1892) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - działający kod wykorzystujący lukę mało prawdopodobny | Ta luka powoduje awarię typu odmowa usługi.                                                                                                                                                        |  
| [MS10-054](http://go.microsoft.com/fwlink/?linkid=190318) | Luka w zabezpieczeniach protokołu SMB związana ze sprawdzaniem poprawności zmiennych                                               | [CVE-2010-2551](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2551) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - działający kod wykorzystujący lukę mało prawdopodobny | Ta luka powoduje awarię typu odmowa usługi.                                                                                                                                                        |  
| [MS10-054](http://go.microsoft.com/fwlink/?linkid=190318) | Luka w zabezpieczeniach protokołu SMB związana z wyczerpywaniem się miejsca w stosie                                               | [CVE-2010-2552](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2552) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - działający kod wykorzystujący lukę mało prawdopodobny | Ta luka powoduje awarię typu odmowa usługi.                                                                                                                                                        |
  
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
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="14">
Windows XP  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS10-046**](http://go.microsoft.com/fwlink/?linkid=197393)
</td>
<td style="border:1px solid black;">
[**MS10-049**](http://go.microsoft.com/fwlink/?linkid=197104)
</td>
<td style="border:1px solid black;">
[**MS10-051**](http://go.microsoft.com/fwlink/?linkid=196268)
</td>
<td style="border:1px solid black;">
[**MS10-052**](http://go.microsoft.com/fwlink/?linkid=194432)
</td>
<td style="border:1px solid black;">
[**MS10-053**](http://go.microsoft.com/fwlink/?linkid=196549)
</td>
<td style="border:1px solid black;">
[**MS10-054**](http://go.microsoft.com/fwlink/?linkid=190318)
</td>
<td style="border:1px solid black;">
[**MS10-055**](http://go.microsoft.com/fwlink/?linkid=194906)
</td>
<td style="border:1px solid black;">
[**MS10-060**](http://go.microsoft.com/fwlink/?linkid=179830)
</td>
<td style="border:1px solid black;">
[**MS10-047**](http://go.microsoft.com/fwlink/?linkid=195812)
</td>
<td style="border:1px solid black;">
[**MS10-048**](http://go.microsoft.com/fwlink/?linkid=194552)
</td>
<td style="border:1px solid black;">
[**MS10-050**](http://go.microsoft.com/fwlink/?linkid=197103)
</td>
<td style="border:1px solid black;">
[**MS10-058**](http://go.microsoft.com/fwlink/?linkid=194562)
</td>
<td style="border:1px solid black;">
[**MS10-059**](http://go.microsoft.com/fwlink/?linkid=196444)
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
Brak
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
[Windows XP z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=12361875-b453-45e8-852b-90f2727894fd)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows XP z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=ff00381c-e74b-48e5-9dd9-34dbedd906a2)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?familyid=dbdbbe5e-2ef9-4704-80c4-27ef28fd95ef)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows XP z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=08159149-17de-4640-8818-cb7bd4811531)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=bc949915-4e16-4897-a295-2f99102548ab)  
(Krytyczny)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=4b489f8c-ada0-4051-8284-0a941c04d2ed)  
(Krytyczny)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=1662780f-370a-425b-9917-c601eb54a375)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows XP z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=6e5e16f8-c140-4a1d-b898-8417a6bfd4d8)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows XP z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=5ddb5e34-f97a-47c6-96c8-ba2ed06ccb77)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=648cfca5-19eb-4658-a6ad-fe546c4c44b9)  
(KB983582)  
(Krytyczny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2 oraz Microsoft .NET Framework 3.5 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1e53f250-2d4b-4f61-86ee-9f9f3a9c0b48)  
(KB983583)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows XP z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=e3574047-5ce5-4461-94aa-4eb3258d5e71)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows XP z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=deeac521-d3a2-4019-8176-c9228e733cf4)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Movie Maker 2.1](http://www.microsoft.com/downloads/details.aspx?familyid=b211664b-434d-4626-816f-c77510cfd44d)<sup>[1]</sup>
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
Windows XP Professional x64 Edition z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3b44bd67-48e2-497f-9165-42a702e2cc0d)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=eaffa70c-6f2b-4e66-b1bc-64bdbbbcd34f)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?familyid=4d4e8eeb-a0b2-41c6-9ee4-3f4beb44195e)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b7f28d7a-6b27-4059-865b-5fd55edb6299)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=96b7a562-af16-4f0d-840c-838fb12e7419)  
(Krytyczny)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=5296fb82-c446-4681-a9a0-0f80a2e248be)  
(Krytyczny)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=f8ae3978-bad6-4201-8357-2d212ab703ef)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fd6cc359-e72e-46ec-a08b-763934e3e115)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/my%20documents/release/5cff5d6e-11a5-40ed-92ac-e12d287919e6)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=648cfca5-19eb-4658-a6ad-fe546c4c44b9)  
(KB983582)  
(Krytyczny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2 oraz Microsoft .NET Framework 3.5 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1e53f250-2d4b-4f61-86ee-9f9f3a9c0b48)  
(KB983583)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d6c5455e-bc31-4842-aef4-ebff92324323)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Movie Maker 2.1](http://www.microsoft.com/downloads/details.aspx?familyid=decb1fe6-adc8-44f7-89c5-f25767f0cefe)<sup>[1]</sup>
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
<th colspan="14">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS10-046**](http://go.microsoft.com/fwlink/?linkid=197393)
</td>
<td style="border:1px solid black;">
[**MS10-049**](http://go.microsoft.com/fwlink/?linkid=197104)
</td>
<td style="border:1px solid black;">
[**MS10-051**](http://go.microsoft.com/fwlink/?linkid=196268)
</td>
<td style="border:1px solid black;">
[**MS10-052**](http://go.microsoft.com/fwlink/?linkid=194432)
</td>
<td style="border:1px solid black;">
[**MS10-053**](http://go.microsoft.com/fwlink/?linkid=196549)
</td>
<td style="border:1px solid black;">
[**MS10-054**](http://go.microsoft.com/fwlink/?linkid=190318)
</td>
<td style="border:1px solid black;">
[**MS10-055**](http://go.microsoft.com/fwlink/?linkid=194906)
</td>
<td style="border:1px solid black;">
[**MS10-060**](http://go.microsoft.com/fwlink/?linkid=179830)
</td>
<td style="border:1px solid black;">
[**MS10-047**](http://go.microsoft.com/fwlink/?linkid=195812)
</td>
<td style="border:1px solid black;">
[**MS10-048**](http://go.microsoft.com/fwlink/?linkid=194552)
</td>
<td style="border:1px solid black;">
[**MS10-050**](http://go.microsoft.com/fwlink/?linkid=197103)
</td>
<td style="border:1px solid black;">
[**MS10-058**](http://go.microsoft.com/fwlink/?linkid=194562)
</td>
<td style="border:1px solid black;">
[**MS10-059**](http://go.microsoft.com/fwlink/?linkid=196444)
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
Brak
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
[Windows Server 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=32fe91ef-5a8d-4095-90ee-2ca216696b09)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f76d68df-97e5-489c-a5f6-0c378c1f62ae)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?familyid=31ce233e-4d2d-404b-84a8-683319ba8ef7)  
(Umiarkowany)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9c2110ec-7e6c-4e73-9785-0a8196095ea0)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=b0370e1e-dedf-4fe8-a06c-0e0f0a674205)  
(Krytyczny)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=8753ae27-60a4-475a-b8bc-6a7764480295)  
(Krytyczny)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=772e765d-0502-4b0b-bde8-d4f62b96db64)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=230e8559-e6df-49d5-acb5-b0cd4bde0bf4)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=648cfca5-19eb-4658-a6ad-fe546c4c44b9)  
(KB983582)  
(Krytyczny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2 oraz Microsoft .NET Framework 3.5 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1e53f250-2d4b-4f61-86ee-9f9f3a9c0b48)  
(KB983583)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=59395f00-90f4-4b68-8dd3-03ff611c1bc8)  
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=923de214-c4fa-41e6-8307-2c5a37f13e8e)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4543bcf0-3505-407b-a5a9-6250ece6fbac)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?familyid=4d784b57-8564-4e7e-8f61-f897398e7ea5)  
(Umiarkowany)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fdfad4ca-37c4-4ac5-bebc-a5ad61299503)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=d92f5e69-43cf-4615-aa3b-41f9f40bb57b)  
(Krytyczny)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=fd3e9d06-1f8b-4ef7-84f6-61e85a1767b8)  
(Krytyczny)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=863edf45-0d3b-4408-a47c-258dc4a4fd94)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=03804f59-748e-4832-98e4-2d88564bd10a)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=648cfca5-19eb-4658-a6ad-fe546c4c44b9)  
(KB983582)  
(Krytyczny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2 oraz Microsoft .NET Framework 3.5 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1e53f250-2d4b-4f61-86ee-9f9f3a9c0b48)  
(KB983583)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9ef1c600-bb93-4800-81b8-8c64b369c194)  
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=63aa5f8a-fe47-4892-b905-b54e4f3b6580)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=9ef992c3-96e9-4533-b844-07424a6054b3)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?familyid=d87ac8b3-41fb-4cdd-b305-181a0024d85c)  
(Umiarkowany)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=782e2963-4a52-4a1d-b99a-34ba841038a7)  
(Krytyczny)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=5e730064-8270-4d63-b497-c5ebeddea1fc)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=e4f4f8b3-7a39-4d77-a46b-02c86ad159c3)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=648cfca5-19eb-4658-a6ad-fe546c4c44b9)  
(KB983582)  
(Krytyczny)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2 oraz Microsoft .NET Framework 3.5 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1e53f250-2d4b-4f61-86ee-9f9f3a9c0b48)  
(KB983583)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=f96b8154-9976-41b0-b9d7-d79887fe9364)  
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
</tr>
<tr>
<th colspan="14">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS10-046**](http://go.microsoft.com/fwlink/?linkid=197393)
</td>
<td style="border:1px solid black;">
[**MS10-049**](http://go.microsoft.com/fwlink/?linkid=197104)
</td>
<td style="border:1px solid black;">
[**MS10-051**](http://go.microsoft.com/fwlink/?linkid=196268)
</td>
<td style="border:1px solid black;">
[**MS10-052**](http://go.microsoft.com/fwlink/?linkid=194432)
</td>
<td style="border:1px solid black;">
[**MS10-053**](http://go.microsoft.com/fwlink/?linkid=196549)
</td>
<td style="border:1px solid black;">
[**MS10-054**](http://go.microsoft.com/fwlink/?linkid=190318)
</td>
<td style="border:1px solid black;">
[**MS10-055**](http://go.microsoft.com/fwlink/?linkid=194906)
</td>
<td style="border:1px solid black;">
[**MS10-060**](http://go.microsoft.com/fwlink/?linkid=179830)
</td>
<td style="border:1px solid black;">
[**MS10-047**](http://go.microsoft.com/fwlink/?linkid=195812)
</td>
<td style="border:1px solid black;">
[**MS10-048**](http://go.microsoft.com/fwlink/?linkid=194552)
</td>
<td style="border:1px solid black;">
[**MS10-050**](http://go.microsoft.com/fwlink/?linkid=197103)
</td>
<td style="border:1px solid black;">
[**MS10-058**](http://go.microsoft.com/fwlink/?linkid=194562)
</td>
<td style="border:1px solid black;">
[**MS10-059**](http://go.microsoft.com/fwlink/?linkid=196444)
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
Windows Vista z dodatkiem Service Pack 1 i Windows Vista z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista z dodatkiem Service Pack 1 i Windows Vista z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=52748886-6280-4247-8cbd-f64db229ee66)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Vista z dodatkiem Service Pack 1 i Windows Vista z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=aca69406-f795-4398-968f-959fe3a74e89)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?familyid=bbfaadf8-ab38-456c-956a-ea18c64236c9)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=535c563e-cdac-4e3d-96b0-9947ea22deca)  
(Krytyczny)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=2062566b-8b81-43c2-875d-9c06d4e3fa82)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Vista z dodatkiem Service Pack 1 i Windows Vista z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9087a3aa-aa55-41f6-8c4c-f322e4aa8681)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Vista z dodatkiem Service Pack 1 i Windows Vista z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=60c81415-b61e-44a4-8dd9-cedec99eb70f)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Tylko Windows Vista z dodatkiem Service Pack 1:  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 1 oraz Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=616c39f7-137a-40b9-b691-bc33c0aef7e1)  
(KB983587)  
(Krytyczny)  
Tylko Windows Vista z dodatkiem Service Pack 1:  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2 oraz Microsoft .NET Framework 3.5 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=155bbb5c-247e-4bed-a287-527d978b7967)  
(KB983588)  
(Krytyczny)  
Tylko Windows Vista z dodatkiem Service Pack 2:  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2 oraz Microsoft .NET Framework 3.5 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7712e8ad-dea4-4a43-8a7b-dc154510c104)  
(KB983589)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Vista z dodatkiem Service Pack 1 i Windows Vista z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4486f97c-4cf8-4236-bfc3-b50e72e2a5c1)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Vista z dodatkiem Service Pack 1 i Windows Vista z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c9345207-7242-4b71-bf80-b52031e08f8c)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Movie Maker 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=8aded9dd-08d6-4b19-955f-0d8414868cf9)<sup>[1]</sup>
(Ważny)  
[Movie Maker 2.6](http://www.microsoft.com/downloads/details.aspx?familyid=a1d8ed0d-a3b5-416a-ab8b-77501da62132)<sup>[2]</sup>
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Vista z dodatkiem Service Pack 1 i Windows Vista z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4684c4df-0a5c-4dba-82e5-059378737118)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Vista z dodatkiem Service Pack 1 i Windows Vista z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=dfb31aa2-7457-4581-9e28-7984a360edf4)  
(Ważny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition z dodatkiem Service Pack 1 i Windows Vista x64 Edition z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition z dodatkiem Service Pack 1 i Windows Vista x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=37648e95-05c2-4802-9a0f-660200baa229)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition z dodatkiem Service Pack 1 i Windows Vista x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e2835ed1-5ca6-4347-8ff1-e694b1ac49ff)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?familyid=577131cd-1229-4746-89d7-84d75f29e1f0)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=cd1185e3-ca22-4197-a53b-e7a2806ac352)  
(Krytyczny)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=65b04e29-8e39-46de-94e8-b653969b1ffd)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition z dodatkiem Service Pack 1 i Windows Vista x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=10c9d5f1-53ed-459b-a663-e69bdb845a6b)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition z dodatkiem Service Pack 1 i Windows Vista x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=469b732d-ca62-4a48-bb55-99f2ae4ddcf5)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Tylko Windows Vista x64 Edition z dodatkiem Service Pack 1:  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 1 oraz Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=616c39f7-137a-40b9-b691-bc33c0aef7e1)  
(KB983587)  
(Krytyczny)  
Tylko Windows Vista x64 Edition z dodatkiem Service Pack 1:  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2 oraz Microsoft .NET Framework 3.5 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=155bbb5c-247e-4bed-a287-527d978b7967)  
(KB983588)  
(Krytyczny)  
Tylko Windows Vista x64 Edition z dodatkiem Service Pack 2:  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2 oraz Microsoft .NET Framework 3.5 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7712e8ad-dea4-4a43-8a7b-dc154510c104)  
(KB983589)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition z dodatkiem Service Pack 1 i Windows Vista x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b547898e-f8a9-49dc-b49d-cffec5a001bc)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition z dodatkiem Service Pack 1 i Windows Vista x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1620e7ac-3913-478d-8120-e9f46d98f453)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Movie Maker 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=4baff9ae-dd25-4942-b45e-f281d0e1f4ac)<sup>[1]</sup>
(Ważny)  
[Movie Maker 2.6](http://www.microsoft.com/downloads/details.aspx?familyid=0a226592-8f98-4f67-ac60-1d00cbc56598)<sup>[2]</sup>
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition z dodatkiem Service Pack 1 i Windows Vista x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=18152cd4-815f-425f-8694-fbabcbe80609)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition z dodatkiem Service Pack 1 i Windows Vista x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=110f932f-d13c-4486-a295-e6068d5d8d7a)  
(Ważny)
</td>
</tr>
<tr>
<th colspan="14">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS10-046**](http://go.microsoft.com/fwlink/?linkid=197393)
</td>
<td style="border:1px solid black;">
[**MS10-049**](http://go.microsoft.com/fwlink/?linkid=197104)
</td>
<td style="border:1px solid black;">
[**MS10-051**](http://go.microsoft.com/fwlink/?linkid=196268)
</td>
<td style="border:1px solid black;">
[**MS10-052**](http://go.microsoft.com/fwlink/?linkid=194432)
</td>
<td style="border:1px solid black;">
[**MS10-053**](http://go.microsoft.com/fwlink/?linkid=196549)
</td>
<td style="border:1px solid black;">
[**MS10-054**](http://go.microsoft.com/fwlink/?linkid=190318)
</td>
<td style="border:1px solid black;">
[**MS10-055**](http://go.microsoft.com/fwlink/?linkid=194906)
</td>
<td style="border:1px solid black;">
[**MS10-060**](http://go.microsoft.com/fwlink/?linkid=179830)
</td>
<td style="border:1px solid black;">
[**MS10-047**](http://go.microsoft.com/fwlink/?linkid=195812)
</td>
<td style="border:1px solid black;">
[**MS10-048**](http://go.microsoft.com/fwlink/?linkid=194552)
</td>
<td style="border:1px solid black;">
[**MS10-050**](http://go.microsoft.com/fwlink/?linkid=197103)
</td>
<td style="border:1px solid black;">
[**MS10-058**](http://go.microsoft.com/fwlink/?linkid=194562)
</td>
<td style="border:1px solid black;">
[**MS10-059**](http://go.microsoft.com/fwlink/?linkid=196444)
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
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 dla systemów 32-bitowych i Windows Server 2008 z dodatkiem Service Pack 2 dla systemów 32-bitowych
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów 32-bitowych i Windows Server 2008 z dodatkiem Service Pack 2 dla systemów 32-bitowych](http://www.microsoft.com/downloads/details.aspx?familyid=3aabd189-7d4c-4c9f-8854-f33127b1c309)\*  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów 32-bitowych i Windows Server 2008 z dodatkiem Service Pack 2 dla systemów 32-bitowych](http://www.microsoft.com/downloads/details.aspx?familyid=6e0253d4-f0c0-4f28-ba08-6907c2fcb339)\*  
(Ważny)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?familyid=73b5f45c-c9d6-491f-8483-98838b2a7c04)\*  
(Umiarkowany)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=8239cb9e-bb5a-4157-8038-33d0b329eaee)\*\*  
(Krytyczny)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=409b9298-1e7d-48cf-9872-ffbdc56ebe53)\*\*  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów 32-bitowych i Windows Server 2008 z dodatkiem Service Pack 2 dla systemów 32-bitowych](http://www.microsoft.com/downloads/details.aspx?familyid=a94e2e38-116a-4b63-9328-6c33e63bbbfe)\*  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
Tylko Windows Server 2008 dla systemów 32-bitowych:  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 1 oraz Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=616c39f7-137a-40b9-b691-bc33c0aef7e1)\*\*  
(KB983587)  
(Krytyczny)  
Tylko Windows Server 2008 dla systemów 32-bitowych:  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2 i Microsoft .NET Framework 3.5 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=155bbb5c-247e-4bed-a287-527d978b7967)\*\*  
(KB983588)  
(Krytyczny)  
Tylko Windows Server 2008 z dodatkiem Service Pack 2 dla systemów 32-bitowych:  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2 i Microsoft .NET Framework 3.5 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7712e8ad-dea4-4a43-8a7b-dc154510c104)\*\*  
(KB983589)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów 32-bitowych i Windows Server 2008 z dodatkiem Service Pack 2 dla systemów 32-bitowych](http://www.microsoft.com/downloads/details.aspx?familyid=611765ab-b3f3-45db-92b2-ee040b9cfd27)\*  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów 32-bitowych i Windows Server 2008 z dodatkiem Service Pack 2 dla systemów 32-bitowych](http://www.microsoft.com/downloads/details.aspx?familyid=a8b1a3f7-7147-494e-bfc0-b1979b9578e6)\*  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów 32-bitowych i Windows Server 2008 z dodatkiem Service Pack 2 dla systemów 32-bitowych](http://www.microsoft.com/downloads/details.aspx?familyid=844404be-f2e8-47bc-9650-9e2bbe383814)\*  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów 32-bitowych i Windows Server 2008 z dodatkiem Service Pack 2 dla systemów 32-bitowych](http://www.microsoft.com/downloads/details.aspx?familyid=4c9b3e60-e166-40c9-8938-3cba0a399c47)\*  
(Ważny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 dla systemów z procesorem x64 i Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem x64
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem x64 i Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=29c6fc2d-d318-4a63-9ab2-82e84272aaf2)\*  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem x64 i Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=a96891ff-8771-47b3-81bb-8640adb6c098)\*  
(Ważny)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?familyid=43ece408-4aa7-4819-b3f6-7f0719ed3213)\*  
(Umiarkowany)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=5ef8abf0-c89e-4911-8d77-42400d9a398f)\*\*  
(Krytyczny)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=9b869bab-0797-4f83-8c64-23dda9983c8d)\*\*  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem x64 i Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=602dd3f6-0d09-4546-b1db-d7b6b04edb66)\*  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
Tylko Windows Server 2008 dla systemów opartych na procesorach x64:  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 1 oraz Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=616c39f7-137a-40b9-b691-bc33c0aef7e1)\*\*  
(KB983587)  
(Krytyczny)  
Tylko Windows Server 2008 dla systemów opartych na procesorach x64:  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2 i Microsoft .NET Framework 3.5 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=155bbb5c-247e-4bed-a287-527d978b7967)\*\*  
(KB983588)  
(Krytyczny)  
Tylko Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem x64:  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2 i Microsoft .NET Framework 3.5 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7712e8ad-dea4-4a43-8a7b-dc154510c104)\*\*  
(KB983589)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem x64 i Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=131f3512-1585-462e-a4f1-3f359aac44bd)\*  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem x64 i Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=c1c25cb7-7e82-4c14-9666-aff52dd308b4)\*  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem x64 i Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=08491c73-66b1-4c4c-8740-ea596a730fc1)\*  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem x64 i Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=fa84e547-2190-402f-9467-2450deeff565)\*  
(Ważny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 dla systemów z procesorem Itanium i Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem Itanium
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem Itanium i Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=cfe227b5-6660-49f8-9d71-a997dd83de0b)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem Itanium i Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=3b16a422-0ee9-4eab-9cfe-e7688ffa0d76)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?familyid=b6faee94-e821-432d-bfa2-9008664566af)  
(Umiarkowany)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=2f1eee63-2cca-4ec5-b196-36de3c0054cf)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem Itanium i Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=24d8f0a3-51a9-46c1-b870-a2239bf600e4)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
Tylko Windows Server 2008 dla systemów z procesorem Itanium:  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 1 oraz Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=616c39f7-137a-40b9-b691-bc33c0aef7e1)  
(KB983587)  
(Krytyczny)  
Tylko Windows Server 2008 dla systemów z procesorem Itanium:  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2 oraz Microsoft .NET Framework 3.5 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=155bbb5c-247e-4bed-a287-527d978b7967)  
(KB983588)  
(Krytyczny)  
Tylko Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem Itanium:  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 2 oraz Microsoft .NET Framework 3.5 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7712e8ad-dea4-4a43-8a7b-dc154510c104)  
(KB983589)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem Itanium i Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=972efd3a-ec1e-49b2-835e-76f4b21b5b79)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem Itanium i Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=45fe5135-aa89-4f60-8cdb-ec0edc9a7e77)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem Itanium i Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=8aa12902-c234-4fd9-bba3-6767eafc38fc)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem Itanium i Windows Server 2008 z dodatkiem Service Pack 2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=84f89dca-108c-4956-9aa2-866e17a872fc)  
(Ważny)
</td>
</tr>
<tr>
<th colspan="14">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS10-046**](http://go.microsoft.com/fwlink/?linkid=197393)
</td>
<td style="border:1px solid black;">
[**MS10-049**](http://go.microsoft.com/fwlink/?linkid=197104)
</td>
<td style="border:1px solid black;">
[**MS10-051**](http://go.microsoft.com/fwlink/?linkid=196268)
</td>
<td style="border:1px solid black;">
[**MS10-052**](http://go.microsoft.com/fwlink/?linkid=194432)
</td>
<td style="border:1px solid black;">
[**MS10-053**](http://go.microsoft.com/fwlink/?linkid=196549)
</td>
<td style="border:1px solid black;">
[**MS10-054**](http://go.microsoft.com/fwlink/?linkid=190318)
</td>
<td style="border:1px solid black;">
[**MS10-055**](http://go.microsoft.com/fwlink/?linkid=194906)
</td>
<td style="border:1px solid black;">
[**MS10-060**](http://go.microsoft.com/fwlink/?linkid=179830)
</td>
<td style="border:1px solid black;">
[**MS10-047**](http://go.microsoft.com/fwlink/?linkid=195812)
</td>
<td style="border:1px solid black;">
[**MS10-048**](http://go.microsoft.com/fwlink/?linkid=194552)
</td>
<td style="border:1px solid black;">
[**MS10-050**](http://go.microsoft.com/fwlink/?linkid=197103)
</td>
<td style="border:1px solid black;">
[**MS10-058**](http://go.microsoft.com/fwlink/?linkid=194562)
</td>
<td style="border:1px solid black;">
[**MS10-059**](http://go.microsoft.com/fwlink/?linkid=196444)
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
[**Umiarkowany**](http://go.microsoft.com/fwlink/?linkid=21140)
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
[Windows 7 dla systemów 32-bitowych](http://www.microsoft.com/downloads/details.aspx?familyid=22e62b5c-e4c1-47d0-ae4a-8bd2d70d0a0a)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows 7 dla systemów 32-bitowych](http://www.microsoft.com/downloads/details.aspx?familyid=71716507-7080-4102-991e-6afc7cc377d5)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?familyid=31d0f5ac-2cff-42a1-8f18-128bbfc4e57d)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=ecaf42e0-a288-40c1-8602-21e967a87408)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows 7 dla systemów 32-bitowych](http://www.microsoft.com/downloads/details.aspx?familyid=8d58ebc4-a5f9-4318-a6f1-168c1bcdae3c)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows 7 dla systemów 32-bitowych](http://www.microsoft.com/downloads/details.aspx?familyid=2e782ac9-b5d5-490e-a01a-7d4481eab224)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=77d0c428-237c-4dab-9645-6400dd9e65f8)  
(KB983590)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows 7 dla systemów 32-bitowych](http://www.microsoft.com/downloads/details.aspx?familyid=a7d60864-5942-47ed-a6f3-1c07b4833a14)  
(Umiarkowany)
</td>
<td style="border:1px solid black;">
[Windows 7 dla systemów 32-bitowych](http://www.microsoft.com/downloads/details.aspx?familyid=68bddf4b-b597-477e-80e4-9293d7160496)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows 7 dla systemów 32-bitowych](http://www.microsoft.com/downloads/details.aspx?familyid=3a5a088e-644a-4a0e-9a09-0370bcd97688)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows 7 dla systemów 32-bitowych](http://www.microsoft.com/downloads/details.aspx?familyid=ce6233f3-2ee5-4329-908d-ba9b28ecc553)  
(Ważny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 dla systemów z procesorem x64
</td>
<td style="border:1px solid black;">
[Windows 7 dla systemów z procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=9499f771-c388-4de3-a5c7-8cc8b00b4395)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows 7 dla systemów z procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=c457d8ec-83b7-446f-b77c-e47d4187e616)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?familyid=a4f6d7c2-b475-4900-82f0-75f5be0b7b63)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=ca57a47a-9111-4abe-9356-4962ca2c1d65)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows 7 dla systemów z procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=ad1ddf94-d714-4b36-8256-42bf79d03a90)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows 7 dla systemów z procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=24751193-592f-4c44-a8d6-f4112d4f011b)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=77d0c428-237c-4dab-9645-6400dd9e65f8)  
(KB983590)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows 7 dla systemów z procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=b00ec47c-402e-4207-a4c9-6c1900f254f8)  
(Umiarkowany)
</td>
<td style="border:1px solid black;">
[Windows 7 dla systemów z procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=5ff09e03-d662-4b23-ab26-d25ca2ba58df)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows 7 dla systemów z procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=163fe2bd-f999-47c1-9a35-c4fc868bda51)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows 7 dla systemów z procesorem x64](http://www.microsoft.com/downloads/details.aspx?familyid=146270fa-cd6f-440a-aa3e-e93af0bff447)  
(Ważny)
</td>
</tr>
<tr>
<th colspan="14">
System Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS10-046**](http://go.microsoft.com/fwlink/?linkid=197393)
</td>
<td style="border:1px solid black;">
[**MS10-049**](http://go.microsoft.com/fwlink/?linkid=197104)
</td>
<td style="border:1px solid black;">
[**MS10-051**](http://go.microsoft.com/fwlink/?linkid=196268)
</td>
<td style="border:1px solid black;">
[**MS10-052**](http://go.microsoft.com/fwlink/?linkid=194432)
</td>
<td style="border:1px solid black;">
[**MS10-053**](http://go.microsoft.com/fwlink/?linkid=196549)
</td>
<td style="border:1px solid black;">
[**MS10-054**](http://go.microsoft.com/fwlink/?linkid=190318)
</td>
<td style="border:1px solid black;">
[**MS10-055**](http://go.microsoft.com/fwlink/?linkid=194906)
</td>
<td style="border:1px solid black;">
[**MS10-060**](http://go.microsoft.com/fwlink/?linkid=179830)
</td>
<td style="border:1px solid black;">
[**MS10-047**](http://go.microsoft.com/fwlink/?linkid=195812)
</td>
<td style="border:1px solid black;">
[**MS10-048**](http://go.microsoft.com/fwlink/?linkid=194552)
</td>
<td style="border:1px solid black;">
[**MS10-050**](http://go.microsoft.com/fwlink/?linkid=197103)
</td>
<td style="border:1px solid black;">
[**MS10-058**](http://go.microsoft.com/fwlink/?linkid=194562)
</td>
<td style="border:1px solid black;">
[**MS10-059**](http://go.microsoft.com/fwlink/?linkid=196444)
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
[**Krytyczny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Umiarkowany**](http://go.microsoft.com/fwlink/?linkid=21140)
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
[Windows Server 2008 R2 dla systemów opartych na procesorach x64](http://www.microsoft.com/downloads/details.aspx?familyid=0d9dd09b-db40-462b-88b0-4dbb8180e81f)\*  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach x64](http://www.microsoft.com/downloads/details.aspx?familyid=c9aeea25-ca14-4b42-9018-a27c9d8899c4)\*  
(Ważny)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?familyid=a48cdac5-4d78-49b5-a6d8-ecf6c58cace2)\*  
(Umiarkowany)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=e7757bbc-3ef0-421d-ab57-0083a302c77b)\*\*  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach x64](http://www.microsoft.com/downloads/details.aspx?familyid=52642a8d-1081-4496-848e-9b03baf3fdac)\*  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=77d0c428-237c-4dab-9645-6400dd9e65f8)\*  
(KB983590)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach x64](http://www.microsoft.com/downloads/details.aspx?familyid=c1ad1248-07f1-42d4-baa4-8a20837ec7b4)\*  
(Umiarkowany)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach x64](http://www.microsoft.com/downloads/details.aspx?familyid=6bbc9cb1-0b59-4473-adf9-2ce2f0f94c0a)\*  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach x64](http://www.microsoft.com/downloads/details.aspx?familyid=a1f95600-34e5-44b3-b2cb-b2b2cbf645cb)\*  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach x64](http://www.microsoft.com/downloads/details.aspx?familyid=333fb6e4-f867-4dcb-beb3-2d88e428ca2e)\*  
(Ważny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 dla systemów opartych na procesorach Itanium
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=ce2bb5d4-f661-44e3-ac28-0b81f7b72670)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=b7c2e91f-ca8a-4237-99c8-ca53c91cf73e)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Microsoft XML Core Services 3.0](http://www.microsoft.com/downloads/details.aspx?familyid=b4d3210e-f3ad-4dbb-9390-6e98eeb99eaa)  
(Umiarkowany)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=7b457d04-03a9-4eb0-ba6a-ab45267e4f74)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=783fb42c-3698-4b1d-a692-3ff319578931)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=77d0c428-237c-4dab-9645-6400dd9e65f8)  
(KB983590)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=f23dec0f-a33b-4d8c-a86d-0e9368ae7ff5)  
(Umiarkowany)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=2543191a-09cb-4417-bbb2-aac4d9a2a756)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=c3cd7f2f-e198-4fbd-a65d-21a1bf51eb61)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 dla systemów opartych na procesorach Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=62034ecb-a6bd-46c5-a03d-9642880bc2d6)  
(Ważny)
</td>
</tr>
</table>
 
**Uwagi dotyczące systemu Windows Server 2008 i Windows Server 2008 R2**

**\*Luka w zabezpieczeniach dotyczy instalacji Server Core.** Ta aktualizacja ma zastosowanie, z takim samym wskaźnikiem ważności, w przypadku obsługiwanych wersji systemu Windows Server 2008 lub Windows Server 2008 R2, niezależnie od tego, czy zostały zainstalowane przy użyciu opcji instalacji Server Core. Więcej informacji na temat tej opcji instalacji można znaleźć w artykułach TechNet, [Managing a Server Core Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) i [Servicing a Server Core Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) (jęz. ang.). Należy pamiętać, że opcja instalacji Server Core nie dotyczy niektórych wersji systemu Windows Server 2008 i Windows Server 2008 R2. Zobacz [Porównanie opcji instalacji Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Luka w zabezpieczeniach nie dotyczy instalacji Server Core.** Luki usuwane przez tę aktualizację zabezpieczeń nie dotyczą obsługiwanych wersji systemu Windows Server 2008 ani Windows Server 2008 R2, jeżeli systemy te zostały zainstalowane przy użyciu opcji instalacji Server Core. Więcej informacji na temat tej opcji instalacji można znaleźć w artykułach TechNet, [Managing a Server Core Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) i [Servicing a Server Core Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) (jęz. ang.). Należy pamiętać, że opcja instalacji Server Core nie dotyczy niektórych wersji systemu Windows Server 2008 i Windows Server 2008 R2. Zobacz [Porównanie opcji instalacji Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**Uwagi dotyczące biuletynu MS10-050**

<sup>[1]</sup>Te wersje programu Windows Movie Maker są dostarczane wraz ze wskazanymi systemami operacyjnymi.

<sup>[2]</sup>Program Windows Movie Maker 2.6 jest dostępny jako opcja do pobrania i można go zainstalować we wskazanych systemach operacyjnych.

**Uwaga dotycząca biuletynu MS10-060**

Zobacz także pozostałe kategorie oprogramowania w sekcji **Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki**, aby uzyskać więcej plików aktualizacji w ramach tego samego identyfikatora biuletynu. Ten biuletyn obejmuje więcej niż jedną kategorię oprogramowania.

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
[**MS10-056**](http://go.microsoft.com/fwlink/?linkid=196938)
</td>
<td style="border:1px solid black;">
[**MS10-057**](http://go.microsoft.com/fwlink/?linkid=196275)
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
[Microsoft Office Word 2002 z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=978eb887-25b6-4dde-a2ec-d2d1e7f1a434)  
(KB2251389)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2002 z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=032e1530-8736-4e1c-a704-967679227619)  
(KB2264397)  
(Ważny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2003 z dodatkiem Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2003 z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=4360bcec-0731-4d4a-89eb-7d28a4607f06)  
(KB2251399)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2003 z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=7cecbce3-bbb7-47d1-bda3-64d7e0f69f62)  
(KB2264403)  
(Ważny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
System Microsoft Office 2007 z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2007 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0d7210a3-662e-41e7-affc-ae94f9d89388)<sup>[1]</sup>
(KB2251419)  
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
[**MS10-056**](http://go.microsoft.com/fwlink/?linkid=196938)
</td>
<td style="border:1px solid black;">
[**MS10-057**](http://go.microsoft.com/fwlink/?linkid=196275)
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
[Microsoft Office 2004 dla komputerów Macintosh](http://www.microsoft.com/downloads/details.aspx?familyid=d2f44d4a-7cd8-4514-b3ff-1770bc47d595)  
(KB2284171)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2004 dla komputerów Macintosh](http://www.microsoft.com/downloads/details.aspx?familyid=d2f44d4a-7cd8-4514-b3ff-1770bc47d595)  
(KB2284171)  
(Ważny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2008 dla komputerów Macintosh
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 dla komputerów Macintosh](http://www.microsoft.com/downloads/details.aspx?familyid=6ece112f-0ca7-4b1f-ad20-603950edee66)  
(KB2284162)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 dla komputerów Macintosh](http://www.microsoft.com/downloads/details.aspx?familyid=6ece112f-0ca7-4b1f-ad20-603950edee66)  
(KB2284162)  
(Ważny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Open XML File Format Converter for Mac
</td>
<td style="border:1px solid black;">
[Open XML File Format Converter dla komputerów Macintosh](http://www.microsoft.com/downloads/details.aspx?familyid=a7b834a3-5a44-42d4-afe9-6ef207333834)  
(KB2284179)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Open XML File Format Converter dla komputerów Macintosh](http://www.microsoft.com/downloads/details.aspx?familyid=a7b834a3-5a44-42d4-afe9-6ef207333834)  
(KB2284179)  
(Ważny)
</td>
</tr>
<tr>
<th colspan="3">
Inne programy pakietu Office
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS10-056**](http://go.microsoft.com/fwlink/?linkid=196938)
</td>
<td style="border:1px solid black;">
[**MS10-057**](http://go.microsoft.com/fwlink/?linkid=196275)
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
Podgląd programu Microsoft Office Word
</td>
<td style="border:1px solid black;">
[Podgląd programu Microsoft Office Word](http://www.microsoft.com/downloads/details.aspx?familyid=39fe2229-9201-4270-bdc1-20bc8e30a766)  
(KB2251437)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Pakiet zgodności formatu plików pakietu Microsoft Office dla programów Word, Excel i PowerPoint 2007 z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Pakiet zgodności formatu plików pakietu Microsoft Office dla programów Word, Excel i PowerPoint 2007 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ed5b9671-651d-41f3-aed3-93ee8a28657f)  
(KB2277947)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Works 9
</td>
<td style="border:1px solid black;">
[Microsoft Works 9](http://www.microsoft.com/downloads/details.aspx?familyid=feb121ad-e5f6-40e2-bf12-045ae5c2a754)  
(KB2092914)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
</table>
 
**Uwaga dotycząca biuletynu MS10-056**

<sup>[1]</sup>Aby uchronić się przed działaniem luk opisanych w biuletynie MS10-056, użytkownicy programu Microsoft Office Word 2007 z dodatkiem Service Pack 2 poza pakietem aktualizacji zabezpieczeń KB2251419 muszą zainstalować także aktualizację zabezpieczeń Pakietu zgodności formatu plików pakietu Microsoft Office dla programów Word, Excel i PowerPoint 2007 z dodatkiem Service Pack 2 (KB2277947).

#### Narzędzia i oprogramowanie firmy Microsoft dla deweloperów

 
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
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
[**MS10-060**](http://go.microsoft.com/fwlink/?linkid=179830)
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
Microsoft Silverlight 2
</td>
<td style="border:1px solid black;">
[Microsoft Silverlight 2](http://www.microsoft.com/getsilverlight/get-started/install/default.aspx)<sup>[1]</sup> na komputerach Macintosh  
(KB982926)  
(Krytyczny)  
[Microsoft Silverlight 2](http://www.microsoft.com/getsilverlight/get-started/install/default.aspx)<sup>[1]</sup> we wszystkich wersjach klientów systemu Microsoft Windows  
(KB982926)  
(Krytyczny)  
[Microsoft Silverlight 2](http://www.microsoft.com/getsilverlight/get-started/install/default.aspx)<sup>[1]</sup> we wszystkich wersjach serwerów systemu Microsoft Windows\*\*  
(KB982926)  
(Krytyczny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Silverlight 3
</td>
<td style="border:1px solid black;">
[Microsoft Silverlight 3](http://www.microsoft.com/downloads/details.aspx?familyid=7e3f6c16-1339-49bc-a60c-ddc6c3a54850)<sup>[2]</sup> na komputerach Macintosh  
(KB978464)  
(Krytyczny)  
[Microsoft Silverlight 3](http://www.microsoft.com/downloads/details.aspx?familyid=7e3f6c16-1339-49bc-a60c-ddc6c3a54850)<sup>[2]</sup> we wszystkich wersjach klientów systemu Microsoft Windows  
(KB978464)  
(Krytyczny)  
[Microsoft Silverlight 3](http://www.microsoft.com/downloads/details.aspx?familyid=7e3f6c16-1339-49bc-a60c-ddc6c3a54850)<sup>[2]</sup> we wszystkich wersjach serwerów systemu Microsoft Windows\*\*  
(KB978464)  
(Krytyczny)
</td>
</tr>
</table>
 
**Uwagi dotyczące biuletynu MS10-060**

**\*\*Luka w zabezpieczeniach nie dotyczy instalacji Server Core.** Luki usuwane przez tę aktualizację zabezpieczeń nie dotyczą obsługiwanych wersji systemu Windows Server 2008 ani Windows Server 2008 R2, jeżeli systemy te zostały zainstalowane przy użyciu opcji instalacji Server Core. Więcej informacji na temat tej opcji instalacji można znaleźć w artykułach TechNet, [Managing a Server Core Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) i [Servicing a Server Core Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) (jęz. ang.). Należy pamiętać, że opcja instalacji Server Core nie dotyczy niektórych wersji systemu Windows Server 2008 i Windows Server 2008 R2. Zobacz [Porównanie opcji instalacji Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

<sup>[1]</sup>Ten plik do pobrania uaktalnia program Microsoft Silverlight 2 do nowszej wersji, która nie podlega lukom opisywanym w tym biuletynie.

<sup>[2]</sup>Ta aktualizacja uaktualnia program Microsoft Silverlight do nowszej kompilacji, która nie podlega lukom opisywanym w tym biuletynie.

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

**Narzędzie Microsoft Baseline Security Analyzer**

Narzędzie Microsoft Baseline Security Analyzer umożliwia administratorom skanowanie lokalnych i zdalnych systemów w poszukiwaniu brakujących aktualizacji zabezpieczeń oraz typowych błędów konfiguracji zabezpieczeń. Więcej informacji na temat narzędzia MBSA można znaleźć w witrynie sieci Web[Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134).

**Windows Server Update Services**

Program Windows Server Update Services (WSUS) pozwala administratorom IT na wdrażanie najnowszych aktualizacji produktów firmy Microsoft w komputerach działających pod kontrolą systemu Windows. Więcej informacji na temat sposobu wdrażania aktualizacji zabezpieczeń za pomocą programu Windows Server Update Services można znaleźć w [witrynie sieci Web usług Windows Server Update Services](http://technet.microsoft.com/en-us/wsus/default.aspx).

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

-   Sergey I. Ulasen i Oleg Kupreev z firmy [VirusBlokAda](http://www.anti-virus.by/) za zgłoszenie problemu opisanego w biuletynie MS10-046
-   Andreas Marx i Maik Morgenstern z firmy [AV-Test](http://www.av-test.org/) za zgłoszenie problemu opisanego w biuletynie MS10-046
-   Will Dormann z firmy [CERT/CC](http://www.cert.org) za współpracę nad problemem opisanym w biuletynie MS10-046
-   Niels Teusink za współpracę nad problemem opisanym w biuletynie MS10-046
-   Stefan Kanthak za współpracę nad problemem opisanym w biuletynie MS10-046
-   Tavis Ormandy z firmy [Google, Inc.](http://www.google.com/) za zgłoszenie trzech problemów opisanych w biuletynie MS10-047
-   Tavis Ormandy z firmy [Google, Inc.](http://www.google.com/) za zgłoszenie problemu opisanego w biuletynie MS10-048
-   Matthieu Suiche z firmy [MoonSols](http://moonsols.com/) za zgłoszenie dwóch problemów opisanych w biuletynie MS10-048
-   Matthieu Suiche z firmy [MoonSols](http://moonsols.com/) za współpracę z firmą Microsoft przy opracowywaniu zmian zabezpieczeń zawartych w biuletynie MS10-048
-   Nicolás Economou z firmy [Core Security Technologies](http://www.coresecurity.com/) za zgłoszenie problemu opisanego w biuletynie MS10-048
-   Marsh Ray i Steve Dispensa z firmy [PhoneFactor](http://www.phonefactor.com/) za zgłoszenie problemu opisanego w biuletynie MS10-049
-   Dyon Balding z firmy [Secunia](http://secunia.com/) za zgłoszenie problemu opisanego w biuletynie MS10-050
-   SkyLined z firmy [Google Inc.](http://www.google.com/) za zgłoszenie problemu opisanego w biuletynie MS10-051
-   Moritz Jodeit z firmy n.runs AG, we współpracy z oddziałem [Zero Day Initiative](http://www.zerodayinitiative.com/) firmy [TippingPoint](http://www.tippingpoint.com/) za zgłoszenie problemu opisanego w biuletynie MS10-052
-   David Bloom z firmy [Google Inc.](http://www.google.com/) za zgłoszenie problemu opisanego w biuletynie MS10-053
-   Nicolas Joly z firmy [VUPEN Vulnerability Research Team](http://www.vupen.com) za zgłoszenie czterech problemów opisanych w biuletynie MS10-053
-   Gambino ZaDarkSide za zgłoszenie problemu opisanego w biuletynie MS10-053
-   Laurent Gaffié z firmy [stratsec](http://www.stratsec.net/) za zgłoszenie problemu opisanego w biuletynie MS10-054
-   Todd Wease i Richard Johnson z firmy [Sourcefire VRT](http://www.sourcefire.com/services/sf_vrt.html) za zgłoszenie problemu opisanego w biuletynie MS10-054
-   Riku Hietamaki i Joshua Morin z firmy [Codenomicon](http://www.codenomicon.com/) za zgłoszenie problemu opisanego w biuletynie MS10-054
-   Anonimowemu analitykowi współpracującemu z oddziałem [Zero Day Initiative](http://www.zerodayinitiative.com/) firmy [TippingPoint](http://www.tippingpoint.com/) za zgłoszenie problemu opisanego w biuletynie MS10-055
-   L.W.Z z firmy [team509](http://www.team509.com/), we współpracy z oddziałem [Zero Day Initiative](http://www.zerodayinitiative.com/) firmy [TippingPoint](http://www.tippingpoint.com/), za zgłoszenie problemu opisanego w biuletynie MS10-056
-   Wushi z firmy [team509](http://www.team509.com/), we współpracy z firmą [VeriSign iDefense Labs](http://labs.idefense.com/), za zgłoszenie problemu opisanego w biuletynie MS10-056
-   [team509](http://www.team509.com/), współpracownikowi firmy [Verisign iDefense Labs](http://labs.idefense.com/), za zgłoszenie problemu opisanego w biuletynie MS10-056
-   Rodrigo Rubira Branco z firmy [Check Point](http://www.checkpoint.com/) IPS Research Team za zgłoszenie problemu opisanego w biuletynie MS10-056
-   Anonimowy analityk współpracujący z oddziałem [Zero Day Initiative](http://www.zerodayinitiative.com/) firmy [TippingPoint](http://www.tippingpoint.com/) za zgłoszenie problemu opisanego w biuletynie MS10-056
-   Damián Frizza z firmy [Core Security Technologies](http://www.coresecurity.com/), za zgłoszenie problemu opisanego w biuletynie MS10-057
-   Darren Willis z firmy [Fourteenforty Research Institute, Inc.](http://www.fourteenforty.jp/) za zgłoszenie problemu opisanego w biuletynie MS10-058
-   Matthieu Suiche z firmy [MoonSols](http://moonsols.com/) za zgłoszenie problemu opisanego w biuletynie MS10-058
-   Cesar Cerrudo z firmy [Argeniss](http://www.argeniss.com/) za współpracę z firmą Microsoft nad dwoma problemami opisanymi w biuletynie MS10-059
-   Carsten Book z firmy za zgłoszenie problemu opisanego w biuletynie MS10-060
-   [Eamon Nerbonne](http://eamon.nerbonne.org/) za zgłoszenie luki opisanej w biuletynie MS10-060

#### Pomoc techniczna

-   Wymienione oprogramowanie zostało przetestowane w celu ustalenia, których wersji dotyczy problem. Dla pozostałych wersji upłynął okres pomocy technicznej. Aby zapoznać się z zasadami cyklu pomocy technicznej dotyczącymi używanej wersji oprogramowania, odwiedź [witrynę zasad cyklu pomocy technicznej firmy Microsoft](http://go.microsoft.com/fwlink/?linkid=21742).
-   Klienci mogą uzyskać pomoc techniczną w [Biurze Obsługi Klienta Microsoft](http://go.microsoft.com/fwlink/?linkid=21131) pod numerem 0 801 308 801 (koszt połączenia to jeden impuls połączenia lokalnego) lub (0-22) 594 19 99 w godzinach od 9:00 do 17:00, od poniedziałku do piątku. Połączenia z działem pomocy technicznej związane z aktualizacjami zabezpieczeń są bezpłatne. Dodatkowe informacje dotyczące możliwości skorzystania z pomocy technicznej można znaleźć w witrynie [Pomoc i obsługa techniczna firmy Microsoft](http://support.microsoft.com/).
-   Klienci międzynarodowi mogą uzyskać pomoc w lokalnych przedstawicielstwach firmy Microsoft. Pomoc techniczna związana z aktualizacjami zabezpieczeń jest bezpłatna. Informacje o sposobie kontaktowania się z pomocą techniczną firmy Microsoft są dostępne w [międzynarodowej witrynie sieci Web pomocy i obsługi technicznej](http://go.microsoft.com/fwlink/?linkid=21155).

#### Zrzeczenie odpowiedzialności

Informacje w bazie wiedzy Microsoft Knowledge Base są dostarczane „tak jak są” bez jakiejkolwiek gwarancji. Firma Microsoft odrzuca wszelkie gwarancje, wyraźne i dorozumiane, w tym gwarancje dotyczące wartości handlowej i przydatności do określonego celu. Firma Microsoft Corporation ani jej dostawcy w żadnym wypadku nie ponoszą odpowiedzialności za jakiekolwiek szkody, w tym bezpośrednie, pośrednie, przypadkowe, wynikowe, utratę zysków handlowych lub szkody specjalne, nawet jeżeli firmę Microsoft Corporation lub jej dostawców powiadomiono o możliwości zaistnienia takich szkód. W niektórych stanach wyłączenie lub ograniczenie odpowiedzialności za straty wynikowe lub przypadkowe, a więc i powyższe ograniczenia, nie mają zastosowania.

#### Wersje

-   Wer. 1.0 (2 sierpnia 2010 r.): Opublikowane podsumowanie biuletynów zabezpieczeń.
-   Wer. 2.0 (10 sierpnia 2010 r.): Dodano biuletyny: MS10-047-MS10-060.
-   Wersja 2.1 (1 września 2010 r.): Do biuletynu MS10-056 dodano informację dla użytkowników programu Word 2007, że oprócz pakietu aktualizacji zabezpieczeń KB2251419 muszą również zainstalować pakiet aktualizacji zabezpieczeń KB2277947.

*Built at 2014-04-18T01:50:00Z-07:00*
