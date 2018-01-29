---
TOCTitle: Korzystanie ze strony głównej administracji
Title: Korzystanie ze strony głównej administracji
ms:assetid: '6c155977-bd0e-47d6-ac65-1746cddb505e'
ms:contentKeyID: 18123304
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720290(v=WS.10)'
---

Korzystanie ze strony głównej administracji
===========================================

Na **stronie głównej administracji** w sieci Web można wyświetlać informacje na temat serwera lub klastra oraz uzyskiwać dostęp do opcji administracyjnych. Ta strona jest dostępna wyłącznie po zastrzeżeniu serwera.

Aby uzyskać dostęp do tej strony sieci Web z serwera, którego ma dotyczyć administrowanie, wykonaj następujące kroki:

1.  Zaloguj się jako administrator lokalny.
2.  Kliknij przycisk **Start**, wskaż polecenie **Wszystkie programy**, wskaż polecenie **Windows RMS**, a następnie wybierz polecenie **Administracja programem Windows RMS**.
3.  Na stronie **Administracja globalna** kliknij łącze **Administruj programem RMS w tej witrynie sieci Web**.

Jeśli włączono administrowanie zdalne za pomocą protokołu SSL (Secure Sockets Layer), dostęp do **strony głównej administracji** można także uzyskać z innego komputera, wykonując następujące czynności:

1.  W pasku adresu przeglądarki sieci Web wpisz następujący adres URL:
    https://*nazwa\_klastra:numer\_portu*/\_wmcs/admin
    Gdzie *nazwa\_klastra:numer\_portu* jest adresem URL, który określono dla danego klastra podczas zastrzegania. Numer portu należy podawać tylko w przypadku, gdy określono port inny od domyślnego o numerze 80.
2.  Po wyświetleniu monitu, wpisz poświadczenia lokalnego administratora na serwerze, do którego uzyskujesz dostęp.

Na **stronie głównej administracji** wyświetlane są informacje na temat klastra, takie jak jego adres URL, nazwa i lokalizacja bazy danych konfiguracji, data wygaśnięcia certyfikatu licencjodawcy serwera itp. Znajdują się tam również łącza do stron, na których można konfigurować następujące opcje administracji dotyczące klastra:

-   **Zasady zaufania.**Umożliwiają dodawanie i usuwanie zaufanych domen. Aby uzyskać więcej informacji, zobacz „[Zarządzanie zaufaniem i zasady zaufania](https://technet.microsoft.com/1c96ee74-fd28-4511-be21-087e2b04c3ee)” w dalszej części tego tematu.
-   **Szablony zasad praw dostępu**. Umożliwiają tworzenie i modyfikowanie szablonów zasad praw dostępu. Aby uzyskać więcej informacji, zobacz „[Zarządzanie szablonami zasad praw dostępu](https://technet.microsoft.com/718286dc-3399-4556-96c9-ec3a33d31877)” w dalszej części tego tematu.
-   **Ustawienia rejestrowania**. Umożliwiają włączanie i wyłączanie rejestrowania oraz wyświetlanie nazwy serwera i bazy danych rejestrowania. Aby uzyskać więcej informacji, zobacz „[Zarządzanie rejestrowaniem](https://technet.microsoft.com/8fccfc57-2135-494e-8e44-f6191bf5e4a0)” w dalszej części tego tematu.
-   **Ustawienia adresu URL klastra ekstranetowego.**Umożliwiają określenie dostępnego na zewnątrz adresu URL na potrzeby żądań licencji i certyfikacji konta. Aby uzyskać więcej informacji, zobacz „[Konfigurowanie adresu URL w sieci ekstranet](https://technet.microsoft.com/88fec9ff-c96c-4d20-8856-0485e7507572)” w dalszej części tego tematu.
-   **Ustawienia serwera proxy programu RMS.** Umożliwiają określenie adresu serwera proxy, typu uwierzytelniania oraz nazwy użytkownika, które należy stosować w sytuacji, gdy serwer programu RMS musi łączyć się z Internetem przez serwer proxy. Aby uzyskać więcej informacji, zobacz „[Konfigurowanie ustawień serwera proxy programu RMS](https://technet.microsoft.com/179d2970-62e9-4487-aa5b-f4334234991e)” w dalszej części tego tematu.
-   **Ustawienia zabezpieczeń.** Umożliwiają resetowanie hasła klucza prywatnego serwera, określanie grup administratorów, których członkowie mogą odszyfrowywać licencjonowaną zawartość, a także likwidowanie programu RMS. Aby uzyskać więcej informacji, zobacz „[Zarządzanie zabezpieczeniami podczas korzystania z programu RMS](https://technet.microsoft.com/62050812-de4f-4392-8d63-f2f89aa01ed4)” w dalszej części tego tematu.
-   **Ustawienia certyfikacji.** Umożliwiają określanie okresu ważności certyfikatów konta praw, a także określanie kontaktu administracyjnego. (Ta opcja jest dostępna tylko w klastrze głównej certyfikacji, nie na serwerach licencji.) Aby uzyskać więcej informacji, zobacz „[Zarządzanie certyfikatami kont praw](https://technet.microsoft.com/49c5c2ba-e197-4e4b-b3b3-b3248f068bcc)” w dalszej części tego tematu.
-   **Zasady wykluczania.** Umożliwiają określanie wykluczeń na podstawie wersji skrytki, certyfikatu konta praw, wersji systemu Windows lub aplikacji obsługującej technologię RMS. Aby uzyskać więcej informacji, zobacz „[Zarządzanie zasadami wykluczania](https://technet.microsoft.com/ee31e099-e095-4648-95da-0009fbeb48cb)” w dalszej części tego tematu.
-   **Raport certyfikacji konta RM.** Umożliwia sprawdzenie liczby wystawionych certyfikatów konta praw. (Ta opcja jest dostępna tylko w klastrze głównej certyfikacji, nie na serwerach licencji.) Aby uzyskać więcej informacji, zobacz „[Śledzenie certyfikatów konta praw](https://technet.microsoft.com/5bb0f3cf-fc44-4e60-a93f-c789d6f8a902)” w dalszej części tego tematu.

W pozostałych tematach zawartych w tej części opisano sposoby korzystania z tych funkcji. Aby uzyskać instrukcje krok po kroku, zobacz „[Jak — RMS...](https://technet.microsoft.com/82032075-f361-438f-a2c4-93ab29ae6cff)” w dalszej części tego tematu.

> [!note]  
> W administracyjnej witrynie sieci Web programu RMS używane są okna wyskakujące służące do konfigurowania niektórych funkcji. W przypadku korzystania z programu do blokowania okien wyskakujących w przeglądarce sieci Web należy skonfigurować ustawienia przeglądarki w taki sposób, aby zezwolić na wyświetlanie okien wyskakujących w administracyjnej witrynie sieci Web programu RMS. 
