---
TOCTitle: Opis procesu likwidacji
Title: Opis procesu likwidacji
ms:assetid: '57bd9949-9433-437b-93ed-ffb2dff9992e'
ms:contentKeyID: 18123268
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720276(v=WS.10)'
---

Opis procesu likwidacji
=======================

Dzięki Internetowym usługom informacyjnym (IIS) można korzystać z różnych usług programu RMS. Na przykład usługa certyfikacji rejestruje użytkowników i ich komputery, a usługa licencjonowania publikuje zawartość i umożliwia dostęp do informacji chronionych za pomocą programu RMS. Aby rozpocząć proces likwidacji, w programie RMS należy włączyć dodatkową usługę, zwaną usługą likwidacji. Po włączeniu usługi likwidacji wszystkie inne usługi programu RMS dostępne na serwerze są wyłączane.

Po włączeniu usługi likwidacji na serwerze programu RMS aplikacje mogą pobrać klucz zawartości z tej usługi. Klucz ten umożliwia aplikacji ciągłe deszyfrowanie zawartości chronionej za pomocą programu RMS.

Gdy serwer programu RMS działa w trybie likwidacji, każdy użytkownik, niezależnie od tego, czy ma prawa do oryginalnej zawartości chronionej za pomocą programu RMS, może otrzymać klucz zawartości i pełne prawa do tej zawartości.

Po odszyfrowaniu zawartości użytkownik powinien zapisać zawartość bez ochrony RMS. Należy pamiętać, że aby korzystać z usługi likwidacji, użytkownik musi wcześniej zarejestrować się w infrastrukturze RMS. Użytkownik bez aktywnego klienta programu RMS nie może używać usługi likwidacji, aby uzyskać dostęp do zawartości chronionej za pomocą programu RMS.
