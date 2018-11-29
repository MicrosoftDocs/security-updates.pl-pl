---
TOCTitle: Rozbudowa infrastruktury podstawowej w celu obsługi klastrowania
Title: Rozbudowa infrastruktury podstawowej w celu obsługi klastrowania
ms:assetid: '78f0f2f0-a075-409c-9f46-26eb62d1d05b'
ms:contentKeyID: 18123323
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747567(v=WS.10)'
---

Rozbudowa infrastruktury podstawowej w celu obsługi klastrowania
================================================================

W przypadku implementowania klastrów w dużych instalacjach należy upewnić się, że infrastruktura jest skonfigurowana do obsługi wymagań klastrów. W planach rozmieszczania należy uwzględnić poniższe elementy.

Rejestracja DNS
---------------

Należy upewnić się, że rejestracja DNS wykonywana w celu prezentacji wirtualnego adresu IP w sieci ekstranet jest także wykonywana w celu prezentacji adresu w sieci intranet.

Jeśli rejestracja DNS nie została wykonana dla sieci intranet, wewnętrzne żądania licencji klientów będą odrzucane. Jeśli nie można zmodyfikować ustawień DNS, można zmodyfikować tabelę hostów na każdym serwerze w klastrze w celu mapowania adresu URL klastra na wirtualny adres IP klastra. Rejestracja DNS musi być wykonana przed zastrzeżeniem usługi. Jeśli już wykonano zastrzeganie usługi, należy usunąć program RMS z serwera i ponownie wykonać proces zastrzegania.

Równoważenie obciążenia
-----------------------

Należy skonfigurować wymagany sprzęt i oprogramowanie, aby umożliwić rozmieszczenie serwerów równoważenia obciążenia, usługi równoważenia obciążenia sieci lub sprzętowego systemu równoważenia obciążenia w celu dystrybucji żądań w klastrze.
