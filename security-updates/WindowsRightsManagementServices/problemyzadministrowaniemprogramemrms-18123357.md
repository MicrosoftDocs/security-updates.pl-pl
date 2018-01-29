---
TOCTitle: Problemy z administrowaniem programem RMS
Title: Problemy z administrowaniem programem RMS
ms:assetid: '97013c08-d3fa-4ea0-8914-995b6c97f900'
ms:contentKeyID: 18123357
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747605(v=WS.10)'
---

Problemy z administrowaniem programem RMS
=========================================

Gdy program RMS zostanie pomyślnie zastrzeżony na serwerze, mogą wystąpić problemy z rutynową administracją programem RMS. Na podstawie informacji zawartych w poniższych sekcjach niektóre z tych problemów można rozwiązać.

Przy próbie otwarcia administracyjnej witryny sieci Web programu RMS pojawia się komunikat „Serwer SQL nie istnieje lub odmówiono dostępu”
------------------------------------------------------------------------------------------------------------------------------------------

Jeśli program RMS zainstalowano przy użyciu nowej instalacji serwera bazy danych SQL Server 2005, usługa serwera SQL może nie być uruchomiona. W przypadku serwera SQL Server 2005 konfiguracja usługi MSSQLSERVER nie przewiduje jej automatycznego uruchamiania przy uruchamianiu serwera. Jeśli od czasu zainstalowania programu RMS serwer SQL Server został ponownie uruchomiony i jeśli nie zmieniono konfiguracji usługi na jej automatyczne uruchamianie, program RMS nie będzie mógł działać, a dostępna będzie jedynie strona Administracja globalna programem RMS.

Po uruchomieniu usługi MSSQLSERVER należy ponownie uruchomić Internetowe usługi informacyjne na serwerze RMS, aby przywrócić funkcjonalność programu RMS.

Nie można ukończyć procesu rejestrowania offline
------------------------------------------------

Jeśli plik żądania rejestracji nie jest kompletny lub został zmodyfikowany przed przesłaniem go na witrynę EnrollService, ukończenie rejestrowania w trybie offline nie będzie możliwe. Plik z żądaniem rejestracji mógł zostać uszkodzony przez szkodliwe oprogramowanie, w wyniku błędu użytkownika lub błędu systemu.

Zależnie od tego, jakich informacji brakuje, witryna EnrollService może mimo wszystko przyjąć plik i zwrócić certyfikat licencjodawcy serwera albo odmówić przyjęcia pliku i wygenerować błąd.

W przypadku zwrócenia certyfikatu licencjodawcy serwera certyfikat będzie odzwierciedlał braki lub uszkodzenia pliku żądania, a program RMS zgłosi błąd przy próbie jego importu.

Jeśli nie da się ukończyć procesu rejestrowania, należy sprawdzić, czy komputer z podłączeniem do Internetu nie jest zarażony wirusem, ponownie wyeksportować plik z żądaniem rejestracji z serwera RMS i użyć innego sposobu przeniesienia pliku na komputer z podłączeniem do Internetu. W razie ponownego wystąpienia błędu należy się skontaktować z działem pomocy technicznej firmy Microsoft.

Pliki dzienników nie są tworzone
--------------------------------

Usługa rejestrowania programu RMS wymaga obecności Usługi kolejkowania wiadomości (MSMQ) oraz dostępu do bazy danych rejestrowania. Jeśli pliki dzienników nie są tworzone, może to wskazywać na niewłaściwą konfigurację składników lub na zakłócenia w komunikacji między składnikami.

Należy sprawdzić, czy serwer RMS i serwer bazy danych mają dobre połączenie z siecią. Jeśli tak, należy przy użyciu poniższych procedur sprawdzić spełnienie wymagań wstępnych dla usługi rejestrowania RMS i zapewnić prawidłową konfigurację wszystkich zależności między programami.

Najpierw sprawdź, czy konfiguracja usługi kolejkowania wiadomości jest prawidłowa. Usługa kolejkowania wiadomości musi być zainstalowana z włączoną integracją z usługą Active Directory.

