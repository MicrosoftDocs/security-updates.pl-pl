---
TOCTitle: 'Często zadawane pytania na temat programu RMS: Certyfikaty, klucze i szyfrowanie'
Title: 'Często zadawane pytania na temat programu RMS: Certyfikaty, klucze i szyfrowanie'
ms:assetid: 'ad8cc088-1dea-44c2-be68-9091129f0f12'
ms:contentKeyID: 18123422
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747725(v=WS.10)'
---

Często zadawane pytania na temat programu RMS: Certyfikaty, klucze i szyfrowanie
================================================================================

Pytania dotyczące certyfikatów, kluczy i szyfrowania w programie RMS
--------------------------------------------------------------------

-   [Jakie algorytmy szyfrowania są stosowane w programie RMS?](#bkmk_10)
-   [Czy program RMS korzysta z algorytmów kryptograficznych FIPS?](#bkmk_11)
-   [Czy w przypadku licencji publikacji lub szablonów, które udzielają uprawnień za pośrednictwem listy rozpowszechniania, licencje użytkowania są traktowane w inny sposób, aby zapewnić możliwość dynamicznego weryfikowania członków listy?](#bkmk_12)
-   [Kiedy program RMS jest używany za pośrednictwem kiosku, następuje wydanie tymczasowego certyfikatu konta praw. Czym certyfikat tymczasowy różni się od certyfikatu zwykłego? W jaki sposób program RMS wykrywa, że został wywołany z kiosku?](#bkmk_13)
-   [W jakich sytuacjach używany jest tymczasowy certyfikat konta praw?](#bkmk_14)
-   [Czy program RMS wydaje certyfikaty typu X.509v3?](#bkmk_15)
-   [Gdzie są przechowywane certyfikaty XrML?](#bkmk_16)
-   [Gdzie są przechowywane klucze prywatny i publiczny komputera?](#bkmk_17)
-   [Gdzie są przechowywane klucze prywatny i publiczny klienta?](#bkmk_18)
-   [AES jest algorytmem symetrycznym. W jaki sposób zapewnia się bezpieczne przekazanie kluczy między serwerem a użytkownikiem?](#bkmk_19)

<span id="BKMK_10"></span>
#### Jakie algorytmy szyfrowania są stosowane w programie RMS?

Program RMS korzysta z 2048-bitowych kluczy RSA w przypadku serwera RMS i z kluczy o długości 1024 bitów w przypadku użytkownika i komputera.

<span id="BKMK_11"></span>
#### Czy program RMS korzysta z algorytmów kryptograficznych FIPS?

W programie RMS z dodatkiem Service Pack 1 lub nowszym skrytki generowane przez aplikację klienta RMS korzystają z algorytmu kryptograficznego AES z certyfikatem FIPS w przypadku klienta zainstalowanego na komputerze z systemem Windows XP lub Windows Server 2003. Jeśli jednak klient RMS jest zainstalowany na komputerze z systemem Windows 2000, biblioteka AES z certyfikatem FIPS nie jest zainstalowana, wskutek czego skrytki nie są zgodne ze standardem FIPS.

<span id="BKMK_12"></span>
#### Czy w przypadku licencji publikacji lub szablonów, które udzielają uprawnień za pośrednictwem listy rozpowszechniania, licencje użytkowania są traktowane w inny sposób, aby zapewnić możliwość dynamicznego weryfikowania członków listy?

Licencje użytkowania są zawsze wydawane indywidualnym użytkownikom. Jeśli licencja publikacji lub szablon odwołuje się do grupy, program RMS uwzględnia przynależność do grup w momencie wydania licencji użytkowania. Jeśli użytkownik żądający licencji należy do odpowiedniej grupy, licencja użytkowania zostaje wystawiona indywidualnie dla użytkownika.

<span id="BKMK_13"></span>
#### Kiedy program RMS jest używany za pośrednictwem kiosku, następuje wydanie tymczasowego certyfikatu konta praw. Czym certyfikat tymczasowy różni się od certyfikatu zwykłego? W jaki sposób program RMS wykrywa, że został wywołany z kiosku?

Aplikacja obsługująca technologię RMS musi ustalić, czy klient RMS powinien żądać tymczasowego czy standardowego certyfikatu konta praw dla użytkownika. Nie istnieje żadna metoda pozwalająca automatycznie wykryć taką sytuację. Microsoft Office 2003 jest przykładem aplikacji obsługującej technologię RMS, która pozwala użytkownikowi wybrać właściwy typ certyfikatu.

Główna różnica między tymczasowym a standardowym certyfikatem konta praw polega na obecności identyfikatora zabezpieczeń użytkownika oraz na określeniu czasu ważności. Certyfikaty tymczasowe nie zawierają identyfikatora zabezpieczeń użytkownika i mają okres ważności wyrażony w minutach. Domyślny czas ważności tymczasowego certyfikatu konta praw wynosi 15 minut. Standardowe certyfikaty konta praw zawierają identyfikator zabezpieczeń użytkownika i mają okres ważności wyrażony w dniach. Domyślny czas ważności standardowego certyfikatu konta praw wynosi 365 dni.

<span id="BKMK_14"></span>
#### W jakich sytuacjach używany jest tymczasowy certyfikat konta praw?

Tymczasowy certyfikat konta praw ma w założeniu umożliwić korzystanie użytkownikowi z zawartości chronionej technologią RMS na komputerze spełniającym dowolny z poniższych warunków:

-   Komputer nie należący do tego samego lasu, co instalacja programu RMS, z której uzyskano certyfikat.
-   Komputer nie należący do lasu, w którym znajduje się konto użytkownika.
-   Komputer, z którego użytkownik może w przyszłości już nie korzystać.

Przykłady komputerów spełniających te kryteria to komputery dostępne publicznie na lotniskach, w bibliotekach i kawiarniach internetowych.

<span id="BKMK_15"></span>
#### Czy program RMS wydaje certyfikaty typu X.509v3?

Nie. Program RMS wydaje certyfikaty XrML mające reprezentować użytkowników i zasady dostępu wykraczające poza zakres stosowania certyfikatów X.509v3.

<span id="BKMK_16"></span>
#### Gdzie są przechowywane certyfikaty XrML?

System RMS korzysta z następujących certyfikatów i licencji zapisywanych w formacie XrML na komputerze klienta.

-   Certyfikat komputera
    Nazwa pliku: Plik CERT-Machine.drm
    Lokalizacja: %USERPROFILE%\\Ustawienia lokalne\\Dane aplikacji\\Microsoft\\DRM\\
-   Certyfikat konta praw dostępu
    Przedrostek nazwy pliku: GIC
    Lokalizacja: %USERPROFILE%\\Ustawienia lokalne\\Dane aplikacji\\Microsoft\\DRM
-   Certyfikat licencjodawcy klienta
    Przedrostek nazwy pliku: CLC
    Lokalizacja: %USERPROFILE%\\Ustawienia lokalne\\Dane aplikacji\\Microsoft\\DRM
-   Licencja użytkowania
    Przedrostek nazwy pliku: EUL
    Lokalizacja: %USERPROFILE%\\Ustawienia lokalne\\Dane aplikacji\\Microsoft\\DRM

> [!note]  
> Z kontem użytkownika skojarzony jest pojedynczy certyfikat komputera, plik GIC i plik CLC oraz wiele plików EUL dla każdej jednostki zawartości, z której użytkownik korzysta. 

> [!note]  
> W przypadku klientów zintegrowanych z systemem Windows Vista® lokalizacja to %USERPROFILE%\\AppData\\Local\\Microsoft\\DRM. 

<span id="BKMK_17"></span>
#### Gdzie są przechowywane klucze prywatny i publiczny komputera?

Klucz prywatny komputera jest przechowywany w bezpiecznym miejscu i chroniony przy użyciu kluczy kryptograficznych związanych z poświadczeniami logowania użytkownika i zależnych od konfiguracji komputera.

<span id="BKMK_18"></span>
#### Gdzie są przechowywane klucze prywatny i publiczny klienta?

Para kluczy związana z kontem użytkownika jest przechowywana w certyfikacie konta praw.

<span id="BKMK_19"></span>
#### AES jest algorytmem symetrycznym. W jaki sposób zapewnia się bezpieczne przekazanie kluczy między serwerem a użytkownikiem?

W systemie są używane zarówno klucze symetryczne, jak i pary kluczy prywatny-publiczny. Zawartość jest szyfrowana przy użyciu klucza symetrycznego, jednak pozostałe klucze używane w systemie (użytkownika, komputera i serwera) są to klucze prywatne/publiczne RSA. Symetryczny klucz zawartości jest zawsze przechowywany w postaci zaszyfrowanej w różnych licencjach — albo w postaci klucza publicznego RSA serwera RMS w licencji publikacji, albo w postaci klucza publicznego RSA użytkownika w licencji użytkowania.
