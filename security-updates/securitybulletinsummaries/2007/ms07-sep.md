---
TOCTitle: 'MS07-SEP'
Title: Microsoft Security Bulletin Summary for wrzesień 2007
ms:assetid: 'ms07-sep'
ms:contentKeyID: 61233083
ms:mtpsurl: 'https://technet.microsoft.com/pl-PL/library/ms07-sep(v=Security.10)'
---


Microsoft Security Bulletin Summary for wrzesień 2007
=====================================================

Opublikowano: 11 września 2007 | Zaktualizowano: 12 września 2007

**Wersja:** 1.1

Niniejsze podsumowanie biuletynów zabezpieczeń zawiera spis biuletynów za wrzesień 2007 r.

Z chwilą opublikowania biuletynów za wrzesień 2007 r. niniejsze podsumowanie biuletynów zastępuje powiadomienie o biuletynach zabezpieczeń wydane 6 września 2007 r. Aby uzyskać więcej informacji na temat usługi powiadamiania o biuletynach, zobacz [Powiadomienia o biuletynach zabezpieczeń firmy Microsoft (j.ang.)](http://technet.microsoft.com/security/bulletin/advance).

Aby dowiedzieć się, jak otrzymywać automatyczne powiadomienia o publikacji biuletynów zabezpieczeń firmy Microsoft, odwiedź stronę [Microsoft Technical Security Notifications (j.ang.)](http://go.microsoft.com/fwlink/?linkid=21163).

12 września 2007 r. o godz. 11:00 czasu Pacyfiku (godz. 20:00 czasu środkowoeuropejskiego) firma Microsoft udostępni emisję internetową, w której znajdą się odpowiedzi na pytania klientów dotyczące tych biuletynów (USA i Kanada). [Zarejestruj się, aby zobaczyć emisję internetową dotyczącą biuletynów zabezpieczeń za wrzesień (j.ang.)](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032344690&amp;eventcategory=4&amp;culture=en-us&amp;countrycode=us). Po tym dniu emisja internetowa będzie dostępna na żądanie. Aby uzyskać więcej informacji, zobacz [podsumowania biuletynów zabezpieczeń](http://technet.microsoft.com/security/bulletin/summary) i [emisje internetowe firmy Microsoft (j.ang.)](http://technet.microsoft.com/security/bulletin/summary).

Firma Microsoft udostępnia także informacje, dzięki którym klienci mogą ustalić priorytety dla aktualizacji zabezpieczeń w związku z niezwiązanymi z zabezpieczeniami aktualizacjami o wysokim priorytecie, które publikowane są w tym samym dniu, co comiesięczne aktualizacje zabezpieczeń. Zapoznaj się z sekcją **Inne informacje**.

### Informacje o biuletynie

#### Streszczenia

W bieżącym miesiącu opublikowano następujące biuletyny (w kolejności wskaźnika ważności):

Krytyczny (1)
-------------


| Identyfikator biuletynu           | Biuletyn zabezpieczeń firmy Microsoft MS07-051                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
|-----------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**               | [**Luka w zabezpieczeniach programu Microsoft Agent umożliwia zdalne wykonanie kodu (938827)**](http://technet.microsoft.com/security/bulletin/ms07-051)                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| **Streszczenie**                  | Niniejsza aktualizacja zabezpieczeń o krytycznym wskaźniku ważności pozwala usunąć lukę w zabezpieczeniach zgłoszoną przez użytkowników. W programie Microsoft Agent występuje luka umożliwiająca zdalne wykonanie kodu, wynikająca ze sposobu, w jaki obsługuje on niektóre specjalnie spreparowane adresy URL. Luka ta może umożliwić osobie atakującej zdalne wykonanie kodu w zagrożonym systemie. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi. |
| **Maksymalny wskaźnik ważności:** | [Krytyczny](http://technet.microsoft.com/security/bulletin/rating)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| **Wpływ luki**                    | Zdalne wykonanie kodu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Wykrywanie**                    | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Aktualizacja będzie wymagać ponownego uruchomienia komputera.                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Podlegające oprogramowanie**    | **Windows.** Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                                                                                                                                                                                                         |

Ważny <sup>[3]</sup>
-----------


| Identyfikator biuletynu           | Biuletyn zabezpieczeń firmy Microsoft MS07-052                                                                                                                                                                                                                                                                                                                                                                                |
|-----------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**               | [**Luka w zabezpieczeniach funkcji Crystal Reports for Visual Studio umożliwia zdalne wykonanie kodu (941522)**](http://technet.microsoft.com/security/bulletin/ms07-052)                                                                                                                                                                                                                                                     |
| **Streszczenie**                  | Ta ważna aktualizacja zabezpieczeń usuwa lukę w zabezpieczeniach, która została zgłoszona przez organizację publiczną. Luka ta może umożliwić zdalne wykonanie kodu, jeśli użytkownik otworzy specjalnie spreparowany plik RPT. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi. |
| **Maksymalny wskaźnik ważności:** | [Ważny](http://technet.microsoft.com/security/bulletin/rating)                                                                                                                                                                                                                                                                                                                                                                |
| **Wpływ luki**                    | Zdalne wykonanie kodu                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Wykrywanie**                    | Narzędzia Microsoft Baseline Security Analyzer oraz Enterprise Update Scan Tool mogą wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Aktualizacja może wymagać ponownego uruchomienia komputera.                                                                                                                                                                                                                 |
| **Podlegające oprogramowanie**    | **Visual Studio.** Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                            |

| Identyfikator biuletynu           | Biuletyn zabezpieczeń firmy Microsoft MS07-053                                                                                                                                                                                                                                                                                                                                                                  |
|-----------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**               | [**Luka w zabezpieczeniach programu Usługi Microsoft Windows dla UNIX umożliwia podniesienie poziomu uprawnień (939778)**](http://technet.microsoft.com/security/bulletin/ms07-053)                                                                                                                                                                                                                             |
| **Streszczenie**                  | Ta ważna aktualizacja zabezpieczeń usuwa jedną lukę w zabezpieczeniach zgłoszoną przez organizację publiczną. W programach Usługi Microsoft Windows dla UNIX 3.0, Usługi Microsoft Windows dla UNIX 3.5 oraz Podsystem aplikacji systemu UNIX występuje luka w zabezpieczeniach i uruchomienie w nich plików binarnych z określonym atrybutem setuid może pozwolić osobie atakującej na podniesienie uprawnień. |
| **Maksymalny wskaźnik ważności:** | [Ważny](http://technet.microsoft.com/security/bulletin/rating)                                                                                                                                                                                                                                                                                                                                                  |
| **Wpływ luki**                    | Podniesienie uprawnień                                                                                                                                                                                                                                                                                                                                                                                          |
| **Wykrywanie**                    | Narzędzia Microsoft Baseline Security Analyzer oraz Enterprise Update Scan Tool mogą wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Aktualizacja będzie wymagać ponownego uruchomienia komputera.                                                                                                                                                                                                 |
| **Podlegające oprogramowanie**    | **Usługi Microsoft Windows dla UNIX, Podsystem aplikacji systemu UNIX.** Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                        |

| Identyfikator biuletynu           | Biuletyn zabezpieczeń firmy Microsoft MS07-054                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
|-----------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**               | [**Luka w zabezpieczeniach programów MSN Messenger i Windows Live Messenger umożliwia zdalne wykonanie kodu (942099)**](http://technet.microsoft.com/security/bulletin/ms07-054)                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| **Streszczenie**                  | Niniejsza aktualizacja zabezpieczeń pozwala usunąć lukę w zabezpieczeniach programu MSN Messenger i Windows Live Messenger zgłoszoną przez organizację publiczną. Luka ta umożliwia zdalne wykonanie kodu po przyjęciu przez użytkownika zaproszenia do rozmowy z użyciem kamery internetowej lub wideorozmowy od osoby atakującej. Osoba atakująca, której uda się wykorzystać tę lukę, może uzyskać pełną kontrolę nad systemem podlegającym luce. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi. |
| **Maksymalny wskaźnik ważności:** | [Ważny](http://technet.microsoft.com/security/bulletin/rating)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| **Wpływ luki**                    | Zdalne wykonanie kodu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Wykrywanie**                    | Produkty te zawierają wbudowane mechanizmy automatycznego wykrywania i wdrażania aktualizacji. Ta aktualizacja może wymagać ponownego uruchomienia komputera.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| **Podlegające oprogramowanie**    | **MSN Messenger, Windows Live Messenger.** Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |

Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki
---------------------------------------------------------------------------------


**How do I use this table?**

Tabela ta pozwala odczytać informacje o aktualizacjach zabezpieczeń, których zainstalowanie może być konieczne. Należy przejrzeć informacje dla każdego wymienionego programu lub składnika oprogramowania w celu sprawdzenia, czy są wymagane aktualizacje zabezpieczeń. Dla każdego programu lub składnika oprogramowania wymienionego na liście podany jest wpływ luki oraz hiperłącze do dostępnej aktualizacji oprogramowania.

**Note** You may have to install several security updates for a single vulnerability. Przejrzyj całą kolumnę dla każdego wymienionego identyfikatora biuletynu, aby sprawdzić, jakie aktualizacje musisz zainstalować, w oparciu o programy bądź składniki zainstalowane w systemie.

**Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki**

 
<p> </p>
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
[**MS07-051**](http://technet.microsoft.com/security/bulletin/ms07-051)
</td>
<td style="border:1px solid black;">
[**MS07-052**](http://technet.microsoft.com/security/bulletin/ms07-052)
</td>
<td style="border:1px solid black;">
[**MS07-053**](http://technet.microsoft.com/security/bulletin/ms07-053)
</td>
<td style="border:1px solid black;">
[**MS07-054**](http://technet.microsoft.com/security/bulletin/ms07-054)
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
[**Ważny**](http://technet.microsoft.com/security/bulletin/rating)
</td>
<td style="border:1px solid black;">
[**Ważny**](http://technet.microsoft.com/security/bulletin/rating)
</td>
</tr>
<tr>
<th colspan="5">
System operacyjny Windows
</th>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 z dodatkiem Service Pack 4
</td>
<td style="border:1px solid black;">
[Krytyczny](http://www.microsoft.com/downloads/details.aspx?familyid=7cd248ed-d154-4dce-89ef-ceefd2700965)
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
Microsoft Windows XP z dodatkiem Service Pack 2
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
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition
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
<th colspan="5">
Składniki systemu operacyjnego Windows:
</th>
</tr>
<tr>
<td style="border:1px solid black;">
Program Usługi Microsoft Windows dla UNIX 3.0 w systemie Windows 2000 z dodatkiem Service Pack 4
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Ważny (j.ang.)](http://www.microsoft.com/downloads/details.aspx?familyid=557f89fc-c5d9-4405-9007-1654abf92277)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Program Usługi Microsoft Windows dla UNIX 3.5 w systemie Windows 2000 z dodatkiem Service Pack 4
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Ważny (j.ang.)](http://www.microsoft.com/downloads/details.aspx?familyid=70ae23c2-3ae8-4ea6-ba8d-8ac7e4f82663)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Program Usługi Microsoft Windows dla UNIX 3.0 w systemie Windows XP z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Ważny (j.ang.)](http://www.microsoft.com/downloads/details.aspx?familyid=557f89fc-c5d9-4405-9007-1654abf92277)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Program Usługi Microsoft Windows dla UNIX 3.5 w systemie Windows XP z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Ważny (j.ang.)](http://www.microsoft.com/downloads/details.aspx?familyid=70ae23c2-3ae8-4ea6-ba8d-8ac7e4f82663)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Program Usługi Microsoft Windows dla UNIX 3.0 w systemach Windows Server 2003 z dodatkiem Service Pack 1 i Windows Server 2003 z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Ważny (j.ang.)](http://www.microsoft.com/downloads/details.aspx?familyid=557f89fc-c5d9-4405-9007-1654abf92277)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Program Usługi Microsoft Windows dla UNIX 3.5 w systemach Windows Server 2003 z dodatkiem Service Pack 1 i Windows Server 2003 z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Ważny (j.ang.)](http://www.microsoft.com/downloads/details.aspx?familyid=70ae23c2-3ae8-4ea6-ba8d-8ac7e4f82663)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Program Podsystem aplikacji systemu UNIX w systemach Windows Server 2003 z dodatkiem Service Pack 1 i Windows Server 2003 z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Ważny](http://www.microsoft.com/downloads/details.aspx?familyid=8ab5cc43-0b9c-45eb-aa51-47568ab6ce3f&amp;displaylang=pl)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Program Podsystem aplikacji systemu UNIX w systemach Windows Server 2003 x64 Edition i Windows Server 2003 x64 Edition z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Ważny (j.ang.)](http://www.microsoft.com/downloads/details.aspx?familyid=1d21e3e8-b5f6-4044-9db6-054af836492b)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Program Podsystem aplikacji systemu UNIX w systemie Windows Vista
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Ważny (j.ang.)](http://www.microsoft.com/downloads/details.aspx?familyid=4d52e4f4-2888-42df-8163-85c648e65b29)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Program Podsystem aplikacji systemu UNIX w systemie Windows Vista x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Ważny (j.ang.)](http://www.microsoft.com/downloads/details.aspx?familyid=4be667cc-c239-480b-a9a0-939bcd27f0de)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<th colspan="5">
Narzędzia i platformy programistyczne
</th>
</tr>
<tr>
<td style="border:1px solid black;">
Visual Studio .NET 2002 z dodatkiem Service Pack 1  
(KB937057)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Ważny (j.ang.)](http://www.microsoft.com/downloads/details.aspx?familyid=2608c83b-e1b2-4449-9a0e-1e566aac3d76)**<sup>[2]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Visual Studio .NET 2003  
(KB937058)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Ważny (j.ang.)](http://www.microsoft.com/downloads/details.aspx?familyid=d612ad41-5a0d-4e13-99ea-d6a5589786d6)**<sup>[2]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Visual Studio .NET 2003 z dodatkiem Service Pack 1  
(KB937059)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Ważny (j.ang.)](http://www.microsoft.com/downloads/details.aspx?familyid=0b10b04b-932c-4bff-9cbc-b3eeb15064b1)**<sup>[2]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Visual Studio 2005  
(KB937060)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Ważny (j.ang.)](http://www.microsoft.com/downloads/details.aspx?familyid=21073cc2-919c-40df-8ebb-aa3db06050d2)**<sup>[2]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Visual Studio 2005 z dodatkiem Service Pack 1  
(KB937061)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Ważny (j.ang.)](http://www.microsoft.com/downloads/details.aspx?familyid=967d43c8-efba-4221-beb0-981e7deef33a)**<sup>[2]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<th colspan="5">
Inne programy, których dotyczy problem
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
MSN Messenger 6.2 w systemie Microsoft Windows 2000 z dodatkiem Service Pack 4
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Ważny](http://www.microsoft.com/downloads/details.aspx?displaylang=pl&familyid=cf49c56c-8b3e-4eae-9904-9505f47bed45)**<sup>[3]</sup>**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
MSN Messenger 7.0 w systemie Microsoft Windows 2000 z dodatkiem Service Pack 4
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Ważny](http://www.microsoft.com/downloads/details.aspx?displaylang=pl&familyid=cf49c56c-8b3e-4eae-9904-9505f47bed45)**<sup>[3]</sup>**
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
MSN Messenger 6.2 w systemie Windows XP z dodatkiem Service Pack 2, Windows XP Professional x64 Edition, Windows XP Professional x64 Edition z dodatkiem Service Pack 2, Windows Server 2003 z dodatkiem Service Pack 1, Windows Server 2003 z dodatkiem Service Pack 2, Windows Server 2003 x64 Edition, Windows Server 2003 x64 Edition z dodatkiem Service Pack 2, Windows Vista i Windows Vista x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Ważny](http://www.microsoft.com/downloads/details.aspx?displaylang=pl&familyid=d78f2ff1-79ea-4066-8ba0-ddbed94864fc)**<sup>[3]</sup>**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
MSN Messenger 7.0 w systemie Windows XP z dodatkiem Service Pack 2, Windows XP Professional x64 Edition, Windows XP Professional x64 Edition z dodatkiem Service Pack 2, Windows Server 2003 z dodatkiem Service Pack 1, Windows Server 2003 z dodatkiem Service Pack 2, Windows Server 2003 x64 Edition, Windows Server 2003 x64 Edition z dodatkiem Service Pack 2, Windows Vista i Windows Vista x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Ważny](http://www.microsoft.com/downloads/details.aspx?displaylang=pl&familyid=d78f2ff1-79ea-4066-8ba0-ddbed94864fc)**<sup>[3]</sup>**
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
MSN Messenger 7.5 w systemie Windows XP z dodatkiem Service Pack 2, Windows XP Professional x64 Edition, Windows XP Professional x64 Edition z dodatkiem Service Pack 2, Windows Server 2003 z dodatkiem Service Pack 1, Windows Server 2003 z dodatkiem Service Pack 2, Windows Server 2003 x64 Edition, Windows Server 2003 x64 Edition z dodatkiem Service Pack 2, Windows Vista i Windows Vista x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Ważny](http://www.microsoft.com/downloads/details.aspx?displaylang=pl&familyid=d78f2ff1-79ea-4066-8ba0-ddbed94864fc)**<sup>[3]</sup>**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Live Messenger 8.0 w systemie Windows XP z dodatkiem Service Pack 2, Windows XP Professional x64 Edition, Windows XP Professional x64 Edition z dodatkiem Service Pack 2, Windows Server 2003 z dodatkiem Service Pack 1, Windows Server 2003 z dodatkiem Service Pack 2, Windows Server 2003 x64 Edition, Windows Server 2003 x64 Edition z dodatkiem Service Pack 2, Windows Vista i Windows Vista x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Ważny](http://www.microsoft.com/downloads/details.aspx?displaylang=pl&familyid=d78f2ff1-79ea-4066-8ba0-ddbed94864fc)**<sup>[3]</sup>**
</td>
</tr>
</table>
 
**Uwagi**

**<sup>[1]</sup>** Dla tego systemu operacyjnego dostępna jest aktualizacja zabezpieczeń. Więcej informacji na temat oprogramowania lub składnika, którego dotyczy problem, znajduje się w tabeli oraz odpowiednim biuletynie zabezpieczeń.

**<sup>[2]</sup>** Problem nie dotyczy niektórych wydań tej wersji programu Visual Studio. Aby uzyskać listę wersji, których dotyczy problem, zapoznaj się z odpowiednim biuletynem zabezpieczeń.

**<sup>[3]</sup>** Można także przeprowadzić uaktualnienie online usługi MSN Messenger lub Windows Live Messenger. Szczegółowe informacje można znaleźć w odpowiednim biuletynie zabezpieczeń.

Narzędzia wykrywania i wdrażania oraz wskazówki
-----------------------------------------------


**Centrum zabezpieczeń**

Zarządzanie oprogramowaniem oraz aktualizacjami zabezpieczeń, które należy zainstalować na serwerach oraz komputerach stacjonarnych i przenośnych w organizacji. Więcej informacji można znaleźć w [Centrum TechNet Update Management Center (j.ang.)](http://go.microsoft.com/fwlink/?linkid=69903). Witryna [TechNet Security Center](http://www.microsoft.com/poland/technet/security/default.mspx) zawiera dodatkowe informacje na temat zabezpieczeń w produktach firmy Microsoft. Użytkownicy mogą także uzyskać dostęp do tych informacji w witrynie [Bezpieczeństwo w domu](http://www.microsoft.com/poland/athome/security/protect/windowsxpsp2/default.mspx), klikając łącze „Najnowsze aktualizacje zabezpieczeń”.

Aktualizacje zabezpieczeń dostępne są w witrynach [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747), [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130) i [Office Update](http://office.microsoft.com/pl-pl/officeupdate/default.aspx). Aktualizacje zabezpieczeń są także dostępne w [Centrum pobierania firmy Microsoft](http://www.microsoft.com/downloads/results.aspx?freetext=poprawka+zabezpiecze%c5%84&amp;productid=&amp;displaylang=pl). Najłatwiej je znaleźć, przeprowadzając wyszukiwanie wyrażenia „poprawka zabezpieczeń”. Aktualizacje zabezpieczeń można także pobierać z Wykazu Windows Update. Więcej informacji na temat Wykazu Windows Update można znaleźć w [artykule 323166 bazy wiedzy Microsoft Knowledge Base](http://support.microsoft.com/kb/323166).

**Porady dotyczące wykrywania i wdrażania**

Firma Microsoft opublikowała porady dotyczące wykrywania i wdrażania, odnoszące się do aktualizacji zabezpieczeń udostępnionych w tym miesiącu. Porady te będą również pomocne dla informatyków, wyjaśniając jak mogą oni wdrażać aktualizacje za pomocą różnych narzędzi, takich jak Windows Update, Microsoft Update, Office Update, Microsoft Baseline Security Analyzer (MBSA), Office Detection Tool, Microsoft Systems Management Server (SMS), Extended Security Update Inventory Tool i Enterprise Update Scan Tool (EST). Więcej informacji na ten temat można znaleźć w [artykule 910723 bazy wiedzy Microsoft Knowledge Base](http://support.microsoft.com/kb/910723).

**Narzędzie Microsoft Baseline Security Analyzer inarzędzia skanowaniaUpdate Scan Tool**

Narzędzie Microsoft Baseline Security Analyzer umożliwia administratorom skanowanie lokalnych i zdalnych systemów w poszukiwaniu brakujących aktualizacji zabezpieczeń oraz typowych błędów konfiguracji zabezpieczeń. Więcej informacji na temat narzędzia MBSA można znaleźć w witrynie sieci Web[Microsoft Baseline Security Analyzer](http://www.microsoft.com/poland/technet/security/tools/mbsa.mspx).

Gdy narzędzie MBSA 1.2.1 nie może obsłużyć wykrywania w odniesieniu do określonej aktualizacji zabezpieczeń, firma Microsoft publikuje dla tej aktualizacji wersję narzędzia Enterprise Update Scan Tool (EST). Więcej informacji na temat narzędzia EST można znaleźć w witrynie [Enterprise Update Scan Tool](http://support.microsoft.com/default.aspx?id=894193).

**Uwaga** Po 9 października 2007 r. używany przez narzędzie MBSA 1.2.1 plik MSSecure.XML nie będzie już aktualizowany. Po upływie tej daty do pliku MSSecure.XML używanego przez narzędzie MBSA 1.2.1 nie będą dodawane nowe aktualizacje zabezpieczeń. Nie będą również publikowane nowe wersje narzędzia Enterprise Scan Tool. Więcej informacji można znaleźć w witrynie sieci Web[Microsoft Baseline Security Analyzer](http://www.microsoft.com/poland/technet/security/tools/mbsa.mspx).

**Windows Server Update Services**

Korzystając z programu Windows Server Update Services (WSUS), administratorzy mogą szybko i niezawodnie wdrożyć najnowsze aktualizacje krytyczne i aktualizacje zabezpieczeń przeznaczonych dla systemu operacyjnego Windows 2000 i nowszych, pakietu Office XP i nowszych, programu Exchange Server 2003 oraz SQL Server 2000 w systemie operacyjnym Windows 2000 i nowszych.

Więcej informacji na temat sposobu wdrażania tej aktualizacji zabezpieczeń za pomocą programu Windows Server Update Services można znaleźć w [witrynie sieci Web programu Windows Server Update Services (j.ang.)](http://go.microsoft.com/fwlink/?linkid=50120).

**Program Systems Management Server**

Program Systems Management Server (SMS) jest przeznaczonym dla przedsiębiorstw i w znacznym stopniu konfigurowalnym rozwiązaniem służącym do zarządzania aktualizacjami. Program SMS umożliwia administratorom znalezienie komputerów z systemem Windows, na których należy zainstalować aktualizację zabezpieczeń, a także przeprowadzić kontrolowane wdrożenie tych aktualizacji w całym przedsiębiorstwie, w minimalnym stopniu zakłócając przy tym pracę użytkowników końcowych. Więcej informacji na temat możliwości wykorzystania przez administratorów programu SMS 2003 do wdrażania aktualizacji zabezpieczeń można znaleźć [w witrynie sieci Web zarządzania poprawkami zabezpieczeń programu SMS 2003 (j.ang.)](http://go.microsoft.com/fwlink/?linkid=22939). Użytkownicy programu SMS 2.0 mogą także skorzystać z dodatku [Software Updates Services Feature Pack (j.ang.)](http://go.microsoft.com/fwlink/?linkid=33340) ułatwiającego wdrożenie aktualizacji zabezpieczeń. Więcej informacji na temat programu SMS można znaleźć w witrynie sieci Web [Microsoft Systems Management Server (j.ang.)](http://go.microsoft.com/fwlink/?linkid=21158).

**Uwaga** Program SMS zapewnia obsługę rozwiązań zawartych w biuletynach zabezpieczeń dzięki narzędziom Microsoft Baseline Security Analyzer oraz Microsoft Office Detection Tool. Narzędzia te mogą nie wykrywać wszystkich aktualizacji oprogramowania. W takich przypadkach administratorzy mogą wykorzystywać dostępne w programie SMS funkcje zarządzania zasobami do przyporządkowania poszczególnych aktualizacji określonym systemom. Aby uzyskać więcej informacji dotyczących tej procedury, zobacz [Wdrażanie aktualizacji oprogramowania za pomocą funkcji Software Distribution programu SMS (j.ang.)](http://go.microsoft.com/fwlink/?linkid=33341). Niektóre aktualizacje oprogramowania wymagają od użytkownika uprawnień administratora po ponownym uruchomieniu systemu. Do zainstalowania tych aktualizacji administratorzy mogą użyć narzędzia Elevated Rights Deployment Tool (dostępnego w dodatkach [SMS 2003 Administration Feature Pack (j.ang.)](http://go.microsoft.com/fwlink/?linkid=33387) oraz [SMS 2.0 Administration Feature Pack (j.ang.)](http://go.microsoft.com/fwlink/?linkid=21161).

### Inne informacje:

#### Narzędzie Microsoft Windows do usuwania złośliwego oprogramowania

Firma Microsoft opublikowała zaktualizowaną wersję narzędzia Microsoft Windows Malicious Software Removal Tool, która dostępna jest w witrynach sieci Web Windows Update i Microsoft Update, poprzez usługi Windows Server Update Services i w witrynie Centrum pobierania.

#### Aktualizacje o wysokim priorytecie niezwiązane z zabezpieczeniami w witrynach MU, WU oraz usługach WSUS

W tym miesiącu:

-   Firma Microsoft opublikowała cztery **niezwiązane z zabezpieczeniami** aktualizacje o wysokim priorytecie, które dostępne są w witrynie Microsoft Update (MU) i poprzez usługi Windows Server Update Services (WSUS).
-   Firma Microsoft opublikowała dwie **niezwiązane z zabezpieczeniami** aktualizacje o wysokim priorytecie dla systemu Windows, które dostępne są w witrynie Windows Update (MU).

Należy pamiętać, że informacje te dotyczą **wyłącznie** aktualizacji o wysokim priorytecie **niezwiązanych z zabezpieczeniami**, które dostępne są w witrynach Microsoft Update i Windows Update oraz poprzez usługi Windows Server Update Services i zostały opublikowane jednocześnie z podsumowaniem biuletynów zabezpieczeń. Informacje na temat aktualizacji **niezwiązanych z zabezpieczeniami**, które zostały opublikowane w innych dniach, **nie** są podawane.

#### Strategie i społeczność związane z zabezpieczeniami

**Strategie zarządzania aktualizacjami**

Na stronie [Security Guidance for Patch Management (j.ang.)](http://go.microsoft.com/fwlink/?linkid=21168) (Wskazówki z zakresu bezpieczeństwa dotyczące zarządzania poprawkami) znajdują się dodatkowe informacje o zalecanych przez firmę Microsoft najlepszych sposobach stosowania aktualizacji zabezpieczeń.

**Uzyskiwanie innych aktualizacji zabezpieczeń**

Aktualizacje dotyczące innych problemów związanych z zabezpieczeniami można uzyskać w następujących lokalizacjach:

-   Aktualizacje zabezpieczeń są dostępne w [Centrum pobierania firmy Microsoft](http://www.microsoft.com/downloads/results.aspx?freetext=poprawka+zabezpiecze%c5%84&amp;productid=&amp;displaylang=pl). Najłatwiej je znaleźć, przeprowadzając wyszukiwanie wyrażenia „poprawka zabezpieczeń”.
-   Aktualizacje dla poszczególnych platform są dostępne w [witrynie sieci Web Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747).
-   Aktualizacje zabezpieczeń dostępne w tym miesiącu w witrynie Windows Update można otrzymać w witrynie Centrum pobierania w postaci plików obrazu dysku CD zawierającego zabezpieczenia i aktualizacje krytyczne. Więcej informacji na ten temat można znaleźć w [artykule 913086 bazy wiedzy Microsoft Knowledge Base](http://support.microsoft.com/kb/913086).

**Społeczność IT Pro Security Community**

Dowiedz się, jak poprawić bezpieczeństwo i zoptymalizować infrastrukturę informatyczną oraz weź udział w dyskusjach dotyczących zabezpieczeń wraz z innymi specjalistami branży IT, odwiedzając witrynę sieci Web społeczności [IT Pro Security Community (j.ang.)](http://go.microsoft.com/fwlink/?linkid=21164).

#### Podziękowania

Firma Microsoft [dziękuje (j.ang.)](http://go.microsoft.com/fwlink/?linkid=21127) wymienionym poniżej organizacjom i osobom za współpracę w dziedzinie ochrony klientów:

-   Zespołowi Vulnerability Research z firmy [Assurent Secure Technologies](http://www.assurent.com/) za zgłoszenie problemu opisanego w biuletynie [MS07-051](http://technet.microsoft.com/security/bulletin/ms07-051).
-   Yamata Li z firmy [Palo Alto Networks](http://www.paloaltonetworks.com/) za zgłoszenie problemu opisanego w biuletynie [MS07-051](http://technet.microsoft.com/security/bulletin/ms07-051).
-   Anonimowemu analitykowi współpracującemu z firmą [iDefense VCP,](http://labs.idefense.com/) za zgłoszenie problemu opisanego w biuletynie [MS07-051](http://technet.microsoft.com/security/bulletin/ms07-051).
-   Brianowi A. Reiterowi z firmy WolfeReiter za współpracę z firmą Microsoft przy rozwiązywaniu problemu zgłoszonego w biuletynie [MS07-053](http://technet.microsoft.com/security/bulletin/ms07-053).
-   Woo Shi z zespołu [team 509](http://www.team509.com/) za zgłoszenie problemu opisanego w biuletynie [MS07-054](http://technet.microsoft.com/security/bulletin/ms07-054).

#### Pomoc techniczna

-   Wymienione oprogramowanie zostało przetestowane w celu ustalenia, których wersji dotyczy problem. Dla pozostałych wersji upłynął okres pomocy technicznej. Aby zapoznać się z zasadami cyklu pomocy technicznej dotyczącymi używanej wersji oprogramowania, odwiedź [witrynę zasad cyklu pomocy technicznej firmy Microsoft](http://go.microsoft.com/fwlink/?linkid=21742).
-   Klienci mogą uzyskać pomoc techniczną w [Biurze Obsługi Klienta Microsoft](http://support.microsoft.com/contactus/?ws=support) pod numerem 0 801 802 000 (Opłata według stawek Twojego operatora) lub (0-22) 594 19 99 w godzinach od 9:00 do 17:00, od poniedziałku do piątku. Połączenia z działem pomocy technicznej związane z aktualizacjami zabezpieczeń są bezpłatne.
-   Klienci międzynarodowi mogą uzyskać pomoc w lokalnych przedstawicielstwach firmy Microsoft. Pomoc techniczna związana z aktualizacjami zabezpieczeń jest bezpłatna. Informacje o sposobie kontaktowania się z pomocą techniczną firmy Microsoft są dostępne w [międzynarodowej witrynie sieci Web pomocy i obsługi technicznej (j.ang.)](http://go.microsoft.com/fwlink/?linkid=21155).

#### Zrzeczenie odpowiedzialności

Informacje w bazie wiedzy Microsoft Knowledge Base są dostarczane „tak jak są” bez jakiejkolwiek gwarancji. Firma Microsoft odrzuca wszelkie gwarancje, wyraźne i dorozumiane, w tym gwarancje dotyczące wartości handlowej i przydatności do określonego celu. Firma Microsoft Corporation ani jej dostawcy w żadnym wypadku nie ponoszą odpowiedzialności za jakiekolwiek szkody, w tym bezpośrednie, pośrednie, przypadkowe, wynikowe, utratę zysków handlowych lub szkody specjalne, nawet jeżeli firmę Microsoft Corporation lub jej dostawców powiadomiono o możliwości zaistnienia takich szkód. W niektórych stanach wyłączenie lub ograniczenie odpowiedzialności za straty wynikowe lub przypadkowe, a więc i powyższe ograniczenia, nie mają zastosowania.

#### Wersje

-   Wersja 1.0 (11 września 2007 r.): Opublikowane podsumowanie biuletynów zabezpieczeń.
-   Wersja 1.1 (12 września 2007 r.): Dodano informację o konieczności ponownego uruchomienia i łącza do pobrania dla biuletynu MS07-054.

*Built at 2014-04-18T01:50:00Z-07:00*
