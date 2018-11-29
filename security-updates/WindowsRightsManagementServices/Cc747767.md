---
TOCTitle: Likwidowanie programu RMS
Title: Likwidowanie programu RMS
ms:assetid: 'dbcacce7-434d-48a7-a11d-ef9690d78b44'
ms:contentKeyID: 18123480
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747767(v=WS.10)'
---

Likwidowanie programu RMS
=========================

Likwidowanie oznacza cały proces usuwania serwera programu RMS i odpowiednich baz danych z organizacji. Proces ten umożliwia usunięcie programu RMS z infrastruktury bez utraty dostępu do informacji chronionych technologią RMS. Poniżej przedstawiono potencjalne przyczyny, dla których organizacja może być zmuszona do usunięcia serwera programu RMS z infrastruktury:

-   Migracja serwera programu RMS w wersji do zatwierdzenia ze środowiska pilotażowego do środowiska produkcyjnego.
-   Uproszczenie architektury poprzez usunięcie i skonsolidowanie serwerów licencji w głównym klastrze programu RMS.
-   Łączenie serwerów programu RMS (np. w wyniku fuzji lub przejęcia firmy) poprzez zintegrowanie dwóch infrastruktur programu RMS w jedną.
-   Decyzja o zaprzestaniu zabezpieczania zawartości za pomocą programu RMS.

Ponieważ aktywny serwer programu RMS jest zintegrowany zarówno z serwerem bazy danych, jak i usługą Active Directory, oraz oczywiście pozostawia cały zestaw zawartości chroniony za pomocą klucza (klucz ten znajduje się na serwerze programu RMS), usunięcie programu RMS z organizacji wymaga wykonania większej liczby czynności niż zwykłe usunięcie go z serwera. W tej sekcji omówiono czynności, dzięki którym można zlikwidować serwer programu RMS, jeśli to konieczne.

W tej części omówiono następujące zagadnienia:

-   [Opis procesu likwidacji](https://technet.microsoft.com/57bd9949-9433-437b-93ed-ffb2dff9992e)
-   [Włączanie usługi likwidowania](https://technet.microsoft.com/45226e85-b50d-41cc-aca7-0f603f8509d5)
-   [Ustawianie uprawnień do katalogu wirtualnego](https://technet.microsoft.com/45112111-9608-45b1-9a86-7b313d0a1579)
-   [Usuwanie ochrony technologią RMS z zawartości](https://technet.microsoft.com/c30361e3-50d2-4474-a87d-d38de502cf9e)
-   [Usuwanie usługi sieci Web (usuwanie zastrzeżenia programu RMS)](https://technet.microsoft.com/68b4e2b0-b1b7-4b0a-8c1a-82ac27c1f12e)
-   [Usuwanie plików programu RMS](https://technet.microsoft.com/d1dc8a8b-f8de-487f-87b4-2174d449f0bc)
-   [Alternatywy do likwidacji programu RMS](https://technet.microsoft.com/4d32f35e-997d-4d10-ab66-efe217e853f7)
