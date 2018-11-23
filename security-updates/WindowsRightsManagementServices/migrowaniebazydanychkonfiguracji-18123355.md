---
TOCTitle: Migrowanie bazy danych konfiguracji
Title: Migrowanie bazy danych konfiguracji
ms:assetid: '980e3e94-7d28-40dd-ad01-d34eb3c8d8e6'
ms:contentKeyID: 18123355
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747607(v=WS.10)'
---

Migrowanie bazy danych konfiguracji
===================================

Zdarzają się sytuacje, w których konieczne jest wycofanie serwera bazy danych. Przykładem może być uaktualnianie sprzętu serwera bazy danych programu RMS. Przed wycofaniem serwera bazy danych konieczne jest przeniesienie bazy danych konfiguracji na inny serwer. Migracja powinna być zaplanowana i przeprowadzona z należytą starannością, aby zapewnić bezpieczeństwo danych w bazie danych konfiguracji, w tym także zawartych w niej par kluczy.

Zaleca się utworzenie aliasu CNAME dla serwera bazy danych RMS, a następnie skonfigurowanie programu RMS do użycia go. Pozwala to uniknąć konieczności ręcznej modyfikacji nazwy serwera bazy danych w bazie danych konfiguracji programu RMS, jeśli nazwa ta ulegnie zmianie. W przypadku korzystania z aliasu CNAME potrzebne będzie tylko zaktualizowanie rekordu aliasu.

Przed rozpoczęciem migracji bazy danych konfiguracji upewnij się, że dostępne są następujące informacje:

-   Nazwa konta i hasło użyte pierwotnie do zastrzeżenia serwerów w klastrze RMS, które używają tej bazy danych.
-   Jeśli do przechowywania klucza prywatnego RMS użyto programowego dostawcy usług kryptograficznych (CSP), potrzebne będzie hasło tego klucza, które podane zostało pierwotnie podczas zastrzegania. Krok ten można pominąć, jeśli do przechowywania hasła klucza prywatnego RMS użyto sprzętowego modułu zabezpieczeń.

> [!note]  
> Migracja bazy danych konfiguracji nie wymaga nowego certyfikatu licencjodawcy serwera ani nowego klucza prywatnego serwera, ponieważ program RMS zachowuje ustawienia z pierwotnej bazy danych konfiguracji. 

