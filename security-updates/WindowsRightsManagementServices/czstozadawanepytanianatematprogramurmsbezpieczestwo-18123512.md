---
TOCTitle: 'Często zadawane pytania na temat programu RMS: Bezpieczeństwo'
Title: 'Często zadawane pytania na temat programu RMS: Bezpieczeństwo'
ms:assetid: 'ff433834-79aa-481f-bd39-3393be12a26f'
ms:contentKeyID: 18123512
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747757(v=WS.10)'
---

Często zadawane pytania na temat programu RMS: Bezpieczeństwo
=============================================================

Pytania dotyczące bezpieczeństwa w programie RMS
------------------------------------------------

-   [Co to jest konto administratora?](#bkmk_43)
-   [Czy RMS jest systemem zabezpieczeń?](#bkmk_44)
-   [Jakie mechanizmy chronią przed sytuacją, w której odbiorca może cofnąć zegar na komputerze klienckim w celu swobodnego korzystania z dokumentu chronionego prawami dostępu po wygaśnięciu licencji użytkowania?](#bkmk_45)
-   [Czy członkowie grupy administratorów domeny mogą odczytywać dokumenty przeznaczone dla użytkowników z ich domeny?](#bkmk_46)
-   [Jak rozumiem, każda skrytka może weryfikować autentyczność każdego certyfikatu lub licencji wygenerowanych w systemie jako pochodzących od usługi zarejestrowanej przez firmę Microsoft. Przed jakimi zagrożeniami taki system ma chronić?](#bkmk_47)
-   [Czy otwarcie jednego dokumentu w drodze ataku siłowego pozwala później wykorzystać znaleziony klucz do otwierania innych dokumentów?](#bkmk_48)
-   [Czy w związku z restrykcjami w kwestii eksportu technologii kryptograficznych jakiekolwiek części kluczy są eksponowane poza firmą, w której dokonano rozmieszczenia programu?](#bkmk_49)
-   [W jaki sposób można się uchronić przed atakiem polegającym na zdalnym włączeniu funkcji likwidowania instalacji?](#bkmk_50)
-   [Czy użytkownik może przechwycić ekran, na którym wyświetlona jest zawartość chroniona prawami dostępu?](#bkmk_51)
-   [Czy administratorzy zajmujący się sporządzaniem kopii zapasowej plików związanych z programem RMS mogą uzyskać dostęp do zawartości chronionej prawami dostępu?](#bkmk_52)
-   [Czy plik wymiany używany przez system Windows zawiera w którymś momencie zawartość w postaci odszyfrowanej, a więc podatnej na ominięcie ochrony praw dostępu?](#bkmk_53)
-   [Czy można ustalić, którzy administratorzy będą mieli dostęp do poszczególnych funkcji administracyjnych w programie RMS?](#bkmk_54)
-   [Czy program RMS może objąć ochroną indywidualne dokumenty bezpośrednio po ich utworzeniu, jeszcze na dysku twardym użytkownika lub w folderze udostępnionym?](#bkmk_55)
-   [Czy podczas gdy plik jest otwarty, jego kopie zapisywane na dysku przez funkcje automatycznego zapisu i zapisywania wersji tymczasowych są zapisywane w postaci szyfrowanej?](#bkmk_56)
-   [Kiedy otrzymuję wiadomość e-mail chronioną prawami dostępu, okazuje się, że wiadomość taka zawiera załącznik. Załącznik ten mogę zapisać, mimo że samej wiadomości zapisać nie można. Czy to oznacza, że program RMS jest uszkodzony?](#bkmk_562)

<span id="BKMK_43"></span>
#### Co to jest konto administratora?

Program RMS tworzy specjalną grupę administratorów, której przysługuje pełna kontrola nad całą zawartością chronioną prawami dostępu. Członkom grupy administratorów udzielane są pełne prawa właścicielskie we wszystkich licencjach użytkowania wystawianych dla nich przez klaster programu RMS, na którym skonfigurowana jest ta grupa. Oznacza to, że członkowie tej grupy mogą odszyfrowywać dowolne pliki z chronioną zawartością i usuwać z nich ochronę. Członek tej grupy może na przykład usunąć ochronę z plików opublikowanych przez pracownika, z którym rozwiązano umowę o pracę, dzięki czemu nowy właściciel jest w stanie publikować te pliki i zarządzać nimi.

<span id="BKMK_44"></span>
#### Czy RMS jest systemem zabezpieczeń?

Nie, RMS nie jest systemem zabezpieczeń. Gdy program ten jest używany w połączeniu z aplikacją obsługującą technologię RMS, jak Office 2007, może być on uznawany za „system egzekwowania zasad dostępu”. Jeśli użytkownik nie ma uprawnień do wyświetlania danych, może zastosować atak siłowy, próbując złamać szyfr. Chociaż algorytm szyfrowania jest silny, można go złamać tak samo, jak każdy inny szyfr programowy. Jeżeli jednak użytkownik ma prawo do wyświetlania danych, może je ręcznie skopiować lub zrobić zdjęcie cyfrowe, które może przekazać użytkownikom nieuprawnionym.

<span id="BKMK_45"></span>
#### Jakie mechanizmy chronią przed sytuacją, w której odbiorca może cofnąć zegar na komputerze klienckim w celu swobodnego korzystania z dokumentu chronionego prawami dostępu po wygaśnięciu licencji użytkowania?

Program RMS wykrywa fakt cofnięcia bądź przyspieszenia zegara w systemie klienckim i uniemożliwia wtedy korzystanie z chronionych dokumentów. Oprócz tego program RMS wykrywa mierzalne różnice w ustawieniach zegara między serwerem a klientem RMS.

<span id="BKMK_46"></span>
#### Czy członkowie grupy administratorów domeny mogą odczytywać dokumenty przeznaczone dla użytkowników z ich domeny?

Użytkownicy grupy administratorów domeny mogą odczytywać zawartość dostępną dla konta zwykłego użytkownika tylko wtedy, gdy należą do grupy administratorów RMS lub gdy chodzi o ich własne konto. Ponieważ członkowie grupy administratorów domeny mają pełną kontrolę nad kontami użytkowników, nie ma żadnego zabezpieczenia przed sytuacją, w której administrator okaże się osobą o złych zamiarach.

Zaleca się, aby członków grupy administratorów domeny dodawać do grupy administratorów, tylko gdy potrzebują dostępu do zawartości chronionej prawami dostępu. Zawsze, gdy członek grupy administratorów RMS uzyskuje licencję dostępu do zawartości, w dzienniku zdarzeń aplikacji serwera RMS zostaje zapisane zdarzenie o identyfikatorze 49. Zdarzenie nr 49 ma komunikat: **„Udzielono licencji użytkownikowi należącemu do grupy administratorów. Użytkownik ma następujący adres poczty e-mail: &lt;Alias użytkownika&gt; ”**, gdzie **alias użytkownika** zostaje zastąpiony właściwym adresem e-mail.

Podobnie jak w przypadku innych grup używanych do limitowania dostępu do zasobów, należy zdefiniować alerty i sprawdzać zabezpieczenia, aby zapobiegać wprowadzaniu do grupy administratorów użytkowników bez wymaganego upoważnienia.

<span id="BKMK_47"></span>
#### Jak rozumiem, każda skrytka może weryfikować autentyczność każdego certyfikatu lub licencji wygenerowanych w systemie jako pochodzących od usługi zarejestrowanej przez firmę Microsoft. Przed jakimi zagrożeniami taki system ma chronić?

Gdyby nie istniał mechanizm weryfikowania wiarygodności certyfikatów, użytkownik mógłby sfałszować certyfikat konta praw wydany w rzeczywistości dla innego użytkownika i uzyskać licencję użytkowania dla siebie albo utworzyć aplikację usuwającą ochronę dokumentu.

<span id="BKMK_48"></span>
#### Czy otwarcie jednego dokumentu w drodze ataku siłowego pozwala później wykorzystać znaleziony klucz do otwierania innych dokumentów?

Każdy dokument chroniony prawami dostępu jest szyfrowany przy użyciu innego, losowo generowanego klucza symetrycznego. Z tego powodu klucz do każdego dokumentu jest niepowtarzalny i bezużyteczny przy odczytywaniu innych dokumentów.

<span id="BKMK_49"></span>
#### Czy w związku z restrykcjami w kwestii eksportu technologii kryptograficznych jakiekolwiek części kluczy są eksponowane poza firmą, w której dokonano rozmieszczenia programu?

Aplikacje podpisane z odwołaniem do certyfikatu głównego firmy Microsoft dają się rozpoznawać jako uczestniczące w hierarchii podpisów klucza firmy Microsoft, ale od tego punktu żadne inne klucze nie są ujawniane ani przez Microsoft, ani system rozmieszczony u klienta.

<span id="BKMK_50"></span>
#### W jaki sposób można się uchronić przed atakiem polegającym na zdalnym włączeniu funkcji likwidowania instalacji?

Atakujący potrzebowałby użyć poświadczeń konta użytkownika mającego uprawnienia administratora w klastrze RMS. Domyślnie interfejs administracyjny RMS jest dostępny tylko lokalnie na serwerze RMS. Jeśli to ustawienie zostanie zachowane, usługa zdalnego pulpitu (protokół RDP) będzie wyłączona, a serwer będzie stał w bezpiecznym miejscu, ryzyko zaistnienia takiej sytuacji będzie minimalne.

<span id="BKMK_51"></span>
#### Czy użytkownik może przechwycić ekran, na którym wyświetlona jest zawartość chroniona prawami dostępu?

Jeśli ustawienia uprawnień w programie RMS przewidują wyłączenie możliwości kopiowania, znany z systemu Windows skrót klawiaturowy Alt+PrtSc nie będzie działać. Jednak w środowiskach bez usług zarządzania pulpitem użytkownik może się posłużyć aplikacją innego producenta do przechwycenia chronionej zawartości.

<span id="BKMK_52"></span>
#### Czy administratorzy zajmujący się sporządzaniem kopii zapasowej plików związanych z programem RMS mogą uzyskać dostęp do zawartości chronionej prawami dostępu?

Nie, możliwość wykonywania kopii zapasowej nie przekłada się u nich na dostęp do zawartości.

<span id="BKMK_53"></span>
#### Czy plik wymiany używany przez system Windows zawiera w którymś momencie zawartość w postaci odszyfrowanej, a więc podatnej na ominięcie ochrony praw dostępu?

Gdy klient RMS odeśle odszyfrowaną zawartość do aplikacji, znajdzie się ona w pliku wymiany. Wśród zaleceń dla programistów, zawartych w pakiecie SDK programu RMS, znajduje się opis sposobu obejścia takiej sytuacji, jednak za jego realizację jest odpowiedzialna aplikacja obsługująca obsługującą technologię RMS.

<span id="BKMK_54"></span>
#### Czy można ustalić, którzy administratorzy będą mieli dostęp do poszczególnych funkcji administracyjnych w programie RMS?

Tak, można tworzyć różne grupy administratorów RMS w katalogu Active Directory, dodawać użytkowników i tworzyć odpowiednie listy kontroli dostępu do stron administracyjnych. Na przykład, zgodnie z domyślną konfiguracją listy praw dostępu do strony administracyjnej programu RMS, strona ta jest dostępna tylko dla użytkownika który rejestrował serwer.

<span id="BKMK_55"></span>
#### Czy program RMS może objąć ochroną indywidualne dokumenty bezpośrednio po ich utworzeniu, jeszcze na dysku twardym użytkownika lub w folderze udostępnionym?

Chociaż program RMS może chronić dokumenty przechowywane na komputerze lokalnym użytkownika, lepszym rozwiązaniem byłoby zastosowanie systemu szyfrowania plików (EFS). System plików EFS zapewnia ochronę dokumentów w sposób niezauważalny dla użytkownika, podczas gdy program RMS wymaga do tego ręcznej interwencji (kilku kliknięć myszy)..

<span id="BKMK_56"></span>
#### Czy podczas gdy plik jest otwarty, jego kopie zapisywane na dysku przez funkcje automatycznego zapisu i zapisywania wersji tymczasowych są zapisywane w postaci szyfrowanej?

Tak, wszystkie pliki tymczasowe są szyfrowane.

<span id="BKMK_562"></span>
#### Kiedy otrzymuję wiadomość e-mail chronioną prawami dostępu, okazuje się, że wiadomość taka zawiera załącznik. Załącznik ten mogę zapisać, mimo że samej wiadomości zapisać nie można. Czy to oznacza, że program RMS jest uszkodzony?

Nie, takie działanie jest zgodne z założeniami. Załącznik jest to szyfrowana wiadomość przed jej odszyfrowaniem przez klienta RMS. Plik ten jest stale chroniony prawami dostępu, a po odszyfrowaniu nie może być zapisany.
