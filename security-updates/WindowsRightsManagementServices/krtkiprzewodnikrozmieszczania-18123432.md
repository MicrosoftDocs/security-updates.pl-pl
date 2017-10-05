---
TOCTitle: Krótki przewodnik rozmieszczania
Title: Krótki przewodnik rozmieszczania
ms:assetid: 'b8fb69b6-3e0b-4836-8c05-8bd93f522a7c'
ms:contentKeyID: 18123432
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747735(v=WS.10)'
---

Krótki przewodnik rozmieszczania
================================

Ten przewodnik ułatwia szybkie skonfigurowanie serwera z programem RMS z dodatkiem Service Pack 1, tak aby można było ocenić i zdecydować, czy rozmieścić ten program w całej organizacji.

**Krok 1 — Przygotowania do używania programu RMS**

Program RMS jest zależny od innych składników, które należy zainstalować i skonfigurować przed rozpoczęciem korzystania z tej usługi. Po wykonaniu poniższych kroków infrastruktura będzie spełniać podstawowe wymagania programu RMS:

1.  Skonfiguruj komputer tak, aby działał na nim system Windows Server 2003, a następnie dołącz komputer do domeny usługi Active Directory. W małych organizacjach mających tylko jeden serwer ten komputer może być także kontrolerem domeny usługi Active Directory. Jednak w takim przypadku na komputerze należy uruchomić system Windows Server 2003 Standard Edition, Windows Server 2003 Enterprise Edition lub Windows Server 2003 Datacenter Edition. Komputer z systemem Windows Server 2003 Web Edition nie może być kontrolerem domeny.
2.  Skonfiguruj serwer tak, aby pełnił funkcję **serwera aplikacji**. W tym celu kliknij przycisk **Start**, kliknij dwukrotnie polecenie **Panel sterowania**, a następnie kliknij dwukrotnie aplet **Dodaj lub usuń programy**. W oknie **Dodaj lub Usuń programy** kliknij przycisk **Dodaj/Usuń składniki systemu Windows**, a następnie upewnij się, że w grupie **Serwer aplikacji** są włączone następujące usługi:
    -   **ASP.NET**
    -   **Internetowe usługi informacyjne (IIS)**
    -   **Usługa kolejkowania wiadomości**

    Należy zaakceptować domyślne opcje każdej usługi. Nie jest wymagana dalsza konfiguracja.
