---
TOCTitle: Certyfikacja konta programu RMS
Title: Certyfikacja konta programu RMS
ms:assetid: 'c9a385c5-6dbb-47f5-a80f-69718e6f9deb'
ms:contentKeyID: 18123452
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747750(v=WS.10)'
---

Certyfikacja konta programu RMS
===============================

W procesie certyfikacji konta tworzony jest certyfikat konta praw, który przypisuje konto użytkownika do określonego komputera i umożliwia użytkownikowi korzystanie na tym komputerze z zawartości chronionej technologią RMS. Gdy użytkownik po raz pierwszy publikuje zawartość chronioną technologią RMS lub próbuje skorzystać z takiej zawartości na komputerze klienckim, aplikacja obsługująca technologię RMS wysyła żądanie certyfikatu konta praw do usługi certyfikacji kont programu RMS.

Usługa certyfikacji może uwierzytelniać użytkownika za pomocą mechanizmu uwierzytelniania systemu Windows lub certyfikatu x.509, przechowywanego w sprzętowym urządzeniu szyfrującym, jak np. karta inteligentna. Po uwierzytelnieniu użytkownika serwer programu RMS tworzy dla niego certyfikat konta praw w oparciu o jego uwierzytelnione poświadczenia. Usługa szyfruje klucz prywatny użytkownika kluczem publicznym certyfikatu komputera klienckiego RMS oraz dołącza zaszyfrowany klucz do certyfikatu konta praw. Następnie wystawia certyfikat konta praw dla aplikacji zgłaszającej żądanie, która zapisuje ten certyfikat w komputerze lub urządzeniu, tak aby był dostępny dla kolejnych żądań licencji publikacji lub użytkowania. Certyfikat konta praw jest również przechowywany w bazie danych konfiguracji.

Certyfikacja konta następuje po procesie aktywacji komputera, ponieważ do żądania certyfikatu konta praw wymagany jest certyfikat komputera RMS.

Użytkownicy muszą uzyskać certyfikat konta praw dla każdego używanego komputera. Jeśli użytkownik pracuje na więcej niż jednym komputerze, to dla każdego komputera wystawiany jest unikatowy certyfikat konta praw, ale wszystkie komputery zawierają tę samą parę kluczy dla tego użytkownika.

Gdy aplikacja obsługująca technologię RMS żąda licencji użytkowania, do żądania dołącza certyfikat konta praw. Usługa licencjonowania używa klucza publicznego certyfikatu konta praw w celu szyfrowania klucza zawartości. Dzięki temu tylko uwierzytelnieni użytkownicy mogą korzystać z licencji użytkowania.

Proces certyfikacji konta składa się z następujących kroków: 

1.  Gdy użytkownik po raz pierwszy publikuje zawartość chronioną technologią RMS lub próbuje użyć takiej zawartości na danym komputerze, aplikacja obsługująca technologię RMS wysyła żądanie certyfikatu konta praw do usługi certyfikacji kont działającej na serwerze głównej certyfikacji.
2.  Usługa certyfikacji kont uwierzytelnia użytkownika za pomocą uwierzytelniania systemu Windows.
3.  Usługa certyfikacji kont tworzy certyfikat konta praw dla użytkownika w oparciu o jego uwierzytelnione poświadczenia. Usługa szyfruje klucz prywatny użytkownika kluczem publicznym certyfikatu komputera RMS oraz dołącza zaszyfrowany klucz do certyfikatu. Następnie wystawia certyfikat konta praw dla aplikacji zgłaszającej żądanie.
4.  Aplikacja przechowuje certyfikat konta praw w komputerze lub urządzeniu, tak aby był dostępny dla kolejnych żądań licencji publikacji lub użytkowania.

Wybór usługi certyfikacji konta, używanej przez klienta dla żądań certyfikatów kont praw, zależy od typu komputera, na którym zainstalowany jest klient programu RMS. Standardowe komputery typu desktop łączą się z usługą certyfikacji konta (certification.asmx). Usługi serwera, którym umożliwiono używanie programu RMS z dodatkiem SP1 otrzymują certyfikaty kont praw od usługi certyfikacji serwera (ServeCertfication.asmx). Urządzenia przenośne, którym umożliwiono używanie programu RMS z dodatkiem SP1 otrzymują certyfikaty kont praw od usługi certyfikacji urządzenia przenośnego (MobileDeviceCertfication.asmx). W domyślnej instalacji programu RMS z dodatkiem SP1 włączona jest tylko usługa certyfikacji kont.

Aby uzyskać więcej informacji dotyczących wykorzystania programu RMS z dodatkiem SP1 dla urządzeń przenośnych i usług serwera, zobacz „Włączanie obsługi serwera programu RMS dla urządzeń przenośnych i usług serwera” w części Obsługa serwerów programu RMS w tym zestawie dokumentacji.
