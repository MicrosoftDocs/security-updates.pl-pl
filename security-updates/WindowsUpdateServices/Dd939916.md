---
TOCTitle: 'Krok 1. Potwierdzanie wymagań dotyczących instalacji programu WSUS 3.0 z dodatkiem SP2'
Title: 'Krok 1. Potwierdzanie wymagań dotyczących instalacji programu WSUS 3.0 z dodatkiem SP2'
ms:assetid: 'ec01bd75-5def-4899-8cee-ddab827bbd83'
ms:contentKeyID: 21798699
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Dd939916(v=WS.10)'
---

Krok 1. Potwierdzanie wymagań dotyczących instalacji programu WSUS 3.0 z dodatkiem SP2
======================================================================================

Przed zainstalowaniem programu Windows Server Update Services 3.0 z dodatkiem Service Pack 2 (WSUS 3.0 z dodatkiem SP2) lub wykonaniem uaktualnienia do tej wersji należy sprawdzić, czy serwer i komputery klienckie spełniają wymagania systemowe programu WSUS 3.0 z dodatkiem SP2 oraz czy są dostępne uprawnienia niezbędne do przeprowadzenie instalacji.

Wymagania sprzętowe i programowe serwera dotyczące instalowania programu WSUS 3.0 z dodatkiem SP2
-------------------------------------------------------------------------------------------------

