---
TOCTitle: Klucze licencjodawcy klienta
Title: Klucze licencjodawcy klienta
ms:assetid: '28781125-2692-4ff9-99b1-e09227d72966'
ms:contentKeyID: 18123207
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720221(v=WS.10)'
---

Klucze licencjodawcy klienta
============================

Autorzy mogą uzyskiwać certyfikaty licencjodawcy klienta w celu publikowania zawartości chronionej technologią RMS, gdy nie są podłączeni do sieci obsługującej technologię RMS. Certyfikat licencjodawcy klienta ma parę 1024-bitowych kluczy RSA.

Klient programu RMS używa klucza publicznego certyfikatu licencjodawcy klienta podczas wystawiania licencji publikacji w celu wykonania następujących zadań:

-   Szyfrowanie symetrycznego klucza zawartości.
-   Podpisywanie licencji publikacji wystawianych lokalnie, gdy użytkownik nie jest podłączony do sieci.
