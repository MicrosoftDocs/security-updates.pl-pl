---
TOCTitle: Rejestrowanie serwera głównej certyfikacji
Title: Rejestrowanie serwera głównej certyfikacji
ms:assetid: 'f08bc919-f090-4843-b2ce-b40d558012ce'
ms:contentKeyID: 18123497
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747734(v=WS.10)'
---

Rejestrowanie serwera głównej certyfikacji
==========================================

Rejestrowanie za pomocą usługi rejestrowania firmy Microsoft jest wymagane dla pierwszego serwera w instalacji programu RMS. Serwer ten, będący serwerem głównej certyfikacji, może być automatycznie rejestrowany w fazie zastrzegania, jeśli serwer dysponuje połączeniem internetowym. Jeśli serwer działa w ramach sieci zamkniętej, można go rejestrować ręcznie. Aby uzyskać więcej informacji na temat ręcznego rejestrowania serwera, zobacz „Ręczne rejestrowanie serwera głównej certyfikacji” w części „Obsługa serwerów programu RMS” w niniejszym zestawie dokumentacji.

Żądanie rejestrowania korzysta z dwóch poniższych parametrów wejściowych:

-   Klucz publiczny o długości 1024 bitów. Jest to klucz publiczny programu RMS.
-   Wersja, nazwa i adres URL serwera RMS, który ma zostać zarejestrowany.

Usługa rejestrowania firmy Microsoft wykorzystuje te informacje tylko do utworzenia certyfikatu licencjodawcy serwera i przechowuje te informacje tylko w celu odwołania.

Usługa rejestrowania firmy Microsoft zwraca łańcuch certyfikatów zawierający łańcuch certyfikatu licencjodawcy serwera dla serwera rejestrowania oraz certyfikat podpisany przez serwer rejestrowania. Certyfikat ten zawiera klucz publiczny serwera podpisany za pomocą klucza prywatnego rejestrowania oraz wersję i adres URL zarejestrowanego serwera. Certyfikat udziela serwerowi głównej certyfikacji prawa do wystawiania certyfikatów licencjodawcy serwera dla serwerów licencji, a także do wystawiania certyfikatów kont praw, certyfikatów licencjodawcy klienta, publikacji oraz licencji użytkowania.

Certyfikat licencjodawcy serwera jest ważny przez rok. Okres ważności rozpoczyna się w momencie wystawienia certyfikatu. Pod koniec okresu ważności certyfikat można odnowić. Certyfikaty i licencje wystawione przez serwer są ważne przez siedem lat. Okres ważności rozpoczyna się w momencie wystawienia certyfikatu lub licencji.

Informacje o odwołaniu certyfikatu są dodawane do certyfikatu licencjodawcy serwera, tak jak wskazano w żądaniu rejestrowania. Klucz publiczny usługi rejestrowania firmy Microsoft jest dodawany do certyfikatu jako klucz odwołania. Ponadto jeśli określono klucz odwołania innej firmy, również zostanie on dodany do certyfikatu jako klucz odwołania.
