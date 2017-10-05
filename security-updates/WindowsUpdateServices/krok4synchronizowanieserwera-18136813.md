---
TOCTitle: 'Krok 4. Synchronizowanie serwera'
Title: 'Krok 4. Synchronizowanie serwera'
ms:assetid: 'a5514e46-a50b-46a6-9e5b-33c87c5b7cef'
ms:contentKeyID: 18136813
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc708523(v=WS.10)'
---

Krok 4. Synchronizowanie serwera
================================

Aktualizacje można pobierać po skonfigurowaniu połączenia sieciowego. Domyślnie program WSUS jest skonfigurowany do pobierania aktualizacji krytycznych oraz aktualizacji zabezpieczeń dotyczących wszystkich produktów firmy Microsoft. Aby pobrać aktualizacje, należy *zsynchronizować* serwer WSUS.

Operacja synchronizacji dotyczy serwera WSUS połączonego z witryną Microsoft Update. Po nawiązaniu połączenia program WSUS ustala, czy od czasu ostatniej synchronizacji zostały udostępnione nowe aktualizacje. W przypadku pierwszej synchronizacji serwera WSUS wszystkie aktualizacje są dostępne i gotowe do zatwierdzenia do instalacji.

| ![](images/Cc708523.note(WS.10).gif)Uwaga                                                                                                                                                                                                                                                                                                         |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| W tym dokumencie została opisana synchronizacja przy użyciu ustawień domyślnych, ale w programie WSUS można skorzystać z opcji pozwalających na zminimalizowanie wykorzystania przepustowości w procesie synchronizacji. Więcej informacji można znaleźć w oficjalnym dokumencie „Deploying Microsoft Windows Server Update Services” (dokument dostępny w języku angielskim). |

**Aby przeprowadzić synchronizację serwera WSUS:**
1.  Na pasku narzędzi konsoli WSUS kliknij ikonę **Opcje**, a następnie kliknij pozycję **Opcje synchronizacji**.

2.  W obszarze **Zadania** kliknij pozycję **Synchronizuj teraz**.

Po zakończeniu synchronizacji na pasku narzędzi konsoli WSUS kliknij ikonę **Aktualizacje** w celu wyświetlenia listy aktualizacji.
