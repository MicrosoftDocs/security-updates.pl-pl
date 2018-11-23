---
TOCTitle: Administracyjna witryna sieci Web programu RMS
Title: Administracyjna witryna sieci Web programu RMS
ms:assetid: 'f003c1d9-9a17-4e50-9e1e-5d67677552a0'
ms:contentKeyID: 18123522
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747796(v=WS.10)'
---

Administracyjna witryna sieci Web programu RMS
==============================================

Każdy klaster główny lub klaster licencji obsługuje administracyjną witrynę sieci Web, która służy do zarządzania programem RMS. Ta witryna sieci Web jest dostępna tylko na administrowanym serwerze programu RMS lub poprzez połączenie pulpitu zdalnego.

W tym temacie opisano możliwości administracyjnej witryny sieci Web. Instrukcje dotyczące administrowania programem RMS za pomocą witryny sieci Web można znaleźć w punktach „RMS - Jak...” i „Zarządzanie programem RMS” w części dotyczącej operacji w programie RMS w niniejszym zestawie dokumentów.

**Uwaga** Konfiguracja klastra jest globalna. Konfiguracją klastra można zarządzać z administracyjnej witryny sieci Web znajdującej się na dowolnym serwerze w klastrze.

Otwarcie strony **Administracja globalna** umożliwia wykonanie następujących zadań:

-   Zastrzeżenie programu RMS w witrynie sieci Web.
-   Zastrzeżenie serwera i dodanie go do klastra.
-   Usunięcie programu RMS z witryny sieci Web.
-   Przejście do stron administracyjnych dla klastra.

Otwarcie strony **Administracja** klastra umożliwia wykonanie następujących zadań:

-   **Wyświetlanie informacji o klastrze.** Można wyświetlić informacje o klastrze, takie jak adres URL instalacji, adres URL serwera, nazwa certyfikatu, serwer bazy danych konfiguracji, nazwa bazy danych konfiguracji oraz data wygaśnięcia certyfikatu.
-   **Rejestrowanie i odnawianie certyfikatu licencjodawcy serwera.** Można zarejestrować lub odnowić certyfikat licencjodawcy klastra.
-   **Ustanawianie zasad zaufania.**Należy kliknąć łącze, aby otworzyć stronę sieci Web Zasady zaufania, za pomocą której można dodawać lub usuwać zaufane domeny użytkowników oraz zaufane domeny publikacji. Można dodać lub usunąć użytkowników z listy wykluczania znajdującej się w zaufanej domenie użytkowników. Można wyeksportować certyfikat licencjodawcy serwera do pliku w celu zaimportowania go w innej instalacji RMS.
-   **Konfigurowanie szablonów zasad praw dostępu.** Należy kliknąć łącze, aby otworzyć stronę sieci Web Szablony zasad praw dostępu, za pomocą której można tworzyć i modyfikować szablony zasad praw dostępu dla firmy.
-   **Konfigurowanie rejestrowania.** Należy kliknąć łącze, aby otworzyć stronę sieci Web Ustawienia rejestrowania, za pomocą której można włączyć i wyłączyć rejestrowanie. Następnie można przejrzeć serwer i bazę danych rejestrowania.
-   **Określanie adresu URL klastra ekstranetowego.** Należy kliknąć łącze, aby otworzyć stronę sieci Web z ustawieniami adresu URL klastra ekstranetowego, za pomocą której można określić adres URL używany do uzyskiwania dostępu z sieci ekstranet do usług certyfikacji klastra głównego.
-   **Określanie ustawień serwera proxy programu RMS.** Należy kliknąć łącze, aby otworzyć stronę sieci Web Ustawienia serwera proxy programu RMS, za pomocą której można określić adres serwera proxy, typ uwierzytelniania oraz nazwę użytkownika stosowaną w sytuacji, gdy serwer programu RMS musi połączyć się z Internetem za pośrednictwem serwera proxy.
-   **Śledzenie liczby rozpowszechnionych certyfikatów kont praw.** Należy kliknąć łącze, aby otworzyć stronę sieci Web śledzenia certyfikatów kont praw, za pomocą której można poznać liczbę certyfikatów kont praw rozpowszechnionych przez klaster główny. Tej liczby można użyć w celu oszacowania liczby wymaganych licencji dostępu klienta.
-   **Zarządzanie ustawieniami zabezpieczeń.** Należy kliknąć łącze, aby otworzyć stronę sieci Web Ustawienia zabezpieczeń, za pomocą której można dodawać i usuwać członków grupy administratorów mających pełną kontrolę nad licencjonowaną zawartością. Można również zresetować hasło klucza prywatnego.
-   **Wyświetlanie i konfigurowanie ustawień certyfikatów kont.** Należy kliknąć łącze, aby otworzyć stronę sieci Web Ustawienia certyfikacji, za pomocą której można określić okres ważności oraz informacje o kontakcie administratora.
-   **Włączanie zasad wykluczania.** Należy kliknąć łącze, aby otworzyć stronę sieci Web Zasady wykluczania, za pomocą której można włączyć zasady wykluczania na podstawie wersji skrytek, wersji systemu Windows, certyfikatów kont oraz aplikacji.
-   **Rejestrowanie punktu połączenia usługi.** Należy kliknąć łącze, aby otworzyć stronę sieci Web Punkt połączenia usługi, za pomocą której można zarejestrować lub wyrejestrować punkt połączenia usługi dla klastra.

Administratorzy mogą wykonywać inne zadania, w tym monitorowanie zdarzeń i zarządzanie usługą Active Directory, Internetowymi usługami informacyjnymi (IIS) oraz programem SQL Server, za pomocą programu Microsoft Management Console (MMC).
