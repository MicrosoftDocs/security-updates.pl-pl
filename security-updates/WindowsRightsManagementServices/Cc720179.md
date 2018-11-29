---
TOCTitle: Przenoszenie kont użytkowników między domenami
Title: Przenoszenie kont użytkowników między domenami
ms:assetid: '0010b0ea-07c0-41c9-81f7-5881343d1d55'
ms:contentKeyID: 18123162
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720179(v=WS.10)'
---

Przenoszenie kont użytkowników między domenami
==============================================

Kiedy w organizacji konfiguruje się i zastrzega serwer głównej certyfikacji, jest on rejestrowany w usłudze Active Directory w odpowiednim lesie jako dostawca usług RMS. Na każdy las usługi Active Directory może przypadać tylko jeden klaster głównej certyfikacji.

Ogólnie rzecz biorąc, przeniesienie konta użytkownika z jednej domeny do drugiej w obrębie tego samego lasu powoduje, że dla konta użytkownika w nowej domenie tworzony jest nowy identyfikator SID. Kiedy następnie użytkownik próbuje uzyskać z serwera nowy certyfikat konta praw, z powodu swojego nowego identyfikatora SID traktowany jest na serwerze jako nowy użytkownik. Serwer generuje dla użytkownika nowe klucze i wystawia nowy certyfikat konta praw przy użyciu oryginalnego adresu e-mail użytkownika. Kiedy użytkownik spróbuje użyć nowego certyfikatu konta praw wraz z istniejącą licencją, identyfikator SID i klucze nie będą do siebie pasować, skutkiem czego użytkownik będzie musiał uzyskać nową licencję. Dotyczy to także przenoszenia konta użytkownika do domeny znajdującej się w innym lesie.
