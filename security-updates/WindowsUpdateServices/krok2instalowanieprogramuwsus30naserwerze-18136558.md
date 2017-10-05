---
TOCTitle: 'Krok 2. Instalowanie programu WSUS 3.0 na serwerze'
Title: 'Krok 2. Instalowanie programu WSUS 3.0 na serwerze'
ms:assetid: '191e62a0-7671-41eb-9841-17c64313fa68'
ms:contentKeyID: 18136558
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720469(v=WS.10)'
---

Krok 2. Instalowanie programu WSUS 3.0 na serwerze
==================================================

Po upewnieniu się, że serwer spełnia wymagania dotyczące instalacji, można rozpocząć instalowanie programu WSUS 3.0. W tym celu należy zalogować się na serwerze, na którym będzie instalowany program WSUS 3.0 (przy użyciu konta przypisanego do lokalnej grupy Administratorzy). Program WSUS 3.0 mogą instalować tylko użytkownicy należący do lokalnej grupy Administratorzy.

W poniższej procedurze są używane domyślne opcje instalacyjne programu WSUS, takie jak instalowanie programu Wewnętrzna baza danych systemu Windows dla bazy danych WSUS 3.0, lokalne przechowywanie aktualizacji oraz korzystanie z domyślnej witryny sieci Web programu IIS przy użyciu portu 80.

**Aby zainstalować program WSUS 3.0**
1.  Kliknij dwukrotnie plik instalatora **WSUSSetup.exe**.

2.  Na stronie **Zapraszamy** kreatora instalacji kliknij przycisk **Dalej**.

3.  Na stronie **Wybór trybu instalacji** kliknij pozycję **Pełna instalacja serwera, w tym konsoli administracyjnej**, jeśli chcesz zainstalować serwer na danym komputerze lub opcję **Tylko konsola administracyjna**, jeśli chcesz zainstalować tylko konsolę administracyjną.

4.  Na stronie **Umowa licencyjna** dokładnie przeczytaj warunki Umowy licencyjnej, zaznacz opcję **Akceptuję warunki Umowy licencyjnej**, a następnie kliknij przycisk **Dalej**.

    ![](images/Cc720469.fa6ac6a6-6814-4b7e-96e8-e08af5e534b8(WS.10).gif)

5.  Na stronie kreatora instalacji **Wybieranie źródła aktualizacji** można określić, skąd komputery klienckie mają pobierać aktualizacje. Jeśli zaznaczysz pole wyboru **Przechowuj aktualizacje lokalnie**, aktualizacje będą przechowywane na serwerze WSUS 3.0, w związku z czym będzie konieczne wybranie dla nich lokalizacji w systemie plików. W innym przypadku komputery klienckie będą łączyć się z witryną Microsoft Update w celu pobrania zatwierdzonych aktualizacji. Zachowaj opcje domyślne i kliknij przycisk **Dalej**.

    ![](images/Cc720469.c8bac396-ca39-4491-8b0c-742a0e470535(WS.10).gif)

6.  Na stronie **Opcje bazy danych** wybierz oprogramowanie używane do zarządzania bazą danych WSUS 3.0. Domyślnie podczas instalacji programu WSUS proponowane jest zainstalowanie oprogramowania Wewnętrzna baza danych systemu Windows (na komputerze z systemem Windows Server 2003).

7.  Jeśli nie chcesz używać oprogramowania Wewnętrzna baza danych systemu Windows, podaj wystąpienie serwera SQL dla programu WSUS. W tym celu zaznacz opcję **Użyj** **istniejącego serwera baz danych na tym komputerze**, a następnie wpisz nazwę wystąpienia w odpowiednim polu. Nazwa wystąpienia powinna mieć strukturę &lt;*nazwa\_serwera*&gt;\\&lt;*nazwa\_wystapienia*&gt;, gdzie *nazwa\_serwera* jest nazwą serwera, a *nazwa\_wystapienia* jest nazwą wystąpienia programu SQL. Dokonaj wyboru, a następnie kliknij przycisk **Dalej**.

8.  Na stronie **Łączenie z wystąpieniem serwera SQL** program WSUS spróbuje połączyć się z określonym wystąpieniem serwera SQL. Po pomyślnym nawiązaniu połączenia kliknij przycisk **Dalej**, aby kontynuować.

    ![](images/Cc720469.36c6af0c-a61e-4151-ae50-c754a106cb1b(WS.10).gif)

9.  Na stronie **Wybieranie witryny sieci Web** określ witrynę sieci Web, która będzie używana przez program WSUS 3.0. Jeśli chcesz użyć domyślnej witryny sieci Web programu IIS przy użyciu portu 80, wybierz pierwszą opcję. Jeśli witryna sieci Web już korzysta z portu 80, może zajść potrzeba utworzenia alternatywnej witryny na porcie 8530 przez wybranie drugiej opcji. Zachowaj opcję domyślną i kliknij przycisk **Dalej**.

10. Na stronie **Gotowy do zainstalowania programu Microsoft Windows Server Update Services** przejrzyj wybrane opcje, a następnie kliknij przycisk **Dalej**.

11. Na ostatniej stronie kreatora instalacji wyświetlana jest informacja o pomyślnym zakończeniu instalacji programu WSUS 3.0 lub o niepowodzeniu instalacji. Po kliknięciu przycisku **Zakończ** zostanie uruchomiony kreator konfiguracji.
