---
TOCTitle: Obsługa serwerów programu RMS
Title: Obsługa serwerów programu RMS
ms:assetid: '1533426b-89c2-43e0-8068-ca97ddab8606'
ms:contentKeyID: 18123249
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720205(v=WS.10)'
---

Obsługa serwerów programu RMS
=============================

Obsługa serwera programu RMS polega na wykonywaniu zadań związanych z zarządzaniem po rozmieszczeniu programu RMS w organizacji. W tym temacie zamieszczono informacje pomocne w zarządzaniu serwerem programu RMS, omówiono także procedury związane z typowymi zadaniami administracyjnymi oraz podano dane zasobów, w których można znaleźć dodatkowe informacje, a także najważniejsze wskazówki.

W tym temacie

-   [Zarządzanie programem RMS](https://technet.microsoft.com/9b573c55-c14c-436c-b3c5-7ba445de1562)
-   [Jak — RMS...](https://technet.microsoft.com/82032075-f361-438f-a2c4-93ab29ae6cff)
-   [RMS — zasoby](https://technet.microsoft.com/d91221cf-e38e-4add-b7b9-50e63aad9a28)

Terminologia używana w tym przewodniku
--------------------------------------

**certyfikacja konta**  
Proces polegający na kojarzeniu kont użytkowników z parami kluczy w certyfikacie konta praw lub certyfikacie RAC.

<!-- -->

**usługa certyfikacji kont**  
Usługa sieci Web programu RMS, która umożliwia tworzenie i rozpowszechnianie certyfikatów konta praw dostępu. Zobacz także: certyfikacja konta.

<!-- -->

**usługa serwera proxy aktywacji**  
Usługa sieci Web programu RMS, która obsługuje aktywację komputerów klienckich programu RMS w wersji 1.0. Służy do przesyłania dalej żądań aktywacji komputerów do usługi aktywacji firmy Microsoft. Usługa aktywacji generuje unikatową skrytkę i odpowiadający jej certyfikat komputera z programem RMS dla komputera klienckiego, które są następnie przesyłane z powrotem przez usługę aktywacji serwera proxy na serwerze programu RMS do klienta wysyłającego żądanie. Zobacz także: skrytka.

<!-- -->

**usługa administracji**  
Usługa sieci Web programu RMS, w której znajduje się administracyjna witryna sieci Web oraz która umożliwia zarządzanie programem RMS i aktualizuje bazę danych konfiguracji klastra.

<!-- -->

**manifest aplikacji**  
Dokument XML opisujący moduły skojarzonej aplikacji obsługującej technologię RMS, a także elementy, które mogą być uruchomione w środowisku aplikacji. Każda aplikacja dokonująca zapisu do interfejsów API klienta programu RMS w celu utworzenia lub wykorzystania informacji chronionych technologią RMS musi w chwili uruchomienia przedstawić manifest.

<!-- -->

**atrybut**  
W usłudze Active Directory jest to właściwość obiektu. W przypadku każdej klasy obiektu schemat definiuje niezbędne i opcjonalne atrybuty instancji klasy.

<!-- -->

**wiązanie**  
Mechanizm realizacji praw do dostępu w systemie RMS, w którym klient RMS sprawdza, czy żądane prawa dostępu są poprawne z punktu widzenia warunków licencji użytkowania. Jeśli warunki te są spełnione, prawa dostępu zostają udzielone.

<!-- -->

**certyfikat**  
Cyfrowy dokument, który jest często stosowany do uwierzytelniania oraz zabezpieczania informacji w sieciach otwartych. Certyfikat w bezpieczny sposób wiąże klucz publiczny z jednostką, która ma odpowiadający mu klucz prywatny. Certyfikaty są cyfrowo podpisywane przez urzędy certyfikacji (CA) i mogą zostać wystawione użytkownikowi, komputerowi lub usłudze. Zobacz także: klucz prywatny, klucz publiczny.

<!-- -->

**rejestrowanie klienta**  
Proces tworzenia certyfikatu licencjodawcy klienta, dzięki któremu komputer lub urządzenie użytkownika może tworzyć licencje publikacji honorowane przez serwer licencji.

<!-- -->

**certyfikat licencjodawcy klienta**  
Certyfikat tworzony przez serwer programu RMS i umieszczany na komputerach klienckich programu RMS, dzięki któremu użytkownicy mogą publikować chronioną zawartość w trybie offline, bez połączenia z siecią obsługującą technologię RMS. Certyfikat licencjodawcy klienta zawiera klucz wykorzystywany przez klienta RMS do cyfrowego podpisywania licencji publikacji.

<!-- -->

**warunek**  
Zestaw określonych ograniczeń i parametrów, które wchodzą w skład grupy praw dostępu związanej z licencją publikacji. Warunki są egzekwowane podczas użytkowania. Warunek czasowy jest powszechnie wykorzystywanym warunkiem, pozwalającym użytkownikowi na określenie daty wygaśnięcia informacji chronionych technologią RMS.

<!-- -->

**baza danych konfiguracji**  
Baza danych zawierająca informacje o konfiguracji programu RMS na potrzeby serwera lub klastra.

<!-- -->

**użytkowanie zawartości**  
Odszyfrowanie i realizacja praw użytkowania względem elementu chronionej zawartości.

<!-- -->

**klucz zawartości**  
Klucz służący zarówno do szyfrowania, jak i odszyfrowywania chronionej zawartości w trakcie publikacji i użytkowania. Nazywany także kluczem symetrycznym. Program RMS wykorzystuje 128-bitowe klucze zawartości w standardzie AES.

<!-- -->

**właściciel zawartości**  
Osoba lub organizacja ustalająca zasady dostępu do chronionej zawartości.

<!-- -->

**odszyfrowywanie**  
Proces odczytywania zaszyfrowanych danych przez przekształcenie tekstu szyfrowanego na tekst zwykły.

<!-- -->

**podpis cyfrowy**  
Rozwiązanie pozwalające autorowi wiadomości, pliku lub innych danych zaszyfrowanych cyfrowo powiązać własną tożsamość z danymi. Proces cyfrowego podpisywania informacji obejmuje przekształcenie informacji oraz niektórych informacji poufnych będących własnością nadawcy w tag nazywany podpisem. Podpisy cyfrowe są używane w środowiskach kluczy publicznych oraz umożliwiają prawidłowe działanie i integralność usług.

<!-- -->

**usługa DRMRemote**  
Usługa sieci Web programu RMS, która uwidacznia usługi poprzez platformę .NET Remoting służącą do komunikacji między różnymi serwerami programu RMS.

<!-- -->

**szyfrowanie**  
Proces konwersji informacji do postaci odczytywanej tylko przez określonego odbiorcę. Szyfrowanie to skuteczny sposób zabezpieczania informacji. Aby odszyfrować zaszyfrowany plik, odbiorca musi mieć klucz poufny oraz hasło umożliwiające jego przetłumaczenie. Zobacz także: szyfrowanie za pomocą klucza publicznego.

<!-- -->

**rejestrowanie**  
Proces polegający na tym, że serwer głównej certyfikacji uzyskuje certyfikat licencjodawcy serwera podpisany przez usługę rejestrowania firmy Microsoft.

<!-- -->

**żądanie rejestrowania**  
Żądanie certyfikatu licencjodawcy serwera wysyłane przez serwer głównej certyfikacji programu RMS do usługi rejestrowania firmy Microsoft.

<!-- -->

**wykluczanie**  
Proces pozwalający serwerowi programu RMS odmówić klientowi licencji użytkowania w oparciu o zasady wykluczania. Zobacz także: lista wykluczania.

<!-- -->

**lista wykluczania**  
Lista podmiotów, którym usługa licencjonowania programu RMS ma odmawiać licencji.

<!-- -->

**zasady wykluczania**  
Ustawienia w bazie danych konfiguracji programu RMS, od których zależy sposób stosowania wykluczeń w danej organizacji.

<!-- -->

**język eXtensible Rights Markup Language**  
Format oparty na języku XML używany przez program RMS we wszystkich obsługiwanych przez niego licencjach: certyfikatach komputerów, certyfikatach RAC, certyfikatach CLC, licencjach użytkowania, licencjach publikacji i certyfikatach licencjodawcy serwera, które są dokumentami określającymi zasady programu RMS dotyczące chronionej zawartości.

<!-- -->

**licencja wystawiania**  
Dane określające zasady zarządzania prawami dostępu stosowane do chronionej zawartości.

<!-- -->

**klaster licencji**  
Jeden lub kilka serwerów, na których uruchomione są usługi licencjonowania i publikacji programu RMS poza klastrem głównej certyfikacji. Serwery te korzystają ze wspólnego adresu URL połączenia oraz bazy danych i powinny być rozmieszczane za oprogramowaniem lub urządzeniem służącym do równoważenia obciążenia w przypadku korzystania z więcej niż jednego serwera. W odróżnieniu od klastra certyfikacji czy klastra głównego serwery programu RMS wchodzące w skład klastra licencji nie mogą przeprowadzać certyfikacji użytkowników.

<!-- -->

**serwer licencji**  
Serwer, na którym uruchomione są usługi licencjonowania i publikacji programu RMS poza klastrem głównej certyfikacji.

<!-- -->

**usługa licencjonowania**  
Usługa sieci Web programu RMS, która odpowiada za wystawianie licencji użytkowania.

<!-- -->

**skrytka**  
Moduł oprogramowania odpowiedzialny za uwierzytelnianie prawidłowego korzystania z chronionej zawartości, szyfrowanie i odszyfrowywanie informacji oraz za ochronę zaufanego przetwarzania programowego przed modyfikacją i obserwacją. Nazywana także bezpiecznym repozytorium.

<!-- -->

**usługa rejestrowania**  
Usługa odbiornika programu RMS, która przenosi rejestrowane dane z kolejki wiadomości do bazy danych rejestrowania danego serwera lub klastra programu RMS.

<!-- -->

**aktywacja komputera**  
Proces uzyskiwania unikatowej skrytki i certyfikatu dla komputera w programie RMS w wersji 1.0. W programie RMS w wersji 1.0 z dodatkiem SP1 aktywacja komputera jest procesem uzyskiwania certyfikatu komputera dla każdego jego użytkownika.

<!-- -->

**manifest**  
Podpisany dokument XML wskazujący biblioteki lub programy, które mogą oraz które nie mogą być ładowane do obszaru przetwarzania aplikacji.

<!-- -->

**usługa aktywacji firmy Microsoft**  
Usługa sieci Web obsługiwana przez firmę Microsoft, która odpowiada za wystawianie certyfikatów komputerów z programem RMS i skrytek w odpowiedzi na żądania klientów z programem RMS w wersji 1.0.

<!-- -->

**usługa rejestrowania firmy Microsoft**  
Usługa sieci Web obsługiwana przez firmę Microsoft, która odpowiada za wystawienie certyfikatu licencjodawcy serwera serwerowi głównej certyfikacji w rozmieszczeniu programu RMS.

<!-- -->

**certyfikacja wstępna**  
Funkcja usługi certyfikacji programu RMS, która umożliwia aplikacji żądanie certyfikatu konta praw dostępu od serwera programu RMS w imieniu użytkownika. Certyfikaty konta praw dostępu uzyskane za pomocą certyfikacji wstępnej zawierają tylko klucz publiczny użytkownika.

<!-- -->

**podmiot**  
Tożsamość (użytkownik, grupa lub menedżer chronionej zawartości), która pełni określoną rolę w schemacie zabezpieczeń technologii RMS i dla której można zabezpieczać obiekty.

<!-- -->

**klucz prywatny**  
Poufna połowa pary klucza kryptograficznego używanego z algorytmem klucza publicznego. Klucze prywatne służą zazwyczaj do odszyfrowywania symetrycznych kluczy sesji, cyfrowego podpisywania danych lub odszyfrowywania danych zaszyfrowanych za pomocą odpowiadającego im klucza publicznego. Zobacz także: klucz publiczny, szyfrowanie za pomocą klucza publicznego.

<!-- -->

**zastrzeganie**  
Konfigurowanie serwera programu RMS do pracy w danej organizacji.

<!-- -->

**klucz publiczny**  
Niepoufna połowa pary klucza kryptograficznego używanego z algorytmem klucza publicznego. Klucze publiczne służą zazwyczaj do szyfrowania kluczy sesji, sprawdzania podpisów cyfrowych, lub szyfrowania danych, które można odszyfrować za pomocą odpowiadającego im klucza prywatnego. Zobacz także: klucz prywatny, szyfrowanie za pomocą klucza publicznego.

<!-- -->

**szyfrowanie za pomocą klucza publicznego**  
Metoda szyfrowania, w której używa się dwóch powiązanych matematycznie kluczy szyfrujących. Jeden klucz jest kluczem prywatnym i jest on poufny. Drugi to tak zwany klucz publiczny, który jest udostępniany wszystkim jednostkom biorącym udział w wymianie korespondencji. W typowym scenariuszu nadawca korzysta z klucza publicznego odbiorcy w celu zaszyfrowania wiadomości. Tylko odbiorca ma powiązany z tym kluczem klucz prywatny umożliwiający odszyfrowanie wiadomości. O ile klucze mają odpowiednią długość, złożoność relacji między kluczem publicznym i prywatnym sprawia, że ich rozróżnienie za pomocą obliczeń jest niemożliwe. Nazywane także szyfrowaniem asymetrycznym. Zobacz także: klucz prywatny, klucz publiczny.

<!-- -->

**licencja publikacji**  
Licencja tworzona przy publikowaniu zawartości chronionej technologią RMS. Określa miedzy innymi użytkowników, którzy będą mieli dostęp do zawartości, przyznawane im prawa oraz warunki uzyskiwania dostępu do takiej zawartości. Nazywana także licencją wystawiania.

<!-- -->

**usługa publikacji**  
Usługa programu RMS, która odpowiada za podpisywanie licencji publikacji i wystawianie certyfikatów licencjodawcy klienta. Zobacz także: certyfikat licencjodawcy klienta, licencja publikacji.

<!-- -->

**RAC**  
Zobacz definicję certyfikatu konta praw.

<!-- -->

**odwołanie**  
Proces, skutkiem którego podmioty figurują jako mające nieprawidłowe licencje.

<!-- -->

**lista odwołania**  
Dokument w języku XrML, w którym wymienione są certyfikaty i licencje odwołane przez wystawcę. Zobacz także: odwołanie.

<!-- -->

**prawo**  
Czynność, którą określeni użytkownicy mogą wykonywać wobec zawartości chronionej za pomocą technologii RMS. Te prawa dostępu można ograniczać przez zastosowanie warunków.

<!-- -->

**certyfikat konta praw dostępu (RAC)**  
Certyfikat, który przy użyciu certyfikatu komputera z aktywacji programu RMS wiąże konto i klucz użytkownika z konkretnymi komputerami lub grupami komputerów. Składniki tego certyfikatu służą do zezwalania użytkownikom na korzystanie z chronionej zawartości. W zestawie RMS SDK nazywany również certyfikatem tożsamości grupowej (GIC).

<!-- -->

**zarządzanie prawami dostępu**  
Technologia zapewniająca trwałą ochronę danych cyfrowych za pomocą szyfrowania, certyfikatów i uwierzytelniania. Autoryzowani adresaci lub użytkownicy muszą uzyskać licencję, dzięki której mogą następnie użytkować chronione pliki zgodnie z prawami dostępu lub regułami firmowymi określonymi przez właściciela zawartości.

<!-- -->

**Klient programu Usługi zarządzania prawami dostępu**  
Zestaw interfejsów API technologii RMS, które muszą być zainstalowane na każdym komputerze klienckim w systemie RMS. Jest on warunkiem wstępnym aktywacji komputera, którego spełnienie jest niezbędne do korzystania z aplikacji obsługujących technologię RMS.

<!-- -->

**szablon zasad praw dostępu**  
Określa standardowy zestaw użytkowników, praw dostępu i warunków, które można zastosować do zawartości chronionej technologią RMS. Kiedy użytkownik zastosuje szablon zasad praw dostępu do elementu zawartości, prawa dostępu i warunki określone w tym szablonie stają się elementem licencji publikacji.

<!-- -->

**aktywacja programu RMS**  
Proces umieszczenia skrytki na komputerze użytkownika końcowego w programie RMS w wersji 1.0. Proces ten może być wykonany tylko przez usługę aktywacji technologii RMS i jest niezbędny do korzystania z technologii RMS. W programie RMS w wersji 1.0 z dodatkiem SP1 jest to proces uzyskiwania certyfikatu komputera dla jego użytkownika i nie wymaga połączenia z usługą aktywacji programu RMS. Nazywany też aktywacją.

<!-- -->

**Usługa certyfikacji programu RMS**  
Usługa sieci Web obsługiwana przez firmę Microsoft, która odpowiada za wystawianie certyfikatów konta praw dostępu użytkownikom na podstawie ich poświadczeń z usługi Microsoft .NET Passport.

<!-- -->

**klient programu RMS**  
Zestaw interfejsów API technologii RMS, które muszą być zainstalowane na każdym komputerze klienckim w systemie RMS. Jest on warunkiem wstępnym aktywacji komputera, którego spełnienie jest niezbędne do korzystania z aplikacji obsługujących technologię RMS.

<!-- -->

**certyfikat komputera z programem RMS**  
Certyfikat umieszczany na komputerze użytkownika końcowego podczas aktywacji technologii RMS. Klucz publiczny zawarty w tym certyfikacie służy do szyfrowania klucza prywatnego zawartego w certyfikatach konta praw dostępu użytkownika.

<!-- -->

**aplikacja obsługująca technologię RMS**  
Aplikacja, której możliwości rozszerzono przy użyciu zestawu Rights Management Services SDK, dzięki czemu pozwala ona użytkownikom na określanie praw dostępu dotyczących tworzonej przez nich zawartości.

<!-- -->

**komputer obsługujący technologię RMS**  
Komputer, na którym zainstalowany jest składnik klienta RMS i który przeszedł proces aktywacji komputera technologii RMS, dzięki czemu może przetwarzać zawartość chronioną za pomocą programu RMS.

<!-- -->

**zawartość chroniona technologią RMS**  
Informacje cyfrowe chronione za pomocą technologii RMS.

<!-- -->

**klaster głównej certyfikacji**  
Jeden lub więcej serwerów w rozmieszczeniu programu RMS, na których uruchomione są usługi administracji, rejestrowania, certyfikacji konta, serwera proxy aktywacji, licencjonowania i publikacji. Serwery te korzystają ze wspólnego adresu URL połączenia oraz bazy danych i powinny być rozmieszczane za oprogramowaniem lub urządzeniem służącym do równoważenia obciążenia. Na jeden las usługi Active Directory może przypadać tylko jeden klaster głównej certyfikacji.

<!-- -->

**serwer głównej certyfikacji**  
Podstawowy serwer w rozmieszczeniu programu RMS, na którym uruchomione są usługi administracji, rejestrowania, certyfikacji konta, serwera proxy aktywacji, licencjonowania i publikacji. Na jeden las usługi Active Directory może przypadać tylko jeden serwer głównej certyfikacji.

<!-- -->

**fundament zaufania**  
Zaufany podmiot stanowiący podstawę zaufania do innych certyfikatów. Fundamentowi zaufania muszą ufać wszyscy dostawcy certyfikatów i ostateczny użytkownik.

<!-- -->

**identyfikator zabezpieczeń (SID)**  
Struktura danych systemu Windows służąca do identyfikacji wszystkich kont użytkowników, grup i komputerów systemu Windows. Podczas pierwszego tworzenia konta, dla każdego konta w sieci jest wystawiany unikatowy identyfikator SID. Wewnętrzne procesy w systemie Windows odnoszą się do identyfikatora SID konta, a nie do użytkownika konta lub nazwy grupy.

<!-- -->

**certyfikat licencjodawcy serwera**  
Certyfikat określający poświadczenia serwera programu RMS, dzięki czemu serwer ten staje się prawidłową usługą certyfikacji i licencjonowania i może zacząć działać. Certyfikat licencjodawcy zawiera klucz publiczny wykorzystywany do szyfrowania kluczy zawartości w licencjach publikacji.

<!-- -->

**usługa serwera**  
Usługa sieci Web programu RMS, która z założenia ma być wykorzystywana przez inną usługę.

<!-- -->

**punkt połączenia usługi (SCP)**  
Obiekt usługi Active Directory, który zawiera odwołanie do adresu URL klastra głównej certyfikacji w rozmieszczeniu programu RMS. Klient programu RMS korzysta z tych informacji w celu lokalizacji jego usług.

<!-- -->

**podrejestrowanie**  
Część procesu zastrzegania dla serwera licencji, w wyniku którego serwer licencji otrzymuje certyfikat licencjodawcy serwera z klastra głównej certyfikacji.

<!-- -->

**żądanie podrejestrowywania**  
Żądanie certyfikatu licencjodawcy serwera, wysłane przez serwer licencji do klastra głównej certyfikacji.

<!-- -->

**usługa podrejestrowywania**  
Usługa sieci Web programu RMS na serwerze głównej certyfikacji, która odpowiada na żądania certyfikatów licencjodawcy serwera zgłaszanych przez serwery licencji podczas zastrzegania.

<!-- -->

**administrator**  
Członek grupy administratorów.

<!-- -->

**grupa administratorów**  
Opcjonalna, administracyjnie zdefiniowana grupa użytkowników każdego klastra programu RMS, która przy otwieraniu zawartości opublikowanej przez dany serwer programu RMS otrzymuje od tego serwera licencje właścicielskie.

<!-- -->

**licencja użytkowania**  
Licencja zawierająca wykaz praw i warunków, określających zasady korzystania przez użytkowników końcowych z chronionej zawartości. Nazywana też licencją użytkownika końcowego (EUL).
