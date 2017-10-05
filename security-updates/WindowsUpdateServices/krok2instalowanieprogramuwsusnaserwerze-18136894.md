---
TOCTitle: 'Krok 2. Instalowanie programu WSUS na serwerze'
Title: 'Krok 2. Instalowanie programu WSUS na serwerze'
ms:assetid: 'f593532c-e92e-47f3-914a-38a6c2519e94'
ms:contentKeyID: 18136894
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc708622(v=WS.10)'
---

Krok 2. Instalowanie programu WSUS na serwerze
==============================================

Po zapoznaniu się z wymaganiami dotyczącymi instalacji można rozpocząć instalowanie programu WSUS. W tym celu należy zalogować się na serwerze, na którym będzie instalowany program WSUS (przy użyciu konta przypisanego do lokalnej grupy Administratorzy). Program WSUS mogą instalować tylko użytkownicy należący do lokalnej grupy Administratorzy.

W poniższej procedurze są używane domyślne opcje instalacyjne programu WSUS dla systemu Windows Server 2003, takie jak instalowanie programu Windows SQL Server 2000 Desktop Engine (WMSDE) dla bazy danych WSUS, lokalne przechowywanie aktualizacji oraz korzystanie z domyślnej witryny sieci Web programu IIS na porcie 80. Procedury związane z niestandardowymi opcjami instalacyjnymi, takimi jak korzystanie z innego systemu operacyjnego, innego oprogramowania bazy danych lub z witryny sieci Web o niestandardowym numerze portu, zostały omówione w oficjalnym dokumencie „Deploying Microsoft Windows Server Update Services” (dokument dostępny w języku angielskim).

**Aby zainstalować program WSUS w systemie Windows Server 2003:**
1.  Kliknij dwukrotnie plik instalatora **WSUSSetup.exe**.

    | ![](images/Cc708622.note(WS.10).gif)Uwaga                                                                                                                                         |
    |----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | The latest version of WSUSSetup.exe is available on the [Microsoft Web site](http://go.microsoft.com/fwlink/?linkid=47374) for Windows Server Update Services at http://go.microsoft.com/fwlink/?LinkId=47374. |

2.  Na stronie **Zapraszamy** kreatora kliknij przycisk **Dalej**.

3.  Dokładnie przeczytaj warunki Umowy licencyjnej, kliknij opcję **Akceptuję warunki Umowy licencyjnej.**, a następnie kliknij przycisk **Dalej**.

4.  Na stronie **Wybieranie źródła aktualizacji** możesz określić, skąd komputery klienckie pobierają aktualizacje. Jeśli zaznaczysz pole wyboru **Przechowuj aktualizacje lokalnie**, aktualizacje będą przechowywane na serwerze WSUS, w związku z czym będzie konieczne wybranie dla nich lokalizacji w systemie plików. W innym przypadku komputery klienckie będą łączyć się z witryną Microsoft Update w celu pobrania zatwierdzonych aktualizacji.

    Zachowaj opcje domyślne i kliknij przycisk **Dalej**.

    ![](images/Cc708622.fa6ac6a6-6814-4b7e-96e8-e08af5e534b8(WS.10).gif)

5.  Na stronie **Opcje bazy danych** wybierz oprogramowanie używane do zarządzania bazą danych WSUS. Domyślnie podczas instalacji programu WSUS proponowane jest zainstalowanie oprogramowania WMSDE (na komputerze z systemem Windows Server 2003).

    Jeśli nie możesz korzystać z programu WMSDE, podaj wystąpienie serwera SQL dla programu WSUS. W tym celu kliknij opcję **Użyj istniejącego serwera baz danych na tym komputerze**, a następnie wpisz nazwę wystąpienia w polu **Nazwa wystąpienia SQL**. Więcej informacji na temat programowych opcji bazy danych można znaleźć w oficjalnym dokumencie „Deploying Microsoft Windows Server Update Services” (dokument dostępny w języku angielskim).

    Zachowaj opcje domyślne i kliknij przycisk **Dalej**.

    ![](images/Cc708622.bc0b73ad-b338-437c-a3c7-0299e819840d(WS.10).gif)

6.  Na stronie **Wybieranie witryny sieci Web** określ witrynę sieci Web, która będzie używana przez program WSUS. Na tej stronie znajdują się także dwa ważne adresy URL (zależne od dokonanego wyboru): adres URL, z którego komputery klienckie WSUS będą pobierać aktualizacje, oraz adres URL dla konsoli WSUS, która będzie używana podczas konfigurowania programu WSUS.

    Jeśli witryna sieci Web już korzysta z portu 80, może zajść potrzeba utworzenia witryny sieci Web programu WSUS na porcie niestandardowym. Więcej informacji na temat uruchamiania programu WSUS na porcie niestandardowym można znaleźć w oficjalnym dokumencie „Deploying Microsoft Windows Server Update Services” (dokument dostępny w języku angielskim).

    Zachowaj opcję domyślną i kliknij przycisk **Dalej**.

    ![](images/Cc708622.64ed7643-a050-4f54-bf9f-04cf7931adc0(WS.10).gif)

7.  Na stronie **Dublowanie ustawień aktualizacji** możesz określić rolę zarządzania serwerem WSUS. Pomiń ten ekran w przypadku konfigurowania pierwszego serwera WSUS w sieci lub definiowania topologii zarządzania rozproszonego.

    W przypadku definiowania topologii zarządzania scentralizowanego, a serwer nie jest pierwszym serwerem WSUS w sieci, zaznacz pole wyboru, a w polu **Nazwa serwera** wpisz nazwę dodatkowego serwera WSUS. Więcej informacji na temat roli zarządzania można znaleźć w oficjalnym dokumencie „Deploying Microsoft Windows Server Update Services” (dokument dostępny w języku angielskim).

    Zachowaj opcję domyślną i kliknij przycisk **Dalej**.

    ![](images/Cc708622.f26e09d5-983c-418d-8511-8960850403ef(WS.10).gif)

8.  Na stronie **Gotowy do zainstalowania programu Microsoft Windows Server Update Services** przejrzyj wybrane opcje, a następnie kliknij przycisk **Dalej**.

    ![](images/Cc708622.20de7d09-3d30-4867-9253-6f353dd1923d(WS.10).gif)

9.  Jeśli na ostatniej stronie kreatora pojawi się komunikat o pomyślnym zakończeniu instalacji programu WSUS, kliknij przycisk **Zakończ**.
