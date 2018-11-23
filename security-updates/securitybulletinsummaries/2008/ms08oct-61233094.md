---
TOCTitle: 'MS08-OCT'
Title: 'Podsumowanie biuletynów zabezpieczeń firmy Microsoft za październik 2008 r.'
ms:assetid: 'ms08-oct'
ms:contentKeyID: 61233094
ms:mtpsurl: 'https://technet.microsoft.com/pl-PL/library/ms08-oct(v=Security.10)'
---

Podsumowanie biuletynów zabezpieczeń firmy Microsoft za październik 2008 r.
===========================================================================

Opublikowano: 14 października 2008 | Zaktualizowano: 23 października 2008

**Wersja:** 3.0

Niniejsze podsumowanie biuletynów zabezpieczeń zawiera spis biuletynów za październik 2008 r.

Z chwilą opublikowania biuletynów za październik 2008 r. niniejsze podsumowanie biuletynów zastępuje powiadomienie o biuletynach zabezpieczeń wydane 9 października 2008 r. Aby uzyskać więcej informacji na temat usługi powiadamiania o biuletynach, zobacz [Powiadomienia o biuletynach zabezpieczeń firmy Microsoft (j. ang.)](http://technet.microsoft.com/security/bulletin/advance).

Aby dowiedzieć się, jak otrzymywać automatyczne powiadomienia o publikacji biuletynów zabezpieczeń firmy Microsoft, odwiedź stronę [Microsoft Technical Security Notifications](http://go.microsoft.com/fwlink/?linkid=21163).

Dla biuletynu bezpieczeństwa poza cyklem produkcyjnym dodano do wersji 3.0 niniejszego biuletynu podsumowującego, Microsoft udostępnia webcast od 23 października 2008, godz 1:00 czasu Pacyfiku (US & Canada). [Zarejestruj się na webcast biuletynu bezpieczeństwa poza cyklem produkcyjnym](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032393978&eventcategory=4&culture=en-us&countrycode=us). Po tym terminie, WebCast jest dostępny na żądanie. Aby uzyskać więcej informacji, zobacz [Microsoft Security Bulletin Summaries and Webcasts](http://technet.microsoft.com/security/bulletin/summary).

15 października 2008 r. o godz. 11:00 czasu Pacyfiku (godz. 20:00 czasu środkowoeuropejskiego) firma Microsoft udostępni emisję internetową, w której znajdą się odpowiedzi na pytania klientów dotyczące tych biuletynów (USA i Kanada). [Zarejestruj się, aby zobaczyć emisję internetową dotyczącą biuletynów zabezpieczeń za październik](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032374639). Po tym dniu emisja internetowa będzie dostępna na żądanie. Aby uzyskać więcej informacji, zobacz [Podsumowania biuletynów zabezpieczeń i emisje internetowe firmy Microsoft](http://technet.microsoft.com/security/bulletin/summary).

Firma Microsoft udostępnia także informacje, dzięki którym klienci mogą ustalić priorytety dla aktualizacji zabezpieczeń w związku z niezwiązanymi z zabezpieczeniami aktualizacjami o wysokim priorytecie, które publikowane są w tym samym dniu, co comiesięczne aktualizacje zabezpieczeń. Zapoznaj się z sekcją **Inne informacje**.

### Informacje o biuletynie

#### Streszczenia

W bieżącym miesiącu opublikowano następujące biuletyny (w kolejności wskaźnika ważności):

Krytyczny (5)
-------------

<span></span>

| Identyfikator biuletynu               | Biuletyn zabezpieczeń firmy Microsoft MS08-067                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
|---------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**                   | [**Luka w zabezpieczeniach usługi Serwer umożliwia zdalne wykonanie kodu (958644)**](http://technet.microsoft.com/security/bulletin/ms08-067)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| **Streszczenie**                      | Niniejsza aktualizacja zabezpieczeń usuwa lukę w zabezpieczeniach usługi Serwer, która została zgłoszona przez użytkowników. Luka ta mogłaby pozwolić na zdalne wykonanie kodu, jeśli użytkownik otrzymałby specjalnie spreparowane żądanie RPC w systemie, którego dotyczy luka. Na komputerach z systemami Microsoft Windows 2000, Windows XP i Windows Server 2003 osoba atakująca może wykorzystać tę lukę bez uwierzytelniania w celu uruchomienia dowolnego kodu. Potencjalnie luka umożliwia spreparowanie programu wykorzystującego luki, pełniącego funkcję robaka. Sprawdzone metody działania stosowane w zaporach oraz standardowe domyślne konfiguracje zapór mogą pomóc w zabezpieczeniu zasobów sieciowych przed atakami spoza obszaru działania przedsiębiorstwa. |
| **Maksymalny wskaźnik ważności**      | [Krytyczny](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Wpływ luki**                        | Zdalne wykonanie kodu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| **Wykrywanie**                        | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Aktualizacja wymaga ponownego uruchomienia systemu.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Programy, których dotyczy problem** | **Microsoft Windows.** Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |

| Identyfikator biuletynu               | Biuletyn zabezpieczeń firmy Microsoft MS08-060                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
|---------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**                   | [**Luka w zabezpieczeniach usługi Active Directory umożliwia zdalne wykonanie kodu (957280)**](http://technet.microsoft.com/security/bulletin/ms08-060)                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Streszczenie**                      | Niniejsza aktualizacja zabezpieczeń pozwala usunąć zgłoszoną przez użytkowników lukę w zabezpieczeniach wdrożeń usługi Active Directory w systemie Microsoft Windows 2000 Server. Osoba atakująca, która uzyska dostęp do sieci podlegającej luce, może zyskać możliwość zdalnego wykonania kodu. Luka ta dotyczy wyłącznie serwerów pracujących pod nadzorem systemu Microsoft Windows 2000 skonfigurowanych jako kontrolery domen. Jeśli serwer z systemem Microsoft Windows 2000 nie funkcjonuje jako kontroler domeny, nie będzie nasłuchiwać zapytań LDAP ani LDAP over SSL (LDAPS) i nie będzie zagrożony przez omawianą lukę. |
| **Maksymalny wskaźnik ważności**      | [Krytyczny](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| **Wpływ luki**                        | Zdalne wykonanie kodu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Wykrywanie**                        | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Aktualizacja wymaga ponownego uruchomienia systemu.                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Programy, których dotyczy problem** | **Microsoft Windows.** Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |

| Identyfikator biuletynu               | Biuletyn zabezpieczeń firmy Microsoft MS08-058                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
|---------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**                   | [**Zbiorcza aktualizacja zabezpieczeń dla programu Internet Explorer (956390)**](http://technet.microsoft.com/security/bulletin/ms08-058)                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Streszczenie**                      | Niniejsza aktualizacja zabezpieczeń usuwa pięć luk w zabezpieczeniach, które zostały zgłoszone przez użytkowników, oraz jedną lukę w zabezpieczeniach, która została zgłoszona przez organizację publiczną. Każda z tych luk może pozwolić na zdalne wykonanie kodu lub ujawnienie informacji, jeśli użytkownik wyświetli specjalnie spreparowaną stronę sieci Web przy użyciu programu Internet Explorer. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi. |
| **Maksymalny wskaźnik ważności**      | [Krytyczny](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Wpływ luki**                        | Zdalne wykonanie kodu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Wykrywanie**                        | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Aktualizacja wymaga ponownego uruchomienia systemu.                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| **Programy, których dotyczy problem** | **Microsoft Windows, Internet Explorer.** Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                                                                                                                                                                                |

| Identyfikator biuletynu               | Biuletyn zabezpieczeń firmy Microsoft MS08-059                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
|---------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**                   | [**Luka w zabezpieczeniach usługi RPC serwera Host Integration Server umożliwia zdalne wykonanie kodu (956695)**](http://technet.microsoft.com/security/bulletin/ms08-059)                                                                                                                                                                                                                                                                                                                                                                           |
| **Streszczenie**                      | Niniejsza aktualizacja zabezpieczeń usuwa lukę w zabezpieczeniach serwera Microsoft Host Integration Server, która została zgłoszona przez użytkowników. Luka ta umożliwia zdalne wykonanie kodu, gdy osoba atakująca wyśle specjalnie spreparowane żądanie RPC do systemu, którego dotyczy luka. Użytkownicy korzystający z najważniejszych wskazówek, którzy skonfigurują konto usługi SNA RPC tak, aby miało niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, których konto usługi SNA RPC posiada uprawnienia administracyjne. |
| **Maksymalny wskaźnik ważności**      | [Krytyczny](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| **Wpływ luki**                        | Zdalne wykonanie kodu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Wykrywanie**                        | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Aktualizacja może wymagać ponownego uruchomienia komputera.                                                                                                                                                                                                                                                                                                                                                                         |
| **Programy, których dotyczy problem** | **Microsoft Host Integration Server.** Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                                                                                                                               |

| Identyfikator biuletynu               | Biuletyn zabezpieczeń firmy Microsoft MS08-057                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
|---------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**                   | [**Luki w zabezpieczeniach programu Microsoft Excel umożliwiają zdalne wykonanie kodu (956416)**](http://technet.microsoft.com/security/bulletin/ms08-057)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| **Streszczenie**                      | Niniejsza aktualizacja zabezpieczeń pozwala usunąć trzy luki w zabezpieczeniach programu Microsoft Office Excel zgłoszone przez osoby prywatne, które mogą pozwolić na zdalne wykonanie kodu, jeśli użytkownik otworzy specjalnie spreparowany plik programu Excel. Osoba atakująca, której uda się wykorzystać te luki, może uzyskać pełną kontrolę nad atakowanym systemem. Osoba taka może wówczas instalować programy, przeglądać, zmieniać i usuwać dane oraz tworzyć nowe konta z pełnymi uprawnieniami. Użytkownicy, których konta zostały skonfigurowane w taki sposób, że mają niewielkie uprawnienia w systemie, ponoszą mniejsze ryzyko niż ci, którzy pracują z uprawnieniami administracyjnymi. |
| **Maksymalny wskaźnik ważności**      | [Krytyczny](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Wpływ luki**                        | Zdalne wykonanie kodu                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Wykrywanie**                        | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Ta aktualizacja nie wymaga ponownego uruchomienia komputera.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Programy, których dotyczy problem** | **Microsoft Office.** Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |

Ważny (6)
---------

<span></span>

| Identyfikator biuletynu               | Biuletyn zabezpieczeń firmy Microsoft MS08-066                                                                                                                                                                                                                                                                                                                                                                                |
|---------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**                   | [**Luka w zabezpieczeniach pomocniczego sterownika funkcji (Ancillary Function Driver) firmy Microsoft umożliwia podniesienie uprawnień (956803)**](http://technet.microsoft.com/security/bulletin/ms08-066)                                                                                                                                                                                                                  |
| **Streszczenie**                      | Niniejsza aktualizacja zabezpieczeń usuwa lukę w zabezpieczeniach pomocniczego sterownika funkcji firmy Microsoft, która została zgłoszona przez użytkowników. Osoba atakująca, której uda się lokalnie wykorzystać tę lukę, może uzyskać pełną kontrolę nad systemem, którego dotyczy luka. Osoba taka może wówczas instalować programy, przeglądać, zmieniać i usuwać dane oraz tworzyć nowe konta z pełnymi uprawnieniami. |
| **Maksymalny wskaźnik ważności**      | [Ważny](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                         |
| **Wpływ luki**                        | Podniesienie uprawnień                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Wykrywanie**                        | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Aktualizacja wymaga ponownego uruchomienia systemu.                                                                                                                                                                                                                                                          |
| **Programy, których dotyczy problem** | **Microsoft Windows.** Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                        |

| Identyfikator biuletynu               | Biuletyn zabezpieczeń firmy Microsoft MS08-061                                                                                                                                                                                                                                                                                                                                |
|---------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**                   | [**Usterki jądra systemu Windows umożliwiają podniesienie poziomu uprawnień (954211)**](http://technet.microsoft.com/security/bulletin/ms08-061)                                                                                                                                                                                                                              |
| **Streszczenie**                      | Niniejsza aktualizacja zabezpieczeń usuwa jedną lukę zgłoszoną przez organizacje publiczne oraz dwie luki zgłoszone przez użytkowników, istniejące w jądrze systemu Windows. Osoba atakująca, której uda się wykorzystać te luki, może uzyskać pełną kontrolę nad atakowanym systemem. Nie jest możliwe wykorzystanie luk w sposób zdalny ani przez użytkowników anonimowych. |
| **Maksymalny wskaźnik ważności**      | [Ważny](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                         |
| **Wpływ luki**                        | Podniesienie uprawnień                                                                                                                                                                                                                                                                                                                                                        |
| **Wykrywanie**                        | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Aktualizacja wymaga ponownego uruchomienia systemu.                                                                                                                                                                                                          |
| **Programy, których dotyczy problem** | **Microsoft Windows.** Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                        |

| Identyfikator biuletynu               | Biuletyn zabezpieczeń firmy Microsoft MS08-062                                                                                                                                                                                                                                                                                                                                                                    |
|---------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**                   | [**Luka w zabezpieczeniach usługi Windows Internet Printing Service umożliwia zdalne wykonanie kodu (953155)**](http://technet.microsoft.com/security/bulletin/ms08-062)                                                                                                                                                                                                                                          |
| **Streszczenie**                      | Ta aktualizacja pozwala usunąć zgłoszoną przez osobę prywatną lukę w zabezpieczeniach usługi drukowania w Internecie systemu Windows, która może pozwolić na zdalne wykonanie kodu. Osoba atakująca, której uda się wykorzystać tę lukę, może uzyskać pełną kontrolę nad systemem, którego dotyczy luka. Osoba taka może wówczas instalować programy, przeglądać, zmieniać i usuwać dane oraz tworzyć nowe konta. |
| **Maksymalny wskaźnik ważności**      | [Ważny](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                             |
| **Wpływ luki**                        | Zdalne wykonanie kodu                                                                                                                                                                                                                                                                                                                                                                                             |
| **Wykrywanie**                        | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Aktualizacja wymaga ponownego uruchomienia systemu.                                                                                                                                                                                                                                              |
| **Programy, których dotyczy problem** | **Microsoft Windows.** Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                            |

| Identyfikator biuletynu               | Biuletyn zabezpieczeń firmy Microsoft MS08-063                                                                                                                                                                                                                                                                                                                                                                                     |
|---------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**                   | [**Usterka usługi SMB umożliwia zdalne wykonanie kodu (957095)**](http://technet.microsoft.com/security/bulletin/ms08-063)                                                                                                                                                                                                                                                                                                         |
| **Streszczenie**                      | Niniejsza aktualizacja zabezpieczeń usuwa lukę w zabezpieczeniach protokołu SMB (Server Message Block) firmy Microsoft, która została zgłoszona przez użytkowników. Luka ta umożliwia zdalne wykonanie kodu na serwerze, na którym udostępniono pliki lub foldery. Osoba atakująca, której uda się wykorzystać lukę, może instalować programy, przeglądać, zmieniać i usuwać dane oraz tworzyć nowe konta z pełnymi uprawnieniami. |
| **Maksymalny wskaźnik ważności**      | [Ważny](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                              |
| **Wpływ luki**                        | Zdalne wykonanie kodu                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Wykrywanie**                        | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Aktualizacja wymaga ponownego uruchomienia systemu.                                                                                                                                                                                                                                                               |
| **Programy, których dotyczy problem** | **Microsoft Windows.** Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                             |

| Identyfikator biuletynu               | Biuletyn zabezpieczeń firmy Microsoft MS08-064                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
|---------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**                   | [**Luka w sposobie przetwarzania struktur Virtual Address Descriptor umożliwia podniesienie poziomu uprawnień (956841)**](http://technet.microsoft.com/security/bulletin/ms08-064)                                                                                                                                                                                                                                                                                                                                                         |
| **Streszczenie**                      | Niniejsza aktualizacja zabezpieczeń usuwa lukę w deskryptorze adresów wirtualnych, która została zgłoszona przez użytkowników. Luka ta umożliwia podniesienie poziomu uprawnień, jeśli użytkownik uruchomi specjalnie spreparowaną aplikację. Uwierzytelniona osoba atakująca, której uda się wykorzystać tę lukę, może podnieść poziom uprawnień w systemie, którego dotyczy ten problem. Osoba taka może wówczas instalować programy, przeglądać, zmieniać i usuwać dane oraz tworzyć nowe konta z pełnymi uprawnieniami administratora. |
| **Maksymalny wskaźnik ważności**      | [Ważny](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| **Wpływ luki**                        | Podniesienie uprawnień                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| **Wykrywanie**                        | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Aktualizacja wymaga ponownego uruchomienia systemu.                                                                                                                                                                                                                                                                                                                                                                       |
| **Programy, których dotyczy problem** | **Microsoft Windows.** Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                                                                                                                                     |

| Identyfikator biuletynu               | Biuletyn zabezpieczeń firmy Microsoft MS08-065                                                                                                                                                                                                                                                                   |
|---------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**                   | [**Luka w zabezpieczeniach kolejkowania wiadomości może pozwolić na zdalne wykonanie kodu (951071)**](http://technet.microsoft.com/security/bulletin/ms08-065)                                                                                                                                                   |
| **Streszczenie**                      | Niniejsza aktualizacja zabezpieczeń usuwa lukę w usłudze kolejkowania wiadomości (MSMQ, Message Queuing Service) systemów Microsoft Windows 2000, która została zgłoszona przez użytkowników. Luka umożliwia zdalne wykonanie kodu w systemach Microsoft Windows 2000 z włączoną usługą kolejkowania wiadomości. |
| **Maksymalny wskaźnik ważności**      | [Ważny](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                            |
| **Wpływ luki**                        | Zdalne wykonanie kodu                                                                                                                                                                                                                                                                                            |
| **Wykrywanie**                        | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Aktualizacja wymaga ponownego uruchomienia systemu.                                                                                                                                             |
| **Programy, których dotyczy problem** | **Microsoft Windows.** Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                           |

Średni (1)
----------

<span></span>

| Identyfikator biuletynu               | Biuletyn zabezpieczeń firmy Microsoft MS08-056                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
|---------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**                   | [**Luka w zabezpieczeniach pakietu Microsoft Office może spowodować ujawnienie informacji (957699)**](http://go.microsoft.com/fwlink/?linkid=128145)                                                                                                                                                                                                                                                                                                                                                                             |
| **Streszczenie**                      | Ta krytyczna aktualizacja zabezpieczeń usuwa lukę w zabezpieczeniach pakietu Microsoft Office, która została zgłoszona przez użytkowników. Luka może pozwolić na ujawnienie informacji, jeśli użytkownik kliknie specjalnie spreparowany adres URL protokołu CDO. Osoba atakująca, której uda się wykorzystać tę lukę, może uruchomić skrypt po stronie klienta, korzystając z przeglądarki użytkownika. Skrypt może sfałszować zawartość witryny, ujawnić informacje lub wykonać każdą czynność, którą może wykonać użytkownik. |
| **Maksymalny wskaźnik ważności**      | [Umiarkowany](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| **Wpływ luki**                        | Ujawnienie informacji                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| **Wykrywanie**                        | Narzędzie Microsoft Baseline Security Analyzer może wykryć, czy komputer wymaga zainstalowania tej aktualizacji. Ta aktualizacja nie wymaga ponownego uruchomienia komputera.                                                                                                                                                                                                                                                                                                                                                    |
| **Programy, których dotyczy problem** | **Microsoft Office.** Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                                                                                                                                                                                                                                                                                                                                            |

Wskaźnik możliwości wykorzystania luki
--------------------------------------

<span></span>
**W jaki sposób korzystać z tej tabeli?**

Tabela ta pozwala sprawdzić prawdopodobieństwo opublikowania działającego kodu wykorzystującego lukę w zabezpieczeniach dla każdej z aktualizacji zabezpieczeń, których zainstalowanie może być potrzebne. Aby ustalić priorytety wdrażania, zapoznaj się z dostępnymi poniżej ocenami, rozpatrując je w kontekście posiadanej konfiguracji. Więcej informacji na temat znaczenia tych ocen oraz sposobu ich wyznaczania można znaleźć na stronie sieci Web [Microsoft Exploit Index](http://technet.microsoft.com/en-us/security/cc998259.aspx).

| Identyfikator biuletynu                                             | Tytuł biuletynu                                                                                                                                                                                                  | CVE ID        | Ocena wskaźnika możliwości wykorzystania luki                                                                          | Najważniejsze uwagi                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
|---------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------|------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [MS08-056](http://go.microsoft.com/fwlink/?linkid=128145)           | [Luki w zabezpieczeniach pakietu Microsoft Office mogą pozwolić na ujawnienie informacji (957699)](http://go.microsoft.com/fwlink/?linkid=128145)                                                                | CVE-2008-4020 | [2 — prawdopodobny niespójny kod wykorzystujący lukę](http://technet.microsoft.com/en-us/security/cc998259.aspx)       | Może zostać stworzony działający kod wykorzystujący lukę. Jego wpływ będzie jednak ograniczony, ponieważ luka, której dotyczy, umożliwia fałszowanie zawartości okna dialogowego wyłącznie w przypadkach określonego wykorzystania sieci Web. W związku z tym może ona nie przyciągnąć uwagi osób atakujących.                                                                                                                                                                              |
| [MS08-057](http://technet.microsoft.com/security/bulletin/ms08-057) | [Luki w zabezpieczeniach programu Microsoft Excel umożliwiają zdalne wykonanie kodu (956416)](http://technet.microsoft.com/security/bulletin/ms08-057)                                                           | CVE-2008-4019 | [1 — prawdopodobny spójny kod wykorzystujący lukę](http://technet.microsoft.com/en-us/security/cc998259.aspx)          |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| [MS08-057](http://technet.microsoft.com/security/bulletin/ms08-057) | [Luki w zabezpieczeniach programu Microsoft Excel umożliwiają zdalne wykonanie kodu (956416)](http://technet.microsoft.com/security/bulletin/ms08-057)                                                           | CVE-2008-3471 | [2 — prawdopodobny niespójny kod wykorzystujący lukę](http://technet.microsoft.com/en-us/security/cc998259.aspx)       |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| [MS08-057](http://technet.microsoft.com/security/bulletin/ms08-057) | [Luki w zabezpieczeniach programu Microsoft Excel umożliwiają zdalne wykonanie kodu (956416)](http://technet.microsoft.com/security/bulletin/ms08-057)                                                           | CVE-2008-3477 | [2 — prawdopodobny niespójny kod wykorzystujący lukę](http://technet.microsoft.com/en-us/security/cc998259.aspx)       |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| [MS08-058](http://technet.microsoft.com/security/bulletin/ms08-058) | [Zbiorcza aktualizacja zabezpieczeń dla programu Internet Explorer (956390)](http://technet.microsoft.com/security/bulletin/ms08-058)                                                                            | CVE-2008-2947 | (dostępne publicznie w chwili wydania biuletynu)                                                                       |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| [MS08-058](http://technet.microsoft.com/security/bulletin/ms08-058) | [Zbiorcza aktualizacja zabezpieczeń dla programu Internet Explorer (956390)](http://technet.microsoft.com/security/bulletin/ms08-058)                                                                            | CVE-2008-3472 | [1 — prawdopodobny spójny kod wykorzystujący lukę](http://technet.microsoft.com/en-us/security/cc998259.aspx)          |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| [MS08-058](http://technet.microsoft.com/security/bulletin/ms08-058) | [Zbiorcza aktualizacja zabezpieczeń dla programu Internet Explorer (956390)](http://technet.microsoft.com/security/bulletin/ms08-058)                                                                            | CVE-2008-3473 | [1 — prawdopodobny spójny kod wykorzystujący lukę](http://technet.microsoft.com/en-us/security/cc998259.aspx)          |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| [MS08-058](http://technet.microsoft.com/security/bulletin/ms08-058) | [Zbiorcza aktualizacja zabezpieczeń dla programu Internet Explorer (956390)](http://technet.microsoft.com/security/bulletin/ms08-058)                                                                            | CVE-2008-3475 | [2 — prawdopodobny niespójny kod wykorzystujący lukę](http://technet.microsoft.com/en-us/security/cc998259.aspx)       |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| [MS08-058](http://technet.microsoft.com/security/bulletin/ms08-058) | [Zbiorcza aktualizacja zabezpieczeń dla programu Internet Explorer (956390)](http://technet.microsoft.com/security/bulletin/ms08-058)                                                                            | CVE-2008-3474 | [3 — działający kod wykorzystujący lukę mało prawdopodobny](http://technet.microsoft.com/en-us/security/cc998259.aspx) |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| [MS08-058](http://technet.microsoft.com/security/bulletin/ms08-058) | [Zbiorcza aktualizacja zabezpieczeń dla programu Internet Explorer (956390)](http://technet.microsoft.com/security/bulletin/ms08-058)                                                                            | CVE-2008-3476 | [3 — działający kod wykorzystujący lukę mało prawdopodobny](http://technet.microsoft.com/en-us/security/cc998259.aspx) |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| [MS08-059](http://technet.microsoft.com/security/bulletin/ms08-059) | [Luka w zabezpieczeniach usługi RPC serwera Host Integration Server umożliwia zdalne wykonanie kodu (956695)](http://technet.microsoft.com/security/bulletin/ms08-059)                                           | CVE-2008-3466 | [1 — prawdopodobny spójny kod wykorzystujący lukę](http://technet.microsoft.com/en-us/security/cc998259.aspx)          | Pomimo że program Host Integration Server zainstalują prawdopodobnie tylko klienci biznesowi określonych typów, pojawienie się działającego kodu wykorzystującego lukę jest prawdopodobne.                                                                                                                                                                                                                                                                                                  |
| [MS08-060](http://technet.microsoft.com/security/bulletin/ms08-060) | [Luka w zabezpieczeniach usługi Active Directory umożliwia zdalne wykonanie kodu (957280)](http://technet.microsoft.com/security/bulletin/ms08-060)                                                              | CVE-2008-4023 | [2 — prawdopodobny niespójny kod wykorzystujący lukę](http://technet.microsoft.com/en-us/security/cc998259.aspx)       | Wykorzystanie luki w celu doprowadzenia do sytuacji typu „odmowa usługi” jest prawdopodobne. Jednakże utworzenie działającego kodu wykorzystującego lukę, który pozwoliłby na zdalne wykonanie kodu, byłoby trudne z powodu braku możliwości kontrolowania potrzebnego adresu zapisu.                                                                                                                                                                                                       |
| [MS08-061](http://technet.microsoft.com/security/bulletin/ms08-061) | [Luki w zabezpieczeniach jądra systemu Windows umożliwiają podniesienie poziomu uprawnień (954211)](http://technet.microsoft.com/security/bulletin/ms08-061)                                                     | CVE-2008-2250 | [1 — prawdopodobny spójny kod wykorzystujący lukę](http://technet.microsoft.com/en-us/security/cc998259.aspx)          |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| [MS08-061](http://technet.microsoft.com/security/bulletin/ms08-061) | [Luki w zabezpieczeniach jądra systemu Windows umożliwiają podniesienie poziomu uprawnień (954211)](http://technet.microsoft.com/security/bulletin/ms08-061)                                                     | CVE-2008-2252 | [1 — prawdopodobny spójny kod wykorzystujący lukę](http://technet.microsoft.com/en-us/security/cc998259.aspx)          | Prawdopodobieństwo powstania działającego kodu wykorzystującego lukę jest największe w odniesieniu do systemów wieloprocesorowych.                                                                                                                                                                                                                                                                                                                                                          |
| [MS08-061](http://technet.microsoft.com/security/bulletin/ms08-061) | [Luki w zabezpieczeniach jądra systemu Windows umożliwiają podniesienie poziomu uprawnień (954211)](http://technet.microsoft.com/security/bulletin/ms08-061)                                                     | CVE-2008-2251 | [3 — działający kod wykorzystujący lukę mało prawdopodobny](http://technet.microsoft.com/en-us/security/cc998259.aspx) | Wyzwolenie tej luki jest możliwe, ale utworzenie działającego kodu wykorzystującego lukę byłoby bardzo trudne.                                                                                                                                                                                                                                                                                                                                                                              |
| [MS08-062](http://technet.microsoft.com/security/bulletin/ms08-062) | [Luka w zabezpieczeniach usługi drukowania w Internecie systemu Windows umożliwia zdalne wykonanie kodu (953155)](http://technet.microsoft.com/security/bulletin/ms08-062)                                       | CVE-2008-1446 | [1 — prawdopodobny spójny kod wykorzystujący lukę](http://technet.microsoft.com/en-us/security/cc998259.aspx)          | Wykryto spójny kod wykorzystujący lukę dla niewielkiej liczby ukierunkowanych ataków. Choć usługa protokołu drukowania internetowego (IPP) jest domyślnie włączona, dostęp do niej przy użyciu programu IIS wymaga także domyślnie uwierzytelnienia na wszystkich platformach.                                                                                                                                                                                                              |
| [MS08-063](http://technet.microsoft.com/security/bulletin/ms08-063) | [Luka w zabezpieczeniach protokołu SMB umożliwia zdalne wykonanie kodu (957095)](http://technet.microsoft.com/security/bulletin/ms08-063)                                                                        | CVE-2008-4038 | [2 — prawdopodobny niespójny kod wykorzystujący lukę](http://technet.microsoft.com/en-us/security/cc998259.aspx)       |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| [MS08-064](http://technet.microsoft.com/security/bulletin/ms08-064) | [Luka w zabezpieczeniach obsługi deskryptora adresów wirtualnych umożliwia podniesienie poziomu uprawnień (956841)](http://technet.microsoft.com/security/bulletin/ms08-064)                                     | CVE-2008-4036 | [2 — prawdopodobny niespójny kod wykorzystujący lukę](http://technet.microsoft.com/en-us/security/cc998259.aspx)       |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| [MS08-065](http://technet.microsoft.com/security/bulletin/ms08-065) | [Luka w zabezpieczeniach kolejkowania wiadomości umożliwia zdalne wykonanie kodu (951071)](http://technet.microsoft.com/security/bulletin/ms08-065)                                                              | CVE-2008-3479 | [3 — działający kod wykorzystujący lukę mało prawdopodobny](http://technet.microsoft.com/en-us/security/cc998259.aspx) | Choć potencjalnie może dojść do ujawnienia informacji, to uzyskanie użytecznej zawartości z pamięci bywa niemożliwe. Można wywołać problem związany z uszkodzeniem pamięci, lecz zdalne wykonanie kodu jest trudne do osiągnięcia.                                                                                                                                                                                                                                                          |
| [MS08-066](http://technet.microsoft.com/security/bulletin/ms08-066) | [Luka w zabezpieczeniach pomocniczego sterownika funkcji (Ancillary Function Driver) firmy Microsoft umożliwia podniesienie poziomu uprawnień (956803)](http://technet.microsoft.com/security/bulletin/ms08-066) | CVE-2008-3464 | [1 — prawdopodobny spójny kod wykorzystujący lukę](http://technet.microsoft.com/en-us/security/cc998259.aspx)          |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| [MS08-067](http://technet.microsoft.com/security/bulletin/ms08-067) | [Luka w zabezpieczeniach usługi Serwer umożliwia zdalne wykonanie kodu (958644)](http://technet.microsoft.com/security/bulletin/ms08-067)                                                                        | CVE-2008-4250 | [1 — prawdopodobny spójny kod wykorzystujący lukę](http://technet.microsoft.com/en-us/security/cc998259.aspx)          | Wykryto spójny kod wykorzystujący lukę dla niewielkiej liczby ukierunkowanych ataków dotyczących systemu Windows XP. Usługa ta jest włączona domyślnie na wszystkich platformach, których dotyczy luka, ale jej wykorzystanie jest najbardziej prawdopodobne w systemach Microsoft Windows 2000, Windows XP i Windows Server 2003. Systemy Windows Vista, Windows Server 2008 wymagają uwierzytelnienia, a nawet po uwierzytelnieniu wykorzystanie luki utrudniają rozszerzenia ASLR i DEP. |

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
<th colspan="10">
Microsoft Windows 2000
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS08-067**](http://technet.microsoft.com/security/bulletin/ms08-067)
</td>
<td style="border:1px solid black;">
[**MS08-060**](http://technet.microsoft.com/security/bulletin/ms08-060)
</td>
<td style="border:1px solid black;">
[**MS08-058**](http://technet.microsoft.com/security/bulletin/ms08-058)
</td>
<td style="border:1px solid black;">
[**MS08-066**](http://technet.microsoft.com/security/bulletin/ms08-066)
</td>
<td style="border:1px solid black;">
[**MS08-061**](http://technet.microsoft.com/security/bulletin/ms08-061)
</td>
<td style="border:1px solid black;">
[**MS08-062**](http://technet.microsoft.com/security/bulletin/ms08-062)
</td>
<td style="border:1px solid black;">
[**MS08-063**](http://technet.microsoft.com/security/bulletin/ms08-063)
</td>
<td style="border:1px solid black;">
[**MS08-064**](http://technet.microsoft.com/security/bulletin/ms08-064)
</td>
<td style="border:1px solid black;">
[**MS08-065**](http://technet.microsoft.com/security/bulletin/ms08-065)
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
<td style="border:1px solid black;">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 z dodatkiem Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 z dodatkiem Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=e22eb3ae-1295-4fe2-9775-6f43c5c2aed3)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Usługi Active Directory w systemie Microsoft Windows 2000 Server z dodatkiem Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=8ed7bb9a-4b26-49d7-8c14-60226d2bc20d)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 5.01 z dodatkiem Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=257c0478-56dd-42eb-a90e-607d01613db7)  
(Krytyczny)  
[Microsoft Internet Explorer 6 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=02390258-08e9-4b75-960d-be081b749558)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 z dodatkiem Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=3a6165a6-d7e7-4526-9291-290caf0639b4)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 z dodatkiem Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=8163d1f6-feb5-4f39-8134-3ed42326b822)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 z dodatkiem Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=9ed29c3a-0682-4586-bbc2-a73deaa18e4c)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 z dodatkiem Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=899e2728-2433-4ccb-a195-05b5d65e5469)  
(Ważny)
</td>
</tr>
<tr>
<th colspan="10">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS08-067**](http://technet.microsoft.com/security/bulletin/ms08-067)
</td>
<td style="border:1px solid black;">
[**MS08-060**](http://technet.microsoft.com/security/bulletin/ms08-060)
</td>
<td style="border:1px solid black;">
[**MS08-058**](http://technet.microsoft.com/security/bulletin/ms08-058)
</td>
<td style="border:1px solid black;">
[**MS08-066**](http://technet.microsoft.com/security/bulletin/ms08-066)
</td>
<td style="border:1px solid black;">
[**MS08-061**](http://technet.microsoft.com/security/bulletin/ms08-061)
</td>
<td style="border:1px solid black;">
[**MS08-062**](http://technet.microsoft.com/security/bulletin/ms08-062)
</td>
<td style="border:1px solid black;">
[**MS08-063**](http://technet.microsoft.com/security/bulletin/ms08-063)
</td>
<td style="border:1px solid black;">
[**MS08-064**](http://technet.microsoft.com/security/bulletin/ms08-064)
</td>
<td style="border:1px solid black;">
[**MS08-065**](http://technet.microsoft.com/security/bulletin/ms08-065)
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
<td style="border:1px solid black;">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP z dodatkiem Service Pack 2 i Windows XP z dodatkiem Service Pack 3
</td>
<td style="border:1px solid black;">
[Windows XP z dodatkiem Service Pack 2 i Windows XP z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=0d5f9b6e-9265-44b9-a376-2067b73d6a03)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=a7f0f47b-b1ee-4516-9fbf-bf8e579963d0)  
(Krytyczny)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=4e73de2b-05e6-4901-9bac-46d8f469e635)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows XP z dodatkiem Service Pack 2 i Windows XP z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=b16d9dac-c430-4dd8-a1e5-9a614801f1d9)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows XP z dodatkiem Service Pack 2 i Windows XP z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=7718bf14-c26c-43f3-be67-4c79ab5b2607)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows XP z dodatkiem Service Pack 2 i Windows XP z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=e7ef571f-c9e8-4e14-95a3-3eeaec55b784)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows XP z dodatkiem Service Pack 2 i Windows XP z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=2f7e5981-6eef-4f08-86c0-c6a7607ea5d0)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows XP z dodatkiem Service Pack 2 i Windows XP z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=25997b73-a640-49c1-b19e-768a18bbe22c)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition oraz Microsoft Windows XP Professional x64 Edition z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition oraz Windows XP Professional x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4c16a372-7bf8-4571-b982-dac6b2992b25)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=234c05fb-988b-4e02-aab6-bb23e447df3d)  
(Krytyczny)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=ccf7a3e3-ec30-4b95-9a86-00032301513c)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition oraz Windows XP Professional x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5b607efc-c6fb-4079-8478-e4f3262386d3)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition oraz Windows XP Professional x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b06d3a02-b6e4-4d40-913a-3759a31f20f3)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition oraz Windows XP Professional x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3ae4b913-bff0-4974-b198-828ca10d2a87)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition oraz Windows XP Professional x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4e1675eb-6b06-48e9-9765-23a2c7737bdc)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition oraz Windows XP Professional x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=50fae854-0bde-46f8-9444-b9e0d9bfecad)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr>
<th colspan="10">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS08-067**](http://technet.microsoft.com/security/bulletin/ms08-067)
</td>
<td style="border:1px solid black;">
[**MS08-060**](http://technet.microsoft.com/security/bulletin/ms08-060)
</td>
<td style="border:1px solid black;">
[**MS08-058**](http://technet.microsoft.com/security/bulletin/ms08-058)
</td>
<td style="border:1px solid black;">
[**MS08-066**](http://technet.microsoft.com/security/bulletin/ms08-066)
</td>
<td style="border:1px solid black;">
[**MS08-061**](http://technet.microsoft.com/security/bulletin/ms08-061)
</td>
<td style="border:1px solid black;">
[**MS08-062**](http://technet.microsoft.com/security/bulletin/ms08-062)
</td>
<td style="border:1px solid black;">
[**MS08-063**](http://technet.microsoft.com/security/bulletin/ms08-063)
</td>
<td style="border:1px solid black;">
[**MS08-064**](http://technet.microsoft.com/security/bulletin/ms08-064)
</td>
<td style="border:1px solid black;">
[**MS08-065**](http://technet.microsoft.com/security/bulletin/ms08-065)
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
<td style="border:1px solid black;">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 z dodatkiem Service Pack 1 i Windows Server 2003 z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem Service Pack 1 i Windows Server 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f26d395d-2459-4e40-8c92-3de1c52c390d)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=ae8d22d5-20aa-471d-a423-f54c9d75febe)  
(Umiarkowany)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=feaf2adf-7892-4dbf-a147-db4d5dbe52f3)  
(Niski)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem Service Pack 1 i Windows Server 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ee88ff2d-1b12-4f4c-a081-9f27a6fba074)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem Service Pack 1 i Windows Server 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6e696762-d652-4a8f-ab8f-622f9746c320)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem Service Pack 1 i Windows Server 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=437a9b68-6a0c-48c8-9348-0d6fda48aa21)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem Service Pack 1 i Windows Server 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=dbbebb3f-f1c7-402c-bd16-6f88da0d042c)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 z dodatkiem Service Pack 1 i Windows Server 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e8ef3d5f-dd8e-4945-92cd-9d3e30b16667)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition i Windows Server 2003 x64 Edition z dodatkiem Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition i Windows Server 2003 x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c04d2afb-f9d0-4e42-9e1f-4b944a2de400)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=07fc88c4-2571-4a4d-b573-ae576798ab4c)  
(Umiarkowany)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=319dba34-07ca-47f9-a1e9-20df2df7966b)  
(Niski)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition i Windows Server 2003 x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ab4d94d3-458c-4946-ab7f-03a279629d25)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition i Windows Server 2003 x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=57ca28ea-e5e1-4191-a3d6-84aa90a3d668)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition i Windows Server 2003 x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d3df6508-a568-449d-ac97-fbf3f97b98ef)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition i Windows Server 2003 x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=989ac6f1-515c-467d-a200-2aabe66d9319)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition i Windows Server 2003 x64 Edition z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c2e754f9-086a-494c-bc19-5feed7df8b65)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Systemy operacyjne Windows Server 2003 z dodatkiem SP1 dla systemów z procesorem Itanium oraz Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium
</td>
<td style="border:1px solid black;">
[System operacyjny Windows Server 2003 z dodatkiem SP1 dla systemów z procesorem Itanium oraz Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=ab590756-f11f-43c9-9dcc-a85a43077acf)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=b68937af-f04a-4d1e-9d7f-ec92af5194de)  
(Umiarkowany)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=47381d91-4a14-4a09-96b3-3345155df52d)  
(Niski)
</td>
<td style="border:1px solid black;">
[System operacyjny Windows Server 2003 z dodatkiem SP1 dla systemów z procesorem Itanium oraz Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=63234f85-6e5d-4ef6-b7cf-d1d2c78a5517)  
(Ważny)
</td>
<td style="border:1px solid black;">
[System operacyjny Windows Server 2003 z dodatkiem SP1 dla systemów z procesorem Itanium oraz Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=1e6c3f81-85bb-48e6-a5af-635a7e540c93)  
(Ważny)
</td>
<td style="border:1px solid black;">
[System operacyjny Windows Server 2003 z dodatkiem SP1 dla systemów z procesorem Itanium oraz Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=748f54f1-40b9-407c-9819-909061b53743)  
(Ważny)
</td>
<td style="border:1px solid black;">
[System operacyjny Windows Server 2003 z dodatkiem SP1 dla systemów z procesorem Itanium oraz Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=91589cfb-15ba-4dd2-9e3b-107899fbcba6)  
(Ważny)
</td>
<td style="border:1px solid black;">
[System operacyjny Windows Server 2003 z dodatkiem SP1 dla systemów z procesorem Itanium oraz Windows Server 2003 z dodatkiem SP2 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=5a3832ec-3f8f-42c1-a603-b1330d527547)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr>
<th colspan="10">
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS08-067**](http://technet.microsoft.com/security/bulletin/ms08-067)
</td>
<td style="border:1px solid black;">
[**MS08-060**](http://technet.microsoft.com/security/bulletin/ms08-060)
</td>
<td style="border:1px solid black;">
[**MS08-058**](http://technet.microsoft.com/security/bulletin/ms08-058)
</td>
<td style="border:1px solid black;">
[**MS08-066**](http://technet.microsoft.com/security/bulletin/ms08-066)
</td>
<td style="border:1px solid black;">
[**MS08-061**](http://technet.microsoft.com/security/bulletin/ms08-061)
</td>
<td style="border:1px solid black;">
[**MS08-062**](http://technet.microsoft.com/security/bulletin/ms08-062)
</td>
<td style="border:1px solid black;">
[**MS08-063**](http://technet.microsoft.com/security/bulletin/ms08-063)
</td>
<td style="border:1px solid black;">
[**MS08-064**](http://technet.microsoft.com/security/bulletin/ms08-064)
</td>
<td style="border:1px solid black;">
[**MS08-065**](http://technet.microsoft.com/security/bulletin/ms08-065)
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
<td style="border:1px solid black;">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista i Windows Vista z dodatkiem Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Vista i Windows Vista z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=18fdff67-c723-42bd-ac5c-cac7d8713b21)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=4756e04b-6e1c-4d78-a3c0-17f6b4b97975)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Vista i Windows Vista z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=3483b400-cedc-441f-ba8e-594e3df89190)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Vista i Windows Vista z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=9b5995df-a3b8-4e81-b118-9bb057e19884)  
(Brak wskaźnika ważności)
</td>
<td style="border:1px solid black;">
[Windows Vista i Windows Vista z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=72dd6015-25d1-45f4-a769-88ac43074b44)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Vista i Windows Vista z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=b4212db5-093e-497d-b999-2e3780f9f7c2)  
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
[Windows Vista x64 Edition i Windows Vista x64 Edition z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=a976999d-264f-4e6a-9bd6-3ad9d214a4bd)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=bd19c72b-4f83-47ab-93be-d2c286e732c4)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition i Windows Vista x64 Edition z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=905ab030-14a5-4a3d-aa11-e8f957f6a1ea)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition i Windows Vista x64 Edition z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=4a0fcf4b-eb8e-456a-b934-400ae18248ee)  
(Brak wskaźnika ważności)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition i Windows Vista x64 Edition z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=f793af16-5464-4db1-a42b-1c5f17c538ed)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition i Windows Vista x64 Edition z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c20808cb-c30a-4b53-91e5-810eb6b4b2e3)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr>
<th colspan="10">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS08-067**](http://technet.microsoft.com/security/bulletin/ms08-067)
</td>
<td style="border:1px solid black;">
[**MS08-060**](http://technet.microsoft.com/security/bulletin/ms08-060)
</td>
<td style="border:1px solid black;">
[**MS08-058**](http://technet.microsoft.com/security/bulletin/ms08-058)
</td>
<td style="border:1px solid black;">
[**MS08-066**](http://technet.microsoft.com/security/bulletin/ms08-066)
</td>
<td style="border:1px solid black;">
[**MS08-061**](http://technet.microsoft.com/security/bulletin/ms08-061)
</td>
<td style="border:1px solid black;">
[**MS08-062**](http://technet.microsoft.com/security/bulletin/ms08-062)
</td>
<td style="border:1px solid black;">
[**MS08-063**](http://technet.microsoft.com/security/bulletin/ms08-063)
</td>
<td style="border:1px solid black;">
[**MS08-064**](http://technet.microsoft.com/security/bulletin/ms08-064)
</td>
<td style="border:1px solid black;">
[**MS08-065**](http://technet.microsoft.com/security/bulletin/ms08-065)
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
<td style="border:1px solid black;">
[**Ważny**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 dla systemów 32-bitowych
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów 32-bitowych](http://www.microsoft.com/downloads/details.aspx?familyid=25c17b07-1efe-43d7-9b01-3dfdf1ce0bd7)\*  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=ec73f416-2204-42d6-8932-c96578ac819f)\*\*  
(Niski)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów 32-bitowych](http://www.microsoft.com/downloads/details.aspx?familyid=8b97114a-71aa-47a2-b9e7-f4e158c18c80)\*  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów 32-bitowych](http://www.microsoft.com/downloads/details.aspx?familyid=3d6290d8-1745-4bc0-9ca9-eeb1ad0be4a5)\*  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów 32-bitowych](http://www.microsoft.com/downloads/details.aspx?familyid=cf6744e6-b54c-40f6-a78d-7ba9453133c0)\*  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów 32-bitowych](http://www.microsoft.com/downloads/details.aspx?familyid=ec9eeb82-0497-4c55-94bb-9a47cb3521b4)\*  
(Ważny)
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
[Windows Server 2008 dla systemów opartych na procesorach X64](http://www.microsoft.com/downloads/details.aspx?familyid=7b12018e-0cc1-4136-a68c-be4e1633c8df)\*  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=baacd1c2-9764-4fea-bd4d-c49791974fef)\*\*  
(Niski)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów opartych na procesorach X64](http://www.microsoft.com/downloads/details.aspx?familyid=6e641db2-90c8-458f-9795-3e46b70a5203)\*  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów opartych na procesorach X64](http://www.microsoft.com/downloads/details.aspx?familyid=a33c833c-d5c5-4e37-8f89-7b9079f92e59)\*  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów opartych na procesorach X64](http://www.microsoft.com/downloads/details.aspx?familyid=223236e8-7b19-4b47-8a90-bfc35eb9318a)\*  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów opartych na procesorach X64](http://www.microsoft.com/downloads/details.aspx?familyid=0bc178b8-f8ae-4f41-8f88-fb6a75be1bca)\*  
(Ważny)
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
[Windows Server 2008 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=2bcf89ef-6446-406c-9c53-222e0f0baf7a)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=250a45dd-7eae-4440-bd10-02a703940976)  
(Niski)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=b6546e1c-bf7b-4354-8574-6c16fa707de0)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=31783e88-76e2-4bc6-b4ae-308443c6d223)  
(Brak wskaźnika ważności)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=077b697c-04a0-45bd-b08c-331d5c30cb47)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 dla systemów z procesorem Itanium](http://www.microsoft.com/downloads/details.aspx?familyid=0af72663-4945-4916-8c55-090ba4d82793)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
</table>
 
**\* Luka w zabezpieczeniach dotyczy instalacji Server Core systemu operacyjnego Windows Server 2008.** W przypadku obsługiwanych wersji systemu Windows Server 2008 ta aktualizacja ma zastosowanie, z takim samym wskaźnikiem ważności, niezależnie od tego, czy system Windows Server 2008 został zainstalowany przy użyciu opcji instalacji Server Core. Aby uzyskać więcej informacji na temat tej opcji instalacji, zobacz [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Należy pamiętać, że opcja instalacji Server Core nie dotyczy niektórych wersji systemu Windows Server 2008; zobacz [Porównanie opcji instalacji Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\* Luka w zabezpieczeniach nie dotyczy instalacji Server Core systemu operacyjnego Windows Server 2008.** Lukom usuwanym przez te aktualizacje zabezpieczeń nie podlegają obsługiwane wersje systemu Windows Server 2008, jeżeli system Windows Server 2008 został zainstalowany przy użyciu opcji instalacji Server Core. Aby uzyskać więcej informacji na temat tej opcji instalacji, zobacz [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Należy pamiętać, że opcja instalacji Server Core nie dotyczy niektórych wersji systemu Windows Server 2008; zobacz [Porównanie opcji instalacji Server Core](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

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
[**MS08-057**](http://technet.microsoft.com/security/bulletin/ms08-057)
</td>
<td style="border:1px solid black;">
[**MS08-056**](http://go.microsoft.com/fwlink/?linkid=128145)
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
[**Umiarkowany**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2000 z dodatkiem Service Pack 3
</td>
<td style="border:1px solid black;">
[Excel 2000 z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=1b2740e0-ecdd-48ca-84e0-eb187c31eb16)  
(KB955461)  
(Krytyczny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office XP z dodatkiem Service Pack 3
</td>
<td style="border:1px solid black;">
[Excel 2002 z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=27cedef1-c47c-472c-a343-cd9b4ebc2bba)  
(KB955464)  
(Ważny)
</td>
<td style="border:1px solid black;">
[Microsoft Office XP z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=b1aee2d5-bfa0-40e3-91b6-98bf65524e8c)  
(KB956464)  
(Umiarkowany)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2003 z dodatkiem Service Pack 2 i Microsoft Office 2003 z dodatkiem Service Pack 3
</td>
<td style="border:1px solid black;">
[Excel 2003 z dodatkiem Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4df27e8a-d803-483b-a700-0177d71bf368)  
(KB955466)  
(Ważny)  
[Excel 2003 z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=4df27e8a-d803-483b-a700-0177d71bf368)  
(KB955466)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2007 i Microsoft Office 2007 z dodatkiem Service Pack 1
</td>
<td style="border:1px solid black;">
[Excel 2007](http://www.microsoft.com/downloads/details.aspx?familyid=2765bbc0-ea2e-4b6e-822c-222ee8e5021f)  
(KB955470)  
(Ważny)  
[Excel 2007 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=2765bbc0-ea2e-4b6e-822c-222ee8e5021f)  
(KB955470)  
(Ważny)
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
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS08-057**](http://technet.microsoft.com/security/bulletin/ms08-057)
</td>
<td style="border:1px solid black;">
[**MS08-056**](http://go.microsoft.com/fwlink/?linkid=128145)
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
[**Umiarkowany**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2004 dla komputerów Macintosh
</td>
<td style="border:1px solid black;">
[Microsoft Office 2004 dla komputerów Macintosh](http://www.microsoft.com/downloads/details.aspx?familyid=ba4fa21a-7e01-4ef8-9b9f-9d51d00ef094)  
(KB958312)  
(Ważny)
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
[Microsoft Office 2008 dla komputerów Macintosh](http://www.microsoft.com/downloads/details.aspx?familyid=e70c5ae0-2858-46de-81f8-dcd1786656b7)  
(KB958267)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Open XML File Format Converter for Mac
</td>
<td style="border:1px solid black;">
[Open XML File Format Converter dla komputerów Macintosh](http://www.microsoft.com/downloads/details.aspx?familyid=2a8d9a3b-b8a4-43b6-82a6-a2e7d16ae11d)  
(KB958304)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
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
[**MS08-057**](http://technet.microsoft.com/security/bulletin/ms08-057)
</td>
<td style="border:1px solid black;">
[**MS08-056**](http://go.microsoft.com/fwlink/?linkid=128145)
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
[**Umiarkowany**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Przeglądarka programu Microsoft Office Excel
</td>
<td style="border:1px solid black;">
[Podgląd programu Microsoft Office Excel 2003](http://www.microsoft.com/downloads/details.aspx?familyid=9769ce08-5207-4c63-b7b9-536266ad6b2b)  
(KB955468)  
(Ważny)  
[Przeglądarka programu Microsoft Office Excel 2003 z dodatkiem Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=9769ce08-5207-4c63-b7b9-536266ad6b2b)  
(KB955468)  
(Ważny)  
[Przeglądarka programu Microsoft Office Excel](http://www.microsoft.com/downloads/details.aspx?familyid=83c88444-75b8-44d1-b280-3671394ade45)  
(KB955935)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Pakiet zgodności formatu plików pakietu Microsoft Office dla programów Word, Excel i PowerPoint 2007
</td>
<td style="border:1px solid black;">
[Pakiet zgodności formatu plików pakietu Microsoft Office dla programów Word, Excel i PowerPoint 2007](http://www.microsoft.com/downloads/details.aspx?familyid=9a7be004-5903-4101-90c5-c0d5f8722af9)  
(KB955936)  
(Ważny)  
[Pakiet zgodności formatu plików pakietu Microsoft Office dla programów Word, Excel i PowerPoint 2007 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=9a7be004-5903-4101-90c5-c0d5f8722af9)  
(KB955936)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office SharePoint Server 2007
</td>
<td style="border:1px solid black;">
[Microsoft Office SharePoint Server 2007](http://www.microsoft.com/downloads/details.aspx?familyid=5c29e646-504c-4455-9d35-9a1bed6d7535)\*  
(KB955937)  
(Ważny)  
[Microsoft Office SharePoint Server 2007 z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=5c29e646-504c-4455-9d35-9a1bed6d7535)\*  
(KB955937)  
(Ważny)  
[Microsoft Office SharePoint Server 2007 x64 Edition](http://www.microsoft.com/downloads/details.aspx?familyid=3c21c405-2c9e-45d0-be4d-8ccd093af31f)\*  
(KB955937)  
(Ważny)  
[Microsoft Office SharePoint Server 2007 x64 Edition z dodatkiem Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=3c21c405-2c9e-45d0-be4d-8ccd093af31f)\*  
(KB955937)  
(Ważny)
</td>
<td style="border:1px solid black;">
Nie dotyczy
</td>
</tr>
</table>
 
\*Ta aktualizacja zabezpieczeń dotyczy serwerów z zainstalowanymi usługami programu Excel, takich jak Microsoft Office SharePoint Server 2007 Enterprise i Microsoft Office SharePoint Server 2007 For Internet Sites w konfiguracji domyślnej. Serwer Microsoft Office SharePoint Server 2007 Standard nie zawiera usług programu Excel.

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
Microsoft Host Integration Server
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Identyfikator biuletynu**
</td>
<td style="border:1px solid black;">
[**MS08-059**](http://technet.microsoft.com/security/bulletin/ms08-059)
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
Microsoft Host Integration Server 2000
</td>
<td style="border:1px solid black;">
[Microsoft Host Integration Server 2000 z dodatkiem Service Pack 2 (Serwer)](http://www.microsoft.com/downloads/details.aspx?familyid=11cca58b-59a4-4e93-9eb1-19b07c290a10)  
(Krytyczny)  
[Microsoft Host Integration Server 2000 Administrator Client](http://www.microsoft.com/downloads/details.aspx?familyid=41b49291-1231-4e23-aef7-818207453d56)  
(Krytyczny)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Host Integration Server 2004
</td>
<td style="border:1px solid black;">
[Microsoft Host Integration Server 2004 (Serwer)](http://www.microsoft.com/downloads/details.aspx?familyid=9ca255ed-9334-4848-af94-49ef3078cdc0)  
(Krytyczny)  
[Microsoft Host Integration Server 2004 z dodatkiem Service Pack 1 (Serwer)](http://www.microsoft.com/downloads/details.aspx?familyid=eca756a1-ca56-4481-b23c-53c159a4e08c)  
(Krytyczny)  
[Microsoft Host Integration Server 2004 (Klient)](http://www.microsoft.com/downloads/details.aspx?familyid=92cb54e7-f4ff-40a4-99cb-6257c4d8d4cd)  
(Krytyczny)  
[Microsoft Host Integration Server 2004 z dodatkiem Service Pack 1 (Klient)](http://www.microsoft.com/downloads/details.aspx?familyid=d776515c-09aa-4a04-876d-606bfc26a006)  
(Krytyczny)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Host Integration Server 2006
</td>
<td style="border:1px solid black;">
[Microsoft Host Integration Server 2006 dla systemów 32-bitowych](http://www.microsoft.com/downloads/details.aspx?familyid=1ae79da3-ec17-4d4b-8011-d777a237ac93)  
(Krytyczny)  
[Microsoft Host Integration Server 2006 dla systemów opartych na procesorach x64](http://www.microsoft.com/downloads/details.aspx?familyid=05da4540-4976-458a-a612-7385d78695a2)  
(Krytyczny)
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

**Narzędzie Microsoft Baseline Security Analyzer**

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

-   Alex Ionescu (<http://www.alex-ionescu.com/>) za zgłoszenie problemu opisanego w biuletynie MS08-056
-   [NetAgent Co., Ltd.](http://www.netagent.co.jp/), za zgłoszenie problemu opisanego w biuletynie MS08-056
-   Joshua J. Drake z firmy [iDefense](http://labs.idefense.com/), za zgłoszenie problemu opisanego w biuletynie MS08-057
-   Wushi, współpracownik firm [TippingPoint](http://www.tippingpoint.com/) i [Zero Day Initiative,](http://www.zerodayinitiative.com/) za zgłoszenie problemu opisanego w biuletynie MS08-057
-   Lionel d'Hauenens z firmy [Labo Skopia](http://www.laboskopia.com/), we współpracy z firmą [iDefense VCP](http://labs.idefense.com/), za zgłoszenie problemu opisanego w biuletynie MS08-057
-   David Bloom, za zgłoszenie problemu opisanego w biuletynie MS08-058
-   Gregory Rubin, za zgłoszenie problemu opisanego w biuletynie MS08-058
-   [Ivan Frantic](http://ifsec.blogspot.com/), współpracownik firm [TippingPoint](http://www.tippingpoint.com/) i [Zero Day Initiative](http://www.zerodayinitiative.com/), za zgłoszenie problemu opisanego w biuletynie MS08-058
-   Thierry Zoller z firmy [n.runs](http://www.nruns.com/), za zgłoszenie problemu opisanego w biuletynie MS08-058
-   Lee Dagon z firmy [Composica](http://www.composica.com/), za zgłoszenie problemu opisanego w biuletynie MS08-058
-   Stephen Fewer z firmy [Harmony Security](http://www.harmonysecurity.com/), współpracownik firmy [iDefense VCP](http://labs.idefense.com/), za zgłoszenie problemu opisanego w biuletynie MS08-059
-   Paul Miseiko z firmy [nCircle](http://www.ncircle.com/), za zgłoszenie problemu opisanego w biuletynie MS08-060
-   Paul Caton z firmy [iShadow](http://www.ishadow.com/), za zgłoszenie problemu opisanego w biuletynie MS08-061
-   Thomas Garnier z firmy [SkyRecon](http://www.skyrecon.com/), za zgłoszenie problemu opisanego w biuletynie MS08-061
-   [CERT/CC](http://www.cert.org/) za zgłoszenie problemu opisanego w biuletynie MS08-062
-   Joshua Morin z firmy [Codenomicon](http://www.codenomicon.com/), za zgłoszenie problemu opisanego w biuletynie MS08-063
-   Cody Pierce i Aaron Portnoy z firmy [TippingPoint DVLabs](http://dvlabs.tippingpoint.com), za zgłoszenie problemu opisanego w biuletynie MS08-065
-   Fabien Le Mentec z firmy [SkyRecon](http://www.skyrecon.com/), za zgłoszenie problemu opisanego w biuletynie MS08-066

#### Pomoc techniczna

-   Wymienione oprogramowanie zostało przetestowane w celu ustalenia, których wersji dotyczy problem. Dla pozostałych wersji upłynął okres pomocy technicznej. Aby zapoznać się z zasadami cyklu pomocy technicznej dotyczącymi używanej wersji oprogramowania, odwiedź [witrynę zasad cyklu pomocy technicznej firmy Microsoft](http://go.microsoft.com/fwlink/?linkid=21742).
-   Klienci mogą uzyskać pomoc techniczną w [Biurze Obsługi Klienta Microsoft](http://go.microsoft.com/fwlink/?linkid=21131) pod numerem 0 801 802 000 (Opłata według stawek Twojego operatora) lub (0-22) 594 19 99 w godzinach od 9:00 do 17:00, od poniedziałku do piątku. Połączenia z działem pomocy technicznej związane z aktualizacjami zabezpieczeń są bezpłatne.
-   Klienci międzynarodowi mogą uzyskać pomoc w lokalnych przedstawicielstwach firmy Microsoft. Pomoc techniczna związana z aktualizacjami zabezpieczeń jest bezpłatna. Informacje o sposobie kontaktowania się z pomocą techniczną firmy Microsoft są dostępne w [międzynarodowej witrynie sieci Web pomocy i obsługi technicznej](http://go.microsoft.com/fwlink/?linkid=21155).

#### Zrzeczenie odpowiedzialności

Informacje w bazie wiedzy Microsoft Knowledge Base są dostarczane „tak jak są” bez jakiejkolwiek gwarancji. Firma Microsoft odrzuca wszelkie gwarancje, wyraźne i dorozumiane, w tym gwarancje dotyczące wartości handlowej i przydatności do określonego celu. Firma Microsoft Corporation ani jej dostawcy w żadnym wypadku nie ponoszą odpowiedzialności za jakiekolwiek szkody, w tym bezpośrednie, pośrednie, przypadkowe, wynikowe, utratę zysków handlowych lub szkody specjalne, nawet jeżeli firmę Microsoft Corporation lub jej dostawców powiadomiono o możliwości zaistnienia takich szkód. W niektórych stanach wyłączenie lub ograniczenie odpowiedzialności za straty wynikowe lub przypadkowe, a więc i powyższe ograniczenia, nie mają zastosowania.

#### Wersje

-   Wersja 1.0 (14 października 2008 r.): Opublikowane podsumowanie biuletynów zabezpieczeń.
-   Wersja 2.0 (15 października 2008 r.): Usunięto wskaźnik ważności dla systemu Windows Server 2008 dla komputerów z procesorem Itanium (MS08-062).
-   Wersja 2.1 (16 października 2008 r.): Zaktualizowano sekcję „Streszczenie” dotyczącą biuletynu zabezpieczeń firmy Microsoft MS08-062.
-   Wersja 3.0 (23 października 2008 r.): Dodano Biuletyn zabezpieczeń firmy Microsoft MS08-067, Luka w zabezpieczeniach usługi Serwer umożliwia zdalne wykonanie kodu (958644). Ponadto dodano link do webcastu dla biuletynu po za cyklem produkcyjnym.

*Built at 2014-04-18T01:50:00Z-07:00*
