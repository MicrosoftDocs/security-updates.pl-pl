---
TOCTitle: Zastrzeganie serwera licencji
Title: Zastrzeganie serwera licencji
ms:assetid: '4d67b898-0ba9-4eef-ab7d-ee0ca55a688e'
ms:contentKeyID: 18123271
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747563(v=WS.10)'
---

Zastrzeganie serwera licencji
=============================

Aby wykonać tę procedurę, należy zalogować się lokalnie w administracyjnej witrynie sieci Web przy użyciu konta należącego do grupy Administratorzy na komputerze, do którego użytkownik uzyskuje dostęp. Członkowie grupy Administratorzy domeny również mogą wykonać tę procedurę. Ponadto w procesie podrejestrowywania wymagane jest, aby konto użytkownika domeny i grupa RMS Service miały uprawnienia do odczytu i wykonywania. Aby uzyskać więcej informacji, zobacz „[Ustawianie uprawnień do pliku usługi podrejestrowywania](https://technet.microsoft.com/737bb69b-fe26-4057-9569-e632f7bbf295)” we wcześniejszej części tego tematu. Jeśli używana jest zdalna baza danych programu SQL Server, konto, za pomocą którego loguje się użytkownik, musi mieć również rolę Database Creators na serwerze programu SQL Server. Ze względu na najważniejsze wskazówki dotyczące bezpieczeństwa należy rozważyć użycie trybu **Uruchom jako** w celu wykonania tej procedury.

Aby otworzyć stronę sieci Web **Administracja globalna**, należy kliknąć przycisk **Start**, wskazać polecenie **Wszystkie programy**, wskazać polecenie **Windows RMS**, a następnie kliknąć polecenie **Administracja programem Windows RMS**.

Na każdym serwerze program RMS można zastrzec tylko w pojedynczej witrynie sieci Web. Aby zastrzec program RMS w witrynie sieci Web innej niż witryna domyślna, przed rozpoczęciem procesu zastrzegania należy za pomocą Menedżera internetowych usług informacyjnych dodać tę witrynę sieci Web. Jeśli witryna sieci Web, w której ma być przeprowadzone zastrzeganie, nie jest wyświetlana na liście witryn sieci Web, należy zamknąć stronę **Administracja globalna**, dodać tę witrynę sieci Web, a następnie ponownie rozpocząć proces zastrzegania.

Jeśli program RMS jest rozmieszczany w środowisku, w którym poziom funkcjonalności domeny usługi Active Directory jest ustawiony na poziom macierzysty systemu Windows 2000, program RMS może nie odczytywać atrybutu **memberOf** obiektów usługi Active Directory podczas próby rozwinięcia przynależności do grupy. Aby program RMS mógł odczytywać atrybut **memberOf**, w koncie usługi programu RMS musi być używane konto na poziomie domeny, które należy do grupy dostępu zgodnej z systemami wcześniejszymi niż Windows 2000 (wbudowanej) znajdującej się w danym lesie.

Jeśli wpisano niestandardowy adres URL klastra, należy zarejestrować go w systemie nazw domen (DNS) i sprawdzić, czy działa. Jeśli to rozmieszczenie obejmuje obsługę sieci Internet, należy sprawdzić, czy ten adres URL jest dostępny w sieci Internet i w organizacji. Jeśli dla plików usług sieci Web włączono protokół SSL, należy określić protokół HTTPS dla adresu URL klastra.

Zastrzeganie serwera licencji
-----------------------------

#### Zastrzeganie serwera licencji

1.  Otwórz stronę **Administracja globalna**, a następnie obok witryny sieci Web, w której chcesz zastrzec program RMS, kliknij opcję **Zastrzeż program RMS w tej witrynie sieci Web**.

    Można wybrać domyślną witrynę sieci Web lub inną witrynę sieci Web utworzoną w tym celu w programie Internetowe usługi informacyjne (IIS).

    > [!Warning]  
    > Uruchamianie dodatkowych witryn lub usług sieci Web na serwerze programu RMS nie jest obsługiwane. Wykonanie tych czynności może spowodować, że wiele aplikacji i usług będzie działać na jednym koncie jako program RMS. 

2.  W obszarze **Baza danych konfiguracji** domyślną opcją jest utworzenie bazy danych konfiguracji na serwerze lokalnym. Do obsługi lokalnej bazy danych można użyć serwera bazy danych, takiego jak SQL Server 2000™ z dodatkiem SP3 lub Microsoft SQL Server 2000 Desktop Engine (MSDE). W przypadku korzystania ze zdalnej bazy danych lub gdy serwer bazy danych znajduje się na serwerze lokalnym, ale instancja serwera bazy danych ma inną nazwę niż nazwa serwera, zaznacz opcję **Zdalna baza danych** , a następnie wprowadź nazwę serwera bazy danych.

    > [!Important]  
    > Zaleca się używanie programu Microsoft SQL Server Desktop Engine do obsługi baz danych programu RMS tylko w środowiskach testowych, ponieważ ten program nie obsługuje żadnych interfejsów sieciowych. Ponadto zasady użytkowania programu Microsoft SQL Server Desktop Engine zabraniają używania narzędzi klienckich programu SQL Server do pracy z bazami danych programu Microsoft SQL Server Desktop Engine. To ograniczenie uniemożliwi przeglądanie informacji rejestrowania lub zmienianie danych przechowywanych w bazie danych konfiguracji.  

3.  W obszarze **Konto usługi programu RMS** określ konto usługi programu RMS, na którym program RMS będzie uruchamiany w większości normalnych operacji. W przypadku instalacji na jednym serwerze można określić konto System lokalny lub konto domeny. W przypadku innych rodzajów instalacji należy określić konto domeny. Dla konta domeny należy podać nazwę konta w formacie *nazwa\_domeny*\\*nazwa\_użytkownika* oraz hasło.

    > [!Warning]  
    > Konto System lokalny umożliwia dostęp do prawie wszystkich zasobów systemu operacyjnego i dlatego jego używanie ma poważne skutki w dziedzinie zabezpieczeń. W miarę możliwości należy unikać używania konta System lokalny jako konta usługi programu RMS. Należy natomiast utworzyć specjalne konto użytkownika domeny, które będzie używane jako konto usługi programu RMS i nie należy udzielać temu kontu żadnych dodatkowych uprawnień. Jako konta usługi programu RMS nie można użyć konta, za pomocą którego instalowano program RMS. 

4.  W obszarze **Adres URL klastra** wpisz adres URL serwera lub klastra, który będzie używany na potrzeby klientów w sieci wewnętrznej. We wpisie domyślnym używana jest nazwa serwera, na przykład Contoso-cert. W razie potrzeby można edytować ten wpis, na przykład w celu skonfigurowania adresu URL klastra lub modułu równoważenia obciążenia obsługującego ten klaster. Można także wybrać protokół HTTP lub HTTPS. W części **Uwagi** na końcu tej procedury znajduje się więcej informacji dotyczących konfigurowania adresu URL klastra. Po zastrzeżeniu można na administracyjnych stronach sieci Web skonfigurować zewnętrzny adres URL klastra na potrzeby klientów znajdujących się poza siecią wewnętrzną.

5.  W obszarze **Ochrona klucza prywatnego i podrejestrowywanie** wybierz mechanizm ochrony klucza prywatnego serwera, wykonując jedną z następujących czynności:

    -   **Użyj domyślnej programowej ochrony klucza prywatnego**. W przypadku wybrania tej opcji klucz prywatny będzie przechowywany w bazie danych konfiguracji programu RMS. Należy podać silne hasło służące do szyfrowania klucza w bazie danych.

    > [!Important]  
    > To hasło należy przechowywać w bezpiecznym archiwum do wykorzystania w przyszłości. Kopię zapasową bazy danych konfiguracji (również zabezpieczoną za pomocą hasła) należy przechowywać w bezpiecznym archiwum. Dzięki temu w przypadku uszkodzenia bazy danych programu SQL Server będzie dostępny mechanizm przywracania programu RMS. Jeśli z dowolnego powodu hasło zostanie zmienione, należy wykonać nową kopię zapasową bazy danych konfiguracji chronioną tym hasłem, a następnie należy umieścić bazę danych i hasło w bezpiecznym archiwum. 

    -   **Używanie dostawcy usług kryptograficznych (CSP)**. Aby używać dostawcy CSP lub sprzętowego modułu zabezpieczeń (HSM), należy wyczyścić pole wyboru **Użyj domyślnej programowej ochrony klucza prywatnego**. Na liście **Wybierz dostawcę usług kryptograficznych** wybierz zainstalowanego dostawcę CSP lub moduł HSM.

    > [!note]  
    > Program RMS wymaga dostawcy Rivest-Shamir-Adleman (RSA) świadczącego pełny zakres usług; tylko tacy dostawcy są uwzględniani na liście dostawców CSP. 

    > [!note]  
    > Zalecane jest używanie domyślnej programowej ochrony klucza prywatnego lub modułu HSM. Jeśli używany jest inny programowy dostawca CSP, przed użyciem tego dostawcy w programie RMS należy upewnić się, czy istnieją organizacyjne zasady kluczowe zarządzania (takie jak procedury wykonywania kopii zapasowych i przywracania) dla tego dostawcy. 

6.  Ten krok ma zastosowanie tylko w przypadku wybrania dostawcy CSP. Aby określić parę kluczy serwera, która będzie używana, wykonaj jedną z następujących czynności:

    -   W przypadku nowej instalacji wybierz opcję **Utwórz nową parę kluczy publiczny-prywatny**.
    -   W przypadku przywracania lub uaktualniania istniejącego serwera programu RMS, wybierz opcję **Użyj istniejącej pary kluczy publiczny-prywatny**. W obszarze Istniejący kontener kluczy kliknij przycisk **Przeglądaj**, a następnie wybierz kontener kluczy dla pary kluczy serwera.

    > [!note]  
    > Podstawowe, rozszerzone oraz silne procedury CSP firmy Microsoft korzystają z tej samej lokalizacji przechowywania kluczy. 

    > [!note]  
    > W przypadku, gdy istniejąca para kluczy nie jest używana podczas odzyskiwania lub uaktualniania istniejącego serwera z programem RMS, wszyscy istniejący klienci programu RMS będą zmuszeni wyczyścić swoje magazyny licencji (usunąć licencje użytkowania oraz certyfikaty kont praw), a następnie uzyskać nowe licencje z serwera, aby móc korzystać z zawartości. 

7.  W polu **Nazwa certyfikatu licencjodawcy serwera** wprowadź nazwę, która będzie używana w certyfikacie licencjodawcy serwera. Domyślnie jest to nazwa serwera.

8.  Jeśli w organizacji połączenie z siecią Internet jest realizowane za pośrednictwem serwera proxy, zaznacz pole wyboru **Ten komputer używa serwera proxy do łączenia się z Internetem**, a następnie wpisz adres i port serwera proxy.

    Jeśli serwer proxy wymaga uwierzytelnienia, wybierz typ uwierzytelniania i podaj nazwę użytkownika oraz hasło do uwierzytelnienia przez serwer proxy. Jeśli stosowane jest zintegrowane uwierzytelnianie systemu Windows, musisz również określić domenę.

9.  Kliknij przycisk **Wyślij**. 

    Usługa podrejestrowywania programu RMS generuje parę kluczy publiczny-prywatny dla serwera licencji i oznacza klucz publiczny za pomocą klucza prywatnego serwera głównej certyfikacji. Ta usługa tworzy także dla serwera licencji certyfikat licencjodawcy serwera. Elementy te zostaną w ciągu kilku minut wysłane do bazy danych konfiguracji.

    > [!Important]  
    > W przypadku wyświetlenia komunikatu o błędzie nie należy zamykać strony. Należy usunąć błędy za pomocą polecenia IISReset w wierszu polecenia w celu zatrzymania i ponownego uruchomienia usług IIS, przejść do poprzedniej strony, ponownie wprowadzić informacje zastrzegania, a następnie ponownie kliknąć przycisk **Wyślij**. W przypadku wystąpienia błędu „Limit czasu żądania minął” należy zamknąć okno, sprawdzić, czy system spełnia minimalne wymagania sprzętowe, i spróbować ponownie zastrzec serwer. 

Aby uzyskać instrukcje dotyczące zastrzegania dodatkowych serwerów licencji i dodawania ich do klastra, zobacz „[Dodawanie serwera do klastra](https://technet.microsoft.com/db635238-5528-4bec-9cc6-8244e2b3d733)” w dalszej części tego tematu.
