---
TOCTitle: 'Krok 2. Instalowanie serwera WSUS lub konsoli administracyjnej programu WSUS'
Title: 'Krok 2. Instalowanie serwera WSUS lub konsoli administracyjnej programu WSUS'
ms:assetid: '6db6fcb0-c55d-43b9-9b07-4040c6267759'
ms:contentKeyID: 21798618
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Dd939859(v=WS.10)'
---

Krok 2. Instalowanie serwera WSUS lub konsoli administracyjnej programu WSUS
============================================================================

Po upewnieniu się, że serwer spełnia minimalne wymagania systemowe i zostały udzielone niezbędne uprawnienia kont, można zainstalować program Windows Server Update Services 3.0 z dodatkiem Service Pack 2 (WSUS 3.0 z dodatkiem SP2). Instalację programu WSUS 3.0 z dodatkiem SP2 należy rozpocząć, wykonując procedurę odpowiednią dla używanego systemu operacyjnego i rodzaju instalacji (za pomocą Menedżera serwera lub pliku WSUSSetup.exe).

Korzystanie z Menedżera serwera
-------------------------------

**Aby rozpocząć instalację serwera WSUS 3.0 z dodatkiem SP2 za pomocą Menedżera serwera**
1.  Zaloguj się na serwerze, na którym chcesz zainstalować program WSUS 3.0 z dodatkiem SP2, przy użyciu konta należącego do lokalnej grupy Administratorzy.

2.  Kliknij przycisk **Start**, wskaż polecenie **Narzędzia administracyjne**, a następnie kliknij polecenie **Menedżer serwera**.

3.  W okienku po prawej stronie okna Menedżer serwera w sekcji Podsumowanie ról kliknij pozycję **Dodaj role**.

4.  Jeśli zostanie wyświetlona strona Zanim rozpoczniesz, kliknij przycisk **Dalej**.

5.  Na stronie Wybieranie ról serwera wybierz pozycję **Windows Server Update Services**.

6.  Na stronie Windows Server Update Services kliknij przycisk **Dalej**.

7.  Na stronie Potwierdzanie opcji instalacji kliknij przycisk **Zainstaluj**.

8.  Gdy zostanie uruchomiony Kreator instalacji programu WSUS 3.0 z dodatkiem SP2, pomiń następną sekcję i przejdź do procedury „Aby kontynuować instalowanie programu WSUS 3.0 z dodatkiem SP2”.

Korzystanie z pliku WSUSSetup.exe
---------------------------------

**Aby rozpocząć instalację serwera WSUS 3.0 z dodatkiem SP2 lub konsoli administracyjnej programu WSUS 3.0 z dodatkiem SP2 za pomocą pliku WSUSSetup.exe**
1.  Zaloguj się na serwerze, na którym chcesz zainstalować program WSUS 3.0 z dodatkiem SP2, przy użyciu konta należącego do lokalnej grupy Administratorzy.

2.  Kliknij dwukrotnie plik instalatora **WSUSSetup.exe**.

3.  Gdy zostanie uruchomiony Kreator instalacji programu Windows Server Update Services 3.0 z dodatkiem SP2, przejdź do procedury „Aby kontynuować instalowanie programu WSUS 3.0 z dodatkiem SP2”.

Korzystanie z Kreatora instalacji programu WSUS 3.0 z dodatkiem SP2
-------------------------------------------------------------------

Kreator instalacji programu WSUS jest uruchamiany z poziomu Menedżera serwera lub pliku WSUSSetup.exe.

**Aby kontynuować instalowanie programu WSUS 3.0 z dodatkiem SP2**
1.  Na stronie powitania Kreatora instalacji programu Windows Server Update Services 3.0 kliknij przycisk **Dalej**.

2.  Na stronie Wybór trybu instalacji kliknij pozycję **Pełna instalacja serwera, w tym konsoli administracyjnej**, aby zainstalować serwer WSUS na tym komputerze, lub pozycję **Tylko konsola administracyjna**, aby zainstalować tylko konsolę administracyjną.

3.  Na stronie Umowa licencyjna przeczytaj warunki umowy licencyjnej, kliknij opcję **Akceptuję warunki Umowy licencyjnej**, a następnie kliknij przycisk **Dalej**.

4.  Na stronie Wybieranie źródła aktualizacji kreatora instalacji można wybrać źródła aktualizacji klientów. Domyślnie pole wyboru **Przechowuj aktualizacje lokalnie** jest zaznaczone, co oznacza, że aktualizacje będą zapisywane na serwerze WSUS w wybranej lokalizacji. Jeśli wyczyścisz pole wyboru **Przechowuj aktualizacje lokalnie**, zatwierdzone aktualizacje będą pobierane z witryny Microsoft Update na komputery klienckie. Dokonaj wyboru, a następnie kliknij przycisk **Dalej**.

5.  Na stronie Opcje bazy danych wybierz oprogramowanie używane do zarządzania bazą danych programu WSUS 3.0. Domyślnie kreator instalacji sugeruje zainstalowanie wewnętrznej bazy danych systemu Windows.

    Jeśli nie chcesz używać wewnętrznej bazy danych systemu Windows, podaj wystąpienie programu SQL Server, które ma być używane przez program WSUS, wybierając opcję **Użyj istniejącego serwera baz danych na tym komputerze** lub opcję **Użyj istniejącego serwera baz danych na komputerze zdalnym**. Wpisz nazwę wystąpienia w odpowiednim polu. Nazwa wystąpienia powinna mieć strukturę &lt;*nazwa\_serwera*&gt;\\&lt;*nazwa\_wystapienia*&gt;, gdzie *nazwa\_serwera* jest nazwą serwera, a *nazwa\_wystapienia* jest nazwą wystąpienia programu SQL. Dokonaj wyboru, a następnie kliknij przycisk **Dalej**.

6.  Jeśli wybrano połączenie z programem SQL Server, na stronie **Łączenie z wystąpieniem serwera SQL** program WSUS podejmie próbę nawiązania połączenia z wybranym wystąpieniem programu SQL Server. Po pomyślnym nawiązaniu połączenia kliknij przycisk **Dalej**, aby kontynuować.

7.  Na stronie Wybieranie witryny sieci Web określ witrynę sieci Web, która będzie używana przez program WSUS. Jeśli domyślna witryna sieci Web ma być używana w porcie 80, wybierz opcję **Użyj istniejącej domyślnej witryny sieci Web IIS**. Jeśli port 80 jest już używany przez inną witrynę sieci Web, można utworzyć inną witrynę w porcie 8530, wybierając opcję **Utwórz witrynę sieci Web Windows Server Update Services 3.0 SP2**. Kliknij przycisk **Dalej**.

8.  Na stronie **Gotowy do zainstalowania programu Microsoft Windows Server Update Services** przejrzyj wybrane opcje, a następnie kliknij przycisk **Dalej**.

9.  Na ostatniej stronie kreatora instalacji zostanie wyświetlona informacja o tym, czy instalacja programu WSUS została ukończona pomyślnie. Po kliknięciu przycisku **Zakończ** zostanie uruchomiony kreator konfiguracji.

Następny krok
-------------

[Krok 3. Konfigurowanie połączeń sieciowych](https://technet.microsoft.com/42a144c5-f08e-4a6e-b360-47ddea77bd24)

Materiały dodatkowe
-------------------

[Program Windows Server Update Services 3.0 z dodatkiem SP2 — przewodnik krok po kroku](https://technet.microsoft.com/4b504edc-93b3-45b0-a7e8-d0107f1a4442)
