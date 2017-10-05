---
TOCTitle: Szyfrowanie i klucze w programie RMS
Title: Szyfrowanie i klucze w programie RMS
ms:assetid: '6ed69817-dab0-4845-b2a4-74203f95f7cf'
ms:contentKeyID: 18123308
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747615(v=WS.10)'
---

Szyfrowanie i klucze w programie RMS
====================================

Zawartość chroniona jest zawsze zaszyfrowana. Certyfikaty i licencje używane przez program RMS mogą również zawierać zaszyfrowaną zawartość, która może zostać odszyfrowana tylko przez odpowiedni podmiot. Aplikacja obsługująca technologię RMS korzysta z klucza zawartości do szyfrowania danych. Wszystkie serwery programu RMS z dodatkiem SP1, komputery klienckie oraz konta użytkowników mają parę 1024-bitowych kluczy RSA. Program RMS używa tych kluczy do szyfrowania klucza zawartości w licencjach publikacji i użytkowania, a także do podpisywania certyfikatów i licencji RMS. Dzięki temu procesowi serwer umożliwia dostęp tylko autoryzowanym użytkownikom i komputerom.

W tej części omówiono następujące zagadnienia:

-   [Definicje kluczy programu RMS](https://technet.microsoft.com/b052305c-1db7-434a-bad9-26d704156776)
-   [Klucze serwera w programie RMS](https://technet.microsoft.com/5f4100a1-9aa5-42af-85c8-4bc691022f06)
-   [Klucze komputera w programie RMS](https://technet.microsoft.com/56e59ec2-f681-4ca2-98c7-72218ab9e9d9)
-   [Klucze licencjodawcy klienta](https://technet.microsoft.com/28781125-2692-4ff9-99b1-e09227d72966)
-   [Klucze użytkownika](https://technet.microsoft.com/12dad6e2-64e7-4bab-bde7-b72f90f5cb05)
-   [Klucze zawartości w programie RMS](https://technet.microsoft.com/63c814bf-2809-477e-a2db-d90370442075)
