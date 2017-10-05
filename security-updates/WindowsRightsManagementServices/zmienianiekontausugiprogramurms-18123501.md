---
TOCTitle: Zmienianie konta usługi programu RMS
Title: Zmienianie konta usługi programu RMS
ms:assetid: 'f257d66d-b823-41e4-bcb7-7c90eb295238'
ms:contentKeyID: 18123501
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747736(v=WS.10)'
---

Zmienianie konta usługi programu RMS
====================================

Podczas instalacji program RMS tworzy na lokalnym komputerze grupę usługi programu RMS i udziela jej odpowiednich uprawnień do wszystkich zasobów, których wymaga działanie programu RMS. Podczas zastrzegania programu RMS na serwerze definiuje się konto usługi programu RMS przy użyciu konta domeny. Jako konta usługi programu RMS nie można użyć konta domeny, za pomocą którego instalowano program RMS. To konto staje się członkiem grupy usługi programu RMS i uzyskuje uprawnienia skojarzone z tą grupą. W normalnych warunkach program RMS działa na koncie usługi programu RMS.

Konto usługi programu RMS można zmienić w dowolnym momencie. W takim przypadku poprzednio określone konto jest automatycznie usuwane z grupy usługi programu RMS, a nowe konto staje się jej członkiem.

| ![](images/Cc747736.Important(WS.10).gif)Ważne                                                                                                                                                                               |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Ze względów bezpieczeństwa zaleca się utworzenie specjalnego konta użytkownika, które będzie używane wyłącznie jako konto usługi programu RMS i nie będzie służyło do innych celów. Ponadto kontu temu nie należy udzielać żadnych dodatkowych uprawnień. |

| ![](images/Cc747736.note(WS.10).gif)Uwaga                                                            |
|-----------------------------------------------------------------------------------------------------------------------------------|
| Jako konta usługi programu RMS nie można użyć konta domeny, za pomocą którego instalowano program RMS z dodatkiem Service Pack 1. |
