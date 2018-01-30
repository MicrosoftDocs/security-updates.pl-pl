---
TOCTitle: Certyfikaty kont praw
Title: Certyfikaty kont praw
ms:assetid: '2ff315cc-211d-4e6e-85e8-56867c2abd94'
ms:contentKeyID: 18123214
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720230(v=WS.10)'
---

Certyfikaty kont praw
=====================

Organizacje muszą zidentyfikować użytkowników, którzy są zaufanymi podmiotami w systemie RMS. W tym celu program RMS wystawia certyfikaty kont praw, które kojarzą konta użytkowników z określonymi komputerami. Certyfikat konta praw użytkownika musi być zawarty w żądaniu certyfikatów licencjodawcy klienta oraz licencji użytkowania. Certyfikat licencjodawcy klienta umożliwia autorowi publikowanie zawartości chronionej technologią RMS, takiej jak pliki i wiadomości e-mail, podczas pracy w trybie offline. Licencja użytkowania umożliwia użytkownikowi korzystanie z zawartości chronionej technologią RMS. Każdy certyfikat konta praw zawiera klucz publiczny użytkownika używany do szyfrowania danych przeznaczonych dla tego użytkownika.

Istnieją dwa typy certyfikatów kont praw: standardowy i tymczasowy. Dla obu typów można określić okresy ważności. Standardowe certyfikaty mają ważność określoną w dniach (domyślnie 365 dni). Tymczasowe certyfikaty kont mają ważność określoną w minutach (domyślnie 15 minut). Tymczasowe certyfikaty kont umożliwiają użytkownikom tymczasowe korzystanie z zawartości, na przykład w kioskach, gdzie nie mogą uzyskać dostępu do swojego komputera. Zapobiega to późniejszemu wykorzystaniu zawartości przez innego użytkownika na tym samym komputerze.
