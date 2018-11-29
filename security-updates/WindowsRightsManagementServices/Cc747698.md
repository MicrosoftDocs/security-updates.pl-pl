---
TOCTitle: Rejestrowanie w programie RMS
Title: Rejestrowanie w programie RMS
ms:assetid: '999db3e1-e3ab-4513-87d9-d584ee334c00'
ms:contentKeyID: 18123398
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747698(v=WS.10)'
---

Rejestrowanie w programie RMS
=============================

W trakcie procesu rejestrowania serwera tworzony i zapewniany jest certyfikat licencjodawcy serwera. Certyfikaty licencjodawcy serwera sprawdzają tożsamość serwerów w instalacji i zawierają mechanizm sprawdzania poprawności poświadczeń podczas korzystania z zawartości chronionej technologią RMS. W ramach procesu zastrzegania w klastrze głównej certyfikacji rejestrowany jest pierwszy serwer z każdego klastra licencji. Kolejne serwery w klastrze nie są oddzielnie rejestrowane.

Początkowy serwer klastra głównej certyfikacji (serwer głównej certyfikacji) musi zostać zarejestrowany w usłudze rejestrowania firmy Microsoft. Proces ten może zostać wykonany automatycznie w ramach procesu zastrzegania, jeżeli serwer głównej certyfikacji jest podłączony do Internetu. W przypadku gdy serwer ten nie jest podłączony do Internetu, żądanie rejestrowania można wyeksportować do pliku, a następnie przesłać ten plik do usługi rejestrowania firmy Microsoft z komputera podłączonego do Internetu. Żądanie rejestrowania zwróci certyfikat licencjodawcy serwera dla serwera głównej certyfikacji, który można zaimportować w administracyjnej witrynie sieci Web programu RMS.

Żądanie rejestrowania zawiera następujące informacje:

-   Revocation information — informacje określające, czy instalacja programu RMS będzie stosować odwoływanie standardowe, czy też niestandardowe (przez niezależny podmiot). W przypadku zastosowania odwoływania przez niezależny podmiot, dołączony zostaje klucz publiczny urzędu odwołującego.
-   Certificate Public Key — klucz publiczny certyfikatu licencjodawcy serwera. Taki klucz publiczny jest generowany na serwerze programu RMS i przesyłany do usługi rejestrowania serwera firmy Microsoft w celu uzyskania certyfikatu licencjodawcy serwera.
-   SKU — oficjalna nazwa SKU programu RMS.
-   Version — numer wersji programu RMS.
-   URL — bazowy adres URL klastra serwerów programu RMS.

W odpowiedzi na żądanie rejestrowania usługa rejestrowania serwera firmy Microsoft zwraca serwerowi programu RMS następujące informacje w formacie XML:

-   Certyfikat licencjodawcy serwera
-   Łańcuch certyfikatów urzędów podpisujących.

Identyczne informacje są przekazywane bez względu na to, czy serwer głównej certyfikacji programu RMS jest rejestrowany w trybie online czy offline. Przy korzystaniu z każdej z tych metod nie są zbierane żadne dodatkowe informacje.

Aby uzyskać instrukcje rejestrowania serwera w trybie offline, zobacz „Rejestrowanie serwera głównej certyfikacji za pomocą rejestrowania w trybie offline” w temacie „Obsługa serwerów programu RMS” niniejszej dokumentacji.

Podczas procesu rejestrowania klienta tworzony i zapewniany jest certyfikat licencjodawcy klienta, który umożliwia autorowi publikowanie zawartości chronionej technologią RMS na komputerze niepodłączonym do sieci firmowej. Autor może zażądać certyfikatu licencjodawcy klienta w dowolnej chwili. Rejestrowanie klientów nie jest konieczne.

Wszystkie żądania rejestrowania są rejestrowane.

W tej części omówiono następujące zagadnienia:

-   [Rejestrowanie serwera głównej certyfikacji](https://technet.microsoft.com/f08bc919-f090-4843-b2ce-b40d558012ce)
-   [Podrejestrowywanie serwera licencji](https://technet.microsoft.com/7bc63397-9186-464c-8824-867038adce9b)
-   [Rejestrowanie klienta programu RMS](https://technet.microsoft.com/9c1d07bf-7235-4694-8291-ac2e5b221f4a)
-   [Aktywacja komputera RMS](https://technet.microsoft.com/09a0d631-9860-477f-9d10-df61b3bfe125)
-   [Certyfikacja konta programu RMS](https://technet.microsoft.com/c9a385c5-6dbb-47f5-a80f-69718e6f9deb)
