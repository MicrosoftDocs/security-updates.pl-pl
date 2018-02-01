---
TOCTitle: Aktywacja komputera RMS
Title: Aktywacja komputera RMS
ms:assetid: '09a0d631-9860-477f-9d10-df61b3bfe125'
ms:contentKeyID: 18123173
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720182(v=WS.10)'
---

Aktywacja komputera RMS
=======================

Aktywacja komputera jest wymagana do publikowania lub używania zawartości chronionej technologią RMS na komputerze klienckim. Aktywacja komputera jest procesem, podczas którego komputer kliencki otrzymuje unikatową skrytkę oraz odpowiadający jej certyfikat komputera RMS. Skrytka zawiera klucz prywatny komputera, a certyfikat komputera zawiera klucz publiczny komputera. Skrytka zawiera klucz prywatny komputera, tak więc jest głównym podmiotem zabezpieczeń dla szyfrowania i deszyfrowania. Każdy użytkownik komputera otrzymuje unikatowy certyfikat, utworzony w procesie aktywacji komputera.

Proces aktywacji komputera z użyciem klienta programu RMS dla dodatku Service Pack 1 różni się znacznie od aktywacji w wersji 1. Klient programu RMS dla dodatku Service Pack 1 ma funkcję automatycznej aktywacji. Klient programu RMS uruchamia proces aktywacji po zainstalowaniu lub przy pierwszym użyciu funkcji tego programu przez zalogowanego użytkownika. Proces ten generuje kilka zestawów kluczy za pomocą API modułu kryptografii, dołączonego do systemu Windows. Klucze te są używane w procesach szyfrowania generujących certyfikat komputera, który wiąże użytkownika, komputer i klienta programu RMS w hierarchii zaufania.
