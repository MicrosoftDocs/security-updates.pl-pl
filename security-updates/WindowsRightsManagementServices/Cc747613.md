---
TOCTitle: Rejestrowanie klienta programu RMS
Title: Rejestrowanie klienta programu RMS
ms:assetid: '9c1d07bf-7235-4694-8291-ac2e5b221f4a'
ms:contentKeyID: 18123369
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747613(v=WS.10)'
---

Rejestrowanie klienta programu RMS
==================================

Komputery klienckie mogą rejestrować się w usłudze publikacji programu RMS w celu uzyskania certyfikatu licencjodawcy klienta, który umożliwia autorom publikowanie zawartości chronionej technologią RMS, gdy ich komputery nie są podłączone do sieci firmowej. W takim przypadku komputer kliencki, a nie usługa publikacji, podpisuje i wystawia licencje publikacji, które zawierają informacje o prawach użytkowania dla zawartości chronionej technologią RMS, publikowanej z tego komputera.

Usługa publikacji programu RMS wystawia certyfikaty licencjodawcy klienta.

Rejestrowanie klienta składa się z następujących kroków:

1.  Komputer kliencki wysyła certyfikat konta praw użytkownika jako część żądania rejestracji do usługi publikacji działającej na serwerze lub klastrze głównej certyfikacji, lub na serwerze albo klastrze licencji.
2.  Serwer sprawdza, czy rejestracja klienta jest dozwolona w oparciu o ustawienia administratora sieci, a także czy certyfikat konta praw nie znajduje się na liście wykluczania w bazie danych konfiguracji. Aby uzyskać więcej informacji dotyczących tworzenia list wykluczania, zobacz „Zarządzanie zasadami wykluczania” w części „Obsługa serwerów programu RMS” w tym zestawie dokumentacji.
3.  Usługa publikacji tworzy parę kluczy dla komputera klienckiego. Tworzy certyfikat licencjodawcy klienta i umieszcza klucz publiczny w certyfikacie. Szyfruje klucz prywatny kluczem publicznym certyfikatu konta praw, a następnie umieszcza go w certyfikacie.
4.  Usługa publikacji wystawia certyfikat licencjodawcy klienta komputerowi klienckiemu.
