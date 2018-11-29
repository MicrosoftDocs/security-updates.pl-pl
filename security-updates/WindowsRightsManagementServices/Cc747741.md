---
TOCTitle: Publikowanie w trybie offline
Title: Publikowanie w trybie offline
ms:assetid: 'f6384ed2-f917-442e-aa63-c1394a1c4d06'
ms:contentKeyID: 18123500
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747741(v=WS.10)'
---

Publikowanie w trybie offline
=============================

Publikowanie w trybie offline jest różne od publikowania w trybie online, ponieważ aplikacja obsługująca technologię RMS uzyskuje licencję publikacji w inny sposób.

Zanim autor opublikuje zawartość w trybie offline, musi uzyskać certyfikat licencjodawcy klienta w momencie, gdy ma dostęp sieciowy do serwera głównej certyfikacji.

Proces publikowania w trybie offline składa się z następujących kroków: 

1.  Autor tworzy dokument, korzystając z aplikacji obsługującej technologię RMS, a następnie określa prawa dostępu i warunki dla zawartości.
2.  Gdy autor zapisuje plik, certyfikat licencjodawcy klienta umożliwia lokalnemu komputerowi lub urządzeniu wystawienie i podpisanie licencji publikacji dla tego pliku.
    Licencja publikacji zawiera dwie kopie klucza zawartości: jedna jest zaszyfrowana kluczem publicznym certyfikatu licencjodawcy klienta, a druga kluczem publicznym serwera, który wystawił certyfikat licencjodawcy klienta. Licencja zawiera także adres URL serwera. Dwa klucze publiczne i adres URL pochodzą z certyfikatu licencjodawcy klienta.
3.  Komputer używa certyfikatu licencjodawcy klienta do utworzenia licencji właściciela będącej specjalnym rodzajem licencji użytkowania, która przyznaje autorowi prawo do korzystania z zawartości chronionej technologią RMS, gdy pracuje w trybie offline. Certyfikat licencjodawcy klienta korzysta ze swojego klucza prywatnego do deszyfrowania symetrycznego klucza zawartości z licencji publikacji, a następnie ponownie szyfruje klucz do licencji właściciela.
4.  Aplikacja szyfruje plik za pomocą klucza zawartości i łączy licencję publikacji z plikiem. Tylko serwer programu RMS, który wystawił licencję publikacji, lub serwer będący członkiem zaufanej domeny publikacji może wystawiać licencje do deszyfrowania tego pliku.
