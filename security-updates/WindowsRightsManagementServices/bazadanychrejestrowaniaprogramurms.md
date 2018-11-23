---
TOCTitle: Baza danych rejestrowania programu RMS
Title: Baza danych rejestrowania programu RMS
ms:assetid: '8ba147f3-16e4-4d9a-ac8f-f05ba2ba11bb'
ms:contentKeyID: 18123342
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747669(v=WS.10)'
---

Baza danych rejestrowania programu RMS
======================================

Dla każdego klastra głównej certyfikacji lub licencji Instalator programu RMS instaluje bazę danych rejestrowania w tym samym wystąpieniu serwera bazy danych, które obsługuje bazę danych konfiguracji. Instalator tworzy również prywatną kolejkę wiadomości na potrzeby rejestrowania w Usłudze kolejkowania wiadomości. Następnie usługa odbiornika rejestrowania przesyła dane z tej kolejki wiadomości do bazy danych rejestrowania.

Grupa RMS Service Group ma uprawienia do wykonywania dla procedur przechowywanych w bazie danych rejestrowania.

Usługa odbiornika rejestrowania wysyła duże ilości danych do bazy danych rejestrowania, więc administratorzy mogą tworzyć filtry, tak aby w bazie danych rejestrowania przechowywane były tylko informacje wymagane przez ich organizacje.