**Aby upewnić się, że usługa kolejkowania wiadomości jest zainstalowana i prawidłowo skonfigurowana:**
1.  W **Panelu sterowania** kliknij ikonę **Dodaj lub usuń programy**, a następnie kliknij opcję **Dodaj/usuń składniki systemu Windows**, aby otworzyć **Kreatora składników systemu Windows**.

2.  W oknie **Kreatora składników systemu Windows** zaznacz pole wyboru **Serwer aplikacji** i kliknij przycisk **Szczegóły**.

3.  Zaznacz pole wyboru **Kolejkowanie wiadomości** i kliknij przycisk **Szczegóły**.

4.  Jeśli pole wyboru **Integracja z usługą Active Directory** jest zaznaczone, przejdź do następnego testu i sprawdź, czy usługa kolejkowania wiadomości jest uruchomiona. Jeśli pole wyboru nie jest zaznaczone, wykonaj czynności od 5 do 9.

5.  Kliknij przycisk **Start**, wskaż polecenie **Wszystkie programy**, wskaż polecenie **Windows RMS**, a następnie kliknij polecenie **Administracja programem Windows RMS**, aby otworzyć stronę Administracja globalna.

6.  Obok witryny sieci Web, w której zastrzeżono program RMS, kliknij opcję **Usuń program RMS z tej witryny sieci Web**, a następnie kliknij przycisk **OK**.

7.  W **Panelu sterowania** kliknij ikonę **Dodaj lub usuń programy**, kliknij przycisk **Dodaj/usuń składniki systemu Windows**, kliknij pozycję **Serwer aplikacji**, a następnie kliknij pozycję **Usługa kolejkowania wiadomości**.

8.  Aby włączyć **Integrację z usługą Active Directory**, kliknij przycisk **Szczegóły**, zaznacz pole wyboru **Integracja z usługą Active Directory**, a następnie kliknij przycisk **OK**.

9.  Otwórz stronę **Administracja globalna**. Obok nazwy witryny sieci Web, w której ma być zastrzeżony program RMS, kliknij opcję **Zastrzeż program RMS w tej witrynie sieci Web**.

Następnie sprawdź, czy usługa kolejkowania wiadomości jest uruchomiona na serwerze.

**Aby sprawdzić, czy usługa kolejkowania wiadomości jest uruchomiona na serwerze:**
1.  W **Panelu sterowania** kliknij pozycję **Narzędzia administracyjne** i wybierz pozycję **Usługi**.

2.  Przewiń listę usług aż do usługi **Kolejkowanie wiadomości**.

3.  W kolumnie **Stan** usługa ta powinna mieć ustawienie **Uruchomiona**; jeśli tak nie jest, kliknij usługę prawym przyciskiem myszy i wybierz polecenie **Uruchom**.

Po trzecie sprawdź, czy usługa rejestrowania ma uprawnienie do zapisywania zdarzeń w bazie danych rejestrowania. Usługa rejestrowania RMS działa przy użyciu konta usługi RMS. Upewnij się, że konto usługi RMS ma przypisaną prawidłową nazwę logowania na serwerze bazy danych oraz że ma uprawnienia wymagane do tworzenia baz danych i zapisywania informacji w plikach.

Gdy wszystkie te warunki są już spełnione, zatrzymaj i uruchom ponownie usługę rejestrowania RMS przy użyciu okna Usługi. Po ponownym uruchomieniu usługi rejestrowania RMS pliki dzienników powinny już być tworzone na serwerze bazy danych. Jeśli serwerem bazy danych jest SQL Server, tworzenie plików dziennika można sprawdzić w opisany poniżej sposób.

**Aby sprawdzić, czy pliki dziennika są tworzone na serwerze SQL Server:**
1.  W przystawce SQL Server Enterprise Manager przejdź do bazy danych rejestrowania, rozwiń element **Databases** (Bazy danych), a następnie rozwiń bazę danych, która zawiera bazę danych rejestrowania programu RMS.