Przed rozpoczęciem jakichkolwiek czynności na serwerze bazy danych należy wykonać kopię zapasową baz danych RMS. Jeśli nie jest to możliwe, należy przynajmniej wyeksportować posiadany certyfikat licencjodawcy serwera. Aby uzyskać więcej informacji na temat eksportu certyfikatu licencjodawcy serwera, zobacz [Eksportowanie certyfikatu licencjodawcy serwera do pliku](https://technet.microsoft.com/d683a629-71b3-4b11-932b-4ab0317334af). Jeśli podczas migracji baz danych wystąpi błąd, można zaimportować certyfikat licencjodawcy serwera do nowej instalacji programu RMS i skorzystać z zawartości, która w poprzedniej instalacji była chroniona prawami dostępu.

Aby przeprowadzić migrację bazy danych konfiguracji, wykonaj następujące czynności:

-   Zaktualizuj bazę danych konfiguracji RMS, podając nazwę nowego serwera bazy danych.
-   Zaktualizuj pliki web.config i rejestry na wszystkich serwerach w klastrze RMS, aby używały nowej nazwy serwera bazy danych

> [!Important]  
> W niniejszym temacie przyjęto, że bazy danych RMS zostały już skopiowane na nowy serwer baz danych obsługujący bazy programu RMS. 

Zaktualizuj bazę danych konfiguracji RMS, tak aby używana była nazwa nowego serwera bazy danych.
------------------------------------------------------------------------------------------------

Nazwa serwera baz danych, który obsługuje bazy programu RMS, przechowywana jest w bazie danych konfiguracji RMS. Po przeniesieniu plików bazy danych na nowy serwer baz danych należy zaktualizować bazę danych konfiguracji programu RMS. W tym celu można posłużyć się narzędziem RMS Config Editor wchodzącym w skład administracyjnego zestawu narzędzi programu RMS lub programem SQL Management Studio.

Wykonaj następujące czynności, aby zaktualizować nazwę serwera bazy danych programu RMS przy użyciu narzędzia RMS Config Editor:

**Aby zaktualizować bazę danych konfiguracji programu RMS przy użyciu narzędzia RMS Config Editor**
1.  Zaloguj się na serwer RMS w klastrze jako członek roli bazy danych Administratorzy systemu.

2.  Zainstaluj administracyjny zestaw narzędzi programu RMS, który dostępny jest w witrynie Microsoft Download Center ([http://go.microsoft.com/fwlink/?LinkId=98961](http://go.microsoft.com/fwlink/?linkid=98961)).

3.  Przejdź do katalogu %SystemDrive%:\\Program Files\\RMS SP2 Administration Toolkit\\RMSConfigEditor i kliknij dwukrotnie plik **RMSCONFIGEDITOR.EXE**.

4.  W polu **Server** wpisz nazwę nowego serwera obsługującego bazę danych konfiguracji programu RMS, a następnie kliknij przycisk **Go**.

5.  W polu **Database** kliknij pozycję **DRMS\_Config\_***&lt;nazwa klastra RMS&gt;***\_***&lt;Port&gt;*, gdzie *&lt;nazwa klastra RMS&gt;* to nazwa klastra RMS a *&lt;Port&gt;* to port TCP , którego program RMS używa do komunikacji, a następnie kliknij przycisk **Go**.

6.  Kliknij pozycję **DRMS\_ClusterPolicies**.

7.  W okienku wyników zmień wartość w kolumnie **PolicyData** wiersza **LoggingDatabaseServer** na nazwę nowego serwera bazy danych programu RMS.

8.  Kliknij polecenie **Persist**.

9.  Zmień wartość w kolumnie **PolicyData** wiersza **CertificationUserKeyStorageConnectionString**, tak aby odpowiadała nowemu serwerowi bazy danych. Wartość ta powinna mieć postać **data source=***&lt;nazwa nowego serwera bazy danych&gt;***;integrated**, gdzie *&lt;nazwa nowego serwera bazy danych&gt;* to nazwa nowego serwera bazy danych.

10. Kliknij polecenie **Persist**.

11. Powtórz kroki 9–10 dla wartości w kolumnie **PolicyData** wiersza **DirectoryServicesCacheDatabase**.

12. W lewym okienku kliknij opcję **DRMS\_PluginProperties**.

13. Dla **PropertyID** 101 o nazwie **PERSISTENT\_STORAGE** zmień wartość z kolumny **PropertyValue**, tak aby odpowiadała nowemu serwerowi bazy danych. Wartość ta powinna mieć postać **data source=***&lt;nazwa nowego serwera bazy danych&gt;***;integrated**, gdzie *&lt;nazwa nowego serwera bazy danych&gt;* to nazwa nowego serwera bazy danych.

14. Kliknij polecenie **Persist**.

15. Zamknij narzędzie RMS Config Editor.

Aby zaktualizować bazę danych konfiguracji RMS przy użyciu programu SQL Server Management Studio, wykonaj następujące czynności:

**Aby zaktualizować bazę danych konfiguracji RMS przy użyciu programu SQL Server Management Studio**
1.  Zaloguj się na serwer bazy danych konfiguracji RMS z konta lokalnego administratora lub innego konta użytkownika należącego do lokalnej grupy Administratorzy.

2.  Kliknij przycisk **Start**, wskaż polecenie **Wszystkie programy**, wskaż polecenie **Microsoft SQL Server 2005**, a następnie kliknij polecenie **SQL Server Management Studio**.

3.  Na stronie **Connect to Server** sprawdź, czy nowa nazwa serwera bazy danych znajduje się na liście w polu **Server name**, a następnie kliknij polecenie **Connect**.

4.  Rozwiń listę **Databases**, rozwiń listę **DRMS\_Config\_***&lt;nazwa klastra RMS&gt;***\_***&lt;Port&gt;*, a następnie rozwiń listę **Tables**.

5.  Prawym przyciskiem myszy kliknij pozycję **DRMS\_ClusterPolicies**, a następnie kliknij polecenie **Open Table**.

6.  W okienku wyników zmień wartość w kolumnie **PolicyData** wiersza **LoggingDatabaseServer** na nazwę nowego serwera bazy danych programu RMS.

7.  Zmień wartość w kolumnie **PolicyData** wiersza **CertificationUserKeyStorageConnectionString**, tak aby odpowiadała nowemu serwerowi bazy danych. Wartość ta powinna mieć postać **data source=***&lt;nazwa nowego serwera bazy danych&gt;***;integrated**, gdzie *&lt;nazwa nowego serwera bazy danych&gt;* to nazwa nowego serwera bazy danych.

8.  Powtórz kroki 6–7 dla wartości w kolumnie **PolicyData** wiersza **DirectoryServicesCacheDatabase**.

9.  W okienku Object Explorer kliknij prawym przyciskiem myszy pozycję **DRMS\_PluginProperties**, a następnie kliknij polecenie **Open Table**.

10. Dla **PropertyID** 101 o nazwie **PERSISTENT\_STORAGE** zmień wartość z kolumny **PropertyValue**, tak aby odpowiadała nowemu serwerowi bazy danych. Wartość ta powinna mieć postać **data source=***&lt;nazwa nowego serwera bazy danych&gt;***;integrated**, gdzie *&lt;nazwa nowego serwera bazy danych&gt;* to nazwa nowego serwera bazy danych.

11. Zamknij program Microsoft SQL Server Management Studio.

Konfigurowanie wszystkich serwerów w klastrze RMS do używania nazwy nowego serwera bazy danych
----------------------------------------------------------------------------------------------

Aby skonfigurować wszystkie serwery w klastrze RMS do używania nazwy nowego serwera bazy danych, należy zaktualizować pliki web.config i trzy wpisy w rejestrze. Po wykonaniu tych czynności należy uruchomić ponownie program Internet Information Services (IIS), aby zmiany odniosły skutek.

Aby zaktualizować pliki web.config na wszystkich serwerach w klastrze RMS:

**Aby zaktualizować pliki web.config na wszystkich serwerach w klastrze RMS**
1.  Zaloguj się na serwer w klastrze RMS jako członek lokalnej grupy Administratorzy .

2.  Przejdź do katalogu %Systemdrive%\\inetpub\\wwwroot\\\_wmcs\\admin.

3.  Kliknij dwukrotnie plik **web.config**, zaznacz opcję **Wybrać program z listy**, a następnie kliknij przycisk **OK**.

4.  Kliknij pozycję **Notatnik**, usuń zaznaczenie pola wyboru **Zawsze używaj wybranego programu do otwierania tego typu plików** i kliknij przycisk **OK**.

5.  Kliknij menu **Edycja**, a następnie polecenie **Zamień**.

6.  W polu **Znajdź** wpisz nazwę przeznaczonego do wycofania serwera bazy danych, który obsługuje bazy danych RMS.

7.  W polu **Zamień na** wpisz nazwę nowego serwera bazy danych, który obsługuje bazy danych RMS.

8.  Kliknij przycisk **Zamień wszystko**, a następnie przycisk **Anuluj**.

9.  Kliknij menu **Plik**, a następnie polecenie **Zapisz**.

10. Zamknij Notatnik.

11. Powtórz kroki 2–9 dla plików web.config znajdujących się w katalogach %Systemdrive%\\inetpub\\wwwroot\\\_wmcs\\certification i %Systemdrive%\\inetpub\\wwwroot\\\_wmcs\\licensing.

12. Powtórz kroki 1–11 dla każdego serwera w klastrze RMS.

Następnie zaktualizuj rejestr na każdym serwerze w klastrze RMS, umieszczając w nim nazwę nowego serwera bazy danych:

> [!Caution]  
> Niepoprawne edytowanie rejestru może spowodować poważne uszkodzenia systemu. Przed wprowadzeniem zmian w rejestrze należy wykonać kopie zapasowe wszystkich ważnych danych przechowywanych na komputerze. 

**Aby zaktualizować rejestr na wszystkich serwerach w klastrze RMS**
1.  Zaloguj się na serwer w klastrze RMS jako członek lokalnej grupy Administratorzy .

2.  Kliknij przycisk **Start**, a następnie polecenie **Uruchom**.

3.  Wpisz **regedit.exe** i naciśnij przycisk **OK**.

4.  Przejdź do klucza **HKEY\_LOCAL\_MACHINE\\Software\\Microsoft\\DRMS\\1.0\\KeyProtection**.

5.  Zmień wpis o nazwie PASSWORDDERIVEDKEY\_*&lt;nazwa starego serwera bazy danych&gt;*\_DRMS\_CONFIG\_*&lt;nazwa klastra RMS&gt;*\_*&lt;port&gt;* na:

    PASSWORDDERIVEDKEY\_*&lt;nazwa nowego serwera bazy danych&gt;*\_DRMS\_CONFIG\_*&lt;nazwa klastra RMS&gt;*\_*&lt;port&gt;*

    gdzie:

    -   *&lt;nazwa starego serwera bazy danych&gt;* to nazwa starego serwera bazy danych
    -   *&lt;nazwa klastra RMS&gt;* to nazwa klastra RMS
    -   *&lt;port&gt;* to port TCP, którego program RMS używa do komunikacji
    -   *&lt;nazwa nowego serwera bazy danych&gt;* to nazwa nowego serwera bazy danych

6.  Przejdź do klucza **HKEY\_LOCAL\_MACHINE\\System\\CurrentControlSet001\\Services\\DRMS\_Logging\_&lt;nazwa klastra RMS&gt;\_&lt;port&gt;\\Params**.

7.  Zmień wpis rejestru **ConnectionString**, tak aby wartość źródła danych odpowiadała nowej nazwie serwera bazy danych.

8.  Powtórz kroki 6–7 dla klucza **HKEY\_LOCAL\_MACHINE\\System\\CurrentControlSet\\Services\\DRMS\_Logging\_&lt;nazwa klastra RMS&gt;\_&lt;port&gt;\\Params**.

9.  W wierszu polecenia wpisz polecenie **IISRESET**, a następnie naciśnij klawisz ENTER.

10. Powtórz kroki 1–9 dla każdego serwera w klastrze RMS.
