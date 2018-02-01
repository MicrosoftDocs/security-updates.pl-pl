---
TOCTitle: Dodawanie serwera do klastra
Title: Dodawanie serwera do klastra
ms:assetid: 'db635238-5528-4bec-9cc6-8244e2b3d733'
ms:contentKeyID: 18123447
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747690(v=WS.10)'
---

Dodawanie serwera do klastra
============================

Aby wykonać tę procedurę, należy zalogować się lokalnie w administracyjnej witrynie sieci Web przy użyciu konta należącego do grupy Administratorzy na komputerze, do którego użytkownik uzyskuje dostęp. Członkowie grupy Administratorzy domeny również mogą wykonać tę procedurę. Ze względu na najważniejsze wskazówki dotyczące bezpieczeństwa należy rozważyć użycie trybu **Uruchom jako** w celu wykonania tej procedury.

Aby otworzyć stronę sieci Web **Administracja globalna**, należy kliknąć przycisk **Start**, wskazać polecenie **Wszystkie programy**, wskazać polecenie **Windows RMS**, a następnie kliknąć polecenie **Administracja programem Windows RMS**.

Na każdym serwerze program RMS można zastrzec tylko w pojedynczej witrynie sieci Web. Aby zastrzec program RMS w witrynie sieci Web innej niż witryna domyślna, przed rozpoczęciem procesu zastrzegania należy za pomocą Menedżera internetowych usług informacyjnych dodać tę witrynę sieci Web. Jeśli witryna sieci Web, w której ma być przeprowadzone zastrzeganie, nie jest wyświetlana na liście witryn sieci Web, należy zamknąć stronę **Administracja globalna**, dodać tę witrynę sieci Web, a następnie ponownie rozpocząć proces zastrzegania.

Jeśli program RMS jest rozmieszczany w środowisku, w którym poziom funkcjonalności domeny usługi Active Directory jest ustawiony na poziom macierzysty systemu Windows 2000, program RMS może nie odczytywać atrybutu **memberOf** obiektów usługi Active Directory podczas próby rozwinięcia przynależności do grupy. Aby program RMS mógł odczytywać atrybut **memberOf**, w koncie usługi programu RMS musi być używane konto na poziomie domeny, które należy do grupy dostępu zgodnej z systemami wcześniejszymi niż Windows 2000 (wbudowanej) znajdującej się w danym lesie.

Dodawanie serwera do klastra
----------------------------

#### Dodawanie serwera do klastra

1.  Po zainstalowaniu programu RMS na serwerze, który ma zostać dołączony do klastra głównej certyfikacji lub klastra licencji, otwórz stronę **Administracja globalna**.

2.  Obok witryny sieci Web, w której ma być zastrzeżony program RMS, kliknij opcję **Dodaj ten serwer do klastra**. Można wybrać domyślną witrynę sieci Web lub inną witrynę sieci Web utworzoną w tym celu w programie Internetowe usługi informacyjne (IIS).

    > [!Warning]  
    > Uruchamianie dodatkowych witryn lub usług sieci Web na serwerze programu RMS nie jest obsługiwane. Wykonanie tych czynności może spowodować, że wiele aplikacji i usług będzie działać na jednym koncie jako program RMS. 

3.  W obszarze **Konto usługi programu RMS** wpisz nazwę konta (w postaci nazwa\_domeny\\nazwa\_użytkownika) i hasło konta usługi programu RMS, na którym program RMS będzie wykonywać większość normalnych operacji. Musi to być konto domeny. Wszystkie serwery w klastrze powinny działać na tym samym koncie usługi programu RMS.

    > [!Important]  
    > Ze względów bezpieczeństwa zalecane jest utworzenie specjalnego konta użytkownika domeny, które będzie używane jako konto usługi programu RMS i nie należy udzielać temu kontu żadnych dodatkowych uprawnień. Jako konta usługi programu RMS nie można użyć konta domeny, za pomocą którego instalowano program RMS z dodatkiem Service Pack 1. 

4.  W obszarze **Baza danych konfiguracji** określ nazwę serwera baz danych programu i nazwę bazy danych konfiguracji tego klastra. Wybrana baza danych określa klaster, do którego zostanie dołączony ten serwer.

5.  W obszarze **Ochrona klucza prywatnego** wybierz mechanizm, który będzie używany w tym klastrze w celu ochrony klucza prywatnego. W przypadku domyślnej programowej ochrony klucza prywatnego podaj hasło, które zostało użyte do zaszyfrowania klucza prywatnego podczas zastrzegania pierwszego serwera w tym klastrze.

6.  Kliknij przycisk **Wyślij**. 

    W przypadku wyświetlenia komunikatu o błędzie nie należy zamykać strony. Należy usunąć błędy za pomocą polecenia IISReset w wierszu polecenia w celu zatrzymania i ponownego uruchomienia usług IIS, przejść do poprzedniej strony, ponownie wprowadzić informacje zastrzegania, a następnie ponownie kliknąć przycisk **Wyślij**. W przypadku wystąpienia błędu „Limit czasu żądania minął” należy zamknąć okno, sprawdzić, czy system spełnia minimalne wymagania sprzętowe, i spróbować ponownie zastrzec serwer.
