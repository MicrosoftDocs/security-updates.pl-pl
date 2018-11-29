---
TOCTitle: Najważniejsze wskazówki dotyczące administrowania programem RMS
Title: Najważniejsze wskazówki dotyczące administrowania programem RMS
ms:assetid: '385f8112-da00-417f-a2b8-42dc1e06b717'
ms:contentKeyID: 18123230
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720245(v=WS.10)'
---

Najważniejsze wskazówki dotyczące administrowania programem RMS
===============================================================

Należy zapoznać się z poniższymi najważniejszymi wskazówkami dotyczącymi administrowania programem RMS.

-   **Nie należy rozmieszczać dodatkowych usług na serwerach programu RMS**
    Jeśli na serwerach zostaną uruchomione usługi inne niż usługi programu RMS, mogą wystąpić konflikty powodujące zagrożenia zabezpieczeń. Do wykrywania awarii usługi lub konfliktów służą liczniki wydajności.
-   **Należy często wykonywać kopie zapasowe baz danych konfiguracji**
    W bazach danych konfiguracji przechowywane są informacje krytyczne dla funkcjonowania programu RMS. Dodatkowo w bazie danych konfiguracji klastra głównej certyfikacji przechowywane są pary kluczy dla całej instalacji. Regularne wykonywanie kopii zapasowych umożliwia szybkie przywrócenie działania programu RMS w przypadku awarii serwera baz danych. Oprócz regularnego wykonywania kopii zapasowych należy regularnie sprawdzać ich ważność, przywracając z nich dane „na sucho” (w niezależnym środowisku testowym). Aby uzyskać więcej informacji, zobacz „Tworzenie kopii zapasowych systemu RMS i jego przywracanie” w części „Planowanie rozmieszczenia programu RMS” w tym zestawie dokumentacji.
-   **Należy regularnie konserwować bazę danych rejestrowania**
-   **Należy monitorować serwer programu RMS za pomocą narzędzia Microsoft Operations Manager (MOM)**
    Narzędzie MOM i pakiet RMS MOM Pack służą do wykrywania krytycznych zdarzeń i wykrywania spadków wydajności oraz wysyłania powiadomień o tych zdarzeniach.
