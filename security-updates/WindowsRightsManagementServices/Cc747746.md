---
TOCTitle: Kopie zapasowe systemu RMS
Title: Kopie zapasowe systemu RMS
ms:assetid: 'c29894da-ee00-428c-8d48-80d8e5a83678'
ms:contentKeyID: 18123445
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747746(v=WS.10)'
---

Kopie zapasowe systemu RMS
==========================

Przed skonfigurowaniem infrastruktury i zainstalowaniem programu RMS należy wykonać kopie zapasowe następujących składników (jeśli występują w systemie użytkownika):

-   Jeśli planowane jest używanie istniejącej bazy danych programu SQL Server do obsługi baz danych konfiguracji i rejestrowania, należy wykonać kopię zapasową wszystkich baz danych i ustawień serwera. Jeśli uaktualniana jest poprzednia wersja programu RMS lub program RMS jest instalowany ponownie, należy wykonać kopię zapasową poprzednich baz danych konfiguracji i rejestrowania.
-   Należy wykonać kopię zapasową stanu systemu serwera, na którym planowane jest zainstalowanie programu RMS. W tej kopii zapasowej będą przechowywane klucze i wartości rejestru, zawierające informacje wymagane do przywrócenia serwera w razie potrzeby.
-   Za pomocą przystawki Certyfikaty należy wyeksportować certyfikaty do pliku. Przystawka Certyfikaty służy również do wykonywania kopii zapasowych danych kluczy prywatnych programu RMS w pliku PKCS \#12, który jest szyfrowany za pomocą hasła. W przypadku uaktualniania lub ponownego instalowania programu RMS, jeśli stosowana była ochrona klucza prywatnego programu RMS za pomocą domyślnego szyfrowania programowego, klucz ten zostanie zaszyfrowany i będzie przechowywany w kopii zapasowej bazy danych konfiguracji.
-   Jeśli do ochrony klucza prywatnego używany jest sprzętowy moduł zabezpieczeń, należy wykonać kopię zapasową jego konfiguracji przy użyciu metody zalecanej przez producenta.

Pliki kopii zapasowych należy przechowywać w bezpiecznej lokalizacji przechowywania razem z hasłem użytym do szyfrowania kluczy prywatnych.
