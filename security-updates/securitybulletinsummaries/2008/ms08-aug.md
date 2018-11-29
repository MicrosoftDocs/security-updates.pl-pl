---
TOCTitle: 'MS08-AUG'
Title: 'Podsumowanie biuletynów zabezpieczeń firmy Microsoft za sierpień 2008 r.'
ms:assetid: 'ms08-aug'
ms:contentKeyID: 61233085
ms:mtpsurl: 'https://technet.microsoft.com/pl-PL/library/ms08-aug(v=Security.10)'
---
Podsumowanie biuletynów zabezpieczeń firmy Microsoft za sierpień 2008 r.
========================================================================

Opublikowano: 12 sierpnia 2008 | Zaktualizowano: 20 sierpnia 2008

**Wersja:** 2.0

Niniejsze podsumowanie biuletynów zabezpieczeń zawiera spis biuletynów za sierpień 2008 r.

Z chwilą opublikowania biuletynów za sierpień 2008 r. niniejsze podsumowanie biuletynów zastępuje powiadomienie o biuletynach zabezpieczeń wydane 7 sierpnia 2008 r. Aby uzyskać więcej informacji na temat usługi powiadamiania o biuletynach, zobacz [Powiadomienia o biuletynach zabezpieczeń firmy Microsoft (j. ang.)](http://technet.microsoft.com/security/bulletin/advance).

Aby dowiedzieć się, jak otrzymywać automatyczne powiadomienia o publikacji biuletynów zabezpieczeń firmy Microsoft, odwiedź stronę [Microsoft Technical Security Notifications](http://go.microsoft.com/fwlink/?linkid=21163).

13 sierpnia 2008 r. o godz. 11:00 czasu Pacyfiku (godz. 20:00 czasu środkowoeuropejskiego) firma Microsoft udostępni emisję internetową, w której znajdą się odpowiedzi na pytania klientów dotyczące tych biuletynów (USA i Kanada). [Zarejestruj się, aby zobaczyć emisję internetową dotyczącą biuletynów zabezpieczeń za sierpień](http://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032374631&culture=en-us). Po tym dniu emisja internetowa będzie dostępna na żądanie. Aby uzyskać więcej informacji, zobacz [Podsumowania biuletynów zabezpieczeń i emisje internetowe firmy Microsoft](http://technet.microsoft.com/security/bulletin/summary).

Firma Microsoft udostępnia także informacje, dzięki którym klienci mogą ustalić priorytety dla aktualizacji zabezpieczeń w związku z niezwiązanymi z zabezpieczeniami aktualizacjami o wysokim priorytecie, które publikowane są w tym samym dniu, co comiesięczne aktualizacje zabezpieczeń. Zapoznaj się z sekcją **Inne informacje**.

### Informacje o biuletynie

#### Streszczenia

W bieżącym miesiącu opublikowano następujące biuletyny (w kolejności wskaźnika ważności):

Krytyczny (6)
-------------

<span></span>

| Identyfikator biuletynu               | Biuletyn zabezpieczeń firmy Microsoft MS08-046                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
|---------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**                   | [**Luka w systemie zarządzania kolorami obrazu w systemie Microsoft Windows umożliwia zdalne wykonanie kodu (952954)**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-046.mspx)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Streszczenie**                      | Niniejsza aktualizacja pozwala usunąć zgłoszoną przez użytkowników lukę w zabezpieczeniach systemu zarządzania kolorami obrazu (ICM) firmy Microsoft, która mogłoby pozwolić na zdalne wykonanie kodu w kontekście bieżącego użytkownika. Jeśli użytkownik jest zalogowany jako administrator, osoba atakująca, która pomyślnie wykorzysta tę lukę, może uzyskać pełną kontrolę nad systemem, którego ta luka dotyczy. Osoba taka może wówczas instalować programy, przeglądać, zmieniać i usuwać dane oraz tworzyć nowe konta z pełnymi uprawnieniami. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi. |
| **Maksymalny wskaźnik ważności:**     | [Krytyczny](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| **Wpływ luki**                        | Zdalne wykonanie kodu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Wykrywanie**                        | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Aktualizacja wymaga ponownego uruchomienia systemu.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **Programy, których dotyczy problem** | **Microsoft Windows.** Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |

| Identyfikator biuletynu               | Biuletyn zabezpieczeń firmy Microsoft MS08-045                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
|---------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**                   | [**Zbiorcza aktualizacja zabezpieczeń dla programu Internet Explorer (953838)**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-045.mspx)                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Streszczenie**                      | Niniejsza aktualizacja zabezpieczeń usuwa pięć luk w zabezpieczeniach, które zostały zgłoszone przez użytkowników, oraz jedną lukę w zabezpieczeniach, która została zgłoszona przez organizację publiczną. Każda z tych luk może pozwolić na zdalne wykonanie kodu, jeśli użytkownik wyświetli specjalnie spreparowaną stronę sieci Web przy użyciu programu Internet Explorer. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi. |
| **Maksymalny wskaźnik ważności:**     | [Krytyczny](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| **Wpływ luki**                        | Zdalne wykonanie kodu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **Wykrywanie**                        | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Aktualizacja wymaga ponownego uruchomienia systemu.                                                                                                                                                                                                                                                                                                                                                                                                           |
| **Programy, których dotyczy problem** | **Microsoft Windows, Internet Explorer.** Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                                                                                                                                                      |

| Identyfikator biuletynu               | Biuletyn zabezpieczeń firmy Microsoft MS08-041                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
|---------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**                   | [**Luka w formancie ActiveX przeglądarki Snapshot Viewer dla programu Microsoft Access umożliwia zdalne wykonanie kodu (955617)**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-041.mspx)                                                                                                                                                                                                                                                                                                       |
| **Streszczenie**                      | Niniejsza aktualizacja zabezpieczeń usuwa zgłoszoną przez użytkowników lukę w zabezpieczeniach formantu ActiveX przeglądarki Snapshot Viewer dla programu Microsoft Access. Osoba atakująca może wykorzystać tę lukę poprzez utworzenie specjalnie spreparowanej strony sieci Web. Gdy użytkownik odwiedza taką stronę sieci Web, luka w zabezpieczeniach może pozwolić na zdalne wykonanie kodu. Osoba atakująca, której uda się wykorzystać tę lukę, może uzyskać takie same uprawnienia, jak zalogowany użytkownik. |
| **Maksymalny wskaźnik ważności:**     | [Krytyczny](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Wpływ luki**                        | Zdalne wykonanie kodu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **Wykrywanie**                        | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Ta aktualizacja nie wymaga ponownego uruchomienia komputera.                                                                                                                                                                                                                                                                                                                                          |
| **Programy, których dotyczy problem** | **Microsoft Office.** Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                                                                                                                  |

| Identyfikator biuletynu               | Biuletyn zabezpieczeń firmy Microsoft MS08-043                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
|---------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**                   | [**Luki w zabezpieczeniach programu Microsoft Excel umożliwiają zdalne wykonanie kodu (954066)**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-043.mspx)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Streszczenie**                      | Niniejsza aktualizacja zabezpieczeń pozwala usunąć cztery luki w zabezpieczeniach programu Microsoft Office Excel zgłoszone przez osoby prywatne, które mogą pozwolić na zdalne wykonanie kodu, jeśli użytkownik otworzy specjalnie spreparowany plik programu Excel. Osoba atakująca, której uda się wykorzystać te luki, może uzyskać pełną kontrolę nad atakowanym systemem. Osoba taka może wówczas instalować programy, przeglądać, zmieniać i usuwać dane oraz tworzyć nowe konta z pełnymi uprawnieniami. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi. |
| **Maksymalny wskaźnik ważności:**     | [Krytyczny](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| **Wpływ luki**                        | Zdalne wykonanie kodu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **Wykrywanie**                        | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Ta aktualizacja nie wymaga ponownego uruchomienia komputera.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **Programy, których dotyczy problem** | **Microsoft Office.** Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |

| Identyfikator biuletynu               | Biuletyn zabezpieczeń firmy Microsoft MS08-051                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
|---------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**                   | [**Luki w zabezpieczeniach programu Microsoft PowerPoint umożliwiają zdalne wykonanie kodu (949785)**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-051.mspx)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Streszczenie**                      | Ta aktualizacja zabezpieczeń usuwa trzy zgłoszone przez użytkowników luki w zabezpieczeniach programu Microsoft Office PowerPoint i apletu Podgląd programu Microsoft Office PowerPoint, które umożliwiają zdalne wykonanie kodu, gdy użytkownik otworzy specjalnie spreparowany plik programu PowerPoint. Osoba atakująca, której uda się wykorzystać jedną z tych luk, może uzyskać pełną kontrolę nad zagrożonym systemem. Osoba taka może wówczas instalować programy, przeglądać, zmieniać i usuwać dane oraz tworzyć nowe konta z pełnymi uprawnieniami. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi. |
| **Maksymalny wskaźnik ważności:**     | [Krytyczny](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Wpływ luki**                        | Zdalne wykonanie kodu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Wykrywanie**                        | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Ta aktualizacja nie wymaga ponownego uruchomienia komputera.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Programy, których dotyczy problem** | **Microsoft Office.** Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |

| Identyfikator biuletynu               | Biuletyn zabezpieczeń firmy Microsoft MS08-044                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
|---------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**                   | [**Luki w zabezpieczeniach filtrów pakietu Microsoft Office umożliwiają zdalne wykonanie kodu (924090)**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-044.mspx)                                                                                                                                                                                                                                                                                                                  |
| **Streszczenie**                      | Niniejsza aktualizacja zabezpieczeń o wskaźniku ważności „krytyczny” pozwala usunąć pięć luk w zabezpieczeniach zgłoszonych przez użytkowników. Omawiane luki mogą pozwolić na zdalne wykonanie kodu, jeśli użytkownik wyświetli specjalnie spreparowany plik obrazu przy użyciu pakietu Microsoft Office. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi. |
| **Maksymalny wskaźnik ważności:**     | [Krytyczny](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Wpływ luki**                        | Zdalne wykonanie kodu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Wykrywanie**                        | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Ta aktualizacja nie wymaga ponownego uruchomienia komputera.                                                                                                                                                                                                                                                                                                                            |
| **Programy, których dotyczy problem** | **Microsoft Office.** Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                                                                                                    |

Ważny (5)
---------

<span></span>

| Identyfikator biuletynu               | Biuletyn zabezpieczeń firmy Microsoft MS08-047                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
|---------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**                   | [**Luka w zabezpieczeniach przetwarzania zasad protokołu IPsec umożliwia ujawnienie informacji (953733)**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-047.mspx)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| **Streszczenie**                      | Niniejsza aktualizacja zabezpieczeń usuwa zgłoszoną przez użytkowników lukę w sposobie stosowania pewnych reguł protokołu IPSec systemu Windows. Ta luka może spowodować, że systemy będą ignorować zasady protokołu IPSec i przesyłać dane w sieci w postaci czystego tekstu. To z kolei umożliwi ujawnienie informacji, które powinny być zaszyfrowane podczas przesyłania w sieci. Osoba atakująca monitorująca ruch sieciowy może wyświetlić i zmodyfikować zawartość pakietów. Należy zauważyć, że luka ta nie pozwala atakującemu na bezpośrednie wykonanie kodu lub podniesienie poziomu swoich uprawnień. Może zostać wykorzystana do zebrania użytecznych informacji celem dalszego spenetrowania systemu lub sieci, których dotyczy luka. |
| **Maksymalny wskaźnik ważności:**     | [Ważny](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Wpływ luki**                        | Ujawnienie informacji                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Wykrywanie**                        | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Aktualizacja wymaga ponownego uruchomienia systemu.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Programy, których dotyczy problem** | **Microsoft Windows.** Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |

| Identyfikator biuletynu               | Biuletyn zabezpieczeń firmy Microsoft MS08-049                                                                                                                                                                                                                                                                                                                                                                                             |
|---------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**                   | [**Luki w zabezpieczeniach Systemu zdarzeń umożliwiają zdalne wykonanie kodu (950974)**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-049.mspx)                                                                                                                                                                                                                                                                     |
| **Streszczenie**                      | Niniejsza aktualizacja usuwa dwie zgłoszone przez użytkowników luki w zabezpieczeniach usługi System zdarzeń systemu Microsoft Windows, które umożliwiają zdalne wykonanie kodu. Osoba atakująca, której uda się wykorzystać te luki, może uzyskać pełną kontrolę nad atakowanym systemem. Osoba taka może wówczas instalować programy, przeglądać, zmieniać i usuwać dane oraz tworzyć nowe konta z pełnymi uprawnieniami administratora. |
| **Maksymalny wskaźnik ważności:**     | [Ważny](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                      |
| **Wpływ luki**                        | Zdalne wykonanie kodu                                                                                                                                                                                                                                                                                                                                                                                                                      |
| **Wykrywanie**                        | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Aktualizacja wymaga ponownego uruchomienia systemu.                                                                                                                                                                                                                                                                       |
| **Programy, których dotyczy problem** | **Microsoft Windows.** Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                                     |

| Identyfikator biuletynu               | Biuletyn zabezpieczeń firmy Microsoft MS08-048                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
|---------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**                   | [**Aktualizacja zabezpieczeń dla programów Outlook Express i Poczta systemu Windows (951066)**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-048.mspx)                                                                                                                                                                                                                                                                                                                            |
| **Streszczenie**                      | Ta aktualizacja zabezpieczeń usuwa lukę w zabezpieczeniach programu Outlook Express i Poczty systemu Windows zgłoszoną przez użytkowników. Omawiana luka może umożliwić ujawnienie informacji, jeśli użytkownik wyświetli specjalnie spreparowaną stronę sieci Web przy użyciu programu Internet Explorer. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi. |
| **Maksymalny wskaźnik ważności:**     | [Ważny](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Wpływ luki**                        | Ujawnienie informacji                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Wykrywanie**                        | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Aktualizacja może wymagać ponownego uruchomienia komputera.                                                                                                                                                                                                                                                                                                                             |
| **Programy, których dotyczy problem** | **Microsoft Windows, Outlook Express, Poczta systemu Windows.** Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                                                          |

| Identyfikator biuletynu               | Biuletyn zabezpieczeń firmy Microsoft MS08-050                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
|---------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**                   | [**Luka w zabezpieczeniach programu Windows Messenger umożliwia ujawnienie informacji (955702)**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-050.mspx)                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Streszczenie**                      | Niniejsza aktualizacja zabezpieczeń usuwa lukę w obsługiwanych wersjach programu Windows Messenger, która została zgłoszona przez organizację publiczną. W wyniku wykorzystania tej luki procedura obsługi skryptów formantu ActiveX umożliwia ujawnienie informacji w kontekście użytkownika zalogowanego. Osoba atakująca może zmienić stan użytkownika zalogowanego, uzyskać informacje kontaktowe oraz zainicjować sesje rozmów audio i wideo bez jego wiedzy. Osoba atakująca może również przechwycić identyfikator logowania użytkownika i zdalnie zalogować się do klienta programu Messenger, podszywając się pod tego użytkownika. |
| **Maksymalny wskaźnik ważności:**     | [Ważny](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Wpływ luki**                        | Ujawnienie informacji                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Wykrywanie**                        | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji tylko w przypadku programu Windows Messenger 4.7 w obsługiwanych wersjach systemu Windows XP. Aktualizacja wymaga ponownego uruchomienia systemu.                                                                                                                                                                                                                                                                                                                                                                            |
| **Programy, których dotyczy problem** | **Microsoft Windows, Windows Messenger.** Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |

| Identyfikator biuletynu               | Biuletyn zabezpieczeń firmy Microsoft MS08-042                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
|---------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**                   | [**Luka w zabezpieczeniach programu Microsoft Word umożliwia zdalne wykonanie kodu (955048)**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-042.mspx)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Streszczenie**                      | Ta aktualizacja usuwa zgłoszoną przez organizacje publiczne lukę w zabezpieczeniach programu Microsoft Word. Luka ta może umożliwić zdalne wykonanie kodu, jeśli użytkownik otworzy specjalnie spreparowany plik programu Word. Osoba atakująca, której uda się wykorzystać tę lukę, może uzyskać pełną kontrolę nad systemem, którego dotyczy luka. Osoba taka może wówczas instalować programy, przeglądać, zmieniać i usuwać dane oraz tworzyć nowe konta z pełnymi uprawnieniami. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi. |
| **Maksymalny wskaźnik ważności:**     | [Ważny](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Wpływ luki**                        | Zdalne wykonanie kodu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Wykrywanie**                        | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Ta aktualizacja nie wymaga ponownego uruchomienia komputera.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Programy, których dotyczy problem** | **Microsoft Office.** Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |

Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki
---------------------------------------------------------------------------------

<span></span>
**W jaki sposób korzystać z tej tabeli?**

Tabela ta pozwala odczytać informacje o aktualizacjach zabezpieczeń, których zainstalowanie może być konieczne. Należy przejrzeć informacje dla każdego wymienionego programu lub składnika oprogramowania w celu sprawdzenia, czy są wymagane aktualizacje zabezpieczeń. Jeśli program lub składnik znajduje się na liście, dostępne jest łącze prowadzące do aktualizacji oprogramowania i podana jest informacja o wskaźniku ważności tej aktualizacji.

**Uwaga** Konieczne może być zainstalowanie kilku aktualizacji zabezpieczeń dotyczących jednej luki. Przejrzyj całą kolumnę dla każdego wymienionego identyfikatora biuletynu, aby sprawdzić, jakie aktualizacje musisz zainstalować, w oparciu o programy bądź składniki zainstalowane w systemie.

#### System operacyjny Windows

 
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
</tr>
<tr>
<th colspan="7">
Microsoft Windows 2000
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS08-046**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-046.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-045**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-045.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-047**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-047.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-049**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-049.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-048**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-048.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-050**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-050.mspx)
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
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 z dodatkiem Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 z dodatkiem Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=db455d17-435f-46d7-b2dd-5babb5a1eeb3)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 5.01 z dodatkiem Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=1557b93b-ecba-4f42-b89d-db0ee067d65b)  
(Krytyczny)  
[Microsoft Internet Explorer 6 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=aa780735-5928-4c46-89a4-63a814954796)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 z dodatkiem Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=1b2ad648-7dc9-407a-99f6-f39922746027)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Microsoft Outlook Express 5.5 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6257bfae-35f0-4c0e-b960-bca7aa6f86f7)  
(Ważny)  
[Microsoft Outlook Express 6 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=dab178f7-c282-41f4-acb1-a86e6aa4c91b)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Messenger 5.1](http://www.microsoft.com/downloads/details.aspx?familyid=a8d9eb73-5f8c-4b9a-940f-9157a3b3d774)  
(KB899283)  
(Ważny)
</td>
</tr>
<tr>
<th colspan="7">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS08-046**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-046.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-045**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-045.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-047**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-047.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-049**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-049.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-048**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-048.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-050**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-050.mspx)
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
[Windows XP z dodatkiem Service Pack 2 i Windows XP z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=d313f42c-f43f-48ea-82ef-3bc33077c7fa)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=69af2f30-138e-4b15-ab8d-4fce44cc0bc2)  
(Krytyczny)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=8e2125c7-52cb-4052-82a3-2d3c6a953752)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows XP z dodatkiem Service Pack 2 i Windows XP z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=01a34aa4-a456-4efc-a93a-c3c682b0181c)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Microsoft Outlook Express 6](http://www.microsoft.com/downloads/details.aspx?familyid=91469f2f-461c-4a67-8738-d42520427f6b)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Messenger 4.7](http://www.microsoft.com/downloads/details.aspx?familyid=8f588f7e-c4ed-42a0-b157-54b1eda60474)  
(KB946648)  
(Ważny)  
[Windows Messenger 5.1](http://www.microsoft.com/downloads/details.aspx?familyid=a8d9eb73-5f8c-4b9a-940f-9157a3b3d774)  
(KB899283)  
(Ważny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition oraz Microsoft Windows XP Professional x64 Edition z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition oraz Windows XP Professional x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3150c6b8-f50b-4b84-a7ce-c8daf77c080c)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=4780b89e-9735-4d3f-8def-34e7337ff604)  
(Krytyczny)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=39b41e4b-3237-409d-a818-ab0517c5e7cf)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition oraz Windows XP Professional x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=246b2686-e330-47a2-b4d4-68f218ad4021)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Microsoft Outlook Express 6](http://www.microsoft.com/downloads/details.aspx?familyid=2220aece-79d2-426f-90ec-24a17470567a)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Messenger 4.7](http://www.microsoft.com/downloads/details.aspx?familyid=a5fc5457-832f-4ee8-be60-4cc8518d1c10)  
(KB946648)  
(Ważny)  
[Windows Messenger 5.1](http://www.microsoft.com/downloads/details.aspx?familyid=a8d9eb73-5f8c-4b9a-940f-9157a3b3d774)  
(KB899283)  
(Ważny)
</td>
</tr>
<tr>
<th colspan="7">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS08-046**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-046.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-045**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-045.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-047**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-047.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-049**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-049.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-048**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-048.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-050**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-050.mspx)
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
Windows Server 2003 z dodatkiem Service Pack 1 i Windows Server 2003 z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem Service Pack 1 i Windows Server 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=828d8fdc-8534-4621-85a5-08aec255496f)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=0617a5dd-dce9-4de0-b0a0-ce38efe13524)  
(Krytyczny)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=b3c2e2fd-1cb9-491b-937c-053dd59a65bf)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem Service Pack 1 i Windows Server 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=92a3d08f-c117-4b24-bc78-2b913d270df6)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Microsoft Outlook Express 6](http://www.microsoft.com/downloads/details.aspx?familyid=30f2244a-f6fd-4fc1-a871-abf6958cb660)  
(Niski)
</td>
<td style="border:1px solid black;">
[Windows Messenger 4.7](http://www.microsoft.com/downloads/details.aspx?familyid=302315a8-ccb2-47c2-9104-b8e1d1f49aa0)  
(KB954723)  
(Umiarkowany)  
[Windows Messenger 5.1](http://www.microsoft.com/downloads/details.aspx?familyid=a8d9eb73-5f8c-4b9a-940f-9157a3b3d774)  
(KB899283)  
(Umiarkowany)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition i Windows Server 2003 x64 Edition z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition i Windows Server 2003 x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0a13776f-d543-41df-b904-d51e368c81cc)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=32a63f52-9fe6-48e3-bb4e-7d4dda5e0a90)  
(Krytyczny)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=88a26b76-f7df-45c9-8ed0-7d3cd71c1987)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition i Windows Server 2003 x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6bfbb6d8-5106-4adf-83cb-35ffc6e8eaf8)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Microsoft Outlook Express 6](http://www.microsoft.com/downloads/details.aspx?familyid=3287f006-cbb2-4c6d-820c-32833e08035a)  
(Niski)
</td>
<td style="border:1px solid black;">
[Windows Messenger 4.7](http://www.microsoft.com/downloads/details.aspx?familyid=be94d138-7d7b-489e-baa6-e214950be6b9)  
(KB954723)  
(Umiarkowany)  
[Windows Messenger 5.1](http://www.microsoft.com/downloads/details.aspx?familyid=a8d9eb73-5f8c-4b9a-940f-9157a3b3d774)  
(KB899283)  
(Umiarkowany)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Systemy operacyjne Windows Server 2003 z dodatkiem SP1 dla systemów z procesorem Itanium oraz Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem SP1 dla systemów z procesorem Itanium oraz Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=9566493f-4260-4072-947a-527887d2cd63)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=1855997e-a3be-46b1-a0bc-bb55eb0045fe)  
(Krytyczny)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=97d0d37d-5d76-4bc3-8cbd-1e3976c82acf)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem SP1 dla systemów z procesorem Itanium oraz Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=45356565-697f-41b3-9879-3edd11dbcb7e)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Microsoft Outlook Express 6](http://www.microsoft.com/downloads/details.aspx?familyid=c8570e40-355b-4a9b-933d-53ae021cbda5)  
(Niski)
</td>
<td style="border:1px solid black;">
[Windows Messenger 4.7](http://www.microsoft.com/downloads/details.aspx?familyid=e4b72618-536b-4a21-bd91-d91be9ca24e5)  
(KB954723)  
(Umiarkowany)  
[Windows Messenger 5.1](http://www.microsoft.com/downloads/details.aspx?familyid=a8d9eb73-5f8c-4b9a-940f-9157a3b3d774)  
(KB899283)  
(Umiarkowany)
</td>
</tr>
<tr>
<th colspan="7">
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS08-046**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-046.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-045**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-045.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-047**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-047.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-049**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-049.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-048**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-048.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-050**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-050.mspx)
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
<tr>
<td style="border:1px solid black;">
Windows Vista i Windows Vista z dodatkiem Service Pack 1
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=13cba012-dd20-48f9-8e44-e4cb104c4cad)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Vista i Windows Vista z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=3f21a8a2-9861-4fef-9d1e-caf5f7822c1a)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Vista i Windows Vista z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6418c78f-f008-4028-beb1-5a5ea8e797a1)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Poczta systemu Windows](http://www.microsoft.com/downloads/details.aspx?familyid=3851bcf8-f971-4d38-b27f-97396854aac0)  
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
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=ead919c2-d548-47b7-9cd6-80f991266428)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition i Windows Vista x64 Edition z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=aa04a754-fbfb-42a7-89d2-14373e3f4742)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition i Windows Vista x64 Edition z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=e03ccfb0-3ea3-4c59-adcf-9882d7086013)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Poczta systemu Windows](http://www.microsoft.com/downloads/details.aspx?familyid=3bf7eb8a-b347-4661-be2d-682adc713769)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr>
<th colspan="7">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS08-046**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-046.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-045**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-045.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-047**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-047.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-049**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-049.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-048**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-048.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-050**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-050.mspx)
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
<tr>
<td style="border:1px solid black;">
Windows Server 2008 dla systemów 32-bitowych
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=4b52ff2f-d2f5-4c20-b6cf-86d86c56b0f8)\*\*  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów 32-bitowych\*](http://www.microsoft.com/downloads/details.aspx?familyid=c3363df6-39dc-4910-9ce5-66553155378e)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów 32-bitowych\*](http://www.microsoft.com/downloads/details.aspx?familyid=0640f95e-1eee-4dd1-b4dd-2b82b7e984b9)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Poczta systemu Windows](http://www.microsoft.com/downloads/details.aspx?familyid=dc3c4b63-acd3-4469-8d47-e0562d99ee65)\*\*  
(Niski)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 dla systemów opartych na procesorach X64
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=df9814a6-5be0-4ac1-a767-a0eae8d5ee5d)\*\*  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów opartych na procesorach X64](http://www.microsoft.com/downloads/details.aspx?familyid=39dd1722-412b-469d-a475-b6513764838c)\*  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów opartych na procesorach X64](http://www.microsoft.com/downloads/details.aspx?familyid=51a93538-5e94-4f81-a6e0-d497a7b4899d)\*  
(Ważny)
</td>
<td style="border:1px solid black;">
[Poczta systemu Windows](http://www.microsoft.com/downloads/details.aspx?familyid=5f973f54-2322-4b41-8c1a-3e712c0da8ae)\*\*  
(Niski)
</td>
<td style="border:1px solid black;">
Nie dotyczy
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
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=ffc3cfcb-73fe-4a6d-9595-e9d7a5b3d3f7)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=e9c6cd46-30ad-46ee-9c8b-d0b446e660c4)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=390da130-749d-4890-aad7-be91e15b32bb)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Poczta systemu Windows](http://www.microsoft.com/downloads/details.aspx?familyid=9226cd85-1445-4976-a126-757c5d142ffd)  
(Niski)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
</table>
 
**\*Luka w zabezpieczeniach dotyczy instalacji Server Core systemu operacyjnego Windows Server 2008.** W przypadku obsługiwanych wersji systemu Windows Server 2008 ta aktualizacja ma zastosowanie, z takim samym wskaźnikiem ważności, niezależnie od tego, czy system Windows Server 2008 został zainstalowany przy użyciu opcji instalacji Server Core. Aby uzyskać więcej informacji na temat tej opcji instalacji, zobacz [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Należy pamiętać, że opcja instalacji Server Core nie dotyczy niektórych wersji systemu Windows Server 2008; zobacz [Porównanie opcji instalacji Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Luka w zabezpieczeniach nie dotyczy instalacji Server Core systemu operacyjnego Windows Server 2008.** Luce usuwanej przez tę aktualizację zabezpieczeń nie podlegają obsługiwane wersje systemu Windows Server 2008, jeżeli system Windows Server 2008 został zainstalowany przy użyciu opcji instalacji Server Core. Aby uzyskać więcej informacji na temat tej opcji instalacji, zobacz [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Należy pamiętać, że opcja instalacji Server Core nie dotyczy niektórych wersji systemu Windows Server 2008; zobacz [Porównanie opcji instalacji Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

#### Pakiety i oprogramowanie Office

 
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
</tr>
<tr>
<th colspan="6">
Pakiety Microsoft Office, systemy i ich składniki
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS08-041**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-041.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-043**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-043.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-051**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-051.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-044**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-044.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-042**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-042.mspx)
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
<td style="border:1px solid black;">
[**Krytyczny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Works 8
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
[Microsoft Works 8](http://www.microsoft.com/downloads/details.aspx?familyid=458985c3-9c6f-4049-81cd-0d0389c81f11)  
(KB955428)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2000 z dodatkiem Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office Access 2000 z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=54e4031d-298f-480c-88d5-0ad3b2b62ba9)  
(KB955441)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Excel 2000 z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=4bf8688e-e5b9-4e53-a1a1-8cf1acfdb80b)  
(KB951582)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft Office PowerPoint 2000 z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=e7c044d8-778a-4985-b25b-4f7f6e4abadd)  
(KB949007)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2000 z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=3ab323ec-9f92-453c-b7c7-9a95a9efcaea)  
(KB921595)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office XP z dodatkiem Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office Access 2002 z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=34b655f8-1922-4246-94ca-ed381c3e3b13)  
(KB955440)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Excel 2002 z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=9bbf7550-f5c4-4b9b-bd86-1e7be6c42eb5)  
(KB951551)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Microsoft Office PowerPoint 2002 z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=f8921074-7985-4d42-ac2b-d2f3b1d466ba)  
(KB948995)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Microsoft Office XP z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=bf566ce6-23da-45e5-9c2b-c47331d30e79)  
(KB921596)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Microsoft Word 2002 z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=c7146dfc-e1be-4d13-877b-1d9bcacc4a64)  
(KB954463)  
(Ważny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2003 z dodatkiem Service Pack 2 i Microsoft Office 2003 z dodatkiem Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office Access 2003 z dodatkiem Service Pack 2 i Microsoft Office Access 2003 z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=fd698517-a504-427d-9e5f-fde8f102142c)  
(KB955439)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Excel 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fc612e9a-bdf3-4952-8ada-0de5a50973f0)  
(KB951548)  
(Ważny)  
[Excel 2003 z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=fc612e9a-bdf3-4952-8ada-0de5a50973f0)  
(KB951548)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Microsoft Office PowerPoint 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7a7c21f0-5e0e-4dee-9710-1ce3d565913f)\*\*\*  
(KB948988)  
(Ważny)  
[Microsoft Office PowerPoint 2003 z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=7a7c21f0-5e0e-4dee-9710-1ce3d565913f)\*\*\*  
(KB948988)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e0df2f6e-1102-461d-829f-5f3e2d7eb4b3)  
(KB921598)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Microsoft Word 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=13a37b76-9fec-426f-8176-3c95f934efe0)  
(KB954464)  
(Ważny)  
[Microsoft Word 2003 z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=13a37b76-9fec-426f-8176-3c95f934efe0)  
(KB954464)  
(Ważny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2007 i Microsoft Office 2007 z dodatkiem Service Pack 1
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Excel 2007](http://www.microsoft.com/downloads/details.aspx?familyid=2753e8d6-e156-49ef-af2d-4c521c808ffd)  
(KB951546)  
(Ważny)  
[Excel 2007 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=2753e8d6-e156-49ef-af2d-4c521c808ffd)  
(KB951546)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Microsoft Office PowerPoint 2007](http://www.microsoft.com/downloads/details.aspx?familyid=55fd618a-e9c5-4f1e-b9a5-b2e47ec98ef1)  
(KB951338)  
(Ważny)  
[Microsoft Office PowerPoint 2007 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=55fd618a-e9c5-4f1e-b9a5-b2e47ec98ef1)  
(KB951338)  
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
<th colspan="6">
Inne programy pakietu Office
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS08-041**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-041.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-043**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-043.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-051**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-051.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-044**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-044.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-042**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-042.mspx)
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
<td style="border:1px solid black;">
[**Krytyczny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Project 2002 z dodatkiem Service Pack 1
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
[Microsoft Office Project 2002 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=bf566ce6-23da-45e5-9c2b-c47331d30e79)  
(KB921596)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr>
<td style="border:1px solid black;">
SnapShot Viewer dla programu Microsoft Access
</td>
<td style="border:1px solid black;">
SnapShot Viewer dla programu Microsoft Access\*
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
Nie dotyczy
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Podgląd programu Microsoft Office PowerPoint 2003
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Podgląd programu Microsoft Office PowerPoint 2003](http://www.microsoft.com/downloads/details.aspx?familyid=911c8872-dec8-4b8e-9708-93dcabd3e036)  
(KB949041)  
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
<td style="border:1px solid black;">
Podgląd programu Microsoft Office Excel 2003 i Podgląd programu Microsoft Office Excel 2003 z dodatkiem Service Pack 3
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Podgląd programu Microsoft Office Excel 2003](http://www.microsoft.com/downloads/details.aspx?familyid=d7ed9e75-15f2-4950-98b3-93023ba0f4c1)  
(KB951589)  
(Ważny)  
[Podgląd programu Microsoft Office Excel 2003 z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=d7ed9e75-15f2-4950-98b3-93023ba0f4c1)  
(KB951589)  
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
Podgląd programu Microsoft Office Excel
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Podgląd programu Microsoft Office Excel](http://www.microsoft.com/downloads/details.aspx?familyid=b574d906-7f09-49b0-80bf-e84dee8c4583)  
(KB955472)  
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
Microsoft Office Converter Pack
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
[Microsoft Office Converter Pack](http://www.microsoft.com/downloads/details.aspx?familyid=199b08c7-6d79-4930-8f0c-31034629c485)  
(KB925256)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Pakiet zgodności formatu plików pakietu Microsoft Office dla programów Word, Excel i PowerPoint 2007 i Pakiet zgodności formatu plików pakietu Microsoft Office dla programów Word, Excel i PowerPoint 2007 z dodatkiem Service Pack 1
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Pakiet zgodności formatu plików pakietu Microsoft Office dla programów Word, Excel i PowerPoint 2007](http://www.microsoft.com/downloads/details.aspx?familyid=7afdae9b-9c74-4af7-9844-0e54221ea3b9)  
(KB951596)  
(Ważny)  
[Pakiet zgodności formatu plików pakietu Microsoft Office dla programów Word, Excel i PowerPoint 2007 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7afdae9b-9c74-4af7-9844-0e54221ea3b9)  
(KB951596)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Pakiet zgodności formatu plików pakietu Microsoft Office dla programów Word, Excel i PowerPoint 2007](http://www.microsoft.com/downloads/details.aspx?familyid=84ce5d58-0010-4945-bce9-67a41f898f2f) (KB954038)  
(Ważny)  
[Pakiet zgodności formatu plików pakietu Microsoft Office dla programów Word, Excel i PowerPoint 2007 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=84ce5d58-0010-4945-bce9-67a41f898f2f) (KB954038)  
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
<td style="border:1px solid black;">
Microsoft Office SharePoint Server 2007 oraz Microsoft Office SharePoint Server 2007 z dodatkiem Service Pack 1
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Microsoft Office SharePoint Server 2007](http://www.microsoft.com/downloads/details.aspx?familyid=a7731749-b026-4765-808a-e151b990f0e1)\*\*  
(KB953397)  
(Ważny)  
[Microsoft Office SharePoint Server 2007 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=a7731749-b026-4765-808a-e151b990f0e1)\*\*  
(KB953397)  
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
Microsoft Office SharePoint Server 2007 x64 Edition i Microsoft Office SharePoint Server 2007 x64 Edition z dodatkiem Service Pack 1
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Microsoft Office SharePoint Server 2007 x64 Edition](http://www.microsoft.com/downloads/details.aspx?familyid=fc95ab88-2d31-44e1-a702-7cb10e83695b)\*\*  
(KB953397)  
(Ważny)  
[Microsoft Office SharePoint Server 2007 x64 Edition z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=fc95ab88-2d31-44e1-a702-7cb10e83695b)\*\*  
(KB953397)  
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
<th colspan="6">
Microsoft Office dla komputerów Macintosh
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS08-041**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-041.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-043**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-043.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-051**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-051.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-044**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-044.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-042**](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-042.mspx)
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
<td style="border:1px solid black;">
[**Krytyczny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Krytyczny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2004 dla komputerów Macintosh
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Microsoft Office 2004 dla komputerów Macintosh](http://www.microsoft.com/downloads/details.aspx?familyid=ebd3af0c-3f62-4d18-bf45-881655683bd5)  
(KB956343)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2004 dla komputerów Macintosh](http://www.microsoft.com/downloads/details.aspx?familyid=ebd3af0c-3f62-4d18-bf45-881655683bd5)  
(KB956343)  
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
Microsoft Office 2008 dla komputerów Macintosh
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 dla komputerów Macintosh](http://www.microsoft.com/downloads/details.aspx?familyid=9515c70d-be80-4ade-856a-ea542f7d84e1)  
(KB956344)  
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
</table>
 
**\*Uwaga dotycząca przeglądarki SnapShot Viewer dla programu Microsoft Access (MS08-041):** Obecnie firma Microsoft opracowuje aktualizację zabezpieczeń dla oprogramowania, którego dotyczy luka w zabezpieczeniach i opublikuje ją w możliwie najkrótszym terminie. Po opublikowaniu aktualizacji zabezpieczeń firma Microsoft zaktualizuje również odpowiedni biuletyn zabezpieczeń oraz niniejsze podsumowanie biuletynów zabezpieczeń.

**\*\*Uwaga dotycząca programów Microsoft Office SharePoint Server 2007, Microsoft Office SharePoint Server 2007 z dodatkiem Service Pack 1, Microsoft Office SharePoint Server 2007 x64 Edition i Microsoft Office SharePoint Server 2007 x64 Edition z dodatkiem Service Pack 1 (MS08-043):** Aktualizacja objęta biuletynem zabezpieczeń MS08-043 dotyczy serwerów z zainstalowanymi usługami programu Excel, takich jak Microsoft Office SharePoint Server 2007 Enterprise i Microsoft Office SharePoint Server 2007 For Internet Sites w konfiguracji domyślnej. Serwer Microsoft Office SharePoint Server 2007 Standard nie zawiera usług programu Excel.

**\*\*\*Uwaga dotycząca programów Microsoft Office PowerPoint 2003 z dodatkiem Service Pack 2 i Microsoft Office PowerPoint 2003 z dodatkiem Service Pack 3 (MS08-051):** Firma Microsoft opublikowała w witrynie Microsoft Download Center nowe pakiety aktualizacyjne, oznaczone numerem wersji 2. Klienci, którzy ręcznie zainstalowali wersję 1 tej aktualizacji, pobraną z witryny Microsoft Download Center, powinni zainstalować jej wersję 2. Klienci, którzy zainstalowali tę aktualizację za pomocą usługi Microsoft Update lub Office Update, nie muszą jej instalować ponownie. Więcej informacji na ten temat, w tym dotyczących innych opcji instalacji lub obejść, można znaleźć w biuletynie [MS08-051](http://www.microsoft.com/poland/technet/security/bulletin/2008/ms08-051.mspx).

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

-   [ISC/SANS](http://isc.sans.org/) za zgłoszenie problemu opisanego w biuletynie MS08-042
-   [VeriSign iDefense VCP](http://www.idefense.com/vcp) za zgłoszenie problemu opisanego w biuletynie MS08-043
-   [TippingPoint](http://www.tippingpoint.com/) oraz [Zero Day Initiative](http://www.zerodayinitiative.com/) za zgłoszenie problemu opisanego w biuletynie MS08-043
-   Jeremy'emu Funkowi za zgłoszenie problemu opisanego w biuletynie MS08-043
-   Shaunowi Colley z firmy [NGS Software](http://www.nextgenss.com/) za zgłoszenie problemu opisanego w biuletynie MS08-044
-   Damianowi Putowi współpracującemu z firmą [Zero Day Initiative (ZDI)](http://www.zerodayinitiative.com/) za zgłoszenie problemu opisanego w biuletynie MS08-044
-   Anonimowemu analitykowi współpracującemu z firmą [iDefense VCP](http://labs.idefense.com/) za zgłoszenie problemu opisanego w biuletynie MS08-044
-   Damianowi Putowi współpracującemu z firmą [iDefense VCP](http://labs.idefense.com/) za zgłoszenie problemu opisanego w biuletynie MS08-044
-   Yamata Li z firmy [Palo Alto Networks](http://www.paloaltonetworks.com/) za zgłoszenie problemu opisanego w biuletynie MS08-045
-   Tavis Ormandy z zespołu [Google Security Team](http://www.google.com/) za zgłoszenie problemu opisanego w biuletynie MS08-045
-   Samowi Thomasowi, współpracownikowi firm [TippingPoint](http://www.tippingpoint.com/) i [Zero Day Initiative,](http://www.zerodayinitiative.com/) za zgłoszenie problemu opisanego w biuletynie MS08-045
-   [TippingPoint](http://www.tippingpoint.com/) oraz [Zero Day Initiative](http://www.zerodayinitiative.com/) za zgłoszenie problemu opisanego w biuletynie MS08-045
-   Jun Mao z firmy [VeriSign iDefense Labs](http://labs.idefense.com/) za zgłoszenie problemu opisanego w biuletynie MS08-046
-   Jorge'owi Luis Alvarez Medina z firmy [Core Security Technologies](http://www.coresecurity.com/) za zgłoszenie problemu opisanego w biuletynie MS08-048
-   Yamata Li z firmy [Palo Alto Networks](http://www.paloaltonetworks.com/) za zgłoszenie problemu opisanego w biuletynie MS08-049
-   Haifei Li z zespołu [FortiGuard Global Security Research Team](http://www.fortiguardcenter.com) firmy Fortinet za zgłoszenie problemu opisanego w biuletynie MS08-050
-   Rubenowi Santamarta z firmy [Reversemode.com](http://reversemode.com/) współpracującemu z firmą [iDefense Labs](http://labs.idefense.com/) za zgłoszenie problemu opisanego w biuletynie MS08-051
-   ADLab z firmy [Venustech](http://www.venustech.com.cn/) za zgłoszenie problemu opisanego w biuletynie MS08-051

#### Pomoc techniczna

-   Wymienione oprogramowanie zostało przetestowane w celu ustalenia, których wersji dotyczy problem. Dla pozostałych wersji upłynął okres pomocy technicznej. Aby zapoznać się z zasadami cyklu pomocy technicznej dotyczącymi używanej wersji oprogramowania, odwiedź [witrynę zasad cyklu pomocy technicznej firmy Microsoft](http://go.microsoft.com/fwlink/?linkid=21742).
-   Klienci mogą uzyskać pomoc techniczną w [Biurze Obsługi Klienta Microsoft](http://go.microsoft.com/fwlink/?linkid=21131) pod numerem 0 801 802 000 (Opłata według stawek Twojego operatora) lub (0-22) 594 19 99 w godzinach od 9:00 do 17:00, od poniedziałku do piątku. Połączenia z działem pomocy technicznej związane z aktualizacjami zabezpieczeń są bezpłatne.
-   Klienci międzynarodowi mogą uzyskać pomoc w lokalnych przedstawicielstwach firmy Microsoft. Pomoc techniczna związana z aktualizacjami zabezpieczeń jest bezpłatna. Informacje o sposobie kontaktowania się z pomocą techniczną firmy Microsoft są dostępne w [międzynarodowej witrynie sieci Web pomocy i obsługi technicznej](http://go.microsoft.com/fwlink/?linkid=21155).

#### Zrzeczenie odpowiedzialności

Informacje w bazie wiedzy Microsoft Knowledge Base są dostarczane „tak jak są” bez jakiejkolwiek gwarancji. Firma Microsoft odrzuca wszelkie gwarancje, wyraźne i dorozumiane, w tym gwarancje dotyczące wartości handlowej i przydatności do określonego celu. Firma Microsoft Corporation ani jej dostawcy w żadnym wypadku nie ponoszą odpowiedzialności za jakiekolwiek szkody, w tym bezpośrednie, pośrednie, przypadkowe, wynikowe, utratę zysków handlowych lub szkody specjalne, nawet jeżeli firmę Microsoft Corporation lub jej dostawców powiadomiono o możliwości zaistnienia takich szkód. W niektórych stanach wyłączenie lub ograniczenie odpowiedzialności za straty wynikowe lub przypadkowe, a więc i powyższe ograniczenia, nie mają zastosowania.

#### Wersje

-   Wersja 1.0 (12 sierpnia 2008 r.): Opublikowane podsumowanie biuletynów zabezpieczeń.
-   Wersja 2.0 (20 sierpnia 2008 r.): Dodano uwagę do tabeli „Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki” w biuletynie MS08-043 w celu wyjaśnienia, że ta aktualizacja zabezpieczeń dotyczy serwerów z zainstalowanymi usługami programu Excel, takich jak Microsoft Office SharePoint Server 2007 Enterprise i Microsoft Office SharePoint Server 2007 For Internet Sites w konfiguracji domyślnej. Serwer Microsoft Office SharePoint Server 2007 Standard nie zawiera usług programu Excel. Ponadto dodano uwagę do tabeli „Programy, których dotyczy problem i lokalizacje, z których można pobrać poprawki” w biuletynie MS08-051 w celu poinformowania o opublikowaniu w witrynie Microsoft Download Center nowych pakietów aktualizacyjnych, oznaczonych numerem wersji 2, dla programów Microsoft Office PowerPoint 2003 z dodatkiem Service Pack 2 oraz Microsoft Office PowerPoint 2003 z dodatkiem Service Pack 3. Klienci, którzy ręcznie zainstalowali wersję 1 tej aktualizacji, pobraną z witryny Microsoft Download Center, powinni zainstalować jej wersję 2. Klienci, którzy zainstalowali tę aktualizację za pomocą usługi Microsoft Update lub Office Update, nie muszą jej instalować ponownie.

*Built at 2014-04-18T01:50:00Z-07:00*
