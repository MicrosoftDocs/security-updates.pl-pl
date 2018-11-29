---
TOCTitle: Podrejestrowywanie serwera licencji
Title: Podrejestrowywanie serwera licencji
ms:assetid: '7bc63397-9186-464c-8824-867038adce9b'
ms:contentKeyID: 18123347
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747640(v=WS.10)'
---

Podrejestrowywanie serwera licencji
===================================

Serwery licencji są automatycznie rejestrowane podczas zastrzegania w procesie nazywanym podrejestrowywaniem. Po dodaniu nowego serwera do klastra serwerów licencji nowy serwer nie jest wprost podrejestrowywany, ponieważ korzysta z certyfikatu licencjodawcy serwera oraz bazy danych konfiguracji klastra.

Zamiast wysyłać żądanie podrejestrowywania do usługi rejestrowania firmy Microsoft, serwer licencji wysyła żądanie do serwera głównej certyfikacji. Żądanie podrejestrowywania serwera licencji jest identyczne z żądaniem rejestrowania serwera głównej certyfikacji.

Gdy serwer głównej certyfikacji otrzyma żądanie podrejestrowywania, sprawdza, czy żądanie zostało prawidłowo sformułowane, a następnie zwraca łańcuch certyfikatu zawierający łańcuch certyfikatu licencjodawcy serwera głównej certyfikacji oraz certyfikat podpisany przez serwer głównej certyfikacji. Certyfikat zawiera klucz publiczny serwera podpisany za pomocą klucza prywatnego serwera głównego certyfikacji. Certyfikat udziela serwerowi licencji prawa do wystawiania licencji użytkowania i publikacji.

Certyfikat licencjodawcy serwera jest ważny przez rok. Okres ważności rozpoczyna się w momencie wystawienia certyfikatu. Pod koniec okresu ważności certyfikat można odnowić. Certyfikaty i licencje wystawione przez serwer są ważne przez siedem lat. Okres ważności rozpoczyna się w momencie wystawienia certyfikatu lub licencji.

Domyślnie usługa wymagana do przetworzenia żądania podrejestrowywania na serwerze głównej certyfikacji, SubEnrollService.asmx, jest skonfigurowana do odmawiania wszelkiego dostępu. Aby żądanie mogło być przetworzone, należy zmienić listy DACL w celu umożliwienia dostępu administratorowi programu RMS.
