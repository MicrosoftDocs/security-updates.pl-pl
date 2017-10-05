---
TOCTitle: 'MS07-JUL'
Title: Microsoft Security Bulletin Summary for lipiec 2007
ms:assetid: 'ms07-jul'
ms:contentKeyID: 61233077
ms:mtpsurl: 'https://technet.microsoft.com/pl-PL/library/ms07-jul(v=Security.10)'
---

Security Bulletin Summary

Microsoft Security Bulletin Summary for lipiec 2007
===================================================

Opublikowano: 10 lipca 2007 | Zaktualizowano: 25 marca 2008

**Wersja:** 2.0

Niniejsze podsumowanie biuletynów zabezpieczeń zawiera spis biuletynów za lipiec 2007 r.

Z chwilą opublikowania biuletynów za lipiec 2007 r. niniejsze podsumowanie biuletynów zastępuje powiadomienie o biuletynach zabezpieczeń wydane 5 lipca 2007 r. Aby uzyskać więcej informacji na temat usługi powiadamiania o biuletynach, zobacz [Powiadomienia o biuletynach zabezpieczeń firmy Microsoft (j.ang.)](http://technet.microsoft.com/security/bulletin/advance).

Aby dowiedzieć się, jak otrzymywać automatyczne powiadomienia o publikacji biuletynów zabezpieczeń firmy Microsoft, odwiedź stronę [Microsoft Technical Security Notifications (j. ang.)](http://go.microsoft.com/fwlink/?linkid=21163).

11 lipca 2007 r. o godz. 11:00 czasu Pacyfiku (godz. 20:00 czasu środkowoeuropejskiego) firma Microsoft udostępni emisję internetową, w której znajdą się odpowiedzi na pytania klientów dotyczące tych biuletynów (USA i Kanada). [Zarejestruj się, aby zobaczyć emisję internetową dotyczącą biuletynów zabezpieczeń za lipiec (j. ang.)](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032343783&eventcategory=4&culture=en-us&countrycode=us). Po tym dniu emisja internetowa będzie dostępna na żądanie. Aby uzyskać więcej informacji, zobacz [Podsumowania biuletynów zabezpieczeń](http://technet.microsoft.com/security/bulletin/summary) i [emisje internetowe (j.ang.)](http://technet.microsoft.com/security/bulletin/summary) firmy Microsoft.

Firma Microsoft udostępnia także informacje, dzięki którym klienci mogą ustalić priorytety dla aktualizacji zabezpieczeń w związku z niezwiązanymi z zabezpieczeniami aktualizacjami o wysokim priorytecie, które publikowane są w tym samym dniu, co comiesięczne aktualizacje zabezpieczeń. Zapoznaj się z sekcją **Inne informacje**.

### Informacje o biuletynie

#### Streszczenia

W bieżącym miesiącu opublikowano następujące biuletyny (w kolejności wskaźnika ważności):

Krytyczny (3)
-------------

<span></span>
| Identyfikator biuletynu           | Biuletyn zabezpieczeń firmy Microsoft MS07-036                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
|-----------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**               | [**Luki w zabezpieczeniach programu Microsoft Excel umożliwiają zdalne wykonanie kodu (936542)**](http://technet.microsoft.com/security/bulletin/ms07-036)                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Streszczenie**                  | Ta krytyczna aktualizacja usuwa lukę w zabezpieczeniach, która została zgłoszona przez organizację publiczną, oraz dwie luki w zabezpieczeniach, które zostały zgłoszone przez użytkowników, a także inne problemy związane z zabezpieczeniami rozpoznane w trakcie dochodzenia. Luki te mogą umożliwić zdalne wykonanie kodu, jeśli użytkownik otworzy specjalnie spreparowany plik programu Excel. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi. |
| **Maksymalny wskaźnik ważności:** | [Krytyczny](http://technet.microsoft.com/security/bulletin/rating)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Wpływ luki**                    | Zdalne wykonanie kodu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Wykrywanie**                    | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Ta aktualizacja nie wymaga ponownego uruchomienia komputera.                                                                                                                                                                                                                                                                                                                                                                                                                      |
| **Podlegające oprogramowanie**    | **Office, Excel**. Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                                                                                                                                                                                                 |

| Identyfikator biuletynu           | Biuletyn zabezpieczeń firmy Microsoft MS07-039                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
|-----------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**               | [**Luka w zabezpieczeniach usługi Active Directory w systemie Windows umożliwia zdalne wykonanie kodu (926122)**](http://technet.microsoft.com/security/bulletin/ms07-039)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Streszczenie**                  | Niniejsza aktualizacja zabezpieczeń o krytycznym wskaźniku ważności pozwala usunąć zgłoszoną przez użytkowników lukę w zabezpieczeniach wdrożeń usługi Active Directory w systemach Windows 2000 Server i Windows Server 2003, która umożliwia zdalne wykonanie kodu lub przeprowadzenie ataku typu „odmowa usługi”. Ataki z próbami wykorzystania tej luki prawdopodobnie skończyłyby się sytuacją typu „odmowa usługi”. Zdalne wykonanie kodu może być jednak możliwe. Aby wykorzystać tę lukę w zabezpieczeniach w systemie Windows Server 2003, osoba atakująca musi dysponować prawidłowymi poświadczeniami logowania. Osoba atakująca, której uda się wykorzystać tę lukę, może uzyskać pełną kontrolę nad systemem, którego dotyczy luka. Osoba taka może wówczas instalować programy, przeglądać, zmieniać i usuwać dane oraz tworzyć nowe konta. |
| **Maksymalny wskaźnik ważności:** | [Krytyczny](http://technet.microsoft.com/security/bulletin/rating)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Wpływ luki**                    | Zdalne wykonanie kodu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| **Wykrywanie**                    | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Aktualizacja będzie wymagać ponownego uruchomienia komputera.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| **Podlegające oprogramowanie**    | **Windows**. Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |

| Identyfikator biuletynu           | Biuletyn zabezpieczeń firmy Microsoft MS07-040                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
|-----------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**               | [**Luki w zabezpieczeniach systemu .NET Framework umożliwiają zdalne wykonanie kodu (931212)**](http://technet.microsoft.com/security/bulletin/ms07-040)                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Streszczenie**                  | Ta aktualizacja usuwa trzy luki w zabezpieczeniach, które zostały zgłoszone przez użytkowników. Dwie z nich umożliwiają zdalne wykonanie kodu na komputerach klienckich z zainstalowanym systemem .NET Framework, a trzecia luka umożliwia ujawnienie informacji na serwerach sieci Web z systemem ASP.NET. We wszystkich przypadkach zdalnego wykonania kodu użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi. |
| **Maksymalny wskaźnik ważności:** | [Krytyczny](http://technet.microsoft.com/security/bulletin/rating)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **Wpływ luki**                    | Zdalne wykonanie kodu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Wykrywanie**                    | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Aktualizacja będzie wymagać ponownego uruchomienia komputera.                                                                                                                                                                                                                                                                                                                                                                              |
| **Podlegające oprogramowanie**    | **.NET Framework**. Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                                                                                                                                                         |

Ważny (2)
---------

<span></span>

| Identyfikator biuletynu           | Biuletyn zabezpieczeń firmy Microsoft MS07-037                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
|-----------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**               | [**Luka w zabezpieczeniach programu Publisher z pakietu Microsoft Office umożliwia zdalne wykonanie kodu (936548)**](http://technet.microsoft.com/security/bulletin/ms07-037)                                                                                                                                                                                                                                                                                                                                                                                        |
| **Streszczenie**                  | Ta ważna aktualizacja zabezpieczeń usuwa jedną lukę w zabezpieczeniach, która została zgłoszona przez organizację publiczną. Ta luka w zabezpieczeniach umożliwia zdalne wykonanie kodu, gdy użytkownik wyświetli specjalnie spreparowany plik programu Microsoft Office Publisher. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi. Aby luka ta została wykorzystana, użytkownik musi wykonywać odpowiednie czynności. |
| **Maksymalny wskaźnik ważności:** | [Ważny](http://technet.microsoft.com/security/bulletin/rating)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Wpływ luki**                    | Zdalne wykonanie kodu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Wykrywanie**                    | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Ta aktualizacja nie wymaga ponownego uruchomienia komputera.                                                                                                                                                                                                                                                                                                                                                                                        |
| **Podlegające oprogramowanie**    | **Office, Publisher**. Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                                                                                                                                                               |

| Identyfikator biuletynu           | Biuletyn zabezpieczeń firmy Microsoft MS07-041                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
|-----------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**               | [**Luka w zabezpieczeniach usług Microsoft Internet Information Services umożliwia zdalne wykonanie kodu (939373)**](http://technet.microsoft.com/security/bulletin/ms07-041)                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **Streszczenie**                  | Ta ważna aktualizacja zabezpieczeń usuwa lukę w zabezpieczeniach zgłoszoną przez użytkowników. Luka ta umożliwia zdalne wykonanie kodu, gdy osoba atakująca wyśle specjalnie spreparowane żądanie URL do strony sieci Web obsługiwanej przez program Internet Information Services (IIS) 5.1 w systemie Windows XP Professional z dodatkiem Service Pack 2. Program IIS 5.1 nie jest składnikiem instalacji domyślnej systemu Windows XP Professional z dodatkiem Service Pack 2. Osoba atakująca, której uda się wykorzystać tę lukę, może uzyskać pełną kontrolę nad systemem, którego dotyczy luka. |
| **Maksymalny wskaźnik ważności:** | [Ważny](http://technet.microsoft.com/security/bulletin/rating)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Wpływ luki**                    | Zdalne wykonanie kodu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **Wykrywanie**                    | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Aktualizacja będzie wymagać ponownego uruchomienia komputera.                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Podlegające oprogramowanie**    | **Windows XP Professional**. Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                                                                                                                                                                                           |

Średni (1)
----------

<span></span>
| Identyfikator biuletynu           | Biuletyn zabezpieczeń firmy Microsoft MS07-038                                                                                                                                                                                                                                                                         |
|-----------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**               | [**Luka w zabezpieczeniach zapory systemu Windows Vista umożliwia ujawnienie informacji (935807)**](http://technet.microsoft.com/security/bulletin/ms07-038)                                                                                                                                                           |
| **Streszczenie**                  | Niniejsza aktualizacja zabezpieczeń o umiarkowanym wskaźniku ważności pozwala usunąć lukę w zabezpieczeniach zgłoszoną przez użytkowników. Luka ta umożliwia dostęp przychodzącemu, niepożądanemu ruchowi sieciowemu do interfejsu sieci. Osoba atakująca może zebrać informacje na temat hosta, którego dotyczy luka. |
| **Maksymalny wskaźnik ważności:** | [Umiarkowany](http://technet.microsoft.com/security/bulletin/rating)                                                                                                                                                                                                                                                   |
| **Wpływ luki**                    | Ujawnienie informacji                                                                                                                                                                                                                                                                                                  |
| **Wykrywanie**                    | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Aktualizacja będzie wymagać ponownego uruchomienia komputera.                                                                                                                                         |
| **Podlegające oprogramowanie**    | **Windows** **Vista**. Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                 |

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
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS07-036**](http://technet.microsoft.com/security/bulletin/ms07-036)
</td>
<td style="border:1px solid black;">
[**MS07-037**](http://technet.microsoft.com/security/bulletin/ms07-037)
</td>
<td style="border:1px solid black;">
[**MS07-038**](http://technet.microsoft.com/security/bulletin/ms07-038)
</td>
<td style="border:1px solid black;">
[**MS07-039**](http://technet.microsoft.com/security/bulletin/ms07-039)
</td>
<td style="border:1px solid black;">
[**MS07-040**](http://technet.microsoft.com/security/bulletin/ms07-040)
</td>
<td style="border:1px solid black;">
[**MS07-041**](http://technet.microsoft.com/security/bulletin/ms07-041)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Maksymalny wskaźnik ważności:**
</td>
<td style="border:1px solid black;">
[**Krytyczny**](http://technet.microsoft.com/security/bulletin/rating)
</td>
<td style="border:1px solid black;">
[**Ważny**](http://technet.microsoft.com/security/bulletin/rating)
</td>
<td style="border:1px solid black;">
[**Umiarkowany**](http://technet.microsoft.com/security/bulletin/rating)
</td>
<td style="border:1px solid black;">
[**Krytyczny**](http://technet.microsoft.com/security/bulletin/rating)
</td>
<td style="border:1px solid black;">
[**Krytyczny**](http://technet.microsoft.com/security/bulletin/rating)
</td>
<td style="border:1px solid black;">
[**Ważny**](http://technet.microsoft.com/security/bulletin/rating)
</td>
</tr>
<tr>
<th colspan="7">
Programy systemu Windows, których dotyczy problem
</th>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 2000 Service Pack 4
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
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 2000 Server z dodatkiem Service Pack 4
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Krytyczny](http://www.microsoft.com/downloads/details.aspx?familyid=812e62c5-6e19-4b3b-8a10-861b871e1b41&displaylang=pl)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP z dodatkiem Service Pack 2
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
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional z dodatkiem Service Pack 2
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
[Ważny](http://www.microsoft.com/downloads/details.aspx?familyid=fccbfe90-f838-47df-8310-352e2fb47132&displaylang=pl)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows XP Professional x64 Edition
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
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition z dodatkiem Service Pack 2
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
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 z dodatkiem Service Pack 1
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Ważny](http://www.microsoft.com/downloads/details.aspx?familyid=28e84603-8159-4429-aaff-a1020531e84f&displaylang=pl)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Ważny](http://www.microsoft.com/downloads/details.aspx?familyid=28e84603-8159-4429-aaff-a1020531e84f&displaylang=pl)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Ważny (j.ang.)](http://www.microsoft.com/downloads/details.aspx?familyid=107902f9-be94-457f-a936-519efbd64779)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Ważny (j.ang.)](http://www.microsoft.com/downloads/details.aspx?familyid=107902f9-be94-457f-a936-519efbd64779)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 z dodatkiem SP1 dla systemów z procesorem Itanium
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Ważny (j.ang.)](http://www.microsoft.com/downloads/details.aspx?familyid=e5e5b425-fe7d-49d5-973f-f3fd7a1e04eb)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Ważny (j.ang.)](http://www.microsoft.com/downloads/details.aspx?familyid=e5e5b425-fe7d-49d5-973f-f3fd7a1e04eb)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Umiarkowany](http://www.microsoft.com/downloads/details.aspx?familyid=e9b64746-6afa-4a30-833d-e058e000c821&displaylang=pl)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista z dodatkiem Service Pack 1
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
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Umiarkowany](http://www.microsoft.com/downloads/details.aspx?familyid=0df5d190-3ad7-42d5-8629-43c47ec450cb&displaylang=pl)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition z dodatkiem Service Pack 1
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
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008
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
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 dla systemów z procesorem Itanium
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
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 x64 Edition
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
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<th colspan="7">
Składniki systemu Windows, których dotyczy problem:
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft .NET Framework 1.0  
(KB928367)
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
[Krytyczny](http://www.microsoft.com/downloads/details.aspx?familyid=91d7afe4-069b-4ce8-976e-9a01345a8603&displaylang=pl)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft .NET Framework 1.0  
(KB930494)
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
[Krytyczny (j.ang.)](http://www.microsoft.com/downloads/details.aspx?familyid=829a2c5b-11ec-4ed7-91ab-6961034147bc)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft .NET Framework 1.1  
(KB928366)
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
[Krytyczny](http://www.microsoft.com/downloads/details.aspx?familyid=281fb2cd-c715-4f05-a01f-0455d2d9ebfb&displaylang=pl)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft .NET Framework 1.1  
(KB933854)
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
[Krytyczny](http://www.microsoft.com/downloads/details.aspx?familyid=2495e656-1e0a-4b83-90da-821e68067a71&displaylang=pl)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft .NET Framework 1.1  
(KB929729)
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
[Krytyczny](http://www.microsoft.com/downloads/details.aspx?familyid=7eea368d-7b82-4583-8537-30351718a4e9&displaylang=pl)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft .NET Framework 2.0  
(KB928365)
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
[Krytyczny](http://www.microsoft.com/downloads/details.aspx?familyid=ba3ceb78-8e1b-4c38-adfd-e8bc95ae548d&displaylang=pl)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft .NET Framework 2.0  
(KB929916)
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
[Krytyczny](http://www.microsoft.com/downloads/details.aspx?familyid=cbc9f3cf-c3c3-45c4-82e3-e11398bc2cd2&displaylang=pl)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<th colspan="7">
Oprogramowanie pakietu Office, którego dotyczy problem
</th>
</tr>
<tr>
<td style="border:1px solid black;">
Excel 2000 z dodatkiem Service Pack 3
</td>
<td style="border:1px solid black;">
[Krytyczny](http://www.microsoft.com/downloads/details.aspx?familyid=83d94d8e-dda6-4d74-b40d-476c2f0a3af4&displaylang=pl)
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
Excel 2003 z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Ważny](http://www.microsoft.com/downloads/details.aspx?familyid=9d93c0ce-5124-4234-ba84-3c27005e010f&displaylang=pl)
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
Przeglądarka Excel 2003
</td>
<td style="border:1px solid black;">
[Ważny](http://www.microsoft.com/downloads/details.aspx?familyid=11f42977-8828-494a-a183-d1aba827b708&displaylang=pl)
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
Excel 2007
</td>
<td style="border:1px solid black;">
[Ważny](http://www.microsoft.com/downloads/details.aspx?familyid=9ab28283-0320-4527-b033-5e80ef32cd34&displaylang=pl)
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
Pakiet zgodności dla systemu Microsoft Office dla formatów plików programów Word, Excel i PowerPoint 2007
</td>
<td style="border:1px solid black;">
[Ważny](http://www.microsoft.com/downloads/details.aspx?familyid=e592ae5b-09ac-4f5b-b457-a54c9850ad4a&displaylang=pl)
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
Publisher 2007
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Ważny](http://www.microsoft.com/downloads/details.aspx?familyid=25d272e7-f2dd-4342-92be-7ebc2e770b44&displaylang=pl)
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
</table>
 
**Uwagi**

**<sup>[1]</sup>** Dla tego systemu operacyjnego dostępna jest aktualizacja zabezpieczeń. Więcej informacji na temat oprogramowania lub składnika, którego dotyczy problem, znajduje się w tabeli oraz odpowiednim biuletynie zabezpieczeń.** **

** **

Narzędzia wykrywania i wdrażania oraz wskazówki
-----------------------------------------------

<span></span>
**Centrum zabezpieczeń**

Zarządzanie oprogramowaniem oraz aktualizacjami zabezpieczeń, które należy zainstalować na serwerach oraz komputerach stacjonarnych i przenośnych w organizacji. Więcej informacji można znaleźć w [Centrum TechNet Update Management Center (j.ang.)](http://go.microsoft.com/fwlink/?linkid=69903). Witryna [TechNet Security Center](http://www.microsoft.com/poland/technet/security/default.mspx) zawiera dodatkowe informacje na temat zabezpieczeń w produktach firmy Microsoft. Użytkownicy mogą także uzyskać dostęp do tych informacji w witrynie [Bezpieczeństwo w domu](http://www.microsoft.com/poland/athome/security/protect/windowsxpsp2/default.mspx), klikając łącze „Najnowsze aktualizacje zabezpieczeń”.

Aktualizacje zabezpieczeń dostępne są w witrynach [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747), [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130) i [Office Update](http://office.microsoft.com/pl-pl/officeupdate/default.aspx). Aktualizacje zabezpieczeń są także dostępne w witrynie [Microsoft Download Center](http://www.microsoft.com/downloads/results.aspx?freetext=poprawka+zabezpiecze%c5%84&productid=&displaylang=pl). Najłatwiej je znaleźć, przeprowadzając wyszukiwanie wyrażenia „poprawka zabezpieczeń”. Aktualizacje zabezpieczeń można także pobierać z Wykazu Windows Update. Więcej informacji na temat Wykazu Windows Update można znaleźć w [artykule 323166 bazy wiedzy Microsoft Knowledge Base](http://support.microsoft.com/kb/323166).

**Porady dotyczące wykrywania i wdrażania**

Firma Microsoft opublikowała porady dotyczące wykrywania i wdrażania, odnoszące się do aktualizacji zabezpieczeń udostępnionych w tym miesiącu. Porady te będą również pomocne dla informatyków, wyjaśniając jak mogą oni wdrażać aktualizacje za pomocą różnych narzędzi, takich jak Windows Update, Microsoft Update, Office Update, Microsoft Baseline Security Analyzer (MBSA), Office Detection Tool, Microsoft Systems Management Server (SMS), Extended Security Update Inventory Tool i Enterprise Update Scan Tool (EST). Więcej informacji na ten temat można znaleźć w [artykule 910723 bazy wiedzy Microsoft Knowledge Base](http://support.microsoft.com/kb/910723).

**Narzędzie Microsoft Baseline Security Analyzer i** **narzędzia skanowania Enterprise** **Update Scan Tool**

Narzędzie Microsoft Baseline Security Analyzer umożliwia administratorom skanowanie lokalnych i zdalnych systemów w poszukiwaniu brakujących aktualizacji zabezpieczeń oraz typowych błędów konfiguracji zabezpieczeń. Więcej informacji na temat narzędzia MBSA można znaleźć w witrynie sieci Web[Microsoft Baseline Security Analyzer](http://www.microsoft.com/poland/technet/security/tools/mbsa.mspx).

Gdy narzędzie MBSA 1.2.1 nie może obsłużyć wykrywania w odniesieniu do określonej aktualizacji zabezpieczeń, firma Microsoft publikuje dla tej aktualizacji wersję narzędzia Enterprise Update Scan Tool (EST). Więcej informacji na temat narzędzia EST można znaleźć w witrynie [Enterprise Update Scan Tool](http://support.microsoft.com/default.aspx?id=894193).

**Uwaga** Po 9 października 2007 r. używany przez narzędzie MBSA 1.2.1 plik MSSecure.XML nie będzie już aktualizowany. Po upływie tej daty do pliku MSSecure.XML używanego przez narzędzie MBSA 1.2.1 nie będą dodawane nowe aktualizacje zabezpieczeń. Nie będą również publikowane nowe wersje narzędzia Enterprise Scan Tool. Więcej informacji można znaleźć w witrynie sieci Web[Microsoft Baseline Security Analyzer](http://www.microsoft.com/poland/technet/security/tools/mbsa.mspx).

**Usługi Software Update Services**

Usługi Microsoft Software Update Services (SUS) umożliwiają administratorom szybkie i niezawodne wdrażanie najnowszych aktualizacji krytycznych i aktualizacji zabezpieczeń na serwerach działających w systemach Windows 2000 oraz Windows Server 2003, a także na komputerach stacjonarnych z systemami Windows 2000 Professional lub Windows XP Professional.

Więcej informacji na temat sposobu wdrażania tej aktualizacji zabezpieczeń za pomocą usług Software Update Services można znaleźć w [witrynie sieci Web usług Software Update Services (j.ang.)](http://go.microsoft.com/fwlink/?linkid=21133).

**Windows Server Update Services**

Korzystając z programu Windows Server Update Services (WSUS), administratorzy mogą szybko i niezawodnie wdrożyć najnowsze aktualizacje krytyczne i aktualizacje zabezpieczeń przeznaczonych dla systemu operacyjnego Windows 2000 i nowszych, pakietu Office XP i nowszych, programu Exchange Server 2003 oraz SQL Server 2000 w systemie operacyjnym Windows 2000 i nowszych.

Więcej informacji na temat sposobu wdrażania tej aktualizacji zabezpieczeń za pomocą programu Windows Server Update Services można znaleźć w [witrynie sieci Web programu Windows Server Update Services (j.ang.)](http://go.microsoft.com/fwlink/?linkid=50120).

**Program Systems Management Server**

Program Systems Management Server (SMS) jest przeznaczonym dla przedsiębiorstw i w znacznym stopniu konfigurowalnym rozwiązaniem służącym do zarządzania aktualizacjami. Program SMS umożliwia administratorom znalezienie komputerów z systemem Windows, na których należy zainstalować aktualizację zabezpieczeń, a także przeprowadzić kontrolowane wdrożenie tych aktualizacji w całym przedsiębiorstwie, w minimalnym stopniu zakłócając przy tym pracę użytkowników końcowych. Więcej informacji na temat możliwości wykorzystania przez administratorów programu SMS 2003 do wdrażania aktualizacji zabezpieczeń można znaleźć [w witrynie sieci Web zarządzania poprawkami zabezpieczeń programu SMS 2003 (j.ang.)](http://go.microsoft.com/fwlink/?linkid=22939). Użytkownicy programu SMS 2.0 mogą także skorzystać z dodatku [Software Updates Services Feature Pack (j.ang.)](http://go.microsoft.com/fwlink/?linkid=33340) ułatwiającego wdrożenie aktualizacji zabezpieczeń. Więcej informacji na temat programu SMS można znaleźć w witrynie sieci Web [Microsoft Systems Management Server (j.ang.)](http://go.microsoft.com/fwlink/?linkid=21158).

**Uwaga** Program SMS zapewnia obsługę rozwiązań zawartych w biuletynach zabezpieczeń dzięki narzędziom Microsoft Baseline Security Analyzer oraz Microsoft Office Detection Tool. Narzędzia te mogą nie wykrywać wszystkich aktualizacji oprogramowania. W takich przypadkach administratorzy mogą wykorzystywać dostępne w programie SMS funkcje zarządzania zasobami do przyporządkowania poszczególnych aktualizacji określonym systemom. Aby uzyskać więcej informacji dotyczących tej procedury, zobacz [Wdrażanie aktualizacji oprogramowania za pomocą funkcji Software Distribution programu SMS (j.ang.)](http://go.microsoft.com/fwlink/?linkid=33341). Niektóre aktualizacje oprogramowania wymagają od użytkownika uprawnień administratora po ponownym uruchomieniu systemu. Do zainstalowania tych aktualizacji administratorzy mogą użyć narzędzia Elevated Rights Deployment Tool (dostępnego w dodatkach [SMS 2003 Administration Feature Pack (j.ang.)](http://go.microsoft.com/fwlink/?linkid=33387) oraz [SMS 2.0 Administration Feature Pack (j.ang.)](http://go.microsoft.com/fwlink/?linkid=21161)).

### Inne informacje:

#### Narzędzie Microsoft Windows do usuwania złośliwego oprogramowania

Firma Microsoft opublikowała zaktualizowaną wersję narzędzia Microsoft Windows Malicious Software Removal Tool, która dostępna jest w witrynach sieci Web Windows Update i Microsoft Update, poprzez usługi Windows Server Update Services i w witrynie Microsoft Download Center.

Należy pamiętać, że narzędzie to **nie** jest rozpowszechniane za pośrednictwem usług Software Update Services (SUS).

#### Aktualizacje o wysokim priorytecie niezwiązane z zabezpieczeniami w witrynach MU, WU oraz usługach WSUS i SUS

W tym miesiącu:

-   Firma Microsoft opublikowała cztery **niezwiązane z zabezpieczeniami** aktualizacje o wysokim priorytecie, które dostępne są w witrynie Microsoft Update (MU) i poprzez usługi Windows Server Update Services (WSUS).
-   Firma Microsoft opublikowała jedną **niezwiązaną z zabezpieczeniami** aktualizację o wysokim priorytecie dla systemu Windows, która dostępna jest w witrynie Windows Update (MU) i poprzez usługi Software Update Services (SUS).

Należy pamiętać, że informacje te dotyczą **wyłącznie** aktualizacji o wysokim priorytecie **niezwiązanych z zabezpieczeniami**, które dostępne są w witrynach Microsoft Update i Windows Update oraz poprzez usługi Windows Server Update Services i Software Update Services i zostały opublikowane jednocześnie z podsumowaniem biuletynów zabezpieczeń. Informacje na temat aktualizacji **niezwiązanych z zabezpieczeniami**, które zostały opublikowane w innych dniach, **nie** są podawane.

#### Strategie i społeczność związane z zabezpieczeniami

**Strategie zarządzania aktualizacjami**

Na stronie [Security Guidance for Patch Management (j.ang.)](http://go.microsoft.com/fwlink/?linkid=21168) (Wskazówki z zakresu bezpieczeństwa dotyczące zarządzania poprawkami) znajdują się dodatkowe informacje o zalecanych przez firmę Microsoft najlepszych sposobach stosowania aktualizacji zabezpieczeń.

**Uzyskiwanie innych aktualizacji zabezpieczeń**

Aktualizacje dotyczące innych problemów związanych z zabezpieczeniami można uzyskać w następujących lokalizacjach:

-   Aktualizacje zabezpieczeń są dostępne w witrynie [Microsoft Download Center](http://www.microsoft.com/downloads/results.aspx?freetext=poprawka+zabezpiecze%c5%84&productid=&displaylang=pl). Najłatwiej je znaleźć, przeprowadzając wyszukiwanie wyrażenia „poprawka zabezpieczeń”.
-   Aktualizacje dla poszczególnych platform są dostępne w [witrynie sieci Web Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747).
-   Aktualizacje zabezpieczeń dostępne w tym miesiącu w witrynie Windows Update można otrzymać w witrynie Microsoft Download Center w postaci plików obrazu dysku CD zawierającego zabezpieczenia i aktualizacje krytyczne. Więcej informacji na ten temat można znaleźć w [artykule 913086 bazy wiedzy Microsoft Knowledge Base](http://support.microsoft.com/kb/913086).

**Społeczność IT Pro Security Community**

Dowiedz się, jak poprawić bezpieczeństwo i zoptymalizować infrastrukturę informatyczną oraz weź udział w dyskusjach dotyczących zabezpieczeń wraz z innymi specjalistami branży IT, odwiedzając witrynę sieci Web społeczności [IT Pro Security Community (j.ang.)](http://go.microsoft.com/fwlink/?linkid=21164).

#### Podziękowania

Firma Microsoft [dziękuje (j.ang.)](http://go.microsoft.com/fwlink/?linkid=21127) wymienionym poniżej organizacjom i osobom za współpracę w dziedzinie ochrony klientów:

-   Dinisowi Cruzowi z firmy [OWASP](http://www.owasp.org/) za zgłoszenie problemu opisanego w biuletynie [MS07-040](http://technet.microsoft.com/security/bulletin/ms07-040).
-   Paulowi Craigowi z firmy [Security Assessment](http://www.smsiinc.com/) za zgłoszenie problemu opisanego w biuletynie [MS07-040](http://technet.microsoft.com/security/bulletin/ms07-040).
-   Jeroenowi Frijters z firmy [Sumatra](http://www.sumatra.nl/) za zgłoszenie problemu opisanego w biuletynie [MS07-040](http://technet.microsoft.com/security/bulletin/ms07-040).
-   [ProCheckUp](http://www.procheckup.com/), współpracującemu z firmą [UK CPNI](http://www.cpni.gov.uk/), za pierwsze zgłoszenie problemu opisanego w biuletynie [MS07-040](http://technet.microsoft.com/security/bulletin/ms07-040).
-   Ferruh T. Mavituna z firmy [Portcullis Computer Security Ltd.](http://www.portcullis-security.com/) za współpracę z firmą Microsoft i dostarczenie dodatkowych informacji na temat problemu opisanego w biuletynie [MS07-040](http://technet.microsoft.com/security/bulletin/ms07-040).
-   Johannesowi Gumbelowi z firmy [TrueSec](http://www.truesec.com/) za współpracę z firmą Microsoft i dostarczenie dodatkowych informacji na temat problemu opisanego w biuletynie [MS07-040](http://technet.microsoft.com/security/bulletin/ms07-040).
-   Peterowi Winterowi-Smithowi z firmy [NGSSoftware](http://www.nextgenss.com/) za zgłoszenie problemu opisanego w biuletynie [MS07-039](http://technet.microsoft.com/security/bulletin/ms07-039).
-   Neel Mehta z [IBM Internet Security Systems x-Force](http://xforce.iss.net/) za zgłoszenie problemu opisanego w biuletynie [MS07-039](http://technet.microsoft.com/security/bulletin/ms07-039).
-   Firmie [eEye](http://www.eeye.com/) za zgłoszenie problemu opisanego w biuletynie [MS07-037](http://technet.microsoft.com/security/bulletin/ms07-037).
-   Jimowi Hoagland i Olli'emu Whitehouse'owi z firmy [Symantec](http://www.symantec.com/) za zgłoszenie problemu opisanego w biuletynie [MS07-038](http://technet.microsoft.com/security/bulletin/ms07-038).
-   Jonathanowi Afek i Adi Sharabani z firmy [Watchfire](http://www.watchfire.com/) za współpracę z firmą Microsoft i dostarczenie dodatkowych informacji na temat problemu opisanego w biuletynie [MS07-041](http://technet.microsoft.com/security/bulletin/ms07-041).
-   Peterowi Winter-Smith z firmy [NGSSoftware](http://www.nextgenss.com/) za współpracę z firmą Microsoft i dostarczenie dodatkowych informacji na temat problemu opisanego w biuletynie [MS07-041](http://technet.microsoft.com/security/bulletin/ms07-041).

#### Pomoc techniczna

-   Wymienione oprogramowanie zostało przetestowane w celu ustalenia, których wersji dotyczy problem. Dla pozostałych wersji upłynął okres pomocy technicznej. Aby zapoznać się z zasadami cyklu pomocy technicznej dotyczącymi używanej wersji oprogramowania, odwiedź [witrynę zasad cyklu pomocy technicznej firmy Microsoft](http://go.microsoft.com/fwlink/?linkid=21742).
-   Klienci mogą uzyskać pomoc techniczną w [Biurze Obsługi Klienta Microsoft](http://support.microsoft.com/contactus/?ws=support) pod numerem 0 801 802 000 (Opłata według stawek Twojego operatora) lub (0-22) 594 19 99 w godzinach od 9:00 do 17:00, od poniedziałku do piątku. Połączenia z działem pomocy technicznej związane z aktualizacjami zabezpieczeń są bezpłatne.
-   Klienci międzynarodowi mogą uzyskać pomoc w lokalnych przedstawicielstwach firmy Microsoft. Pomoc techniczna związana z aktualizacjami zabezpieczeń jest bezpłatna. Informacje o sposobie kontaktowania się z pomocą techniczną firmy Microsoft są dostępne w [międzynarodowej witrynie sieci Web pomocy i obsługi technicznej (j.ang.)](http://go.microsoft.com/fwlink/?linkid=21155).

#### Zrzeczenie odpowiedzialności

Informacje w bazie wiedzy Microsoft Knowledge Base są dostarczane „tak jak są” bez jakiejkolwiek gwarancji. Firma Microsoft odrzuca wszelkie gwarancje, wyraźne i dorozumiane, w tym gwarancje dotyczące wartości handlowej i przydatności do określonego celu. Firma Microsoft Corporation ani jej dostawcy w żadnym wypadku nie ponoszą odpowiedzialności za jakiekolwiek szkody, w tym bezpośrednie, pośrednie, przypadkowe, wynikowe, utratę zysków handlowych lub szkody specjalne, nawet jeżeli firmę Microsoft Corporation lub jej dostawców powiadomiono o możliwości zaistnienia takich szkód. W niektórych stanach wyłączenie lub ograniczenie odpowiedzialności za straty wynikowe lub przypadkowe, a więc i powyższe ograniczenia, nie mają zastosowania.

#### Wersje

-   V1.0 (10 lipca 2007 r.): Opublikowane podsumowanie biuletynów zabezpieczeń.
-   V2.0 (25 marca 2008 r.): Do tabeli „Programy, których dotyczy problem” dodano systemy Windows Vista z dodatkiem Service Pack 1, Windows Vista x64 Edition z dodatkiem Service Pack 1, Windows Server 2008, Windows Server 2008 dla systemów z procesorem Itanium i Windows Server 2008 x64 Edition.

*Built at 2014-04-18T01:50:00Z-07:00*
