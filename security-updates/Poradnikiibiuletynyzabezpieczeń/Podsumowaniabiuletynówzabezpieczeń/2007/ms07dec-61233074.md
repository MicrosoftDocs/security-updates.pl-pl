---
TOCTitle: 'MS07-DEC'
Title: Microsoft Security Bulletin Summary for grudzień 2007
ms:assetid: 'ms07-dec'
ms:contentKeyID: 61233074
ms:mtpsurl: 'https://technet.microsoft.com/pl-PL/library/ms07-dec(v=Security.10)'
---

Security Bulletin Summary

Microsoft Security Bulletin Summary for grudzień 2007
=====================================================

Opublikowano: 11 grudnia 2007 | Zaktualizowano: 23 stycznia 2008

**Wersja:** 1.0

Niniejsze podsumowanie biuletynów zabezpieczeń zawiera spis biuletynów za grudzień 2007 r.

Z chwilą opublikowania biuletynów za grudzień 2007 r. niniejsze podsumowanie biuletynów zastępuje powiadomienie o biuletynach zabezpieczeń wydane 6 grudnia 2007 r. Aby uzyskać więcej informacji na temat usługi powiadamiania o biuletynach, zobacz [Powiadomienia o biuletynach zabezpieczeń firmy Microsoft (j.ang.)](http://technet.microsoft.com/security/bulletin/advance).

Aby dowiedzieć się, jak otrzymywać automatyczne powiadomienia o publikacji biuletynów zabezpieczeń firmy Microsoft, odwiedź stronę [Microsoft Technical Security Notifications (j.ang.)](http://go.microsoft.com/fwlink/?linkid=21163).

12 grudnia 2007 r. o godz. 11:00 czasu Pacyfiku (godz. 20:00 czasu środkowoeuropejskiego) firma Microsoft udostępni emisję internetową, w której znajdą się odpowiedzi na pytania klientów dotyczące tych biuletynów (USA i Kanada). [Zarejestruj się, aby zobaczyć emisję internetową dotyczącą biuletynów zabezpieczeń za grudzień (j.ang.)](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032344696&eventcategory=4&culture=en-us&countrycode=us). Po tym dniu emisja internetowa będzie dostępna na żądanie. Aby uzyskać więcej informacji, zobacz [podsumowania biuletynów zabezpieczeń](http://technet.microsoft.com/security/bulletin/summary) i [emisje internetowe firmy Microsoft (j.ang.)](http://technet.microsoft.com/security/bulletin/summary).

Firma Microsoft udostępnia także informacje, dzięki którym klienci mogą ustalić priorytety dla aktualizacji zabezpieczeń w związku z niezwiązanymi z zabezpieczeniami aktualizacjami o wysokim priorytecie, które publikowane są w tym samym dniu, co comiesięczne aktualizacje zabezpieczeń. Zapoznaj się z sekcją **Inne informacje**.

### Informacje o biuletynie

#### Streszczenia

W bieżącym miesiącu opublikowano następujące biuletyny (w kolejności wskaźnika ważności):

Krytyczny (3)
-------------

<span></span>

| Identyfikator biuletynu           | Biuletyn zabezpieczeń firmy Microsoft MS07-064                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
|-----------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**               | [**Luki w zabezpieczeniach interfejsu DirectX umożliwiają zdalne wykonanie kodu (941568)**](http://technet.microsoft.com/security/bulletin/ms07-064)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Streszczenie**                  | Ta aktualizacja zabezpieczeń o krytycznym wskaźniku ważności usuwa dwie luki w zabezpieczeniach programu Microsoft DirectX, które zostały zgłoszone przez użytkowników Luki te mogą umożliwić wykonanie kodu, jeśli użytkownik otworzy specjalnie spreparowany plik służący do strumieniowego przesyłania mediów w programie DirectX. Jeśli użytkownik jest zalogowany jako administrator, osoba atakująca, która pomyślnie wykorzysta tę lukę, może uzyskać pełną kontrolę nad systemem, którego ta luka dotyczy. Osoba taka może wówczas instalować programy, przeglądać, zmieniać i usuwać dane oraz tworzyć nowe konta z pełnymi uprawnieniami. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi. |
| **Maksymalny wskaźnik ważności:** | [Krytyczny](http://technet.microsoft.com/security/bulletin/rating)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Wpływ luki**                    | Zdalne wykonanie kodu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| **Wykrywanie**                    | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Aktualizacja nie będzie wymagać ponownego uruchomienia komputera z wyjątkiem niektórych sytuacji.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Podlegające oprogramowanie**    | **Windows, DirectX, DirectShow.** Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |

| Identyfikator biuletynu           | Biuletyn zabezpieczeń firmy Microsoft MS07-068                                                                                                                                                                                                                                                                                                                                                                                                                                     |
|-----------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**               | [**Luka w zabezpieczeniach formatu plików pakietu Windows Media może umożliwić zdalne wykonanie kodu (941569 i 944275)**](http://technet.microsoft.com/security/bulletin/ms07-068)                                                                                                                                                                                                                                                                                                 |
| **Streszczenie**                  | Ta krytyczna aktualizacja zabezpieczeń usuwa zgłoszoną przez użytkowników lukę w zabezpieczeniach formatu Windows Media. Ta luka w zabezpieczeniach umożliwia zdalne wykonanie kodu, gdy użytkownik wyświetli specjalnie spreparowany plik w programie Windows Media Format Runtime. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi. |
| **Maksymalny wskaźnik ważności:** | [Krytyczny](http://technet.microsoft.com/security/bulletin/rating)                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Wpływ luki**                    | Zdalne wykonanie kodu                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Wykrywanie**                    | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Aktualizacja nie będzie wymagać ponownego uruchomienia komputera z wyjątkiem niektórych sytuacji.                                                                                                                                                                                                                                                                 |
| **Podlegające oprogramowanie**    | **Windows, Windows Media Format Runtime. **Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                                                         |

| Identyfikator biuletynu           | Biuletyn zabezpieczeń firmy Microsoft MS07-069                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
|-----------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**               | [**Zbiorcza aktualizacja zabezpieczeń dla programu Internet Explorer (942615)**](http://technet.microsoft.com/security/bulletin/ms07-069)                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Streszczenie**                  | Niniejsza aktualizacja zabezpieczeń o krytycznym wskaźniku ważności pozwala usunąć cztery luki w zabezpieczeniach zgłoszone przez użytkowników. Luka o największym znaczeniu dla bezpieczeństwa może pozwolić na zdalne wykonanie kodu, jeśli użytkownik wyświetli specjalnie spreparowaną stronę sieci Web przy użyciu programu Internet Explorer. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi. |
| **Maksymalny wskaźnik ważności:** | [Krytyczny](http://technet.microsoft.com/security/bulletin/rating)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Wpływ luki**                    | Zdalne wykonanie kodu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| **Wykrywanie**                    | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Aktualizacja będzie wymagać ponownego uruchomienia komputera.                                                                                                                                                                                                                                                                                                                                                                    |
| **Podlegające oprogramowanie**    | **Windows, Internet Explorer. **Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                                                                                                                                   |

Ważne (4)
---------

<span></span>

| Identyfikator biuletynu           | Biuletyn zabezpieczeń firmy Microsoft MS07-063                                                                                                                                                                                                                                                                                                                                                                                   |
|-----------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**               | [**Luka w zabezpieczeniach usługi SMBv2 umożliwia zdalne wykonanie kodu (942624)**](http://technet.microsoft.com/security/bulletin/ms07-063)                                                                                                                                                                                                                                                                                     |
| **Streszczenie**                  | Niniejsza aktualizacja zabezpieczeń o wskaźniku ważności „ważny” pozwala usunąć zgłoszoną przez użytkowników lukę w zabezpieczeniach usługi Server Message Block Version 2 (SMBv2). Ta luka w zabezpieczeniach potencjalnie może pozwolić osobie atakującej na manipulację danymi przesyłanymi za pośrednictwem usługi SMBv2, co może umożliwić zdalne wykonanie kodu w konfiguracjach domen komunikujących się przy jej użyciu. |
| **Maksymalny wskaźnik ważności:** | [Ważny](http://technet.microsoft.com/security/bulletin/rating)                                                                                                                                                                                                                                                                                                                                                                   |
| **Wpływ luki**                    | Zdalne wykonanie kodu                                                                                                                                                                                                                                                                                                                                                                                                            |
| **Wykrywanie**                    | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Aktualizacja będzie wymagać ponownego uruchomienia komputera.                                                                                                                                                                                                                                                   |
| **Podlegające oprogramowanie**    | **Windows. **Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                                     |

| Identyfikator biuletynu           | Biuletyn zabezpieczeń firmy Microsoft MS07-065                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
|-----------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**               | [**Luka w zabezpieczeniach kolejkowania wiadomości może pozwolić na zdalne wykonanie kodu (937894)**](http://technet.microsoft.com/security/bulletin/ms07-065)                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **Streszczenie**                  | Niniejsza aktualizacja zabezpieczeń o wskaźniku ważności „ważny” pozwala usunąć zgłoszoną przez użytkowników lukę w zabezpieczeniach w usłudze kolejkowania wiadomości (MSMQ), która może zezwolić na zdalne wykonanie kodu we wdrożeniach w systemie Microsoft Windows 2000 Server lub na podniesienie uprawnień we wdrożeniach w systemie Microsoft Windows 2000 Professional i Windows XP. Aby wykorzystać tę lukę, osoba atakująca musi dysponować prawidłowymi poświadczeniami logowania. Osoba taka może wówczas instalować programy, przeglądać, zmieniać i usuwać dane oraz tworzyć nowe konta. |
| **Maksymalny wskaźnik ważności:** | [Ważny](http://technet.microsoft.com/security/bulletin/rating)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **Wpływ luki**                    | Zdalne wykonanie kodu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| **Wykrywanie**                    | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Aktualizacja będzie wymagać ponownego uruchomienia komputera.                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **Podlegające oprogramowanie**    | **Windows. **Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                                                                                                                                                                                                            |

| Identyfikator biuletynu           | Biuletyn zabezpieczeń firmy Microsoft MS07-066                                                                                                                                                                                                                                                                                                                                                                                   |
|-----------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**               | [**Luka w zabezpieczeniach jądra systemu Windows może pozwolić na podniesienie poziomu uprawnień (943078)**](http://technet.microsoft.com/security/bulletin/ms07-066)                                                                                                                                                                                                                                                            |
| **Streszczenie**                  | Niniejsza aktualizacja zabezpieczeń o wskaźniku ważności „ważny” pozwala usunąć zgłoszoną przez użytkowników lukę w zabezpieczeniach jądra systemu Windows. Osoba atakująca, której uda się wykorzystać tę lukę, może uzyskać pełną kontrolę nad systemem, którego dotyczy luka. Osoba taka może wówczas instalować programy, przeglądać, zmieniać i usuwać dane oraz tworzyć nowe konta z pełnymi uprawnieniami administratora. |
| **Maksymalny wskaźnik ważności:** | [Ważny](http://technet.microsoft.com/security/bulletin/rating)                                                                                                                                                                                                                                                                                                                                                                   |
| **Wpływ luki**                    | Podniesienie uprawnień                                                                                                                                                                                                                                                                                                                                                                                                           |
| **Wykrywanie**                    | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Aktualizacja będzie wymagać ponownego uruchomienia komputera.                                                                                                                                                                                                                                                   |
| **Podlegające oprogramowanie**    | **Windows. **Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                                     |

| Identyfikator biuletynu           | Biuletyn zabezpieczeń firmy Microsoft MS07-067                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
|-----------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**               | [**Luka w zabezpieczeniach sterownika Macrovision umożliwia lokalne podniesienie uprawnień (944653)**](http://technet.microsoft.com/security/bulletin/ms07-067)                                                                                                                                                                                                                                                                                                                                                                 |
| **Streszczenie**                  | Ta ważna aktualizacja zabezpieczeń usuwa jedną lukę w zabezpieczeniach, która została zgłoszona przez organizację publiczną. W zabezpieczeniach sterownika Macrovision występuje luka związana z nieprawidłową obsługą parametrów konfiguracji, która umożliwia lokalne podniesienie uprawnień. Osoba atakująca, której uda się wykorzystać tę lukę, może uzyskać pełną kontrolę nad systemem. Osoba taka może wówczas instalować programy, przeglądać, zmieniać i usuwać dane oraz tworzyć nowe konta z pełnymi uprawnieniami. |
| **Maksymalny wskaźnik ważności:** | [Ważny](http://technet.microsoft.com/security/bulletin/rating)                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **Wpływ luki**                    | Lokalne podniesienie uprawnień                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **Wykrywanie**                    | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Aktualizacja będzie wymagać ponownego uruchomienia komputera.                                                                                                                                                                                                                                                                                                                                                  |
| **Podlegające oprogramowanie**    | **Windows. **Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                                                                                                                                    |

Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki
---------------------------------------------------------------------------------

<span></span>
**How do I use this table?**

Tabela ta pozwala odczytać informacje o aktualizacjach zabezpieczeń, których zainstalowanie może być konieczne. Należy przejrzeć informacje dla każdego wymienionego programu lub składnika oprogramowania w celu sprawdzenia, czy są wymagane aktualizacje zabezpieczeń. Dla każdego programu lub składnika oprogramowania wymienionego na liście podany jest wpływ luki oraz hiperłącze do dostępnej aktualizacji oprogramowania.

**Note** You may have to install several security updates for a single vulnerability. Przejrzyj całą kolumnę dla każdego wymienionego identyfikatora biuletynu, aby sprawdzić, jakie aktualizacje musisz zainstalować, w oparciu o programy bądź składniki zainstalowane w systemie.

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
[**MS07-063**](http://technet.microsoft.com/security/bulletin/ms07-063)
</td>
<td style="border:1px solid black;">
[**MS07-064**](http://technet.microsoft.com/security/bulletin/ms07-064)
</td>
<td style="border:1px solid black;">
[**MS07-065**](http://technet.microsoft.com/security/bulletin/ms07-065)
</td>
<td style="border:1px solid black;">
[**MS07-066**](http://technet.microsoft.com/security/bulletin/ms07-066)
</td>
<td style="border:1px solid black;">
[**MS07-067**](http://technet.microsoft.com/security/bulletin/ms07-067)
</td>
<td style="border:1px solid black;">
[**MS07-068**](http://technet.microsoft.com/security/bulletin/ms07-068)
</td>
<td style="border:1px solid black;">
[**MS07-069**](http://technet.microsoft.com/security/bulletin/ms07-069)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Maksymalny wskaźnik ważności:**
</td>
<td style="border:1px solid black;">
[**Ważny**](http://technet.microsoft.com/security/bulletin/rating)
</td>
<td style="border:1px solid black;">
[**Krytyczny**](http://technet.microsoft.com/security/bulletin/rating)
</td>
<td style="border:1px solid black;">
[**Ważny**](http://technet.microsoft.com/security/bulletin/rating)
</td>
<td style="border:1px solid black;">
[**Ważny**](http://technet.microsoft.com/security/bulletin/rating)
</td>
<td style="border:1px solid black;">
[**Ważny**](http://technet.microsoft.com/security/bulletin/rating)
</td>
<td style="border:1px solid black;">
[**Krytyczny**](http://technet.microsoft.com/security/bulletin/rating)
</td>
<td style="border:1px solid black;">
[**Krytyczny**](http://technet.microsoft.com/security/bulletin/rating)
</td>
</tr>
<tr>
<th colspan="8">
System operacyjny Windows
</th>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 Server z dodatkiem Service Pack 4 i Microsoft Windows 2000 Professional z dodatkiem Service Pack 4
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
[Ważny](http://www.microsoft.com/downloads/details.aspx?familyid=bda9d0b4-f7cb-4d9d-b030-043d7437734b&displaylang=pl)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
[Umiarkowany](http://www.microsoft.com/downloads/details.aspx?familyid=09d4e6ae-5d19-4f11-bb7e-60cee8263bc8&displaylang=pl)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Ważny](http://www.microsoft.com/downloads/details.aspx?familyid=c7d368d0-f7bf-4946-a4a6-3e88315e5317&displaylang=pl)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows XP Professional x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Ważny (j.ang.)](http://www.microsoft.com/downloads/details.aspx?familyid=5f4fa8e9-fcf2-4daf-93c0-8bb267da69aa)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Ważny (j.ang.)](http://www.microsoft.com/downloads/details.aspx?familyid=5f4fa8e9-fcf2-4daf-93c0-8bb267da69aa)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 z dodatkiem Service Pack 1
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Ważny](http://www.microsoft.com/downloads/details.aspx?familyid=0f84f5e2-1dd8-4882-b796-444ab70b6b02&displaylang=pl)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Ważny](http://www.microsoft.com/downloads/details.aspx?familyid=0f84f5e2-1dd8-4882-b796-444ab70b6b02&displaylang=pl)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Ważny (j.ang.)](http://www.microsoft.com/downloads/details.aspx?familyid=1f416b71-783f-4cbc-9b85-9a9be7daa0d7)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Ważny (j.ang.)](http://www.microsoft.com/downloads/details.aspx?familyid=1f416b71-783f-4cbc-9b85-9a9be7daa0d7)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 z dodatkiem SP1 dla systemów z procesorem Itanium
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
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
Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
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
Windows Vista
</td>
<td style="border:1px solid black;">
[Ważny](http://www.microsoft.com/downloads/details.aspx?familyid=9d22a9ee-cc08-4b2d-af4e-55d326f82761&displaylang=pl)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Ważny](http://www.microsoft.com/downloads/details.aspx?familyid=9787619f-1297-411e-8b9c-3ad3e6a99797&displaylang=pl)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition
</td>
<td style="border:1px solid black;">
[Ważny](http://www.microsoft.com/downloads/details.aspx?familyid=05a9501c-4da3-4fa1-901e-99cb262e5e36&displaylang=pl)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Ważny](http://www.microsoft.com/downloads/details.aspx?familyid=5f382050-8df6-43aa-82e9-8fad5ff8ecec&displaylang=pl)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr>
<th colspan="8">
Składniki systemu operacyjnego Windows:
</th>
</tr>
<tr>
<td style="border:1px solid black;">
DirectX 7.0 w systemie Microsoft Windows 2000 z dodatkiem Service Pack 4
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny](http://www.microsoft.com/downloads/details.aspx?familyid=06196774-5a11-4525-b53c-8cb000738949&displaylang=pl)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
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
DirectX 8.1 w systemie Microsoft Windows 2000 z dodatkiem Service Pack 4
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny](http://www.microsoft.com/downloads/details.aspx?familyid=ccb872bd-fc06-4a3f-ac70-3c9a42d57b37&displaylang=pl)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
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
DirectX 9.0\* w systemie Microsoft Windows 2000 z dodatkiem Service Pack 4
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny](http://www.microsoft.com/downloads/details.aspx?familyid=03b14ce0-5189-4803-8151-6ac5cb6a9179&displaylang=pl)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
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
DirectX 9.0\* w systemie Windows XP Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny](http://www.microsoft.com/downloads/details.aspx?familyid=04a8f8d3-69f9-4445-baab-f45616a6b9b7&displaylang=pl)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
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
DirectX 9.0\* w systemie Windows XP Professional x64 Edition i Windows XP Professional x64 Edition z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny (j.ang.)](http://www.microsoft.com/downloads/details.aspx?familyid=f096c500-e765-4e75-8443-7ffec4ddf149)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
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
DirectX 9.0\* w systemie Windows Server 2003 z dodatkiem Service Pack 1 i Windows Server 2003 z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny](http://www.microsoft.com/downloads/details.aspx?familyid=d80a295a-baf9-4981-8a28-1b4207ecc5f7&displaylang=pl)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
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
DirectX 9.0\* w systemie Windows Server 2003 x64 Edition i Windows Server 2003 x64 Edition z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny (j.ang.)](http://www.microsoft.com/downloads/details.aspx?familyid=378086ea-60b8-409f-970a-fcfd62025150)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
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
DirectX 9.0\* w systemie Windows Server 2003 z dodatkiem SP1 dla systemów z procesorem Itanium i Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny](http://www.microsoft.com/downloads/details.aspx?familyid=2e6ea4bb-9f4f-46fb-9d51-e20b15e61a89&displaylang=pl)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
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
DirectX 10.0 w systemie Windows Vista
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny (j.ang.)](http://www.microsoft.com/downloads/details.aspx?familyid=bfa571bc-e43f-45e3-bc98-4086985c99aa)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
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
DirectX 10.0 w systemie Windows Vista x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny](http://www.microsoft.com/downloads/details.aspx?familyid=3d8803da-108b-4b9d-a039-84932dce8e42&displaylang=pl)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
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
Internet Explorer 5.01 z dodatkiem Service Pack 4 w systemie Microsoft Windows 2000 z dodatkiem Service Pack 4
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny](http://www.microsoft.com/downloads/details.aspx?familyid=b3bd16ea-5d69-4ae3-84b3-ab773052ceeb&displaylang=pl)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Internet Explorer 6 z dodatkiem Service Pack 1 zainstalowany w systemie Microsoft Windows 2000 z dodatkiem Service Pack 4
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny](http://www.microsoft.com/downloads/details.aspx?familyid=bc8edf05-262a-4d1d-b196-4fc1a844970c&displaylang=pl)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Internet Explorer 6 dla systemu Windows XP z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny](http://www.microsoft.com/downloads/details.aspx?familyid=6e4ebafc-34c3-4dc7-b712-152c611d3f0a&displaylang=pl)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Internet Explorer 6 dla systemu Windows XP Professional x64 Edition i Windows XP Professional x64 Edition z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny (j.ang.)](http://www.microsoft.com/downloads/details.aspx?familyid=f5a5af23-30fb-4e47-94bd-3b05b55c92f2)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Internet Explorer 6 dla systemu Windows Server 2003 z dodatkiem Service Pack 1 i Windows Server 2003 z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Umiarkowany](http://www.microsoft.com/downloads/details.aspx?familyid=bf466060-a585-4c2e-a48d-70e080c3bbe7&displaylang=pl)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Internet Explorer 6 dla systemów Windows Server 2003 x64 Edition i Windows Server 2003 x64 Edition z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Umiarkowany (j.ang.)](http://www.microsoft.com/downloads/details.aspx?familyid=074697f2-18c8-4521-bbf7-1d0e7395d27d)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Internet Explorer 6 dla systemu Windows Server 2003 z dodatkiem SP1 dla systemów z procesorem Itanium i Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Umiarkowany (j.ang.)](http://www.microsoft.com/downloads/details.aspx?familyid=b3f390a6-0361-4553-b627-5e7ad6bf5055)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Internet Explorer 7 dla systemu Windows XP z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny](http://www.microsoft.com/downloads/details.aspx?familyid=b15a6506-02dd-43c2-aef4-e10c1c76ee97&displaylang=pl)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Internet Explorer 7 dla systemu Windows XP Professional x64 Edition i Windows XP Professional x64 Edition z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny (j.ang.)](http://www.microsoft.com/downloads/details.aspx?familyid=c092a6bb-8e62-4d90-bdb1-5f3a15968f75)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Internet Explorer 7 dla systemu Windows Server 2003 z dodatkiem Service Pack 1 i Windows Server 2003 z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Umiarkowany](http://www.microsoft.com/downloads/details.aspx?familyid=34759c10-16a5-42a2-974d-9d532fb5a0a7&displaylang=pl)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Internet Explorer 7 dla systemów Windows Server 2003 x64 Edition i Windows Server 2003 x64 Edition z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Umiarkowany (j.ang.)](http://www.microsoft.com/downloads/details.aspx?familyid=7dccce5a-7562-448b-a345-cf1cc758e35c)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Internet Explorer 7 dla systemu Windows Server 2003 z dodatkiem SP1 dla systemów z procesorem Itanium i Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Umiarkowany (j.ang.)](http://www.microsoft.com/downloads/details.aspx?familyid=8414f3fb-216a-4d46-b590-4c1f304dff91)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Program Internet Explorer 7 w systemie Windows Vista
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny](http://www.microsoft.com/downloads/details.aspx?familyid=26d303da-bb2e-4555-96f1-becb0e277341&displaylang=pl)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Internet Explorer 7 w systemie Windows Vista x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny (j.ang.)](http://www.microsoft.com/downloads/details.aspx?familyid=c5e88e0b-a4c2-4690-91d9-326800030a16)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Media Format Runtime 7.1 w systemie Microsoft Windows 2000 z dodatkiem Service Pack 4 (KB941569)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny](http://www.microsoft.com/downloads/details.aspx?familyid=eecdf2ce-9aa7-4f0c-b62b-2fa7a32f369e&displaylang=pl)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Media Format Runtime 9 w systemie Microsoft Windows 2000 z dodatkiem Service Pack 4 (KB941569)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny](http://www.microsoft.com/downloads/details.aspx?familyid=eecdf2ce-9aa7-4f0c-b62b-2fa7a32f369e&displaylang=pl)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Media Format Runtime 9 w systemie Windows XP z dodatkiem Service Pack 2 (KB941569)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny](http://www.microsoft.com/downloads/details.aspx?familyid=bece702a-6e61-433e-8275-20f4e84f2c92&displaylang=pl)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Media Format Runtime 9.5 w systemie Windows XP z dodatkiem Service Pack 2 (KB941569)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny](http://www.microsoft.com/downloads/details.aspx?familyid=bece702a-6e61-433e-8275-20f4e84f2c92&displaylang=pl)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Program Windows Media Format Runtime 9.5 w systemie Windows XP Professional x64 Edition i Windows XP Professional x64 Edition z dodatkiem Service Pack 2 (KB941569)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny (j.ang.)](http://www.microsoft.com/downloads/details.aspx?familyid=81f20b45-dfc7-4ddf-a4b4-6c0e9476ed51)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Program Windows Media Format Runtime 9.5 w systemie Windows Server 2003 z dodatkiem Service Pack 1 i Windows Server 2003 z dodatkiem Service Pack 2 (KB941569)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny](http://www.microsoft.com/downloads/details.aspx?familyid=8fea7da8-a7f3-4786-97c2-fb5ea7018159&displaylang=pl)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Program Windows Media Format Runtime 9.5 w systemie Windows Server 2003 x64 Edition i Windows Server 2003 x64 Edition z dodatkiem Service Pack 2 (KB941569)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny (j.ang.)](http://www.microsoft.com/downloads/details.aspx?familyid=ffc69c76-02f1-4b15-8ec1-dab8c7e33bd4)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Program Windows Media Format Runtime 9.5 x64 Edition w systemie Windows Server 2003 x64 Edition i Windows Server 2003 x64 Edition z dodatkiem Service Pack 2 (KB941569)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny (j.ang.)](http://www.microsoft.com/downloads/details.aspx?familyid=ffc69c76-02f1-4b15-8ec1-dab8c7e33bd4)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Program Windows Media Format Runtime 9.5 x64 Edition w systemie Windows XP Professional x64 Edition i Windows XP Professional x64 Edition z dodatkiem Service Pack 2 (KB941569)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny (j.ang.)](http://www.microsoft.com/downloads/details.aspx?familyid=72d2ca0e-da81-45ee-9321-4970b80f4a5a)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Media Format Runtime 11 w systemie Windows XP z dodatkiem Service Pack 2 (KB941569)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny](http://www.microsoft.com/downloads/details.aspx?familyid=bece702a-6e61-433e-8275-20f4e84f2c92&displaylang=pl)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Program Windows Media Format Runtime 11 w systemie Windows XP Professional x64 Edition i Windows XP Professional x64 Edition z dodatkiem Service Pack 2 (KB941569)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny (j.ang.)](http://www.microsoft.com/downloads/details.aspx?familyid=1037b224-ac89-4efd-b189-6f3da77a88e6)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Media Format Runtime 11 w systemie Windows Vista (KB941569)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny](http://www.microsoft.com/downloads/details.aspx?familyid=9a98ef96-bc2e-42b7-9a24-c82c8fb379db&displaylang=pl)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Media Format Runtime 11 w systemie Windows Vista x64 Edition (KB941569)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny](http://www.microsoft.com/downloads/details.aspx?familyid=3ce02c95-d695-4f14-9fb3-30c83a9cfb9c&displaylang=pl)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Program Windows Media Services 9.1 w systemie Windows Server 2003 z dodatkiem Service Pack 1 i Windows Server 2003 z dodatkiem Service Pack 2 (KB944275)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny](http://www.microsoft.com/downloads/details.aspx?familyid=096711d4-ce01-45d0-9c2d-ebfa5c671b9f&displaylang=pl)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Program Windows Media Services 9.1 x64 Edition w systemie Windows Server 2003 x64 Edition i Windows Server 2003 x64 Edition z dodatkiem Service Pack 2 (KB944275)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny (j.ang.)](http://www.microsoft.com/downloads/details.aspx?familyid=23c23800-5aaa-455b-96bf-4ead4dfdd95d)
</td>
<td style="border:1px solid black;">
</td>
</tr>
</table>
 
**Uwagi**

**<sup>[1]</sup>** Dla tego systemu operacyjnego dostępna jest aktualizacja zabezpieczeń. Więcej informacji na temat oprogramowania lub składnika, którego dotyczy problem, znajduje się w tabeli oraz odpowiednim biuletynie zabezpieczeń.** **

**\*** Zawiera DirectX 9.0b i DirectX 9.0c

Narzędzia wykrywania i wdrażania oraz wskazówki
-----------------------------------------------

<span></span>
**Centrum zabezpieczeń**

Zarządzanie oprogramowaniem oraz aktualizacjami zabezpieczeń, które należy zainstalować na serwerach oraz komputerach stacjonarnych i przenośnych w organizacji. Więcej informacji można znaleźć w [Centrum TechNet Update Management Center (j.ang.)](http://go.microsoft.com/fwlink/?linkid=69903). Witryna [TechNet Security Center](http://www.microsoft.com/poland/technet/security/) zawiera dodatkowe informacje na temat zabezpieczeń w produktach firmy Microsoft. Użytkownicy mogą także uzyskać dostęp do tych informacji w witrynie [Bezpieczeństwo w domu](http://www.microsoft.com/poland/athome/security/default.mspx), klikając łącze „Najnowsze aktualizacje zabezpieczeń”.

Aktualizacje zabezpieczeń dostępne są w witrynach [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747), [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130) i [Office Update](http://office.microsoft.com/pl-pl/officeupdate/default.aspx). Aktualizacje zabezpieczeń są także dostępne w witrynie [Microsoft Download Center](http://www.microsoft.com/downloads/results.aspx?freetext=poprawka+zabezpiecze%c5%84&productid=&displaylang=pl). Najłatwiej je znaleźć, przeprowadzając wyszukiwanie wyrażenia „poprawka zabezpieczeń”.

Aktualizacje zabezpieczeń można także pobierać z [Wykazu usługi Microsoft Update](http://go.microsoft.com/fwlink/?linkid=96155). Wykaz usługi Microsoft Update zawiera katalog zawartości z możliwością przeszukiwania, który udostępniany jest poprzez usługi Windows Update i Microsoft Update i obejmuje aktualizacje zabezpieczeń, sterowniki i dodatki Service Pack. Wyszukiwanie przy użyciu numeru biuletynu zabezpieczeń (np. „MS07-036”) pozwala dodać do koszyka wszystkie odpowiednie aktualizacje (w tym różne wersje językowe aktualizacji) i pobrać pliki do wybranego folderu. Więcej informacji na temat Wykazu usługi Microsoft Update można znaleźć w [Często zadawanych pytaniach dotyczących Wykazu usługi Microsoft Update](http://go.microsoft.com/fwlink/?linkid=97900).

**Porady dotyczące wykrywania i wdrażania**

Firma Microsoft opublikowała porady dotyczące wykrywania i wdrażania, odnoszące się do aktualizacji zabezpieczeń udostępnionych w tym miesiącu. Porady te będą również pomocne dla informatyków, wyjaśniając jak mogą oni wdrażać aktualizacje za pomocą różnych narzędzi, takich jak Windows Update, Microsoft Update, Office Update, Microsoft Baseline Security Analyzer (MBSA), Office Detection Tool, Microsoft Systems Management Server (SMS), Extended Security Update Inventory Tool i Enterprise Update Scan Tool (EST). Więcej informacji na ten temat można znaleźć w [artykule 910723 bazy wiedzy Microsoft Knowledge Base](http://support.microsoft.com/kb/910723).

**Narzędzie Microsoft Baseline Security Analyzer (MBSA)**

Narzędzie Microsoft Baseline Security Analyzer umożliwia administratorom skanowanie lokalnych i zdalnych systemów w poszukiwaniu brakujących aktualizacji zabezpieczeń oraz typowych błędów konfiguracji zabezpieczeń. Więcej informacji na temat narzędzia MBSA można znaleźć w witrynie sieci Web[Microsoft Baseline Security Analyzer](http://www.microsoft.com/poland/technet/security/tools/mbsa.mspx).

**Uwaga** Po 9 października 2007 r. używany przez narzędzie MBSA 1.2.1 plik MSSecure.XML nie będzie już aktualizowany. Po upływie tej daty do pliku MSSecure.XML używanego przez narzędzie MBSA 1.2.1 nie będą dodawane nowe aktualizacje zabezpieczeń. Nie będą również publikowane nowe wersje narzędzia Enterprise Scan Tool. Nie dotyczy to narzędzi Security Update Inventory Tool (SUIT) ani Extended Security Update Inventory Tool (ESUIT) dla programów SMS 2.0 i SMS 2003. Więcej informacji można znaleźć w witrynie sieci Web [Microsoft Baseline Security Analyzer](http://www.microsoft.com/poland/technet/security/tools/mbsa.mspx).

**Windows Server Update Services**

Korzystając z programu Windows Server Update Services (WSUS), administratorzy mogą szybko i niezawodnie wdrożyć najnowsze aktualizacje krytyczne i aktualizacje zabezpieczeń przeznaczonych dla systemu operacyjnego Windows 2000 i nowszych, pakietu Office XP i nowszych, programu Exchange Server 2003 oraz SQL Server 2000 w systemie operacyjnym Windows 2000 i nowszych.

Więcej informacji na temat sposobu wdrażania tej aktualizacji zabezpieczeń za pomocą programu Windows Server Update Services można znaleźć w [witrynie sieci Web programu Windows Server Update Services (j.ang.)](http://go.microsoft.com/fwlink/?linkid=50120).

**Program Systems Management Server**

Program Systems Management Server (SMS) jest przeznaczonym dla przedsiębiorstw i w znacznym stopniu konfigurowalnym rozwiązaniem służącym do zarządzania aktualizacjami. Program SMS umożliwia administratorom znalezienie komputerów z systemem Windows, na których należy zainstalować aktualizację zabezpieczeń, a także przeprowadzić kontrolowane wdrożenie tych aktualizacji w całym przedsiębiorstwie, w minimalnym stopniu zakłócając przy tym pracę użytkowników końcowych. Więcej informacji na temat możliwości wykorzystania przez administratorów programu SMS 2003 do wdrażania aktualizacji zabezpieczeń można znaleźć [w witrynie sieci Web zarządzania poprawkami zabezpieczeń programu SMS 2003 (j.ang.)](http://go.microsoft.com/fwlink/?linkid=22939). Użytkownicy programu SMS 2.0 mogą także skorzystać z dodatku [Software Updates Services Feature Pack (j.ang.)](http://go.microsoft.com/fwlink/?linkid=33340) ułatwiającego wdrożenie aktualizacji zabezpieczeń. Więcej informacji na temat programu SMS można znaleźć w witrynie sieci Web [Microsoft Systems Management Server (j.ang.)](http://go.microsoft.com/fwlink/?linkid=21158).

**Uwaga** Program SMS zapewnia obsługę rozwiązań zawartych w biuletynach zabezpieczeń dzięki narzędziom Microsoft Baseline Security Analyzer oraz Microsoft Office Detection Tool. Narzędzia te mogą nie wykrywać wszystkich aktualizacji oprogramowania. W takich przypadkach administratorzy mogą wykorzystywać dostępne w programie SMS funkcje zarządzania zasobami do przyporządkowania poszczególnych aktualizacji określonym systemom. Aby uzyskać więcej informacji dotyczących tej procedury, zobacz [Wdrażanie aktualizacji oprogramowania za pomocą funkcji Software Distribution programu SMS (j.ang.)](http://go.microsoft.com/fwlink/?linkid=33341). Niektóre aktualizacje oprogramowania wymagają od użytkownika uprawnień administratora po ponownym uruchomieniu systemu. Do zainstalowania tych aktualizacji administratorzy mogą użyć narzędzia Elevated Rights Deployment Tool (dostępnego w dodatkach [SMS 2003 Administration Feature Pack (j.ang.)](http://go.microsoft.com/fwlink/?linkid=33387) oraz [SMS 2.0 Administration Feature Pack (j.ang.)](http://go.microsoft.com/fwlink/?linkid=21161).

### Inne informacje:

#### Narzędzie Microsoft Windows do usuwania złośliwego oprogramowania

Firma Microsoft opublikowała zaktualizowaną wersję narzędzia Microsoft Windows Malicious Software Removal Tool, która dostępna jest w witrynach sieci Web Windows Update i Microsoft Update, poprzez usługi Windows Server Update Services i w witrynie Microsoft Download Center.

#### Aktualizacje o wysokim priorytecie niezwiązane z zabezpieczeniami, dostępne w witrynach MU, WU oraz usługach WSUS

W tym miesiącu:

-   Firma Microsoft opublikowała trzy **niezwiązane z zabezpieczeniami** aktualizacje o wysokim priorytecie oraz dodatek Service Pack 1 dla pakietu Microsoft Office, dostępne w witrynie Microsoft Update (MU) i za pośrednictwem usług Windows Server Update Services (WSUS).
-   Firma Microsoft opublikowała trzy **niezwiązane z zabezpieczeniami** aktualizacje o wysokim priorytecie dla systemu Windows oraz dodatek Service Pack 1 dla programu Windows SharePoint Services 3.0, dostępne w witrynie Windows Update (WU) i za pośrednictwem usług WSUS.

Należy pamiętać, że informacje te dotyczą **wyłącznie** aktualizacji o wysokim priorytecie **niezwiązanych z zabezpieczeniami**, które dostępne są w witrynach Microsoft Update i Windows Update oraz poprzez usługi Windows Server Update Services i zostały opublikowane jednocześnie z podsumowaniem biuletynów zabezpieczeń. Informacje na temat aktualizacji **niezwiązanych z zabezpieczeniami**, które zostały opublikowane w innych dniach, **nie** są podawane.

#### Strategie i społeczność związane z zabezpieczeniami

**Strategie zarządzania aktualizacjami**

Na stronie [Security Guidance for Patch Management (j.ang.)](http://go.microsoft.com/fwlink/?linkid=21168) (Wskazówki z zakresu bezpieczeństwa dotyczące zarządzania poprawkami) znajdują się dodatkowe informacje o zalecanych przez firmę Microsoft najlepszych sposobach stosowania aktualizacji zabezpieczeń.

**Uzyskiwanie innych aktualizacji zabezpieczeń**

Aktualizacje dotyczące innych problemów związanych z zabezpieczeniami można uzyskać w następujących lokalizacjach:

-   Aktualizacje zabezpieczeń są dostępne w witrynie [Microsoft Download Center](http://www.microsoft.com/downloads/results.aspx?freetext=poprawka+zabezpiecze%c5%84&productid=&displaylang=pl). Najłatwiej je znaleźć, wyszukując wyrażenie „aktualizacja zabezpieczeń”.
-   Aktualizacje dla poszczególnych platform są dostępne w [witrynie sieci Web Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747).
-   Aktualizacje zabezpieczeń dostępne w tym miesiącu w witrynie Windows Update można otrzymać w witrynie Microsoft Download Center w postaci plików obrazu dysku CD zawierającego zabezpieczenia i aktualizacje krytyczne. Więcej informacji na ten temat można znaleźć w [artykule 913086 bazy wiedzy Microsoft Knowledge Base](http://support.microsoft.com/kb/913086).

**Społeczność IT Pro Security Community**

Dowiedz się, jak poprawić bezpieczeństwo i zoptymalizować infrastrukturę informatyczną oraz weź udział w dyskusjach dotyczących zabezpieczeń wraz z innymi specjalistami branży IT, odwiedzając witrynę sieci Web społeczności [IT Pro Security Community (j.ang.)](http://go.microsoft.com/fwlink/?linkid=21164).

#### Podziękowania

Firma Microsoft [dziękuje (j.ang.)](http://go.microsoft.com/fwlink/?linkid=21127) wymienionym poniżej organizacjom i osobom za współpracę w dziedzinie ochrony klientów:

-   Jun Mao z firmy [VeriSign iDefense Labs](http://labs.idefense.com/) za współpracę przy rozwiązywaniu problemu opisanego w biuletynie MS07-064
-   Peterowi Winter Smithowi z firmy [NGSSoftware](http://www.ngssoftware.com/) za współpracę przy rozwiązywaniu problemu opisanego w biuletynie MS07-064
-   Jung-Hyung Lee z firmy [AhnLab](http://global.ahnlab.com/) za współpracę przy zmianie zabezpieczeń w programie DirectX opisanych w biuletynie MS07-064
-   [Zero Day Initiative](http://www.zerodayinitiative.com/) za współpracę przy rozwiązywaniu problemu opisanego w biuletynie MS07-065
-   Venustech z [ADLABS](http://www.venustech.com.cn/) za współpracę przy rozwiązywaniu problemu opisanego w biuletynie MS07-065.
-   Thomasowi Garnierowi z firmy [SkyRecon](http://www.skyrecon.com/) za zgłoszenie problemu opisanego w biuletynie MS07-066
-   Ryanowi Smithowi z firmy [ISS X-Force](http://xforce.iss.net/) za współpracę przy rozwiązywaniu problemu opisanego w biuletynie MS07-068
-   Alexowi Wheelerowi z firmy [ISS X-Force](http://xforce.iss.net/) za współpracę przy rozwiązywaniu problemu opisanego w biuletynie MS07-068
-   Peterowi Vreugdenhilowi, współpracownikowi firmy [iDefense VCP](http://idefense.com/), za zgłoszenie problemu opisanego w biuletynie MS07-069
-   Anonimowemu analitykowi współpracującemu z firmami [TippingPoint](http://www.tippingpoint.com/) i [Zero Day Initiative](http://www.zerodayinitiative.com/), za zgłoszenie problemu opisanego w biuletynie MS07-69.
-   Samowi Thomasowi, współpracownikowi firm [TippingPoint](http://www.tippingpoint.com/) i [Zero Day Initiative,](http://www.zerodayinitiative.com/) za zgłoszenie problemu opisanego w biuletynie MS07-069
-   Peterowi Vreugdenhilowi, współpracownikowi firm [TippingPoint](http://www.tippingpoint.com/) i [Zero Day Initiative,](http://www.zerodayinitiative.com/) za zgłoszenie problemu opisanego w biuletynie MS07-069

#### Pomoc techniczna

-   Wymienione oprogramowanie zostało przetestowane w celu ustalenia, których wersji dotyczy problem. Dla pozostałych wersji upłynął okres pomocy technicznej. Aby zapoznać się z zasadami cyklu pomocy technicznej dotyczącymi używanej wersji oprogramowania, odwiedź [witrynę zasad cyklu pomocy technicznej firmy Microsoft](http://go.microsoft.com/fwlink/?linkid=21742).
-   Klienci mogą uzyskać pomoc techniczną w [Biurze Obsługi Klienta Microsoft](http://www.microsoft.com/poland/cok/default.mspx) pod numerem 0 801 802 000 (Opłata według stawek Twojego operatora) lub (0-22) 594 19 99 w godzinach od 9:00 do 17:00, od poniedziałku do piątku. Połączenia z działem pomocy technicznej związane z aktualizacjami zabezpieczeń są bezpłatne.
-   Klienci międzynarodowi mogą uzyskać pomoc w lokalnych przedstawicielstwach firmy Microsoft. Pomoc techniczna związana z aktualizacjami zabezpieczeń jest bezpłatna. Informacje o sposobie kontaktowania się z pomocą techniczną firmy Microsoft są dostępne w [międzynarodowej witrynie sieci Web pomocy i obsługi technicznej](http://go.microsoft.com/fwlink/?linkid=21155).

#### Zrzeczenie odpowiedzialności

Informacje w bazie wiedzy Microsoft Knowledge Base są dostarczane „tak jak są” bez jakiejkolwiek gwarancji. Firma Microsoft odrzuca wszelkie gwarancje, wyraźne i dorozumiane, w tym gwarancje dotyczące wartości handlowej i przydatności do określonego celu. Firma Microsoft Corporation ani jej dostawcy w żadnym wypadku nie ponoszą odpowiedzialności za jakiekolwiek szkody, w tym bezpośrednie, pośrednie, przypadkowe, wynikowe, utratę zysków handlowych lub szkody specjalne, nawet jeżeli firmę Microsoft Corporation lub jej dostawców powiadomiono o możliwości zaistnienia takich szkód. W niektórych stanach wyłączenie lub ograniczenie odpowiedzialności za straty wynikowe lub przypadkowe, a więc i powyższe ograniczenia, nie mają zastosowania.

#### Wersje

-   V1.0 (11 grudnia 2007 r.): Opublikowane podsumowanie biuletynów zabezpieczeń.
-   V1.2 (23 stycznia 2008 r.) :Zaktualizowano biuletyn, odzwierciedlając zmiany na liście oprogramowania dotkniętego usterką opisaną w biuletynie MS07-064

*Built at 2014-04-18T01:50:00Z-07:00*
