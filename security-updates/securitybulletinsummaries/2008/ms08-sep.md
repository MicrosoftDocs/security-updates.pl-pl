---
TOCTitle: 'MS08-SEP'
Title: 'Podsumowanie biuletynów zabezpieczeń firmy Microsoft za wrzesień 2008 r.'
ms:assetid: 'ms08-sep'
ms:contentKeyID: 61233095
ms:mtpsurl: 'https://technet.microsoft.com/pl-PL/library/ms08-sep(v=Security.10)'
---

Podsumowanie biuletynów zabezpieczeń firmy Microsoft za wrzesień 2008 r.
========================================================================

Opublikowano: 9 września 2008 | Zaktualizowano: 9 grudnia 2008

**Wersja:** 3.0

Niniejsze podsumowanie biuletynów zabezpieczeń zawiera spis biuletynów za wrzesień 2008 r.

Z chwilą opublikowania biuletynów za wrzesień 2008 r. niniejsze podsumowanie biuletynów zastępuje powiadomienie o biuletynach zabezpieczeń wydane 4 września 2008 r. Aby uzyskać więcej informacji na temat usługi powiadamiania o biuletynach, zobacz [Powiadomienia o biuletynach zabezpieczeń firmy Microsoft (j. ang.)](http://technet.microsoft.com/security/bulletin/advance).

Aby dowiedzieć się, jak otrzymywać automatyczne powiadomienia o publikacji biuletynów zabezpieczeń firmy Microsoft, odwiedź stronę [Microsoft Technical Security Notifications](http://go.microsoft.com/fwlink/?linkid=21163).

10 września 2008 r. o godz. 11:00 czasu Pacyfiku (godz. 20:00 czasu środkowoeuropejskiego) firma Microsoft udostępni emisję internetową, w której znajdą się odpowiedzi na pytania klientów dotyczące tych biuletynów (USA i Kanada). [Zarejestruj się, aby zobaczyć emisję internetową dotyczącą biuletynów zabezpieczeń za wrzesień](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032374633&eventcategory=4&culture=en-us&countrycode=us). Po tym dniu emisja internetowa będzie dostępna na żądanie. Aby uzyskać więcej informacji, zobacz [Podsumowania biuletynów zabezpieczeń i emisje internetowe firmy Microsoft](http://technet.microsoft.com/security/bulletin/summary).

Firma Microsoft udostępnia także informacje, dzięki którym klienci mogą ustalić priorytety dla aktualizacji zabezpieczeń w związku z niezwiązanymi z zabezpieczeniami aktualizacjami o wysokim priorytecie, które publikowane są w tym samym dniu, co comiesięczne aktualizacje zabezpieczeń. Zapoznaj się z sekcją **Inne informacje**.

### Informacje o biuletynie

#### Streszczenia

W bieżącym miesiącu opublikowano następujące biuletyny (w kolejności wskaźnika ważności):

Krytyczny (4)
-------------

<span></span>

| Identyfikator biuletynu               | Biuletyn zabezpieczeń firmy Microsoft MS08-054                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
|---------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**                   | [**Luka w zabezpieczeniach programu Windows Media Player potencjalnie umożliwia zdalne wykonanie kodu (954154)**](http://go.microsoft.com/fwlink/?linkid=121739)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| **Streszczenie**                      | Niniejsza aktualizacja zabezpieczeń usuwa zgłoszoną przez użytkowników lukę w zabezpieczeniach programu Windows Media Player, która potencjalnie umożliwia zdalne wykonanie kodu przy strumieniowym przesyłaniu specjalnie spreparowanego pliku audio z serwera Windows Media. Jeśli użytkownik jest zalogowany jako administrator, osoba atakująca, która pomyślnie wykorzysta tę lukę, może uzyskać pełną kontrolę nad systemem, którego ta luka dotyczy. Osoba taka może wówczas instalować programy, przeglądać, zmieniać i usuwać dane oraz tworzyć nowe konta z pełnymi uprawnieniami. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi. |
| **Maksymalny wskaźnik ważności:**     | [Krytyczny](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **Wpływ luki**                        | Zdalne wykonanie kodu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| **Wykrywanie**                        | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Ta aktualizacja nie wymaga ponownego uruchomienia komputera.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Programy, których dotyczy problem** | **Microsoft Windows.** Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |

| Identyfikator biuletynu               | Biuletyn zabezpieczeń firmy Microsoft MS08-052                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
|---------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**                   | [**Luki w zabezpieczeniach interfejsu GDI+ umożliwiają zdalne wykonanie kodu (954593)**](http://go.microsoft.com/fwlink/?linkid=125468)                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| **Streszczenie**                      | Ta aktualizacja zabezpieczeń usuwa kilka luk w zabezpieczeniach interfejsu Microsoft Windows GDI+, które zostały zgłoszone przez użytkowników. Luki te umożliwiają zdalne wykonanie kodu, jeśli użytkownik wyświetli specjalnie spreparowany plik obrazu przy użyciu oprogramowania dotkniętego problemem, lub jeśli przejdzie do witryny sieci Web zawierającej specjalnie spreparowaną zawartość. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi. |
| **Maksymalny wskaźnik ważności:**     | [Krytyczny](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Wpływ luki**                        | Zdalne wykonanie kodu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| **Wykrywanie**                        | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Aktualizacja wymaga ponownego uruchomienia systemu.                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Programy, których dotyczy problem** | **Microsoft Windows, Internet Explorer, .NET Framework, Office, SQL Server, Visual Studio.** Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                                                                                                                      |

| Identyfikator biuletynu               | Biuletyn zabezpieczeń firmy Microsoft MS08-053                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
|---------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**                   | [**Luka w zabezpieczeniach programu Windows Media Encoder 9 potencjalnie umożliwia zdalne wykonanie kodu (954156)**](http://go.microsoft.com/fwlink/?linkid=123091)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| **Streszczenie**                      | Ta aktualizacja zabezpieczeń usuwa zgłoszoną przez użytkowników lukę w zabezpieczeniach programu Windows Media Encoder 9 Series. Ta luka w zabezpieczeniach umożliwia zdalne wykonanie kodu, jeśli użytkownik wyświetli specjalnie spreparowaną stronę sieci Web. Jeśli użytkownik jest zalogowany jako administrator, osoba atakująca, która pomyślnie wykorzysta tę lukę, może uzyskać pełną kontrolę nad systemem, którego ta luka dotyczy. Osoba taka może wówczas instalować programy, przeglądać, zmieniać i usuwać dane oraz tworzyć nowe konta z pełnymi uprawnieniami. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi. |
| **Maksymalny wskaźnik ważności:**     | [Krytyczny](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| **Wpływ luki**                        | Zdalne wykonanie kodu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Wykrywanie**                        | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Aktualizacja może wymagać ponownego uruchomienia komputera.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **Programy, których dotyczy problem** | **Microsoft Windows.** Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |

| Identyfikator biuletynu               | Biuletyn zabezpieczeń firmy Microsoft MS08-055                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
|---------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**                   | [**Luka w zabezpieczeniach pakietu Microsoft Office umożliwia zdalne wykonanie kodu (955047)**](http://go.microsoft.com/fwlink/?linkid=125229)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Streszczenie**                      | Ta krytyczna aktualizacja zabezpieczeń usuwa lukę w zabezpieczeniach pakietu Microsoft Office, która została zgłoszona przez użytkowników. Luka ta może pozwolić na zdalne wykonanie kodu, jeśli użytkownik kliknie specjalnie spreparowany adres URL programu OneNote. Osoba atakująca, której uda się wykorzystać tę lukę, może uzyskać pełną kontrolę nad systemem, którego dotyczy luka. Osoba taka może wówczas instalować programy, przeglądać, zmieniać i usuwać dane oraz tworzyć nowe konta z pełnymi uprawnieniami. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi. |
| **Maksymalny wskaźnik ważności:**     | [Krytyczny](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| **Wpływ luki**                        | Zdalne wykonanie kodu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Wykrywanie**                        | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Ta aktualizacja zazwyczaj nie wymaga ponownego uruchomienia komputera.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| **Programy, których dotyczy problem** | **Microsoft Office.** Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |

Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki
---------------------------------------------------------------------------------

<span></span>
**W jaki sposób korzystać z tej tabeli?**

Tabela ta pozwala odczytać informacje o aktualizacjach zabezpieczeń, których zainstalowanie może być konieczne. Należy przejrzeć informacje dla każdego wymienionego programu lub składnika oprogramowania w celu sprawdzenia, czy są wymagane aktualizacje zabezpieczeń. Jeśli program lub składnik znajduje się na liście, dostępne jest łącze prowadzące do aktualizacji oprogramowania i podana jest informacja o wskaźniku ważności tej aktualizacji.

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
[**MS08-054**](http://go.microsoft.com/fwlink/?linkid=121739)
</td>
<td style="border:1px solid black;">
[**MS08-052**](http://go.microsoft.com/fwlink/?linkid=125468)
</td>
<td style="border:1px solid black;">
[**MS08-053**](http://go.microsoft.com/fwlink/?linkid=123091)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Maksymalny wskaźnik ważności biuletynu**
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
Microsoft Windows 2000 z dodatkiem Service Pack 4
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=a860d2d9-653d-4ddb-bbff-323d3ccdb866)  
(KB938464)  
(Krytyczny)  
[Microsoft .NET Framework 1.0 z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=c7cbcd19-acc1-4a89-adfa-99b2f431510d)  
(KB947739)  
(Brak wskaźnika ważności)  
[Microsoft .NET Framework 1.1 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6013f866-3ea1-4672-b1bf-e516204c3a7a)  
(KB947742)  
(Brak wskaźnika ważności)  
[Microsoft .NET Framework 2.0](http://www.microsoft.com/downloads/details.aspx?familyid=7f1cd013-2c4b-4582-9114-cb840a96124a)  
(KB947746)  
(Brak wskaźnika ważności)  
[Microsoft .NET Framework 2.0 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=215b73a3-46ab-44a8-a0fb-6d37bd1c39b8)  
(KB947748)  
(Brak wskaźnika ważności)
</td>
<td style="border:1px solid black;">
[Windows Media Encoder 9 Series](http://www.microsoft.com/downloads/details.aspx?familyid=0cabfbc0-db5d-4a6a-a4cd-e6df89ac2b25)  
(Krytyczny)
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
[**MS08-054**](http://go.microsoft.com/fwlink/?linkid=121739)
</td>
<td style="border:1px solid black;">
[**MS08-052**](http://go.microsoft.com/fwlink/?linkid=125468)
</td>
<td style="border:1px solid black;">
[**MS08-053**](http://go.microsoft.com/fwlink/?linkid=123091)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Maksymalny wskaźnik ważności biuletynu**
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
Windows XP z dodatkiem Service Pack 2 i Windows XP z dodatkiem Service Pack 3
</td>
<td style="border:1px solid black;">
[Windows Media Player 11](http://www.microsoft.com/downloads/details.aspx?familyid=d5891180-5dd1-49ec-bcc6-3030a544202c)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows XP z dodatkiem Service Pack 2 i Windows XP z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=e0bd6fbe-f46e-4961-9a79-49ec77d39439)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Media Encoder 9 Series](http://www.microsoft.com/downloads/details.aspx?familyid=57bcb3c2-49d3-4f18-8d03-36abd03d7403)  
(Krytyczny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition oraz Microsoft Windows XP Professional x64 Edition z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Media Player 11](http://www.microsoft.com/downloads/details.aspx?familyid=caf8a45e-a9f8-4e91-98fd-87eddbeae64c)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition oraz Windows XP Professional x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c5d26771-1f49-4bbf-902c-bf92e527cadb)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Media Encoder 9 Series](http://www.microsoft.com/downloads/details.aspx?familyid=18efea9e-b103-46de-90d9-5e295854cec3)  
(Krytyczny)  
[Windows Media Encoder 9 Series x64 Edition](http://www.microsoft.com/downloads/details.aspx?familyid=ebc1737c-6e78-4244-a1b2-a56d031f16e9)  
(Krytyczny)
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
[**MS08-054**](http://go.microsoft.com/fwlink/?linkid=121739)
</td>
<td style="border:1px solid black;">
[**MS08-052**](http://go.microsoft.com/fwlink/?linkid=125468)
</td>
<td style="border:1px solid black;">
[**MS08-053**](http://go.microsoft.com/fwlink/?linkid=123091)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Maksymalny wskaźnik ważności biuletynu**
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
Windows Server 2003 z dodatkiem Service Pack 1 i Windows Server 2003 z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem Service Pack 1 i Windows Server 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ac03f138-eca4-46e1-9782-e811820e547f)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Media Encoder 9 Series](http://www.microsoft.com/downloads/details.aspx?familyid=54ce1080-94cf-4e4f-8e09-a7dbab2757c5)  
(Umiarkowany)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition i Windows Server 2003 x64 Edition z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition i Windows Server 2003 x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=93f1451b-5b62-47e5-8f0c-b720b957999a)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Media Encoder 9 Series](http://www.microsoft.com/downloads/details.aspx?familyid=c83011cd-90b8-494c-9cad-fa055e101992)  
(Umiarkowany)  
[Windows Media Encoder 9 Series x64 Edition](http://www.microsoft.com/downloads/details.aspx?familyid=d8f1b782-136b-443f-b5f2-63aa4d1fd94a)  
(Umiarkowany)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Systemy operacyjne Windows Server 2003 z dodatkiem SP1 dla systemów z procesorem Itanium oraz Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem SP1 dla systemów z procesorem Itanium oraz Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=14e99f8a-cdd4-40d7-8cfc-73ae6bd6dfad)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
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
[**MS08-054**](http://go.microsoft.com/fwlink/?linkid=121739)
</td>
<td style="border:1px solid black;">
[**MS08-052**](http://go.microsoft.com/fwlink/?linkid=125468)
</td>
<td style="border:1px solid black;">
[**MS08-053**](http://go.microsoft.com/fwlink/?linkid=123091)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Maksymalny wskaźnik ważności biuletynu**
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
Windows Vista i Windows Vista z dodatkiem Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Media Player 11](http://www.microsoft.com/downloads/details.aspx?familyid=2f4118fd-1ffb-46da-b922-cd4ca4f9d84e)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Vista i Windows Vista z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=16f3ad21-ed77-4c32-93df-3b650b2b32a5)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Media Encoder 9 Series](http://www.microsoft.com/downloads/details.aspx?familyid=99beebc4-553a-46f8-8245-e3d932306c93)  
(Krytyczny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition i Windows Vista x64 Edition z dodatkiem Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Media Player 11](http://www.microsoft.com/downloads/details.aspx?familyid=334352e7-d41f-494f-866d-f1f1745ffd17)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition i Windows Vista x64 Edition z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=aa47d016-f5c9-4586-8876-f1f4f255f54d)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Media Encoder 9 Series](http://www.microsoft.com/downloads/details.aspx?familyid=99beebc4-553a-46f8-8245-e3d932306c93)  
(Krytyczny)  
[Windows Media Encoder 9 Series x64 Edition](http://www.microsoft.com/downloads/details.aspx?familyid=54d1279a-7f26-4727-a39d-5505bcd4fc53)  
(Krytyczny)
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
[**MS08-054**](http://go.microsoft.com/fwlink/?linkid=121739)
</td>
<td style="border:1px solid black;">
[**MS08-052**](http://go.microsoft.com/fwlink/?linkid=125468)
</td>
<td style="border:1px solid black;">
[**MS08-053**](http://go.microsoft.com/fwlink/?linkid=123091)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Maksymalny wskaźnik ważności biuletynu**
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
Windows Server 2008 dla systemów 32-bitowych
</td>
<td style="border:1px solid black;">
[Windows Media Player 11](http://www.microsoft.com/downloads/details.aspx?familyid=72fc6028-6af4-44ec-8d2a-28c53807d6bc)\*  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów 32-bitowych\*](http://www.microsoft.com/downloads/details.aspx?familyid=23bd3be5-cc66-46f8-9420-49d65d8afe1d)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Media Encoder 9 Series](http://www.microsoft.com/downloads/details.aspx?familyid=5434ca66-5a6b-4517-92fb-72dea0a172ec)\*  
(Umiarkowany)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 dla systemów opartych na procesorach X64
</td>
<td style="border:1px solid black;">
[Windows Media Player 11](http://www.microsoft.com/downloads/details.aspx?familyid=3906512b-26db-473e-b522-3883ff34a21c)\*  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów opartych na procesorach X64](http://www.microsoft.com/downloads/details.aspx?familyid=7f1e0f05-6c9d-4ad1-9b19-50ee4fa7bd7e)\*  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Media Encoder 9 Series](http://www.microsoft.com/downloads/details.aspx?familyid=5434ca66-5a6b-4517-92fb-72dea0a172ec)\*  
(Umiarkowany)  
[Windows Media Encoder 9 Series x64 Edition](http://www.microsoft.com/downloads/details.aspx?familyid=e30f9427-26d0-4e86-b9b8-bc637c3b5734)\*  
(Umiarkowany)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 dla systemów z procesorem Itanium
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=5159bdba-3825-4816-a2be-ab035332b9e2)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
</table>
 
**\*Luka w zabezpieczeniach nie dotyczy instalacji Server Core systemu operacyjnego Windows Server 2008.** Lukom usuwanym przez te aktualizacje zabezpieczeń nie podlegają obsługiwane wersje systemu Windows Server 2008, jeśli został on zainstalowany przy użyciu opcji instalacji Server Core, mimo że na komputerze mogą znajdować się pliki, których dotyczą omawiane luki. Aktualizacja ta będzie jednak w dalszym ciągu oferowana użytkownikom posiadającym pliki podlegające luce, ponieważ zaktualizowane pliki są nowsze (mają wyższe numery wersji) niż pliki znajdujące się obecnie w systemie. Aby uzyskać więcej informacji na temat tej opcji instalacji, zobacz [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Należy pamiętać, że opcja instalacji Server Core nie dotyczy niektórych wersji systemu Windows Server 2008; zobacz [Porównanie opcji instalacji Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

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
[**MS08-052**](http://go.microsoft.com/fwlink/?linkid=125468)
</td>
<td style="border:1px solid black;">
[**MS08-055**](http://go.microsoft.com/fwlink/?linkid=125229)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Maksymalny wskaźnik ważności biuletynu**
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
Microsoft Office XP z dodatkiem Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office XP z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=ef3de64c-fc17-4500-9da4-a3bba97fda6d)  
(KB953405)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Microsoft Office XP z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=ef3de64c-fc17-4500-9da4-a3bba97fda6d)  
(KB953405)  
(Ważny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2003 z dodatkiem Service Pack 2 i Microsoft Office 2003 z dodatkiem Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e9f8e309-d721-4bab-b485-5eede8d49eb8)  
(KB954478)  
(Ważny)  
[Microsoft Office 2003 z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=e9f8e309-d721-4bab-b485-5eede8d49eb8)  
(KB954478)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e670ad22-d3c1-41f7-ba30-6a67139feaa3)  
(KB953404)  
(Ważny)  
[Microsoft Office 2003 z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=e670ad22-d3c1-41f7-ba30-6a67139feaa3)  
(KB953404)  
(Ważny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2007 i Microsoft Office 2007 z dodatkiem Service Pack 1
</td>
<td style="border:1px solid black;">
[System Microsoft Office 2007](http://www.microsoft.com/downloads/details.aspx?familyid=4b656fe8-6253-490c-a81a-e4e8f0bb58d2)  
(KB954326)  
(Ważny)  
[Pakiet Microsoft Office 2007 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=4b656fe8-6253-490c-a81a-e4e8f0bb58d2)  
(KB954326)  
(Ważny)
</td>
<td style="border:1px solid black;">
[System Microsoft Office 2007](http://www.microsoft.com/downloads/details.aspx?familyid=fb457536-26c5-428b-97e4-1fc13718266e)  
(KB951944)  
(Ważny)  
[Pakiet Microsoft Office 2007 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=fb457536-26c5-428b-97e4-1fc13718266e)  
(KB951944)  
(Ważny)
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
[**MS08-052**](http://go.microsoft.com/fwlink/?linkid=125468)
</td>
<td style="border:1px solid black;">
[**MS08-055**](http://go.microsoft.com/fwlink/?linkid=125229)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Maksymalny wskaźnik ważności biuletynu**
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
Microsoft Office Project 2002 z dodatkiem Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Office Project 2002 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ef3de64c-fc17-4500-9da4-a3bba97fda6d)  
(KB953405)\*  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visio 2002 z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Visio 2002 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a6d9d3ef-f087-4f61-9ec1-522b7d4b9c48)  
(KB954479)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Podgląd programu Microsoft Office Word, Podgląd programu Microsoft Word 2003, Podgląd programu Microsoft Word 2003 z dodatkiem Service Pack 3, Podgląd programu Microsoft Office Excel 2003, Podgląd programu Microsoft Office Excel 2003 z dodatkiem Service Pack 3
</td>
<td style="border:1px solid black;">
[Podgląd programu Microsoft Office Word, Podgląd programu Microsoft Word 2003, Podgląd programu Microsoft Word 2003 z dodatkiem Service Pack 3, Podgląd programu Microsoft Office Excel 2003, Podgląd programu Microsoft Office Excel 2003 z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=e9f8e309-d721-4bab-b485-5eede8d49eb8)  
(KB954478)\*\*  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Podgląd programu Microsoft Office PowerPoint 2003
</td>
<td style="border:1px solid black;">
[Podgląd programu Microsoft Office PowerPoint 2003](http://www.microsoft.com/downloads/details.aspx?familyid=cd503f08-1831-45ff-bdf4-dd918ca40505)  
(KB956500)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Podgląd programu Microsoft Office Excel, Podgląd programu Microsoft Office PowerPoint 2007, Podgląd programu Microsoft Office PowerPoint 2007 z dodatkiem Service Pack 1
</td>
<td style="border:1px solid black;">
[Podgląd programu Microsoft Office Excel, Podgląd programu Microsoft Office PowerPoint 2007, Podgląd programu Microsoft Office PowerPoint 2007 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=4b656fe8-6253-490c-a81a-e4e8f0bb58d2)  
(KB954326)\*\*\*  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Pakiet zgodności formatu plików pakietu Microsoft Office dla programów Word, Excel i PowerPoint 2007 i Pakiet zgodności formatu plików pakietu Microsoft Office dla programów Word, Excel i PowerPoint 2007 z dodatkiem Service Pack 1
</td>
<td style="border:1px solid black;">
[Pakiet zgodności formatu plików pakietu Microsoft Office dla programów Word, Excel i PowerPoint 2007 i Pakiet zgodności formatu plików pakietu Microsoft Office dla programów Word, Excel i PowerPoint 2007 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=4b656fe8-6253-490c-a81a-e4e8f0bb58d2)  
(KB954326)\*\*\*  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Expression Web i Microsoft Expression Web 2
</td>
<td style="border:1px solid black;">
[Microsoft Expression Web i Microsoft Expression Web 2](http://www.microsoft.com/downloads/details.aspx?familyid=4b656fe8-6253-490c-a81a-e4e8f0bb58d2)  
(KB954326)\*\*\*  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Groove 2007 i Microsoft Office Groove 2007 z dodatkiem Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Office Groove 2007 i Microsoft Office Groove 2007 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=4b656fe8-6253-490c-a81a-e4e8f0bb58d2)  
(KB954326)\*\*\*  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Works
</td>
<td style="border:1px solid black;">
[Microsoft Works 8](http://www.microsoft.com/downloads/details.aspx?familyid=eb0d224e-a517-40d9-9fc6-2345fa12a841)  
(KB956483)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Digital Image Suite 2006
</td>
<td style="border:1px solid black;">
[Microsoft Digital Image Suite 2006](http://www.microsoft.com/downloads/details.aspx?familyid=04afd760-8173-4069-9e82-d3bf053d9eae)  
(KB955992)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office OneNote 2007
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Microsoft Office OneNote 2007](http://www.microsoft.com/downloads/details.aspx?familyid=8ac3576c-7873-4ac6-8bbc-033f6a7bb395)  
(KB950130)  
(Krytyczny)  
[Microsoft Office OneNote 2007 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=8ac3576c-7873-4ac6-8bbc-033f6a7bb395)  
(KB950130)  
(Krytyczny)
</td>
</tr>
</table>
 
\*Aktualizacja dla tego oprogramowania, którego dotyczy problem, jest tożsama z aktualizacją dla pakietu Microsoft Office XP z dodatkiem Service Pack 3.

\*\*Aktualizacja dla tego oprogramowania, którego dotyczy problem, jest tożsama z aktualizacją dla pakietu Microsoft Office 2003 z dodatkiem Service Pack 2 i Microsoft Office 2003 z dodatkiem Service Pack 3.

\*\*\*Aktualizacja dla tego oprogramowania, którego dotyczy problem, jest tożsama z aktualizacją dla pakietów Microsoft Office System 2007 i Microsoft Office System 2007 z dodatkiem Service Pack 1.

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
[**MS08-052**](http://go.microsoft.com/fwlink/?linkid=125468)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Maksymalny wskaźnik ważności biuletynu**
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
Aktualizacja GDR:  
Nie dotyczy  
Aktualizacja QFE:  
[SQL Server 2000 Reporting Services z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5f9e7f78-7439-414b-a9dc-a779b89427db)  
(KB954609)  
(Krytyczny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
SQL Server 2005 z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
Aktualizacja GDR:  
[SQL Server 2005 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4603c722-2468-4adb-b945-2ed0458b8f47)  
(KB954606)  
(Krytyczny)  
Aktualizacja QFE:  
[SQL Server 2005 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5148b887-f323-4adb-9721-61e1c0cfd213)  
(KB954607)  
(Krytyczny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
SQL Server 2005 x64 Edition z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
Aktualizacja GDR:  
[SQL Server 2005 x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4603c722-2468-4adb-b945-2ed0458b8f47)  
(KB954606)  
(Krytyczny)  
Aktualizacja QFE:  
[SQL Server 2005 x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5148b887-f323-4adb-9721-61e1c0cfd213)  
(KB954607)  
(Krytyczny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
SQL Server 2005 dla systemów z procesorem Itanium z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
Aktualizacja GDR:  
[SQL Server 2005 dla systemów z procesorem Itanium z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4603c722-2468-4adb-b945-2ed0458b8f47)  
(KB954606)  
(Krytyczny)  
Aktualizacja QFE:  
[SQL Server 2005 dla systemów z procesorem Itanium z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5148b887-f323-4adb-9721-61e1c0cfd213)  
(KB954607)  
(Krytyczny)
</td>
</tr>
</table>
 

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
Microsoft Visual Studio
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS08-052**](http://go.microsoft.com/fwlink/?linkid=125468)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Maksymalny wskaźnik ważności biuletynu**
</td>
<td style="border:1px solid black;">
[**Krytyczny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visual Studio .NET 2002 z dodatkiem Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio .NET 2002 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7848a652-4025-44bb-9c98-37a078b56d01)  
(KB947736)  
(Brak wskaźnika ważności)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual Studio .NET 2003 z dodatkiem Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio .NET 2003 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=9bc1e8f8-6c30-4aa0-90f5-fbb0ad5fd90e)  
(KB947737)  
(Brak wskaźnika ważności)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visual Studio 2005 z dodatkiem Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio 2005 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=a7bf790b-3249-4ee8-9440-fa911ebbc08a)  
(KB947738)  
(Brak wskaźnika ważności)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual Studio 2008
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio 2008](http://www.microsoft.com/downloads/details.aspx?familyid=a8c80b29-6d00-4949-a005-5d706122919a)  
(KB952241)  
(Brak wskaźnika ważności)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Pakiet redystrybucyjny narzędzia Microsoft Report Viewer 2005 z dodatkiem Service Pack 1
</td>
<td style="border:1px solid black;">
[Pakiet redystrybucyjny narzędzia Microsoft Report Viewer 2005 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=82833f27-081d-4b72-83ef-2836360a904d)  
(KB954765)  
(Krytyczny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Pakiet redystrybucyjny narzędzia Microsoft Report Viewer 2008
</td>
<td style="border:1px solid black;">
[Pakiet redystrybucyjny narzędzia Microsoft Report Viewer 2008](http://www.microsoft.com/downloads/details.aspx?familyid=6ae0aa19-3e6c-474c-9d57-05b2347456b1)  
(KB954766)  
(Krytyczny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visual FoxPro 8.0 z dodatkiem Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Visual FoxPro 8.0 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1f4371b9-b8be-4455-94d2-2304ee340543) zainstalowany w systemie Microsoft Windows 2000 z dodatkiem Service Pack 4  
(KB955368)  
(Brak wskaźnika ważności)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual FoxPro 9.0 z dodatkiem Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Visual FoxPro 9.0 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=49b21e30-722d-446e-9020-aceb3870db69) zainstalowany w systemie Microsoft Windows 2000 z dodatkiem Service Pack 4  
(KB955369)  
(Brak wskaźnika ważności)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visual FoxPro 9.0 z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Visual FoxPro 9.0 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=36957f47-9d8b-477d-bd60-5959e5a2eafa) zainstalowany w systemie Microsoft Windows 2000 z dodatkiem Service Pack 4  
(KB955370)  
(Brak wskaźnika ważności)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Zestaw SDK platformy Microsoft do dystrybucji: GDI+
</td>
<td style="border:1px solid black;">
[Zestaw SDK platformy Microsoft do dystrybucji: GDI+](http://www.microsoft.com/downloads/details.aspx?familyid=6a63ab9c-df12-4d41-933c-be590feaa05a)  
(Brak wskaźnika ważności)
</td>
</tr>
</table>
 

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
[**MS08-052**](http://go.microsoft.com/fwlink/?linkid=125468)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Maksymalny wskaźnik ważności biuletynu**
</td>
<td style="border:1px solid black;">
[**Krytyczny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Forefront Client Security 1.0
</td>
<td style="border:1px solid black;">
[Microsoft Forefront Client Security 1.0](http://www.microsoft.com/downloads/details.aspx?familyid=1eb1a79f-44ca-499e-90bb-ac51894e9d1e) zainstalowany w systemie Microsoft Windows 2000 z dodatkiem Service Pack 4  
(KB957177)  
(Ważny)
</td>
</tr>
</table>
 

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

-   [Artykuł 894199 bazy wiedzy Microsoft Knowledge Base](http://support.microsoft.com/kb/894199): Opis zmian zawartości Usług aktualizacji oprogramowania i usług Windows Server Update Services na rok 2008. Zawiera wszystkie treści dotyczące systemu Windows.
-   [Nowe, zmienione i opublikowane aktualizacje dla produktów firmy Microsoft innych niż Microsoft Windows](http://technet.microsoft.com/en-us/wsus/bb466214.aspx).

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

-   Greg MacManus z firmy [VeriSign iDefense Labs](http://labs.idefense.com/) za zgłoszenie problemu opisanego w biuletynie MS08-052
-   Bing Liu z zespołu [FortiGuard Global Security Research Team](http://www.fortiguardcenter.com/) firmy Fortinet, za zgłoszenie problemu opisanego w biuletynie MS08-052
-   Peter Winter-Smith z firmy [NGSSoftware](http://www.ngssoftware.com/) i Ivan Fratric współpracujący z firmą [Zero Day Initiative](http://www.zerodayinitiative.com/), za zgłoszenie problemu opisanego w biuletynie MS08-052
-   [Zespołowi Vulnerability Research z firmy Assurent Secure Technologie](http://www.assurent.com/)s za zgłoszenie problemu opisanego w biuletynie MS08-052
-   Anonimowemu analitykowi współpracującemu z firmą [Zero Day Initiative](http://www.zerodayinitiative.com/) za zgłoszenie problemu opisanego w biuletynie MS08-052
-   Nguyen Minh Duc i Le Manh Tung, wraz z [ośrodkiem Bach Khoa Internetwork Security Center (BKIS) Hanoi University of Technology (Wietnam)](http://security.bkis.vn/), za zgłoszenie problemu opisanego w biuletynie MS08-053
-   Brett Moore z firmy [Insomnia Security](http://www.insomniasec.com/), za zgłoszenie problemu opisanego w biuletynie MS08-055

#### Pomoc techniczna

-   Wymienione oprogramowanie zostało przetestowane w celu ustalenia, których wersji dotyczy problem. Dla pozostałych wersji upłynął okres pomocy technicznej. Aby zapoznać się z zasadami cyklu pomocy technicznej dotyczącymi używanej wersji oprogramowania, odwiedź [witrynę zasad cyklu pomocy technicznej firmy Microsoft](http://go.microsoft.com/fwlink/?linkid=21742).
-   Klienci mogą uzyskać pomoc techniczną w [Biurze Obsługi Klienta Microsoft](http://go.microsoft.com/fwlink/?linkid=21131) pod numerem 0 801 802 000 (Opłata według stawek Twojego operatora) lub (0-22) 594 19 99 w godzinach od 9:00 do 17:00, od poniedziałku do piątku. Połączenia z działem pomocy technicznej związane z aktualizacjami zabezpieczeń są bezpłatne.
-   Klienci międzynarodowi mogą uzyskać pomoc w lokalnych przedstawicielstwach firmy Microsoft. Pomoc techniczna związana z aktualizacjami zabezpieczeń jest bezpłatna. Informacje o sposobie kontaktowania się z pomocą techniczną firmy Microsoft są dostępne w [międzynarodowej witrynie sieci Web pomocy i obsługi technicznej](http://go.microsoft.com/fwlink/?linkid=21155).

#### Zrzeczenie odpowiedzialności

Informacje w bazie wiedzy Microsoft Knowledge Base są dostarczane „tak jak są” bez jakiejkolwiek gwarancji. Firma Microsoft odrzuca wszelkie gwarancje, wyraźne i dorozumiane, w tym gwarancje dotyczące wartości handlowej i przydatności do określonego celu. Firma Microsoft Corporation ani jej dostawcy w żadnym wypadku nie ponoszą odpowiedzialności za jakiekolwiek szkody, w tym bezpośrednie, pośrednie, przypadkowe, wynikowe, utratę zysków handlowych lub szkody specjalne, nawet jeżeli firmę Microsoft Corporation lub jej dostawców powiadomiono o możliwości zaistnienia takich szkód. W niektórych stanach wyłączenie lub ograniczenie odpowiedzialności za straty wynikowe lub przypadkowe, a więc i powyższe ograniczenia, nie mają zastosowania.

#### Wersje

-   V1.0 (9 września 2008 r.): Opublikowane podsumowanie biuletynów zabezpieczeń.
-   Wersja 2.0 (9 września 2008 r.): Podsumowanie biuletynów zaktualizowano w celu dodania do biuletynu MS08-052 pakietu Microsoft Office Project 2002 z dodatkiem Service Pack 2, całego oprogramowania Office Viewer dla pakietu Microsoft Office 2003 i całego oprogramowania Office Viewer dla pakietu Microsoft Office System 2007 jako oprogramowania, którego dotyczy problem.
-   Wersja 2.1 (17 września 2008 r.): Zaktualizowano podsumowanie biuletynów w celu zmiany programu Microsoft Office Project 2002 z dodatkiem Service Pack 2 w tabeli „Oprogramowanie, którego dotyczy problem” na program Microsoft Office Project 2002 z dodatkiem Service Pack 1. Zmiana ta dotyczy tylko nazwy. Nie wprowadzono żadnych zmian do plików binarnych ani sposobu wykrywania.
-   Wersja 2.2 (29 października 2008 r.): Zaktualizowano podsumowanie biuletynów w celu usunięcia programów Podgląd programu Microsoft Visio 2003, Podgląd programu Microsoft Visio 2007 i Podgląd programu Microsoft Visio 2007 z dodatkiem Service Pack 1 z listy programów, których dotyczy problem, dla biuletynu MS08-052.
-   V3.0 (9 grudnia 2008 r.): Zaktualizowano podsumowanie biuletynów w celu dodania Pakietu zgodności formatu plików pakietu Microsoft Office dla programów Word, Excel i PowerPoint 2007 oraz Pakietu zgodności formatu plików pakietu Microsoft Office dla programów Word, Excel i PowerPoint 2007 z dodatkiem Service Pack 1, Microsoft Expression Web i Microsoft Expression Web 2 oraz Microsoft Office Groove 2007 i Microsoft Office Groove 2007 z dodatkiem Service Pack 1 do listy programów, których dotyczy problem, dla biuletynu MS08-052.

*Built at 2014-04-18T01:50:00Z-07:00*
