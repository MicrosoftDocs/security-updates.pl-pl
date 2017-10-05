---
TOCTitle: Odnajdowanie usługi rejestrowania
Title: Odnajdowanie usługi rejestrowania
ms:assetid: 'bbeb00bd-04e0-4df6-8615-76aa8125b620'
ms:contentKeyID: 18123433
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747737(v=WS.10)'
---

Odnajdowanie usługi rejestrowania
=================================

Pierwszy z zastrzeganych serwerów programu RMS w lesie musi połączyć się z usługą rejestrowania firmy Microsoft w celu zarejestrowania się i uzyskania certyfikatu licencjodawcy serwera. Aby uzyskać adres URL usługi rejestrowania, Instalator programu RMS wysyła żądanie rejestru UDDI do [witryny sieci Web usług UDDI firmy Microsoft](http://go.microsoft.com/fwlink/?linkid=14794)(http://go.microsoft.com/fwlink/?LinkId=14794). Kolejne serwery zastrzegane jako część klastra głównej certyfikacji nie muszą uzyskiwać certyfikatów licencjodawcy serwera, ponieważ korzystają z konfiguracji pierwszego serwera głównej certyfikacji.
