---
TOCTitle: 'MS08-APR'
Title: Microsoft Security Bulletin Summary for kwiecień 2008
ms:assetid: 'ms08-apr'
ms:contentKeyID: 61233084
ms:mtpsurl: 'https://technet.microsoft.com/pl-PL/library/ms08-apr(v=Security.10)'
---
Microsoft Security Bulletin Summary for kwiecień 2008
=====================================================

Opublikowano: 8 kwietnia 2008 | Zaktualizowano: 18 lutego 2009

**Wersja:** 1.3

Niniejsze podsumowanie biuletynów zabezpieczeń zawiera spis biuletynów za kwiecień 2008 r.

Z chwilą opublikowania biuletynów za kwiecień 2008 r. niniejsze podsumowanie biuletynów zastępuje powiadomienie o biuletynach zabezpieczeń wydane 3 kwietnia 2008 r. Aby uzyskać więcej informacji na temat usługi powiadamiania o biuletynach, zobacz [Powiadomienia o biuletynach zabezpieczeń firmy Microsoft (j. ang.)](http://technet.microsoft.com/security/bulletin/advance).

Aby dowiedzieć się, jak otrzymywać automatyczne powiadomienia o publikacji biuletynów zabezpieczeń firmy Microsoft, odwiedź stronę [Microsoft Technical Security Notifications](http://go.microsoft.com/fwlink/?linkid=21163).

9 kwietnia 2008 r. o godz. 11:00 czasu Pacyfiku (godz. 20:00 czasu środkowoeuropejskiego) firma Microsoft udostępni emisję internetową, w której znajdą się odpowiedzi na pytania klientów dotyczące tych biuletynów (USA i Kanada). [Zarejestruj się, aby zobaczyć emisję internetową dotyczącą biuletynów zabezpieczeń za kwiecień](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032357219&eventcategory=4&culture=en-us&countrycode=us). Po tym dniu emisja internetowa będzie dostępna na żądanie. Aby uzyskać więcej informacji, zobacz [Podsumowania biuletynów zabezpieczeń i emisje internetowe firmy Microsoft](http://technet.microsoft.com/security/bulletin/summary).

Firma Microsoft udostępnia także informacje, dzięki którym klienci mogą ustalić priorytety dla aktualizacji zabezpieczeń w związku z niezwiązanymi z zabezpieczeniami aktualizacjami o wysokim priorytecie, które publikowane są w tym samym dniu, co comiesięczne aktualizacje zabezpieczeń. Zapoznaj się z sekcją **Inne informacje**.

### Informacje o biuletynie

#### Streszczenia

W bieżącym miesiącu opublikowano następujące biuletyny (w kolejności wskaźnika ważności):

Krytyczny (5)
-------------

<span></span>

| Identyfikator biuletynu               | Biuletyn zabezpieczeń firmy Microsoft MS08-018                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
|---------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**                   | [**Luka w zabezpieczeniach programu Microsoft Project może pozwolić na zdalne wykonanie kodu (950183)**](http://go.microsoft.com/fwlink/?linkid=115454)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **Streszczenie**                      | Ta aktualizacja zabezpieczeń pozwala usunąć lukę w zabezpieczeniach programu Microsoft Project zgłoszoną przez osobę prywatną, która może pozwolić na zdalne wykonanie kodu, jeśli użytkownik otworzy specjalnie spreparowany plik programu Project. Osoba atakująca, której uda się wykorzystać tę lukę, może uzyskać pełną kontrolę nad systemem, którego dotyczy luka. Osoba taka może wówczas instalować programy, przeglądać, zmieniać i usuwać dane oraz tworzyć nowe konta z pełnymi uprawnieniami. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi. |
| **Maksymalny wskaźnik ważności:**     | [Krytyczny](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Wpływ luki**                        | Zdalne wykonanie kodu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Wykrywanie**                        | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Ta aktualizacja nie wymaga ponownego uruchomienia komputera.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| **Programy, których dotyczy problem** | **Microsoft Office.** Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |

| Identyfikator biuletynu               | Biuletyn zabezpieczeń firmy Microsoft MS08-021                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
|---------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**                   | [**Luki w zabezpieczeniach interfejsu GDI umożliwiają zdalne wykonanie kodu (948590)**](http://go.microsoft.com/fwlink/?linkid=111955)                                                                                                                                                                                                                                                                                                                                                                                   |
| **Streszczenie**                      | Ta aktualizacja zabezpieczeń usuwa dwie luki w zabezpieczeniach interfejsu GDI, które zostały zgłoszone przez użytkowników. Wykorzystanie każdej z tych luk może pozwolić na zdalne wykonanie kodu, jeśli użytkownik otworzy specjalnie spreparowany plik obrazu EMF lub WMF. Osoba atakująca, której uda się wykorzystać te luki, może uzyskać pełną kontrolę nad atakowanym systemem. Osoba taka może wówczas instalować programy, przeglądać, zmieniać i usuwać dane oraz tworzyć nowe konta z pełnymi uprawnieniami. |
| **Maksymalny wskaźnik ważności:**     | [Krytyczny](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Wpływ luki**                        | Zdalne wykonanie kodu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Wykrywanie**                        | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Aktualizacja wymaga ponownego uruchomienia systemu.                                                                                                                                                                                                                                                                                                                                                     |
| **Programy, których dotyczy problem** | **Microsoft Windows.** Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                                                                                                                   |

| Identyfikator biuletynu               | Biuletyn zabezpieczeń firmy Microsoft MS08-022                                                                                                                                                                                                                                                                                                                                                                                      |
|---------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**                   | [**Luka w zabezpieczeniach aparatu skryptów VBScript i JScript umożliwia zdalne wykonanie kodu**](http://go.microsoft.com/fwlink/?linkid=108169)                                                                                                                                                                                                                                                                                    |
| **Streszczenie**                      | Niniejsza aktualizacja zabezpieczeń usuwa lukę w zabezpieczeniach aparatu obsługi skryptów VBScript i JScript w systemie Windows, która została zgłoszona przez użytkowników. Osoba atakująca, której uda się wykorzystać tę lukę, może uzyskać pełną kontrolę nad systemem, którego dotyczy luka. Osoba taka może wówczas instalować programy, przeglądać, zmieniać i usuwać dane oraz tworzyć nowe konta z pełnymi uprawnieniami. |
| **Maksymalny wskaźnik ważności:**     | [Krytyczny](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                           |
| **Wpływ luki**                        | Zdalne wykonanie kodu                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Wykrywanie**                        | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Aktualizacja wymaga ponownego uruchomienia systemu.                                                                                                                                                                                                                                                                |
| **Programy, których dotyczy problem** | **Microsoft Windows.** Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                              |

| Identyfikator biuletynu               | Biuletyn zabezpieczeń firmy Microsoft MS08-023                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
|---------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**                   | [**Aktualizacja zabezpieczeń bitów „zabicia” dla formantów ActiveX (948881)**](http://go.microsoft.com/fwlink/?linkid=112366)                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Streszczenie**                      | Ta aktualizacja zabezpieczeń usuwa jedną lukę w zabezpieczeniach produktu firmy Microsoft zgłoszoną przez użytkowników. Aktualizacja ta obejmuje również bit „zabicia” dla produktu Yahoo! Music Jukebox. Luka ta może pozwolić na zdalne wykonanie kodu, jeśli użytkownik wyświetli specjalnie spreparowaną stronę sieci Web przy użyciu programu Internet Explorer. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi. |
| **Maksymalny wskaźnik ważności:**     | [Krytyczny](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| **Wpływ luki**                        | Zdalne wykonanie kodu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Wykrywanie**                        | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Aktualizacja może wymagać ponownego uruchomienia komputera.                                                                                                                                                                                                                                                                                                                                                                                        |
| **Programy, których dotyczy problem** | **Microsoft Windows, Internet Explorer.** Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                                                                                                                                           |

| Identyfikator biuletynu               | Biuletyn zabezpieczeń firmy Microsoft MS08-024                                                                                                                                                                                                                                                                                                                                                                                                           |
|---------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**                   | [**Zbiorcza aktualizacja zabezpieczeń dla programu Internet Explorer (947864)**](http://go.microsoft.com/fwlink/?linkid=110557)                                                                                                                                                                                                                                                                                                                          |
| **Streszczenie**                      | Ta aktualizacja zabezpieczeń usuwa jedną lukę w zabezpieczeniach zgłoszoną przez użytkowników. Luka ta może pozwolić na zdalne wykonanie kodu, jeśli użytkownik wyświetli specjalnie spreparowaną stronę sieci Web przy użyciu programu Internet Explorer. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi. |
| **Maksymalny wskaźnik ważności:**     | [Krytyczny](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                |
| **Wpływ luki**                        | Zdalne wykonanie kodu                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Wykrywanie**                        | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Aktualizacja wymaga ponownego uruchomienia systemu.                                                                                                                                                                                                                                                                                     |
| **Programy, których dotyczy problem** | **Microsoft Windows, Internet Explorer.** Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                                |

Ważny <sup>[3]</sup>
-----------

<span></span>

| Identyfikator biuletynu               | Biuletyn zabezpieczeń firmy Microsoft MS08-020                                                                                                                                                                                                                                                                                   |
|---------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**                   | [**Luka w zabezpieczeniach klienta DNS może pozwolić na fałszowanie (945553)**](http://go.microsoft.com/fwlink/?linkid=108231)                                                                                                                                                                                                   |
| **Streszczenie**                      | Ta aktualizacja zabezpieczeń usuwa lukę w zabezpieczeniach zgłoszoną przez użytkowników. Luka ta występuje w klientach DNS systemu Windows i może pozwolić osobie atakującej na wysyłanie specjalnie spreparowanych odpowiedzi na żądania DNS i fałszowanie lub przekierowywanie ruchu internetowego z uprawnionych lokalizacji. |
| **Maksymalny wskaźnik ważności:**     | [Ważny](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                            |
| **Wpływ luki**                        | Fałszowanie                                                                                                                                                                                                                                                                                                                      |
| **Wykrywanie**                        | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Aktualizacja wymaga ponownego uruchomienia systemu.                                                                                                                                                             |
| **Programy, których dotyczy problem** | **Microsoft Windows.** Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                           |

| Identyfikator biuletynu               | Biuletyn zabezpieczeń firmy Microsoft MS08-025                                                                                                                                                                                                                                                                                                                        |
|---------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**                   | [**Luka w zabezpieczeniach jądra systemu Windows może pozwolić na podniesienie poziomu uprawnień (941693)**](http://go.microsoft.com/fwlink/?linkid=111956)                                                                                                                                                                                                           |
| **Streszczenie**                      | Niniejsza aktualizacja zabezpieczeń pozwala usunąć zgłoszoną przez użytkowników lukę w zabezpieczeniach jądra systemu Windows. Osoba atakująca, której uda się lokalnie wykorzystać tę lukę, może uzyskać pełną kontrolę nad systemem, którego dotyczy luka. Osoba taka może wówczas instalować programy, przeglądać, zmieniać i usuwać dane oraz tworzyć nowe konta. |
| **Maksymalny wskaźnik ważności:**     | [Ważny](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                 |
| **Wpływ luki**                        | Podniesienie uprawnień                                                                                                                                                                                                                                                                                                                                                |
| **Wykrywanie**                        | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Aktualizacja wymaga ponownego uruchomienia systemu.                                                                                                                                                                                                  |
| **Programy, których dotyczy problem** | **Microsoft Windows.** Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                |

| Identyfikator biuletynu               | Biuletyn zabezpieczeń firmy Microsoft MS08-019                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
|---------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**                   | [**Luki w zabezpieczeniach programu Microsoft Visio umożliwiają zdalne wykonanie kodu (949032)**](http://go.microsoft.com/fwlink/?linkid=115455)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Streszczenie**                      | Ta aktualizacja pozwala usunąć luki w zabezpieczeniach programu Microsoft Office Visio zgłoszone przez osoby prywatne, które mogą pozwolić na zdalne wykonanie kodu, jeśli użytkownik otworzy specjalnie spreparowany plik programu Visio. Osoba atakująca, której uda się wykorzystać tę lukę, może uzyskać pełną kontrolę nad systemem, którego dotyczy luka. Osoba taka może wówczas instalować programy, przeglądać, zmieniać i usuwać dane oraz tworzyć nowe konta z pełnymi uprawnieniami. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi. |
| **Maksymalny wskaźnik ważności:**     | [Ważny](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **Wpływ luki**                        | Zdalne wykonanie kodu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **Wykrywanie**                        | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Ta aktualizacja nie wymaga ponownego uruchomienia komputera.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **Programy, których dotyczy problem** | **Microsoft Office.** Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |

Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki
---------------------------------------------------------------------------------

<span></span>
**W jaki sposób korzystać z tej tabeli?**

Tabela ta pozwala odczytać informacje o aktualizacjach zabezpieczeń, których zainstalowanie może być konieczne. Należy przejrzeć informacje dla każdego wymienionego programu lub składnika oprogramowania w celu sprawdzenia, czy są wymagane aktualizacje zabezpieczeń. Jeśli program lub składnik znajduje się na liście, dostępne jest łącze prowadzące do aktualizacji oprogramowania i podana jest informacja o wskaźniku ważności tej aktualizacji.

**Uwaga** Konieczne może być zainstalowanie kilku aktualizacji zabezpieczeń dotyczących jednej luki. Przejrzyj całą kolumnę dla każdego wymienionego identyfikatora biuletynu, aby sprawdzić, jakie aktualizacje musisz zainstalować, w oparciu o programy bądź składniki zainstalowane w systemie.

#### System operacyjny Windows i jego składniki:

 
<table style="border:1px solid black;">
<caption>Microsoft Windows 2000</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Identyfikator biuletynu</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111955"><strong>MS08-021</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=108169"><strong>MS08-022</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=112366"><strong>MS08-023</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=110557"><strong>MS08-024</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=108231"><strong>MS08-020</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111956"><strong>MS08-025</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Maksymalny wskaźnik ważności:</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Krytyczny</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Krytyczny</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Krytyczny</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Krytyczny</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Ważny</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Ważny</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Windows 2000 z dodatkiem Service Pack 4</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=caac000a-22b6-48cb-aa00-1a0bfe886de2">Microsoft Windows 2000 z dodatkiem Service Pack 4</a><br />
(Krytyczny)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=8e3ff44f-145b-4a68-9ad4-4a55d74b216e">VBScript 5.1 i JScript 5.1</a><br />
(Krytyczny)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=8e3ff44f-145b-4a68-9ad4-4a55d74b216e">VBScript 5.6 i JScript 5.6</a><br />
(Krytyczny)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=0395451f-b719-4f71-a7b4-403d0c7e8fcc">Microsoft Internet Explorer 5.01 z dodatkiem Service Pack 4</a><br />
(Krytyczny)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=ba6d3aeb-e35a-47cc-bace-7bd9d58a9d3f">Microsoft Internet Explorer 6 z dodatkiem Service Pack 1</a><br />
(Krytyczny)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=b051ae04-fe81-440d-9136-d6b239ca954e">Microsoft Internet Explorer 5.01 z dodatkiem Service Pack 4</a><br />
(Krytyczny)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=75d2dc78-e3a4-4ff6-9e2d-bf1935003e8e">Microsoft Internet Explorer 6 z dodatkiem Service Pack 1</a><br />
(Krytyczny)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=41326ade-96b6-47ce-9291-d4e3039471c4">Microsoft Windows 2000 z dodatkiem Service Pack 4</a><br />
(Ważny)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=8db9f328-da0e-4fb8-96c4-6d368b47c224">Microsoft Windows 2000 z dodatkiem Service Pack 4</a><br />
(Ważny)</td>
</tr>
</tbody>
</table>
 

 
<table style="border:1px solid black;">
<caption>Windows XP</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Identyfikator biuletynu</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111955"><strong>MS08-021</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=108169"><strong>MS08-022</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=112366"><strong>MS08-023</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=110557"><strong>MS08-024</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=108231"><strong>MS08-020</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111956"><strong>MS08-025</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Maksymalny wskaźnik ważności:</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Krytyczny</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Krytyczny</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Krytyczny</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Krytyczny</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Ważny</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Ważny</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows XP z dodatkiem Service Pack 2</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=c2763dd8-a03e-4a48-aa86-a7ec00250a7a">Windows XP z dodatkiem Service Pack 2</a><br />
(Krytyczny)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=c0124698-3b94-4474-9473-22a2f39a4a56">VBScript 5.6 i JScript 5.6</a><br />
(Krytyczny)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=9dbf002f-fe53-4cc7-a430-35f45c520d10">Windows XP z dodatkiem Service Pack 2</a><br />
(Krytyczny)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=36c641ad-953f-4b09-ba1c-9c383295e180">Microsoft Internet Explorer 6</a><br />
(Krytyczny)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=e771efe8-8881-4f23-b5b0-15651a390ba9">Windows Internet Explorer 7</a><br />
(Krytyczny)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=893f4cef-0395-4c44-ba28-7a10b6e7dd48">Windows XP z dodatkiem Service Pack 2</a><br />
(Ważny)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=0e937f65-abd0-46dd-8883-5bfd70ea1178">Windows XP z dodatkiem Service Pack 2</a><br />
(Ważny)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows XP Professional x64 Edition oraz Microsoft Windows XP Professional x64 Edition z dodatkiem Service Pack 2</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=166f2ab5-913c-47a9-86fe-b814797b751e">Windows XP Professional x64 Edition oraz Windows XP Professional x64 Edition z dodatkiem Service Pack 2</a><br />
(Krytyczny)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=87b80ae3-e299-4d15-a135-3b1bcf943652">VBScript 5.6 i JScript 5.6</a><br />
(Krytyczny)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=01400970-df68-4daf-aa39-2fc4f969974c">Windows XP Professional x64 Edition oraz Windows XP Professional x64 Edition z dodatkiem Service Pack 2</a><br />
(Krytyczny)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=85beacc0-8ca2-4ded-9c24-23348d05c735">Microsoft Internet Explorer 6</a><br />
(Krytyczny)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=9364bf81-6505-4788-958d-a4bd29dc98ad">Windows Internet Explorer 7</a><br />
(Krytyczny)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=8fdd1207-6e93-4c43-bacc-fe3623a6ebe7">Windows XP Professional x64 Edition oraz Windows XP Professional x64 Edition z dodatkiem Service Pack 2</a><br />
(Ważny)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=a29bbd13-761f-44fa-8948-e1a8c244bd7a">Windows XP Professional x64 Edition oraz Windows XP Professional x64 Edition z dodatkiem Service Pack 2</a><br />
(Ważny)</td>
</tr>
</tbody>
</table>
 

 
<table style="border:1px solid black;">
<caption>Windows Server 2003</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Identyfikator biuletynu</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111955"><strong>MS08-021</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=108169"><strong>MS08-022</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=112366"><strong>MS08-023</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=110557"><strong>MS08-024</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=108231"><strong>MS08-020</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111956"><strong>MS08-025</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Maksymalny wskaźnik ważności:</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Krytyczny</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Krytyczny</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Krytyczny</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Krytyczny</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Ważny</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Ważny</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Server 2003 z dodatkiem Service Pack 1 i Windows Server 2003 z dodatkiem Service Pack 2</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=bee91d80-d49a-4d3d-82d6-d5aa63f54979">Windows Server 2003 z dodatkiem Service Pack 1 i Windows Server 2003 z dodatkiem Service Pack 2</a><br />
(Krytyczny)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=88518aa6-e334-4529-aa63-0bf2ef417ce3">VBScript 5.6 i JScript 5.6</a><br />
(Krytyczny)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=ad384fea-53be-4be3-8acb-1cd23a7f5405">Windows Server 2003 z dodatkiem Service Pack 1 i Windows Server 2003 z dodatkiem Service Pack 2</a><br />
(Umiarkowany)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=0444b76e-93fa-43c2-b1bc-a5c054529eb5">Microsoft Internet Explorer 6</a><br />
(Krytyczny)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=9acd2a03-5530-49c8-9ea1-0bfaf259700d">Windows Internet Explorer 7</a><br />
(Krytyczny)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=214bd8f5-6eb2-414c-b013-c516a306d692">Windows Server 2003 z dodatkiem Service Pack 1 i Windows Server 2003 z dodatkiem Service Pack 2</a><br />
(Ważny)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=d3b855a6-4648-4771-826d-11a151828eac">Windows Server 2003 z dodatkiem Service Pack 1 i Windows Server 2003 z dodatkiem Service Pack 2</a><br />
(Ważny)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows Server 2003 x64 Edition i Windows Server 2003 x64 Edition z dodatkiem Service Pack 2</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=e3dde449-e062-4ce0-a9f4-433bff23e224">Windows Server 2003 x64 Edition i Windows Server 2003 x64 Edition z dodatkiem Service Pack 2</a><br />
(Krytyczny)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=12cefefc-8553-4dca-9850-c653371de61e">VBScript 5.6 i JScript 5.6</a><br />
(Krytyczny)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=ffc5c893-cb24-4875-b0a7-6d5c7aa4d642">Windows Server 2003 x64 Edition i Windows Server 2003 x64 Edition z dodatkiem Service Pack 2</a><br />
(Umiarkowany)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=5ebb5ef9-615f-4cab-bac5-6f45f1b94952">Microsoft Internet Explorer 6</a><br />
(Krytyczny)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=a9e406aa-33e2-49b8-ab54-4a7328e46147">Windows Internet Explorer 7</a><br />
(Krytyczny)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=fd123394-a5d6-4b55-be74-2938f52ce922">Windows Server 2003 x64 Edition i Windows Server 2003 x64 Edition z dodatkiem Service Pack 2</a><br />
(Ważny)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=320fd100-35e1-4345-9399-796393235cbc">Windows Server 2003 x64 Edition i Windows Server 2003 x64 Edition z dodatkiem Service Pack 2</a><br />
(Ważny)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Systemy operacyjne Windows Server 2003 z dodatkiem SP1 dla systemów z procesorem Itanium oraz Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=7886a802-f2b5-489c-b14b-631f4c4c0742">Windows Server 2003 z dodatkiem SP1 dla systemów z procesorem Itanium oraz Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium</a><br />
(Krytyczny)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=fe22a828-cca4-4b51-bbd5-995c65fead21">VBScript 5.6 i JScript 5.6</a><br />
(Krytyczny)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=94cf78d3-b6c3-41bc-993e-3af3be0d70f1">Windows Server 2003 z dodatkiem SP1 dla systemów z procesorem Itanium oraz Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium</a><br />
(Umiarkowany)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=63da8040-fda2-42c7-8543-26ad6f9811f2">Microsoft Internet Explorer 6</a><br />
(Krytyczny)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=75a05d3a-92a0-4a00-95d4-e2b2f6755180">Windows Internet Explorer 7</a><br />
(Krytyczny)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=e0e63f03-904d-47ee-94fc-51a8dea668eb">Windows Server 2003 z dodatkiem SP1 dla systemów z procesorem Itanium oraz Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium</a><br />
(Ważny)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=126426a7-be38-4327-89db-02d99d76589d">Windows Server 2003 z dodatkiem SP1 dla systemów z procesorem Itanium oraz Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium</a><br />
(Ważny)</td>
</tr>
</tbody>
</table>
 

 
<table style="border:1px solid black;">
<caption>Windows Vista</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Identyfikator biuletynu</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111955"><strong>MS08-021</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=108169"><strong>MS08-022</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=112366"><strong>MS08-023</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=110557"><strong>MS08-024</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=108231"><strong>MS08-020</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111956"><strong>MS08-025</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Maksymalny wskaźnik ważności:</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Krytyczny</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Krytyczny</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Krytyczny</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Krytyczny</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Ważny</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Ważny</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Vista i Windows Vista z dodatkiem Service Pack 1</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=9b51deb8-3873-4146-977f-7e3d0840a4c5">Windows Vista i Windows Vista z dodatkiem Service Pack 1</a><br />
(Krytyczny)</td>
<td style="border:1px solid black;">Brak</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=d7f14001-7f42-4ca0-9193-cdf061179b59">Windows Vista i Windows Vista z dodatkiem Service Pack 1</a><br />
(Ważny)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=d4e24966-6530-463a-9ee2-f6a9d000f998">Windows Internet Explorer 7</a><br />
(Krytyczny)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=8203d303-c855-4579-9bbf-b06ddf5c1b87">Windows Vista</a><br />
(Ważny)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=9640cd8b-d749-4ddd-8af9-b298cebed969">Windows Vista i Windows Vista z dodatkiem Service Pack 1</a><br />
(Ważny)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows Vista x64 Edition i Windows Vista x64 Edition z dodatkiem Service Pack 1</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=4ad6dcd1-6ea5-43bf-8bee-a5f507beadc6">Windows Vista x64 Edition i Windows Vista x64 Edition z dodatkiem Service Pack 1</a><br />
(Krytyczny)</td>
<td style="border:1px solid black;">Brak</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=d33462b6-7391-482d-babe-fb4cd0beaa21">Windows Vista x64 Edition i Windows Vista x64 Edition z dodatkiem Service Pack 1</a><br />
(Ważny)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=295cf8f2-265e-4570-b708-21033337fe05">Windows Internet Explorer 7</a><br />
(Krytyczny)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=73f3a234-3973-4467-be7e-69efa7ee978c">Windows Vista x64 Edition</a><br />
(Ważny)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=d56bb4fe-304e-45e0-95f2-fde2f47b2a04">Windows Vista x64 Edition i Windows Vista x64 Edition z dodatkiem Service Pack 1</a><br />
(Ważny)</td>
</tr>
</tbody>
</table>
 

 
<table style="border:1px solid black;">
<caption>Windows Server 2008</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Identyfikator biuletynu</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111955"><strong>MS08-021</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=108169"><strong>MS08-022</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=112366"><strong>MS08-023</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=110557"><strong>MS08-024</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=108231"><strong>MS08-020</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111956"><strong>MS08-025</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Maksymalny wskaźnik ważności:</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Krytyczny</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Krytyczny</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Krytyczny</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Krytyczny</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Ważny</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Ważny</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Server 2008 dla systemów 32-bitowych</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=006d5c47-53e6-4ee1-932c-497611804938">Windows Server 2008 dla systemów 32-bitowych</a><br />
(Krytyczny)</td>
<td style="border:1px solid black;">Brak</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=95691924-2813-4a86-9e11-99d853f8e606">Windows Server 2008 dla systemów 32-bitowych</a><br />
(Niski)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=e57b4d94-19ad-4818-8311-a3f94be01a4b">Windows Internet Explorer 7</a>*<br />
(Krytyczny)</td>
<td style="border:1px solid black;">Brak</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=4497333c-9418-4b91-83dc-0155735421c0">Windows Server 2008 dla systemów 32-bitowych</a><br />
(Ważny)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows Server 2008 dla systemów opartych na procesorach X64</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=8909f144-655b-4f07-916f-fd967f1efb2b">Windows Server 2008 dla systemów opartych na procesorach X64</a><br />
(Krytyczny)</td>
<td style="border:1px solid black;">Brak</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=920ae29b-19d0-4089-ac79-f2da824a2256">Windows Server 2008 dla systemów opartych na procesorach X64</a><br />
(Niski)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=93e9f52a-c7d0-4033-9c12-740665a219af">Windows Internet Explorer 7</a>*<br />
(Krytyczny)</td>
<td style="border:1px solid black;">Brak</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=5aefc7a6-79a4-45a2-b534-35d0ec400dda">Windows Server 2008 dla systemów opartych na procesorach X64</a><br />
(Ważny)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Server 2008 dla systemów z procesorem Itanium</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=b7771a4a-4e4f-48d1-8551-bb8b778ca5a7">Windows Server 2008 dla systemów z procesorem Itanium</a><br />
(Krytyczny)</td>
<td style="border:1px solid black;">Brak</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=66df79ac-8364-4922-9688-ebc7ec76d89f">Windows Server 2008 dla systemów z procesorem Itanium</a><br />
(Niski)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=acf948e8-c4a9-40da-b282-f5e584e77b05">Windows Internet Explorer 7</a><br />
(Krytyczny)</td>
<td style="border:1px solid black;">Brak</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=3080c26b-7456-41ef-8668-28f15bc7b8ce">Windows Server 2008 dla systemów z procesorem Itanium</a><br />
(Ważny)</td>
</tr>
</tbody>
</table>
 

**\*Luka w zabezpieczeniach nie dotyczy instalacji Server Core systemu operacyjnego Windows Server 2008.** Lukom usuwanym przez te aktualizacje zabezpieczeń nie podlegają obsługiwane wersje systemu Windows Server 2008, jeśli został on zainstalowany przy użyciu opcji instalacji Server Core, mimo że na komputerze mogą znajdować się pliki, których dotyczą omawiane luki. Aktualizacja ta będzie jednak w dalszym ciągu oferowana użytkownikom posiadającym pliki podlegające luce, ponieważ zaktualizowane pliki są nowsze (mają wyższe numery wersji) niż pliki znajdujące się obecnie w systemie. Aby uzyskać więcej informacji na temat tej opcji instalacji, zobacz [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Należy pamiętać, że opcja instalacji Server Core nie dotyczy niektórych wersji systemu Windows Server 2008; zobacz [Porównanie opcji instalacji Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

#### Pakiety i oprogramowanie Office

 
<table style="border:1px solid black;">
<caption>Microsoft Project</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Identyfikator biuletynu</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=115454"><strong>MS08-018</strong></a></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Maksymalny wskaźnik ważności:</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Krytyczny</strong></a></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Project 2000 z dodatkiem Service Release 1</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=fbe46241-b9da-40c6-803d-42eb6234be77">Project 2000 z dodatkiem Service Release 1</a><br />
(KB949043)<br />
(Krytyczny)</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft Project 2002 z dodatkiem Service Pack 1</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=07a90718-6597-426d-9dca-a336d60c01b8">Project 2002 z dodatkiem Service Pack 1</a><br />
(KB949005)<br />
(Ważny)</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Project 2003 z dodatkiem Service Pack 2</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=aaba07d6-e972-4e85-bccd-406aa2c4a4f4">Project 2003 z dodatkiem Service Pack 2</a><br />
(KB948962)<br />
(Ważny)</td>
<td style="border:1px solid black;"></td>
</tr>
</tbody>
</table>

 
<table style="border:1px solid black;">
<caption>Microsoft Visio</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Identyfikator biuletynu</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=115455"><strong>MS08-019</strong></a></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Maksymalny wskaźnik ważności:</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Ważny</strong></a></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Visio 2002 z dodatkiem Service Pack 2</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=0056a936-def5-40fa-bcfc-0ab0dd5c3964">Microsoft Visio 2002 z dodatkiem Service Pack 2</a><br />
(KB947896)<br />
(Ważny)</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft Visio 2003 z dodatkiem Service Pack 2</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=18af0ce6-99a0-4471-8d26-9700a8a8e631">Visio 2003 z dodatkiem Service Pack 2</a><br />
(KB947650)<br />
(Ważny)</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Visio 2003 z dodatkiem Service Pack 3</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=18af0ce6-99a0-4471-8d26-9700a8a8e631">Visio 2003 z dodatkiem Service Pack 3</a><br />
(KB947650)<br />
(Ważny)</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft Visio 2007</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=0510a1bb-b464-452c-900f-7f4e58ed9c7e">Visio 2007</a><br />
(KB947590)<br />
(Ważny)</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Visio 2007 z dodatkiem Service Pack 1</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=0510a1bb-b464-452c-900f-7f4e58ed9c7e">Visio 2007 z dodatkiem Service Pack 1</a><br />
(KB947590)<br />
(Ważny)</td>
<td style="border:1px solid black;"></td>
</tr>
</tbody>
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
  
-   Organizacji [National Cyber Security Center](http://www.ncsc.go.kr/eng/) z Republiki Korei za zgłoszenie problemu opisanego w biuletynie MS08-018  
-   Anonimowej osobie za zgłoszenie problemu opisanego w biuletynie MS08-019.  
-   Anonimowej osobie za zgłoszenie innego problemu opisanego w biuletynie MS08-019.  
-   Amitowi Kleinowi z firmy [Trusteer](http://www.trusteer.com/) za zgłoszenie problemu opisanego w biuletynie MS08-020  
-   Alli Berzroutchko z firmy [Scanit](http://www.scanit.be/) za zgłoszenie problemu opisanego w biuletynie MS08-020  
-   Royowi Arendsowi z firmy [Nominet UK](http://www.nominet.org.uk/) za zgłoszenie problemu opisanego w biuletynie MS08-020  
-   Jun Mao z firmy [iDefense Labs](http://labs.idefense.com/) za zgłoszenie problemu opisanego w biuletynie MS08-021  
-   Sebastianowi Apeltowi z firmy [Zero Day Initiative](http://www.zerodayinitiative.com/) za zgłoszenie problemu opisanego w biuletynie MS08-021  
-   Thomasowi Garnierowi z firmy [SkyRecon](http://www.skyrecon.com/) za zgłoszenie problemu opisanego w biuletynie MS08-021  
-   Yamata Li z firmy [Palo Alto Networks](http://www.paloaltonetworks.com/) za zgłoszenie problemu opisanego w biuletynie MS08-021.  
-   Peterowi Ferrie z firmy [Symantec](http://www.symantec.com/) za zgłoszenie problemu opisanego w biuletynie MS08-022  
-   Anonimowemu analitykowi współpracującemu z firmą [iDefense VCP](http://labs.idefense.com/vcp/) za zgłoszenie problemu opisanego w biuletynie MS08-023  
-   Carsten Eiram z firmy [Secunia](http://secunia.com/) za zgłoszenie problemu opisanego w biuletynie MS08-024  
-   Thomasowi Garnierowi z firmy [SkyRecon](http://www.skyrecon.com/) za zgłoszenie problemu opisanego w biuletynie MS08-025
  
#### Pomoc techniczna
  
-   Wymienione oprogramowanie zostało przetestowane w celu ustalenia, których wersji dotyczy problem. Dla pozostałych wersji upłynął okres pomocy technicznej. Aby zapoznać się z zasadami cyklu pomocy technicznej dotyczącymi używanej wersji oprogramowania, odwiedź [witrynę zasad cyklu pomocy technicznej firmy Microsoft](http://go.microsoft.com/fwlink/?linkid=21742).  
-   Klienci mogą uzyskać pomoc techniczną w [Biurze Obsługi Klienta Microsoft](http://go.microsoft.com/fwlink/?linkid=21131) pod numerem 0 801 802 000 (Opłata według stawek Twojego operatora) lub (0-22) 594 19 99 w godzinach od 9:00 do 17:00, od poniedziałku do piątku. Połączenia z działem pomocy technicznej związane z aktualizacjami zabezpieczeń są bezpłatne.  
-   Klienci międzynarodowi mogą uzyskać pomoc w lokalnych przedstawicielstwach firmy Microsoft. Pomoc techniczna związana z aktualizacjami zabezpieczeń jest bezpłatna. Informacje o sposobie kontaktowania się z pomocą techniczną firmy Microsoft są dostępne w [międzynarodowej witrynie sieci Web pomocy i obsługi technicznej](http://go.microsoft.com/fwlink/?linkid=21155).
  
#### Zrzeczenie odpowiedzialności
  
Informacje w bazie wiedzy Microsoft Knowledge Base są dostarczane „tak jak są” bez jakiejkolwiek gwarancji. Firma Microsoft odrzuca wszelkie gwarancje, wyraźne i dorozumiane, w tym gwarancje dotyczące wartości handlowej i przydatności do określonego celu. Firma Microsoft Corporation ani jej dostawcy w żadnym wypadku nie ponoszą odpowiedzialności za jakiekolwiek szkody, w tym bezpośrednie, pośrednie, przypadkowe, wynikowe, utratę zysków handlowych lub szkody specjalne, nawet jeżeli firmę Microsoft Corporation lub jej dostawców powiadomiono o możliwości zaistnienia takich szkód. W niektórych stanach wyłączenie lub ograniczenie odpowiedzialności za straty wynikowe lub przypadkowe, a więc i powyższe ograniczenia, nie mają zastosowania.
  
#### Wersje
  
-   V1.0 (8 kwietnia 2008 r.): Opublikowane podsumowanie biuletynów zabezpieczeń.  
-   V1.1 (9 kwietnia 2008 r.): Zaktualizowano sekcję Streszczenie biuletynu zabezpieczeń firmy Microsoft MS08-018.  
-   V1.2 (16 kwietnia 2008 r.): Zaktualizowano informacje na temat osób, które odkryły luki w zabezpieczeniach opisane w biuletynie MS08-021, a w sekcji Programy, których dotyczy problem wyjaśniono informacje dotyczące pakietów i programów pakietu Microsoft Office.  
-   Wersja 1.3 (18 lutego 2009 r.): W biuletynie MS08-024 dodano zapis o niepodlegającej luce instalacji Server Core systemu Windows Server 2008 dla systemów 32-bitowych oraz Windows Server 2008 dla systemów opartych na procesorach X64.
  
*Built at 2014-04-18T01:50:00Z-07:00*