3.  Skonfiguruj serwer bazy danych za pomocą jednej z następujących aplikacji baz danych:
    -   Microsoft® SQL Server 2000 z dodatkiem SP3a. Może być to lokalna instalacja programu SQL Server 2000 lub instalacja zdalna w tej samej domenie.
    -   Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) wydanie A. Ten program musi być zainstalowany lokalnie. Program MSDE 2000 można pobrać z [witryny firmy Microsoft w sieci Web](http://go.microsoft.com/fwlink/?linkid=17799) (http://go.microsoft.com/fwlink/?LinkID=17799).

    Zaleca się używanie programu Microsoft SQL Server Desktop Engine do obsługi baz danych programu RMS tylko w środowiskach testowych, ponieważ nie są w nim dostępne narzędzia niezbędne do pełnej obsługi bazy danych w całym przedsiębiorstwie. Ponadto ponieważ program MSDE nie obsługuje sieci zdalnej, należy zainstalować go na tym samym serwerze, co program RMS. Nie można także dodawać nowych serwerów RMS do klastra programu RMS. Zasady użytkowania programu Microsoft SQL Server Desktop Engine zabraniają używania narzędzi klienckich programu SQL Server do pracy z bazami danych programu Microsoft SQL Server Desktop Engine. Dlatego nie można tworzyć kopii zapasowych bazy danych konfiguracji programu RMS i przywracać z nich danych, przeglądać informacji dotyczących logowania ani bezpośrednio modyfikować danych przechowywanych w bazie danych konfiguracji.
4.  Wybierz nazwę, pod jaką ta usługa będzie dostępna dla użytkowników łączących się z nią w sieci intranet (na przykład http://certification.contoso.com). Skonfiguruj usługę nazw domen (DNS) w celu przyporządkowania tego adresu URL do adresu IP komputera programu RMS. Należy użyć w pełni kwalifikowanej nazwy domeny DNS dla adresu URL klastra, aby klienci w innych strefach DNS mogli przyporządkować adres IP serwera lub serwerów RMS.
5.  Utwórz konto administratora, którego będzie używać program RMS.
6.  Następnie można zainstalować program RMS z dodatkiem SP1. Aby uzyskać dalsze instrukcje dotyczące tego kroku, zobacz „Instalowanie programu RMS z dodatkiem Service Pack 1” w sekcji „Obsługa serwerów programu RMS” w tym zestawie dokumentacji.

**Często używane funkcje opcjonalne**

Funkcje opisane poniżej są opcjonalne. Jeśli zostaną wybrane i będą używane, należy wykonać odpowiednie czynności przygotowawcze przed rozpoczęciem procesu instalacji i zastrzegania programu RMS:

-   Program RMS można skonfigurować tak, aby do przechowywania kluczy prywatnych używany był w nim sprzętowy moduł zabezpieczeń (HSM). Aby używać sprzętowego modułu zabezpieczeń, należy upewnić się, że jego sterowniki zostały prawidłowo skonfigurowane i że zdefiniowano środowisko zabezpieczeń.
-   Jeżeli komputer z programem RMS może łączyć się z Internetem, można automatycznie pobrać certyfikat licencjodawcy serwera podczas procesu zastrzegania. Jeśli w organizacji połączenie z siecią Internet jest realizowane za pośrednictwem serwera proxy, sprawdź ustawienia serwera proxy w programie Internet Explorer, w tym ewentualne wymagania związane z uwierzytelnianiem, i zapisz je w celu późniejszego wykorzystania.
-   Jeśli program RMS będzie uruchamiany na kontrolerze domeny i do uruchamiania usług programu RMS planowane jest używanie konta użytkownika, należy upewnić się, że zasady zabezpieczeń kontrolera domeny są skonfigurowane tak, aby kontu użytkownika udzielano uprawnienia do logowania lokalnego. Aby uzyskać więcej informacji dotyczących zasad zabezpieczeń kontrolera domeny, zobacz Centrum pomocy i obsługi technicznej systemu Windows Server 2003.

**Krok 2 — Zastrzeganie pierwszego serwera programu RMS**

Zastrzeganie to proces konfigurowania witryny sieci Web z programem RMS. Umożliwi on użytkownikom rozpoczęcie korzystania z usługi. Aby zastrzec serwer głównej certyfikacji w organizacji, należy wykonać następujące kroki:

1.  Zaloguj się na komputerze jako użytkownik domeny z uprawnieniami lokalnego administratora. Jeśli program RMS jest instalowany na kontrolerze domeny, zaloguj się jako administrator domeny.
2.  Kliknij przycisk **Start**, wskaż polecenie **Wszystkie programy**, wskaż polecenie **Windows RMS**, a następnie kliknij polecenie **Administracja programem Windows RMS**, aby otworzyć stronę **Administracja globalna**. Na tej stronie wyświetlana jest lista witryn sieci Web, które są dostępne na tym serwerze.
3.  Kliknij witrynę sieci Web, którą chcesz zastrzec przy użyciu programu RMS, a następnie kliknij opcję **Zastrzeż program RMS w tej witrynie sieci Web**. Gdy strona zostanie otwarta, u góry strony będzie wyświetlany komunikat **Zastrzeganie serwera głównej certyfikacji programu RMS**.
4.  Wypełnij stronę informacjami o organizacji.
    -   W polu **Adres URL klastra** wpisz nazwę usługi (np. certification.contoso.com) skonfigurowanej w kroku 4 poprzedniej procedury. Jeśli w instalacji ma być używany protokół SSL, na liście protokołów kliknij protokół HTTPS. Wykonanie tej czynności spowoduje włączenie protokołu SSL; jednak wybranie tej opcji nie spowoduje, że protokół SSL będzie wymagany dla usług sieci Web programu RMS. Te funkcję należy skonfigurować osobno za pośrednictwem protokołu IIS.
    -   Jeśli serwer jest połączony z Internetem za pośrednictwem serwera proxy, w obszarze **Ustawienia serwera proxy programu RMS** należy wprowadzić informacje z programu Internet Explorer (informacje na ten temat znajdują się w części poświęconej funkcjom opcjonalnym w poprzedniej procedurze).
    -   W obszarze **Łączność z Internetem serwera** wybierz opcję **Tryb online**, jeżeli chcesz, aby serwer łączył się z usługą rejestrowania firmy Microsoft za pomocą Internetu i automatycznie uzyskiwał certyfikat licencjodawcy serwera podczas procesu zastrzegania. Wybierz opcję **Tryb offline**, jeżeli chcesz ręcznie łączyć się z usługą rejestrowania firmy Microsoft i pobrać certyfikat licencjodawcy serwera, a następnie zaimportować go po ukończeniu procesu zastrzegania programu RMS.
5.  Kliknij przycisk **Wyślij**. 
    Po około 60-90 sekundach zastrzeganie zakończy się pomyślnie, co umożliwi powrót do strony **Administracja globalna**, na której będzie można administrować nowo zastrzeżonym serwerem programu RMS.
6.  Na stronie **Administracja globalna** wybierz opcję **Administruj programem RMS w tej witrynie sieci Web**, aby otworzyć stronę główną **Administracja** dla serwera programu RMS.
    W przypadku wybrania opcji Tryb offline w obszarze Łączność z Internetem serwera w kroku 4 przed wykonaniem kolejnych czynności wykonaj procedurę opisaną w części „Ręczna rejestracja serwera głównej certyfikacji”.
7.  Na stronie głównej Administracja kliknij łącze **Punkt połączenia usługi programu RMS**.

| ![](images/Cc747735.note(WS.10).gif)Uwaga                                                                                                                                                                                                                                                                                        |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Następny krok tej procedury, rejestracja punktu połączenia usługi, wymaga użycia konta domeny o odpowiednich uprawnieniach w celu utworzenia obiektu kontenera pod kontenerem Usługi w kontenerze Konfiguracja lasu usługi Active Directory. Predefiniowana grupa zabezpieczeń — **Enterprise Admins** — jest przykładem konta mającego wymagane uprawnienia. |

1.  Na stronie **Punkt połączenia usługi programu RMS** kliknij przycisk **Zarejestruj URL**. Spowoduje to zarejestrowanie punktu połączenia usługi programu RMS w usłudze Active Directory, co umożliwi aplikacjom obsługującym technologię RMS odszukiwanie usług licencjonowania, aktywacji serwera proxy oraz certyfikacji udostępnianych przez program RMS.

**Krok 3 — Testowanie programu RMS**

Zanim można będzie w pełni korzystać z programu RMS, należy zainstalować klienta programu Usługi zarządzania prawami dostępu w systemie Windows i aplikację obsługującą technologię RMS na komputerach klienckich. Użytkownicy powinni być członkami domeny usługi Active Directory, a komputery klienckie powinny być dołączone do domeny. Ponadto użytkownicy domeny powinni mieć adresy e-mail zdefiniowane w usłudze Active Directory. Aby przetestować program RMS:

1.  Zaloguj się na komputerze klienckim jako prawidłowy użytkownik domeny.
2.  Zainstaluj klienta programu RMS dla dodatku Service Pack 1.
3.  Zainstaluj aplikację obsługującą technologię RMS.
4.  Utwórz plik chroniony technologią RMS, przyznaj dowolnemu użytkownikowi prawa tylko do odczytu tego pliku, a następnie zapisz plik w udostępnionym folderze, do którego użytkownicy mają pełny dostęp.
5.  Zaloguj się na komputerze jako inny użytkownik. Otwórz ten plik i spróbuj wprowadzić w nim zmiany. Jeśli program RMS został prawidłowo zainstalowany, wprowadzenie zmian w tym pliku nie będzie możliwe.