2.  Kliknij bazę danych rejestrowania, kliknij pozycję **Tables** (Tabele), kliknij prawym przyciskiem myszy tabelę **DRMS\_log\_master**, a następnie kliknij polecenie **Open table – return all rows** (Otwórz tabelę – zwróć wszystkie wiersze). Jeśli pliki dzienników są tworzone, będzie widoczny jeden lub kilka plików dzienników.

Przywracanie bazy danych konfiguracji
-------------------------------------

Program RMS nie może pracować bez sprawnej bazy danych konfiguracji. W razie wystąpienia problemów z bazą danych konfiguracji, takich jak uszkodzenie bazy danych lub awaria dysku twardego na serwerze bazy danych, przywrócenie sprawności programu RMS zależy od możliwości odtworzenia bazy danych konfiguracji z kopii zapasowej. Do przywrócenia bazy danych konfiguracji RMS z kopii zapasowej niezbędne będą następujące informacje:

-   Nazwa najbardziej aktualnej kopii zapasowej bazy danych
-   Nazwa komputera, na którym baza danych zostanie przywrócona z kopii.
-   Nazwa konta i hasło, których użyto do zastrzeżenia programu RMS.
-   Hasło określone dla programowej ochrony klucza prywatnego (jeśli było używane).

Przywracanie bazy danych z kopii zapasowej nie wymaga nowego certyfikatu licencjodawcy serwera ani nowego klucza prywatnego, ponieważ program RMS zachowuje wszystkie ustawienia (które pobiera z kopii zapasowej bazy danych konfiguracji).

Bazę danych można przywrócić z kopii zapasowej, wykonując poniższą procedurę:

**Aby przywrócić bazę danych z kopii zapasowej:**
1.  Kliknij przycisk **Start**, wskaż polecenie **Wszystkie programy**, wskaż polecenie **Windows RMS**, a następnie kliknij polecenie **Administracja programem Windows RMS**, aby otworzyć stronę **Administracja globalna**.

2.  Obok witryny sieci Web, w której zastrzeżono program RMS, kliknij opcję **Usuń program RMS z tej witryny sieci Web**, a następnie kliknij przycisk **OK**.

3.  Przywróć kopię zapasową plików bazy danych dla bazy danych konfiguracji. Jeśli utworzono kopię zapasową bazy danych podczas procedury tworzenia kopii zapasowej i chcesz zachować ciągłość danych, przywróć również bazę danych rejestrowania.

    -   Jeśli system jest przywracany po całkowitej awarii systemu, przywróć rejestr, korzystając z kopii zapasowej stanu systemu jeszcze przed przywróceniem plików bazy danych.

