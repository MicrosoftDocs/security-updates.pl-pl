---
TOCTitle: 'MS08-MAR'
Title: Microsoft Security Bulletin Summary for marzec 2008
ms:assetid: 'ms08-mar'
ms:contentKeyID: 61233091
ms:mtpsurl: 'https://technet.microsoft.com/pl-PL/library/ms08-mar(v=Security.10)'
---


Microsoft Security Bulletin Summary for marzec 2008
===================================================

Opublikowano: 11 marca 2008 | Zaktualizowano: 16 kwietnia 2008

**Wersja:** 2.0

Niniejsze podsumowanie biuletynów zabezpieczeń zawiera spis biuletynów za marzec 2008 r.

Z chwilą opublikowania biuletynów za marzec 2008 r. niniejsze podsumowanie biuletynów zastępuje powiadomienie o biuletynach zabezpieczeń wydane 6 marca 2008 r. Aby uzyskać więcej informacji na temat usługi powiadamiania o biuletynach, zobacz [Powiadomienia o biuletynach zabezpieczeń firmy Microsoft (jęz. ang.)](http://technet.microsoft.com/security/bulletin/advance).

Aby dowiedzieć się, jak otrzymywać automatyczne powiadomienia o publikacji biuletynów zabezpieczeń firmy Microsoft, odwiedź stronę [Microsoft Technical Security Notifications](http://go.microsoft.com/fwlink/?linkid=21163).

12 marca 2008 r. o godz. 11:00 czasu Pacyfiku (godz. 20:00 czasu środkowoeuropejskiego) firma Microsoft udostępni emisję internetową, w której znajdą się odpowiedzi na pytania klientów dotyczące tych biuletynów (USA i Kanada). Zarejestruj się, aby zobaczyć [emisję internetową dotyczącą biuletynów zabezpieczeń za marzec](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032357217&eventcategory=4&culture=en-us&countrycode=us). Po tym dniu emisja internetowa będzie dostępna na żądanie. Aby uzyskać więcej informacji, zobacz [Podsumowania biuletynów zabezpieczeń i emisje internetowe firmy Microsoft](http://technet.microsoft.com/security/bulletin/summary).

Firma Microsoft udostępnia także informacje, dzięki którym klienci mogą ustalić priorytety dla aktualizacji zabezpieczeń w związku z niezwiązanymi z zabezpieczeniami aktualizacjami o wysokim priorytecie, które publikowane są w tym samym dniu, co comiesięczne aktualizacje zabezpieczeń. Zapoznaj się z sekcją **Inne informacje**.

### Informacje o biuletynie

#### Streszczenia

W bieżącym miesiącu opublikowano następujące biuletyny (w kolejności wskaźnika ważności):

Krytyczny (4)
-------------

<span></span>
| Identyfikator biuletynu               | Biuletyn zabezpieczeń firmy Microsoft MS08-014                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
|---------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**                   | [**Luki w zabezpieczeniach programu Microsoft Excel umożliwiają zdalne wykonanie kodu (949029)**](http://go.microsoft.com/fwlink/?linkid=112111)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| **Streszczenie**                      | Ta aktualizacja pozwala usunąć kilka zgłoszonych przez osoby prywatne luk w zabezpieczeniach programu Microsoft Office Excel, które mogą pozwolić na zdalne wykonanie kodu, jeśli użytkownik otworzy specjalnie spreparowany plik programu Excel. Osoba atakująca, której uda się wykorzystać te luki, może uzyskać pełną kontrolę nad atakowanym systemem. Osoba taka może wówczas instalować programy, przeglądać, zmieniać i usuwać dane oraz tworzyć nowe konta z pełnymi uprawnieniami. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi. |
| **Maksymalny wskaźnik ważności**      | [Krytyczny](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **Wpływ luki**                        | Zdalne wykonanie kodu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| **Wykrywanie**                        | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Aktualizacja nie będzie wymagać ponownego uruchomienia komputera.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Programy, których dotyczy problem** | **Microsoft Office.** Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |

| Identyfikator biuletynu               | Biuletyn zabezpieczeń firmy Microsoft MS08-015                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
|---------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**                   | [**Luka w zabezpieczeniach programu Microsoft Outlook może pozwolić na zdalne wykonanie kodu (949031)**](http://go.microsoft.com/fwlink/?linkid=112113)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| **Streszczenie**                      | Ta krytyczna aktualizacja zabezpieczeń usuwa lukę w zabezpieczeniach programu Microsoft Office Outlook, która została zgłoszona przez użytkowników. Luka ta umożliwia zdalne wykonanie kodu, jeśli do programu Outlook zostanie przekazany specjalnie spreparowany identyfikator URI mailto. Osoba taka może wówczas instalować programy, przeglądać, zmieniać i usuwać dane oraz tworzyć nowe konta z pełnymi uprawnieniami. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi. Aby wykorzystać tę lukę nie wystarczy wyświetlić wiadomości e-mail w okienku podglądu programu Outlook. |
| **Maksymalny wskaźnik ważności**      | [Krytyczny](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| **Wpływ luki**                        | Zdalne wykonanie kodu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Wykrywanie**                        | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Aktualizacja nie będzie wymagać ponownego uruchomienia komputera.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **Programy, których dotyczy problem** | **Microsoft Office.** Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |

| Identyfikator biuletynu               | Biuletyn zabezpieczeń firmy Microsoft MS08-016                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
|---------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**                   | [**Luki w zabezpieczeniach pakietu Microsoft Office umożliwiają zdalne wykonanie kodu (949030)**](http://go.microsoft.com/fwlink/?linkid=112112)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Streszczenie**                      | Ta krytyczna aktualizacja pozwala usunąć dwie zgłoszone przez osoby prywatne luki w zabezpieczeniach pakietu Microsoft Office, które mogą pozwolić na zdalne wykonanie kodu, jeśli użytkownik otworzy nieprawidłowo utworzony plik pakietu Office. Osoba atakująca, której uda się wykorzystać tę lukę, może uzyskać pełną kontrolę nad systemem, którego dotyczy luka. Osoba taka może wówczas instalować programy, przeglądać, zmieniać i usuwać dane oraz tworzyć nowe konta z pełnymi uprawnieniami. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi. |
| **Maksymalny wskaźnik ważności**      | [Krytyczny](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Wpływ luki**                        | Zdalne wykonanie kodu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **Wykrywanie**                        | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Aktualizacja nie będzie wymagać ponownego uruchomienia komputera.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| **Programy, których dotyczy problem** | **Microsoft Office.** Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |

| Identyfikator biuletynu               | Biuletyn zabezpieczeń firmy Microsoft MS08-017                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
|---------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**                   | [**Luki w zabezpieczeniach składników Microsoft Office Web Components umożliwiają zdalne wykonanie kodu (933103)**](http://go.microsoft.com/fwlink/?linkid=112114)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **Streszczenie**                      | Ta aktualizacja zabezpieczeń o krytycznym wskaźniku ważności usuwa dwie luki w zabezpieczeniach składników Microsoft Office Web Components. Te luki w zabezpieczeniach umożliwiają zdalne wykonanie kodu, jeśli użytkownik wyświetli specjalnie spreparowaną witrynę sieci Web. Osoba atakująca, której uda się wykorzystać tę lukę, może uzyskać pełną kontrolę nad systemem, którego dotyczy luka. Osoba taka może wówczas instalować programy, przeglądać, zmieniać i usuwać dane oraz tworzyć nowe konta z pełnymi uprawnieniami. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi. |
| **Maksymalny wskaźnik ważności**      | [Krytyczny](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| **Wpływ luki**                        | Zdalne wykonanie kodu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Wykrywanie**                        | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Aktualizacja może wymagać ponownego uruchomienia komputera.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Programy, których dotyczy problem** | **Składniki Microsoft Office Web Components.** Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |

Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki
---------------------------------------------------------------------------------

<span></span>
**W jaki sposób korzystać z tej tabeli?**

Tabela ta pozwala odczytać informacje o aktualizacjach zabezpieczeń, których zainstalowanie może być konieczne. Należy przejrzeć informacje dla każdego wymienionego programu lub składnika oprogramowania w celu sprawdzenia, czy są wymagane aktualizacje zabezpieczeń. Dla każdego programu lub składnika oprogramowania wymienionego na liście podany jest wpływ luki oraz hiperłącze do dostępnej aktualizacji oprogramowania.

**Uwaga** Konieczne może być zainstalowanie kilku aktualizacji zabezpieczeń dotyczących jednej luki. Przejrzyj całą kolumnę dla każdego wymienionego identyfikatora biuletynu, aby sprawdzić, jakie aktualizacje musisz zainstalować, w oparciu o programy bądź składniki zainstalowane w systemie.

**Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki**

 
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
Szczegóły
</th>
<th style="border:1px solid black;" >
Szczegóły
</th>
<th style="border:1px solid black;" >
Szczegóły
</th>
<th style="border:1px solid black;" >
Szczegóły
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS08-014**](http://go.microsoft.com/fwlink/?linkid=112111)
</td>
<td style="border:1px solid black;">
[**MS08-015**](http://go.microsoft.com/fwlink/?linkid=112113)
</td>
<td style="border:1px solid black;">
[**MS08-016**](http://go.microsoft.com/fwlink/?linkid=112112)
</td>
<td style="border:1px solid black;">
[**MS08-017**](http://go.microsoft.com/fwlink/?linkid=112114)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Maksymalny wskaźnik ważności**
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
</tr>
<tr>
<th colspan="5">
Pakiety i oprogramowanie Office
</th>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2000 z dodatkiem Service Pack 3
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny](http://www.microsoft.com/downloads/details.aspx?familyid=72735aa1-e22c-40ed-8c79-38fba89979aa)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office XP z dodatkiem Service Pack 3
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Ważny](http://www.microsoft.com/downloads/details.aspx?familyid=9cf8aafa-71a5-4017-b53c-4e80ef6e1188)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2003 z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Ważny](http://www.microsoft.com/downloads/details.aspx?familyid=9f25922c-d3c2-4ef1-b164-8a21a77d29aa)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Excel 2000 z dodatkiem Service Pack 3
</td>
<td style="border:1px solid black;">
[Krytyczny](http://www.microsoft.com/downloads/details.aspx?familyid=f7f90c30-1bfd-406b-a77f-612443e30185)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Excel 2002 z dodatkiem Service Pack 3
</td>
<td style="border:1px solid black;">
[Ważny](http://www.microsoft.com/downloads/details.aspx?familyid=907f96d5-d1e9-4471-b41c-3ac811e63038)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Excel 2003 z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Ważny](http://www.microsoft.com/downloads/details.aspx?familyid=296e5f2c-f594-41c8-a20a-3e4c40ae3948)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Podgląd programu Microsoft Office Excel 2003
</td>
<td style="border:1px solid black;">
[Ważny](http://www.microsoft.com/downloads/details.aspx?familyid=280bb2ac-b21a-46b5-8751-5a50fbebf107)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Ważny](http://www.microsoft.com/downloads/details.aspx?familyid=9f25922c-d3c2-4ef1-b164-8a21a77d29aa)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Podgląd programu Microsoft Office Excel 2003 z dodatkiem Service Pack 3
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Ważny](http://www.microsoft.com/downloads/details.aspx?familyid=9f25922c-d3c2-4ef1-b164-8a21a77d29aa)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Podgląd programu Microsoft Office Word 2003
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Ważny](http://www.microsoft.com/downloads/details.aspx?familyid=9f25922c-d3c2-4ef1-b164-8a21a77d29aa)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Podgląd programu Microsoft Office Word 2003 z dodatkiem Service Pack 3
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Ważny](http://www.microsoft.com/downloads/details.aspx?familyid=9f25922c-d3c2-4ef1-b164-8a21a77d29aa)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Excel 2007
</td>
<td style="border:1px solid black;">
[Ważny](http://www.microsoft.com/downloads/details.aspx?familyid=e7634cb5-9531-4284-9554-4168fc488e0c)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Pakiet zgodności dla Microsoft Office dla formatów plików programów Word, Excel i PowerPoint 2007
</td>
<td style="border:1px solid black;">
[Ważny](http://www.microsoft.com/downloads/details.aspx?familyid=e9251d71-9098-4125-ae91-7d4c83ea58ad)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Outlook 2000 z dodatkiem Service Pack 3
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny](http://www.microsoft.com/downloads/details.aspx?familyid=714a49cd-5bca-4719-96a1-e1077f279533)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Outlook 2002 z dodatkiem Service Pack 3
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny](http://www.microsoft.com/downloads/details.aspx?familyid=59853687-d885-4059-9460-ee403855dbd8)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Outlook 2003 z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny](http://www.microsoft.com/downloads/details.aspx?familyid=fccc7c4c-8496-4682-bd46-6590503c1bf2)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Outlook 2003 z dodatkiem Service Pack 3
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny](http://www.microsoft.com/downloads/details.aspx?familyid=fccc7c4c-8496-4682-bd46-6590503c1bf2)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Outlook 2007
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny](http://www.microsoft.com/downloads/details.aspx?familyid=4e2baf00-88eb-4eb6-961a-54245b363c21)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2004 dla komputerów Macintosh
</td>
<td style="border:1px solid black;">
[Ważny](http://www.microsoft.com/downloads/details.aspx?familyid=95dceb37-b35f-46db-b280-db0f3b298aa9)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Ważny](http://www.microsoft.com/downloads/details.aspx?familyid=95dceb37-b35f-46db-b280-db0f3b298aa9)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2008 dla komputerów Macintosh
</td>
<td style="border:1px solid black;">
[Ważny](http://www.microsoft.com/downloads/details.aspx?familyid=8fe8c32a-6d7a-482b-97c6-42562f089ee4)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<th colspan="5">
Inne oprogramowanie
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Web Components 2000  
(KB931660)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny](http://www.microsoft.com/downloads/details.aspx?familyid=806c654a-35e3-4385-855a-4b803249bfcf)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Web Components 2000  
(KB932031)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny](http://www.microsoft.com/downloads/details.aspx?familyid=f54d2a5e-c0ed-4f70-9746-38dd61c8e9d7)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Web Components 2000  
(KB933367)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny](http://www.microsoft.com/downloads/details.aspx?familyid=d71b23fa-a873-406d-bad7-e38e565dee39)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Web Components 2000  
(KB933369)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny](http://www.microsoft.com/downloads/details.aspx?familyid=2fe10ccd-40cb-4090-b83d-eae3d4eca174)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Web Components 2000  
(KB939714)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny](http://www.microsoft.com/downloads/details.aspx?familyid=5fddd54f-7a33-4ea3-b68d-b96a9bae509d)  
**<sup>[2]</sup>**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Web Components 2000  
(KB939714)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny](http://www.microsoft.com/downloads/details.aspx?familyid=5fddd54f-7a33-4ea3-b68d-b96a9bae509d)  
**<sup>[3]</sup>**
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Web Components 2000  
(KB941305)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny](http://www.microsoft.com/downloads/details.aspx?familyid=71de76ba-b62c-4a7a-a78a-9317f5255b13)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Web Components 2000  
(KB948257)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny](http://www.microsoft.com/downloads/details.aspx?familyid=526d87bd-c3da-412e-8765-c15987ae9b01)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Visual Studio .NET 2002 z dodatkiem Service Pack 1  
(KB933367)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Visual Studio .NET 2003 z dodatkiem Service Pack 1  
(KB933369)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft BizTalk Server 2000  
(KB939714)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft BizTalk Server 2002  
(KB939714)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Commerce Server 2000  
(KB941305)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Internet Security and Acceleration Server 2000 z dodatkiem Service Pack 2  
(KB948257)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
</table>
 
**Uwagi**

**<sup>[1]</sup>** Dla tego oprogramowania dostępna jest aktualizacja zabezpieczeń. Więcej informacji na temat oprogramowania lub składnika, którego dotyczy problem, znajduje się w tabeli oraz odpowiednim biuletynie zabezpieczeń.****

**<sup>[2]</sup>** Ta aktualizacja zabezpieczeń jest powiązana z oprogramowaniem Microsoft BizTalk Server 2000. Szczegółowe informacje znajdują się w odpowiednim biuletynie zabezpieczeń.

**<sup>[3]</sup>** Ta aktualizacja zabezpieczeń jest powiązana z oprogramowaniem Microsoft BizTalk Server 2002. Szczegółowe informacje znajdują się w odpowiednim biuletynie zabezpieczeń.

Narzędzia wykrywania i wdrażania oraz wskazówki
-----------------------------------------------

<span></span>
**Centrum zabezpieczeń**

Zarządzanie oprogramowaniem oraz aktualizacjami zabezpieczeń, które należy zainstalować na serwerach oraz komputerach stacjonarnych i przenośnych w organizacji. Więcej informacji można znaleźć w [Centrum TechNet Update Management Center](http://go.microsoft.com/fwlink/?linkid=69903). Witryna [TechNet Security Center](http://go.microsoft.com/fwlink/?linkid=21171) zawiera dodatkowe informacje na temat zabezpieczeń w produktach firmy Microsoft. Użytkownicy mogą także uzyskać dostęp do tych informacji w witrynie [Bezpieczeństwo w domu](http://go.microsoft.com/fwlink/?linkid=85102), klikając łącze „Najnowsze aktualizacje zabezpieczeń”.

Aktualizacje zabezpieczeń dostępne są w witrynach [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747), [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130) i [Office Update](http://go.microsoft.com/fwlink/?linkid=21135). Aktualizacje zabezpieczeń są także dostępne w witrynie [Microsoft Download Center](http://go.microsoft.com/fwlink/?linkid=21129). Najłatwiej je znaleźć, wyszukując wyrażenie „aktualizacja zabezpieczeń”.

Aktualizacje zabezpieczeń można także pobierać z [Wykazu usługi Microsoft Update](http://go.microsoft.com/fwlink/?linkid=96155). Wykaz usługi Microsoft Update zawiera katalog zawartości z możliwością przeszukiwania, który udostępniany jest poprzez usługi Windows Update i Microsoft Update i obejmuje aktualizacje zabezpieczeń, sterowniki i dodatki Service Pack. Wyszukiwanie przy użyciu numeru biuletynu zabezpieczeń (np. „MS07-036”) pozwala dodać do koszyka wszystkie odpowiednie aktualizacje (w tym różne wersje językowe aktualizacji) i pobrać pliki do wybranego folderu. Więcej informacji na temat Wykazu usługi Microsoft Update można znaleźć w [Często zadawanych pytaniach dotyczących Wykazu usługi Microsoft Update](http://go.microsoft.com/fwlink/?linkid=97900).

**Porady dotyczące wykrywania i wdrażania**

Firma Microsoft opublikowała porady dotyczące wykrywania i wdrażania, odnoszące się do aktualizacji zabezpieczeń udostępnionych w tym miesiącu. Porady te będą również pomocne dla informatyków, wyjaśniając, jak mogą oni wdrażać aktualizacje za pomocą różnych narzędzi, takich jak Windows Update, Microsoft Update, Office Update, Microsoft Baseline Security Analyzer (MBSA), Office Detection Tool, Microsoft Systems Management Server (SMS) i Extended Security Update Inventory Tool (ESUIT). Więcej informacji na ten temat można znaleźć w [artykule 910723 bazy wiedzy Microsoft Knowledge Base](http://support.microsoft.com/kb/910723).

**Narzędzie Microsoft Baseline Security Analyzer**

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

W tym miesiącu:

-   Firma Microsoft opublikowała dwie **niezwiązane z zabezpieczeniami** aktualizacje o wysokim priorytecie, które dostępne są w witrynie Microsoft Update (MU) i poprzez usługi Windows Server Update Services (WSUS).
-   Firma Microsoft opublikowała trzy **niezwiązane z zabezpieczeniami** aktualizacje o wysokim priorytecie dla systemu Windows, które dostępne są w witrynie Windows Update (WU) i za pośrednictwem usług WSUS.

Należy pamiętać, że informacje te dotyczą **wyłącznie** aktualizacji o wysokim priorytecie **niezwiązanych z zabezpieczeniami**, które dostępne są w witrynach Microsoft Update i Windows Update oraz poprzez usługi Windows Server Update Services i zostały opublikowane jednocześnie z podsumowaniem biuletynów zabezpieczeń. Informacje na temat aktualizacji **niezwiązanych z zabezpieczeniami**, które zostały opublikowane w innych dniach, **nie** są podawane.

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

-   Mike'owi Scottowi z firmy [SAIC](http://www.saic.com/), za zgłoszenie problemu opisanego w biuletynie MS08-014.
-   Mattowi Richardowi z firmy [VeriSign](http://www.verisign.com/), za zgłoszenie problemu opisanego w biuletynie MS08-014.
-   Gregowi MacManusowi z firmy[iDefense Labs](http://labs.idefense.com/), za zgłoszenie problemu opisanego w biuletynie MS08-014.
-   Yoshiyi Sasaki z firmy [JFE Systems](http://www.jfe-systems.com/), za zgłoszenie problemu opisanego w biuletynie MS08-014.
-   Bing Liu z firmy [Fortinet](http://www.fortinet.com/), za zgłoszenie problemu opisanego w biuletynie MS08-014.
-   Firmie [iDefense Labs](http://labs.idefense.com/) za zgłoszenie problemu opisanego w biuletynie MS08-014.
-   Cody'emu Pierce'owi z firmy [TippingPoint DVLabs](http://dvlabs.tippingpoint.com/), za zgłoszenie problemu opisanego w biuletynie MS08-014.
-   Moti Josephowi i Danowi Hubbardowi z firmy [Websense Security Labs](http://www.websense.com/), za zgłoszenie problemu opisanego w biuletynie MS08-014.
-   Gregowi MacManusowi z firmy[iDefense Labs](http://labs.idefense.com/) za zgłoszenie problemu opisanego w biuletynie MS08-015.
-   Arnaud Dovi z firmy [Zero Day Initiative (ZDI)](http://www.zerodayinitiative.com/), za zgłoszenie problemu opisanego w biuletynie MS08-016
-   Anonimowej osobie za zgłoszenie problemu opisanego w biuletynie MS08-016.
-   Chrisowi Riesowi z firmy [VigilantMinds Inc.](http://www.vigilantminds.com/), za zgłoszenie problemu opisanego w biuletynie MS08-017.
-   Xiao Hui z firmy [NCNIPC](http://www.nipc.org.cn/), za zgłoszenie problemu opisanego w biuletynie MS08-017.
-   Golanowi Yosefowi z firmy [Finjan](http://www.finjan.com/), za zgłoszenie problemu opisanego w biuletynie MS08-017.
-   Yuvalowi Ben-Itzhakowi z firmy [Finjan](http://www.finjan.com/), za zgłoszenie problemu opisanego w biuletynie MS08-017.

#### Pomoc techniczna

-   Wymienione oprogramowanie zostało przetestowane w celu ustalenia, których wersji dotyczy problem. Dla pozostałych wersji upłynął okres pomocy technicznej. Aby zapoznać się z zasadami cyklu pomocy technicznej dotyczącymi używanej wersji oprogramowania, odwiedź [witrynę zasad cyklu pomocy technicznej firmy Microsoft](http://go.microsoft.com/fwlink/?linkid=21742).
-   Klienci mogą uzyskać pomoc techniczną w [Biurze Obsługi Klienta Microsoft](http://go.microsoft.com/fwlink/?linkid=21131) pod numerem 0 801 802 000 (Opłata według stawek Twojego operatora) lub (0-22) 594 19 99 w godzinach od 9:00 do 17:00, od poniedziałku do piątku. Połączenia z działem pomocy technicznej związane z aktualizacjami zabezpieczeń są bezpłatne.
-   Klienci międzynarodowi mogą uzyskać pomoc w lokalnych przedstawicielstwach firmy Microsoft. Pomoc techniczna związana z aktualizacjami zabezpieczeń jest bezpłatna. Informacje o sposobie kontaktowania się z pomocą techniczną firmy Microsoft są dostępne w [międzynarodowej witrynie sieci Web pomocy i obsługi technicznej](http://go.microsoft.com/fwlink/?linkid=21155).

#### Zrzeczenie odpowiedzialności

Informacje w bazie wiedzy Microsoft Knowledge Base są dostarczane „tak jak są” bez jakiejkolwiek gwarancji. Firma Microsoft odrzuca wszelkie gwarancje, wyraźne i dorozumiane, w tym gwarancje dotyczące wartości handlowej i przydatności do określonego celu. Firma Microsoft Corporation ani jej dostawcy w żadnym wypadku nie ponoszą odpowiedzialności za jakiekolwiek szkody, w tym bezpośrednie, pośrednie, przypadkowe, wynikowe, utratę zysków handlowych lub szkody specjalne, nawet jeżeli firmę Microsoft Corporation lub jej dostawców powiadomiono o możliwości zaistnienia takich szkód. W niektórych stanach wyłączenie lub ograniczenie odpowiedzialności za straty wynikowe lub przypadkowe, a więc i powyższe ograniczenia, nie mają zastosowania.

#### Wersje

-   Wersja 1.0 (11 marca 2008 r.): Opublikowane podsumowanie biuletynów zabezpieczeń.
-   Wersja 1.1 (12 marca 2008 r.): Podsumowanie biuletynów zaktualizowano, aby podać nowe łącze pobierania składników Microsoft Office Web Components 2000 dla programu BizTalk Server 2000 i 2002.
-   V1.2 (26 marca 2008 r.): Zaktualizowano podsumowanie biuletynów w celu dodania osoby, która zgłosiła lukę opisaną w biuletynie MS08-017.
-   V2.0 (16 kwietnia 2008 r.): Podsumowanie biuletynów zaktualizowano w celu dodania apletu Podgląd programu Microsoft Office Word 2003 i apletu Podgląd programu Microsoft Office Word 2003 z dodatkiem Service Pack 3 do listy programów, których dotyczy problem w przypadku biuletynu MS08-016.

*Built at 2014-04-18T01:50:00Z-07:00*
