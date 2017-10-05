---
TOCTitle: Klucze serwera w programie RMS
Title: Klucze serwera w programie RMS
ms:assetid: '5f4100a1-9aa5-42af-85c8-4bc691022f06'
ms:contentKeyID: 18123285
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720280(v=WS.10)'
---

Klucze serwera w programie RMS
==============================

Serwer programu RMS ma parę 1024-bitowych kluczy RSA.

Klucz publiczny serwera jest używany do szyfrowania klucza zawartości w licencji publikacji, aby tylko serwer programu RMS mógł pobrać klucz zawartości i wystawić licencję użytkowania dla tej licencji publikacji. Certyfikat licencjodawcy serwera zawiera klucz publiczny serwera.

Klucz prywatny serwera jest używany do podpisywania wszystkich certyfikatów i licencji wystawianych przez serwer.

Ochrona klucza prywatnego serwera
---------------------------------

Domyślnie podczas zastrzegania klucz prywatny serwera jest tworzony i przechowywany w postaci zaszyfrowanej w bazie danych programu RMS. Alternatywnie podczas zastrzegania można określić dostawcę usług kryptograficznych (CSP), który jest już zainstalowany na serwerze.

Dostawcy CSP można używać na dwa różne sposoby:

-   Wybrać spośród programowych implementacji dostawcy CSP, instalowanych domyślnie wraz z serwerem.
    — lub —
-   Użyć oprogramowania CSP firm trzecich, które zainstalowano na serwerze.

| ![](images/Cc720280.note(WS.10).gif)Uwaga                                                                                 |
|--------------------------------------------------------------------------------------------------------------------------------------------------------|
| W przypadku korzystania ze sprzętowego modułu zabezpieczeń należy upewnić się, że wybrano dostawcę CSP, który obsługuje sprzętowe moduły zabezpieczeń. |

Jeśli wybrano ochronę klucza prywatnego serwera za pomocą dostawcy CSP, program RMS będzie przechowywać nazwę dostawcy oraz nazwę kontenera klucza znajdującego się w bazie danych konfiguracji.
