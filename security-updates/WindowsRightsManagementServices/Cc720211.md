---
TOCTitle: Licencje publikacji
Title: Licencje publikacji
ms:assetid: '187228fc-370b-4e23-a53a-21bb296b84a1'
ms:contentKeyID: 18123193
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720211(v=WS.10)'
---

Licencje publikacji
===================

Użytkownicy aplikacji obsługujących technologię RMS mogą przypisywać określone prawa użytkowania do plików i danych cyfrowych, zgodnie z zasadami istniejącymi w firmie. Te prawa użytkowania są przechowywane w licencjach publikacji określających użytkowników, którzy mogą przeglądać zawartość, oraz dopuszczalny sposób edycji i rozpowszechniania zawartości.

Licencję publikacji może wystawić aplikacja klienta obsługującego technologię RMS, serwer głównej certyfikacji lub serwer licencji programu RMS. Jeżeli licencja publikacji jest wystawiana przez aplikację klienta obsługującego technologię RMS, serwer programu RMS przyznaje tej aplikacji certyfikat licencjodawcy klienta. Proces ten jest nazywany publikowaniem w trybie offline. Jest to powszechna metoda publikowania ze względu na możliwość tworzenia zawartości chronionej bez konieczności posiadania połączenia z serwerem programu RMS. Jeżeli aplikacja klienta obsługującego technologię RMS nie wykorzystuje certyfikatu licencjodawcy klienta, użytkownik musi mieć możliwość połączenia z serwerem programu RMS, aby otrzymać licencję publikacji dla zawartości chronionej.

Licencja publikacji zawiera symetryczny klucz zawartości do deszyfrowania zawartości zaszyfrowanej kluczem publicznym serwera programu RMS. Dzięki temu tylko serwer może odszyfrowywać zawartość i wystawiać licencje użytkowania.

Licencja publikacji jest podpisana za pomocą klucza prywatnego serwera wystawiającego lub klucza prywatnego certyfikatu licencjodawcy klienta.
