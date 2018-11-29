---
TOCTitle: Resetowanie hasła klucza prywatnego
Title: Resetowanie hasła klucza prywatnego
ms:assetid: 'ceba927e-a7fd-4b06-bb70-5e5d9d6d099c'
ms:contentKeyID: 18123428
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747675(v=WS.10)'
---

Resetowanie hasła klucza prywatnego
===================================

Podczas zastrzegania serwera należy wybrać metodę ochrony klucza prywatnego programu RMS. Jeśli wybrano domyślną opcję programowej ochrony klucza prywatnego, użytkownik podał silne hasło, za pomocą którego został zaszyfrowany klucz prywatny serwera w bazie danych konfiguracji. W przypadku zgubienia lub zapomnienia hasła członek grupy administratorów może je zresetować w sposób opisany w części „[Resetowanie hasła klucza prywatnego](https://technet.microsoft.com/f71df255-fe19-4e07-810e-87309a5e8e88)” w dalszej części tego tematu.

Jeśli program RMS wykorzystywany jest w środowisku klastrowym, należy zresetować klucz prywatny na każdym serwerze frontonu programu RMS w posiadanej instalacji. W przeciwnym razie serwery takie nie będą działać, gdyż nie będą mogły odszyfrować swoich kluczy w bazie danych konfiguracji.

Więcej informacji na temat silnych haseł można znaleźć w Centrum pomocy i obsługi technicznej systemu Windows Server 2003.