1.  Serwer musi spełniać wymagania systemowe programu WSUS 3.0 z dodatkiem SP2 dotyczące konfiguracji sprzętowej, systemu operacyjnego i innego wymaganego oprogramowania. Wymagania systemowe są wymienione w informacjach o wersji programu WSUS 3.0 z dodatkiem SP2 pod adresem [http://go.microsoft.com/fwlink/?LinkId=139840](http://go.microsoft.com/fwlink/?linkid=139840) (strona może zostać wyświetlona w języku angielskim). Jeśli jest planowane zainstalowanie serwera WSUS 3.0 z dodatkiem SP2 za pomocą Menedżera serwera, można sprawdzić, czy wymagania dotyczące oprogramowania są spełnione, wykonując procedurę w sekcji „Przygotowywanie do instalacji programu WSUS 3.0 z dodatkiem SP2”.
2.  Jeśli zainstalowano role lub aktualizacje oprogramowania wymagające ponownego uruchomienia serwera po ukończeniu instalacji, należy ponownie uruchomić serwer przed zainstalowaniem programu WSUS 3.0 z dodatkiem SP2.

Wymagania dotyczące oprogramowania klienta
------------------------------------------

Klientem programu WSUS 3.0 jest funkcja Aktualizacje automatyczne. Jedynym wymaganiem sprzętowym dla tej funkcji jest podłączenie do sieci.

1.  Komputer, na którym ma zostać zainstalowana funkcja Aktualizacje automatyczne, musi spełniać wymagania systemowe programu WSUS 3.0 z dodatkiem SP2 dotyczące komputerów klienckich. Wymagania systemowe są wymienione w informacjach o wersji programu WSUS 3.0 z dodatkiem SP2 pod adresem [http://go.microsoft.com/fwlink/?LinkId=139840](http://go.microsoft.com/fwlink/?linkid=139840) (strona może zostać wyświetlona w języku angielskim).
2.  Jeśli zainstalowano aktualizacje oprogramowania wymagające ponownego uruchomienia komputera, należy ponownie uruchomić komputer przed zainstalowaniem programu WSUS 3.0 z dodatkiem SP2.

Uprawnienia
-----------

Uprawnienia wymagane dla określonych użytkowników i katalogów:

1.  Aby przystawka administracyjna programu WSUS była wyświetlana poprawnie, konto Zarządzanie NT\\Usługa sieciowa musi mieć uprawnienie Pełna kontrola do następujących folderów:
    -   %windir%\\Microsoft .NET\\Framework\\v2.0.50727\\Temporary ASP.NET Files
    -   %windir%\\Temp
2.  Konto, za pomocą którego ma zostać zainstalowany program WSUS 3.0 z dodatkiem SP2, musi należeć do grupy Administratorzy lokalni.

Przygotowywanie do instalacji programu WSUS 3.0 z dodatkiem SP2
---------------------------------------------------------------

Na komputerach z systemem Windows 7 lub Windows Server 2008 z dodatkiem SP2 program WSUS 3.0 z dodatkiem SP2 można zainstalować za pomocą Menedżera serwera. W przypadku korzystania z innego obsługiwanego systemu operacyjnego lub instalowania tylko konsoli administracyjnej programu WSUS należy przejść do następnej sekcji tego przewodnika, aby zainstalować program WSUS 3.0 z dodatkiem SP2 za pomocą pliku WSUSSetup.exe.

**Aby przeprowadzić przygotowanie do instalacji serwera WSUS 3.0 z dodatkiem SP2 za pomocą Menedżera serwera**
1.  Zaloguj się na serwerze, na którym chcesz zainstalować program WSUS 3.0 z dodatkiem SP2, przy użyciu konta należącego do lokalnej grupy Administratorzy.

2.  Kliknij przycisk **Start**, wskaż polecenie **Narzędzia administracyjne**, a następnie kliknij polecenie **Menedżer serwera**.

3.  W okienku po prawej stronie okna Menedżer serwera w sekcji Podsumowanie ról kliknij pozycję **Dodaj role**.

4.  Jeśli zostanie wyświetlona strona Zanim rozpoczniesz, kliknij przycisk **Dalej**.

5.  Na stronie Wybieranie ról serwera upewnij się, że są zaznaczone pola wyboru **Serwer aplikacji** i **Serwer sieci Web (IIS)**. Jeśli są one zaznaczone, wykonaj pozostałą część tego kroku, aby upewnić się, że są wybrane wymagane usługi ról. W przeciwnym wypadku zainstaluj role Serwer aplikacji i Serwer sieci Web (IIS) zgodnie z poniższą procedurą.

    1.  Na stronie Wybieranie ról serwera wybierz role **Serwer aplikacji** i **Serwer sieci Web (IIS)**. Kliknij przycisk **Dalej**.
    2.  W przypadku instalowania usług ról aplikacji na stronie Serwer aplikacji kliknij przycisk **Dalej**. Na stronie Usługi roli serwera aplikacji zaakceptuj ustawienia domyślne, a następnie kliknij przycisk **Dalej**.
    3.  W przypadku instalowania roli Serwer sieci Web (IIS) na stronie Serwer sieci Web (IIS) kliknij przycisk **Dalej**. Na stronie Usługi roli serwera sieci Web (IIS) pozostaw bez zmian ustawienia domyślne i wybierz usługi **ASP.NET**, **Uwierzytelnianie systemu Windows**, **Kompresja zawartości dynamicznej** oraz **Zgodność z narzędziami zarządzania usługami IIS w wersji 6**. Jeśli zostanie wyświetlone okno Kreator dodawania ról, kliknij pozycję **Dodaj wymagane usługi ról**. Kliknij przycisk **Dalej**.
    4.  Na stronie Potwierdzanie opcji instalacji kliknij przycisk **Zainstaluj**.
    5.  Na stronie Wyniki instalacji sprawdź, czy został wyświetlony komunikat informujący o pomyślnym zakończeniu instalacji usług ról wybranych w tym kroku, a następnie kliknij przycisk **Zamknij**.

Następny krok
-------------

[Krok 2. Instalowanie serwera WSUS lub konsoli administracyjnej programu WSUS](https://technet.microsoft.com/6db6fcb0-c55d-43b9-9b07-4040c6267759)

Materiały dodatkowe
-------------------

[Program Windows Server Update Services 3.0 z dodatkiem SP2 — przewodnik krok po kroku](https://technet.microsoft.com/4b504edc-93b3-45b0-a7e8-d0107f1a4442)
