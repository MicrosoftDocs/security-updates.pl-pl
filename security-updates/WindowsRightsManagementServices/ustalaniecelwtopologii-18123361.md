---
TOCTitle: Ustalanie celów topologii
Title: Ustalanie celów topologii
ms:assetid: '8275a04d-3e5b-40b0-be9d-2f31b7aeca6b'
ms:contentKeyID: 18123361
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747652(v=WS.10)'
---

Ustalanie celów topologii
=========================

Jednym z najważniejszych etapów projektowania topologii jest ustalenie odpowiednich celów. Niektóre kluczowe obszary, które należy uwzględnić w projekcie topologii programu RMS, to:

-   **Koszty administracyjne**. Topologia lokacji musi minimalizować koszty administracyjne. Minimalizacja kosztów obejmuje scentralizowane zarządzanie serwerami (jeśli jest możliwe) oraz minimalizację liczby używanych serwerów.
-   **Czas oczekiwania sieci**. Użytkownicy mogą zaobserwować czas oczekiwania w sieci między klientem i serwerem jako dodatkowe opóźnienie przy otwieraniu wiadomości e-mail i dokumentów. Ogólnie czas oczekiwania nie powinien przekraczać dwóch sekund w każdym kierunku przez co najmniej 90 procent czasu.
-   **Niezawodność**. Sieć między klientem a serwerem powinna być niezawodna do tego stopnia, aby w przypadku pojedynczego żądania i odpowiedzi HTTP współczynnik błędu (utraty lub uszkodzenia transakcji) był mniejszy niż 5 procent.

Są to tylko ogólne wskazówki; należy ustalić własne cele na podstawie wymagań i zasobów organizacji. Ustalenie celów jest punktem wyjścia w procesie sprawdzania, czy topologia spełnia wymagania. Istnieje wiele czynników mających wpływ na spełnienie wymagań. Są to między innymi liczba użytkowników, żądań licencji, kwerend, wiadomości i inne czynniki dotyczące ruchu związanego z programem RMS. Ponadto strategia rozmieszczania, w tym ustalenie, w których domenach i lasach zostanie rozmieszczony program RMS, może mieć znaczący wpływ na osiągniecie celów topologii. Po ukończeniu procesu projektowania topologii należy zapamiętać cele i określić, w jaki sposób poszczególne procesy projektowania będą wpływać na ustalone cele.
