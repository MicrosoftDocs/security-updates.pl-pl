---
TOCTitle: Publikowanie w trybie online
Title: Publikowanie w trybie online
ms:assetid: '962c4e83-cf34-4c61-9589-31d24b0299fb'
ms:contentKeyID: 18123470
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747694(v=WS.10)'
---

Publikowanie w trybie online
============================

Poniższy diagram przedstawia proces publikowania w trybie online.

![](images/Cc747694.897e47b6-fffe-4b11-bc9f-be58539b9f19(WS.10).gif)

Proces publikowania w trybie online składa się z następujących kroków:

1.  Autor zawartości tworzy dokument i używa aplikacji obsługującej technologię RMS w celu określenia użytkowników i zastosowania praw dostępu oraz warunków względem zawartości.
2.  Aplikacja obsługująca technologię RMS generuje symetryczny klucz zawartości i wysyła żądanie licencji publikacji do serwera certyfikacji lub serwera licencji. Żądanie zawiera klucz zawartości i ustawienia użytkowania.
3.  Serwer licencji generuje licencję publikacji, szyfruje klucz zawartości kluczem publicznym serwera, a następnie zwraca licencję publikacji do aplikacji obsługującej technologię RMS.
4.  Aplikacja szyfruje plik za pomocą klucza zawartości i łączy licencję publikacji z plikiem.
5.  Aplikacja obsługująca technologię RMS na komputerze użytkownika korzystającego z zawartości wysyła żądanie zawierające certyfikat konta praw użytkownika do serwera programu RMS, który wystawił licencję publikacji w celu zażądania licencji użytkowania dla dokumentu.
6.  Serwer programu RMS sprawdza poświadczenia użytkownika. Jeśli użytkownik zostanie pomyślnie zweryfikowany, licencja użytkowania zostanie wygenerowana i przekazana do aplikacji obsługującej technologię RMS na komputerze użytkownika.
7.  Aplikacja obsługująca technologię RMS otwiera dokument i udziela użytkownikowi praw dostępu zgodnie z parametrami zdefiniowanymi w licencji użytkowania.