4.  Jeśli przywracana baza danych jest przeznaczona dla pojedynczego serwera głównej certyfikacji, zmodyfikuj następujący klucz rejestru przed rozpoczęciem ponownego zastrzegania usługi:

    -   W komputerach z 32-bitową wersją systemu Windows Server 2003
        `HKEY_LOCAL_MACHINE\Software\Microsoft\DRMS\1.0\`
    -   W komputerach z 64-bitową wersją systemu Windows Server 2003
        `HKEY_LOCAL_MACHINE\Software\WOW6432Node\Microsoft\DRMS\1.0\`

    Dodaj następujący wpis jako wartość ciągu, pozostawiając samą wartość pustą:

    `GicURL`

    Ta wartość zastępuje wykrywanie serwera głównej certyfikacji w usłudze Active Directory i umożliwia uzyskanie dostępu do stron zastrzegania serwera głównej certyfikacji.

5.  Jeśli używano sprzętowego modułu zabezpieczeń do zabezpieczania klucza prywatnego programu RMS, przywróć kopię zapasową środowiska zabezpieczeń, aby można było pobrać klucze.

6.  Wykonaj jeden z poniższych kroków:

    -   Aby przywrócić bazę danych dla pojedynczego serwera, a nie dla klastra, kliknij polecenie Zastrzeż program RMS w tej witrynie sieci Web obok witryny sieci Web, w której chcesz zastrzec program RMS.
        — lub —
    -   Aby przywrócić bazę danych dla klastra, kliknij łącze Dodaj ten serwer do klastra obok witryny sieci Web, w której chcesz zastrzec program RMS.

7.  Określ konto usługi programu RMS, którego użyto do pierwszego zastrzeżenia serwera.

8.  Określ kopię zapasową bazy danych konfiguracji (w tym nazwę bazy danych oraz nazwę komputera, na którym znajduje się ta baza danych), której chcesz użyć.

9.  Określ to samo hasło, które podano podczas pierwszego zastrzegania tego serwera.

10. Kliknij przycisk **Wyślij**.

Zostanie uruchomiony proces zastrzegania, w wyniku którego program RMS zostanie ponownie zastrzeżony na serwerze.

Aby uzyskać więcej informacji, zobacz „Planowanie przywracania systemu” oraz „Tworzenie kopii zapasowych systemu RMS i jego przywracanie” w części „Planowanie rozmieszczenia programu RMS” w tym zestawie dokumentacji.

Przedawnione hasło konta usługi programu RMS
--------------------------------------------

Jeśli program RMS przestanie działać, przyczyną może być wygaśnięcie hasła konta usługi programu RMS. Uruchom Menedżera usług IIS. Jeśli pule aplikacji programu RMS zostały zatrzymane i nie można ich ponownie uruchomić, prawdopodobnie hasło konta usługi programu RMS wygasło.

Jeśli hasło konta usługi programu RMS wygaśnie, należy zmienić hasło na każdym z serwerów programu RMS, który korzysta z tego hasła, a następnie należy ponownie uruchomić usługi IIS. Aby uzyskać więcej informacji, zobacz „Zmienianie hasła konta usługi programu” w podręczniku „Obsługa serwerów programu RMS” w niniejszym zestawie dokumentacji.

Przywracanie poprzedniej instalacji programu RMS
------------------------------------------------

W razie awarii sprzętowej lub programowej serwera RMS, serwer RMS można przywrócić, korzystając z uprzednio zainstalowanej bazy danych konfiguracji w celu zastrzeżenia nowego wystąpienia serwera.

> [!note]  
> Ta procedura ma zastosowanie, tylko jeśli serwer programu RMS ulegnie awarii. Jeśli awarii uległ serwer, na którym działa baza danych konfiguracji, patrz „Przywracanie bazy danych konfiguracji” we wcześniejszej części niniejszego tematu. Jeśli serwer RMS jest jednocześnie serwerem bazy danych, konieczne będzie odtworzenie całego serwera z kopii zapasowej. 

Wykonaj poniższą procedurę, aby wskazać tę samą bazę danych konfiguracji, której używano dla oryginalnej instalacji:

**Aby przywrócić poprzednią instalację programu RMS:**
1.  Zaloguj się na komputerze, który chcesz skonfigurować jako serwer programu RMS, za pomocą konta z uprawnieniami administratora. Upewnij się, że ten komputer spełnia minimalne wymagania systemowe dla programu RMS. Aby uzyskać więcej informacji na temat wymagań systemowych programu RMS, zobacz „Wymagania dotyczące sprzętu” dla RMS w podręczniku „Planowanie rozmieszczenia programu RMS” w niniejszym zestawie dokumentacji.

2.  Jeśli do ochrony kluczy prywatnych programu RMS używany jest sprzętowy moduł zabezpieczeń, upewnij się, że moduł jest prawidłowo skonfigurowany z użyciem tego samego środowiska ustawień i zabezpieczeń, którego używano w poprzedniej instalacji programu RMS.

3.  Zainstaluj program RMS na komputerze.

4.  Po zakończeniu instalacji programu RMS kliknij przycisk **Start**, wskaż polecenie **Wszystkie programy**, wskaż polecenie **Windows RMS**, a następnie kliknij polecenie **Administracja programem Windows RMS**, aby otworzyć stronę **Administracja globalna**.

5.  Obok witryny sieci Web, w której ma być zastrzeżony program RMS, kliknij opcję **Dodaj ten serwer do klastra**.

6.  W obszarze **Konto usługi programu RMS** wpisz nazwę konta usługi RMS (w postaci nazwa\_domeny\\nazwa\_użytkownika) i hasło konta usługi programu RMS, na którym program RMS będzie wykonywać większość rutynowych operacji. Musi to być konto domeny.

7.  W obszarze **Baza danych konfiguracji** określ nazwę serwera baz danych oraz nazwę bazy danych konfiguracji dla oryginalnej instalacji programu RMS, którą chcesz przywrócić.

8.  W obszarze **Ochrona klucza prywatnego** wybierz mechanizm, który będzie używany w tym klastrze w celu ochrony klucza prywatnego. Jeśli używano programowej ochrony kluczy prywatnych, należy podać hasło używane do szyfrowania klucza prywatnego po pierwszym zastrzeżeniu tego klastra.

9.  Kliknij przycisk **Wyślij**.

Klienci nie mogą otwierać materiałów chronionych przez program RMS ze względu na utratą ważności uprawnień
----------------------------------------------------------------------------------------------------------

Jeśli uprawnienia użytkownika straciły ważność, użytkownik nie może korzystać z zawartości chronionej technologią RMS.. W przypadku gdy zegar na serwerze RMS wskazuje czas późniejszy niż zegar klienta RMS, użytkownik także nie będzie miał dostępu do zawartości chronionej przez RMS, nawet jeśli jego uprawnienia jeszcze są ważne. Gdy zegary w obu systemach nie są zsynchronizowane, przy próbie dostępu do zawartości może być wyświetlany następujący błąd:

**Nie masz uprawnień do otwarcia tej wiadomości, ponieważ twoje uprawnienia wygasły. Czy chcesz ją otworzyć przy użyciu innego zestawu poświadczeń?**

Licencja klienta i licencja zawartości są jeszcze ważne, ale różnica w ustawieniach czasu sprawia, że klient interpretuje licencję zawartości jako nieważną i zwraca użytkownikowi ten błąd. W efekcie użytkownik może odnieść wrażenie, że problem dotyczy certyfikatu konta RMS albo przydzielonych mu praw względem dokumentu. Gdy zegar na komputerze klienta będzie wskazywał godzinę mieszczącą się w okresie ważności licencji publikacji treści, użytkownik będzie mógł otwierać dokument.

Zaleca się, aby zarówno komputer serwera, jak i komputery klientów w systemie RMS były synchronizowane za pomocą tej samej usługi ustawiania czasu.

Błąd „Brak dostępu”, gdy program RMS próbuje zapisywać zdarzenia w dzienniku zdarzeń aplikacji
----------------------------------------------------------------------------------------------

Według ustawień domyślnych, składniki w rodzaju RMS, uruchamiane za pośrednictwem strony ASP, są tworzone przy użyciu konta IUŻYTKOWNIK\_NAZWAKOMPUTERA. To konto jest przypisane do grupy Goście. Tymczasem uprawnienia systemu zabezpieczeń przypisane do grupy Goście uniemożliwiają dokonywanie zapisów w dzienniku zdarzeń aplikacji.

Aby wyeliminować ten problem, można zmienić klucz sterujący tym zachowaniem za pomocą Edytora rejestru.

> [!Caution]  
> Nieprawidłowa edycja rejestru może spowodować poważne uszkodzenie systemu. Przed wprowadzaniem zmian w rejestrze należy wykonać kopię zapasową wszystkich wartościowych danych przechowywanych na komputerze. 

Następującemu kluczowi rejestru nadaj ustawienie 0 zamiast 1, a następnie uruchom ponownie komputer, aby zmiana odniosła skutek.

`HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\EventLog\Application`

Nazwa: `RestrictGuestAccess`

Typ: `REG_DWORD`

> [!note]  
> Dzięki tej zmianie wszystkie konta należące do grupy Goście uzyskają możliwość wprowadzania wpisów w dzienniku zdarzeń aplikacji. 

Więcej informacji na temat przyczyn tego błędu można znaleźć w artykule na temat włączania zapisywania w dzienniku z poziomu stron ASP w [bazie wiedzy firmy Microsoft](http://go.microsoft.com/fwlink/?linkid=44167.)
