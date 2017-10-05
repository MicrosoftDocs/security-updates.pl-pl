---
TOCTitle: Wykluczanie wersji skrytek
Title: Wykluczanie wersji skrytek
ms:assetid: 'e287f026-aab2-43ab-93bc-48087da82f36'
ms:contentKeyID: 18123464
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747700(v=WS.10)'
---

Wykluczanie wersji skrytek
==========================

Aby klienci korzystali z minimalnej wersji oprogramowania klienckiego RMS, należy użyć wersji skrytki skojarzonej z klientem w celu wykluczenia poprzednich wersji oprogramowania klienckiego RMS. W przypadku włączenia tej funkcji należy określić najnowszą minimalną wersję skrytki, która została podpisana przez usługę aktywacji firmy Microsoft. Następnie należy włączyć wykluczanie skrytki w administracyjnej witrynie sieci Web każdego klastra, w którym ma działać ta funkcja. Wszystkie żądania certyfikacji i licencji będą wówczas sprawdzane w celu upewnienia się, że skrytka spełnia kryterium minimalnej wersji.

Jeśli włączone jest wykluczanie na podstawie wersji skrytki, klienci korzystający z wersji oprogramowania skrytki wcześniejszych niż określona wersja nie mogą uzyskiwać certyfikatów konta praw ani licencji użytkowania, ponieważ ich żądania zostaną odrzucone. Na tych klientach należy zainstalować nowe wersje oprogramowania klienckiego RMS w celu uzyskania nowej skrytki, która używa bieżącej wersji oprogramowania.

Klient programu RMS dla dodatku Service Pack 1 (SP1) używa wersji skrytki 5.0.0.0 lub nowszej. Dzięki ustawieniu wykluczenia skrytki na tę wersję minimalną można wymusić uaktualnienie klientów programu RMS w danej organizacji do klienta programu RMS dla dodatku SP1, co umożliwia korzystanie z zawartości chronionej technologią RMS.

Jeśli użytkownikowi dysponującemu wykluczoną skrytką wcześniej wystawiono licencje na zawartość, może on w dalszym ciągu korzystać z tej zawartości bez uzyskiwania nowej skrytki.
