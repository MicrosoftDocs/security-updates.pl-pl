---
TOCTitle: Usuwanie ochrony technologią RMS z zawartości
Title: Usuwanie ochrony technologią RMS z zawartości
ms:assetid: 'c30361e3-50d2-4474-a87d-d38de502cf9e'
ms:contentKeyID: 18123405
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747658(v=WS.10)'
---

Usuwanie ochrony technologią RMS z zawartości
=============================================

Przed przystąpieniem do procesu likwidacji należy określić, które pliki mają zostać przywrócone, przez kogo i kiedy, tak by zachować wszystkie ważne informacje. Po usunięciu ochrony technologią RMS ze wszystkich zabezpieczonych plików można usunąć serwer z infrastruktury.

Proces usuwania ochrony technologią RMS z zawartości przebiega następująco:

1.  Użytkownik powinien usunąć z komputera wszystkie istniejące licencje użytkowania. Dzięki temu klient programu RMS połączy się z serwerem, aby pobrać licencję w celu otwarcia zawartości. Licencje użytkowania są przechowywane w folderze %USERPROFILE%\\Local Settings\\Application Data\\Microsoft\\DRM na komputerze klienckim, a ich nazwy mają prefiks EUL.
2.  Użytkownik mający dostęp do serwera likwidowania usiłuje otworzyć plik chroniony technologią RMS.
3.  Aplikacja łączy się z serwerem likwidowania i pobiera klucz zawartości.
4.  Zawartość jest odszyfrowywana, dzięki czemu można ją edytować, zapisywać, przesyłać dalej lub drukować.
5.  Użytkownik zapisuje zawartość bez zabezpieczeń RMS. Teraz wszyscy użytkownicy mogą otworzyć zawartość bez konieczności łączenia się z serwerem RMS.
