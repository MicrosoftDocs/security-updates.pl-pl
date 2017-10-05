---
TOCTitle: Jak wdrażać klienta programu RMS
Title: Jak wdrażać klienta programu RMS
ms:assetid: 'c84f1724-cf71-4385-9003-ff68bc23c927'
ms:contentKeyID: 18123524
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747749(v=WS.10)'
---

Jak wdrażać klienta programu RMS
================================

Aby korzystać z funkcji programu RMS, np. usługi zarządzania prawami pakietu Microsoft® Office System 2003 i dodatku zarządzania prawami dla programu Internet Explorer w systemie Microsoft Windows XP lub Microsoft Windows 2000, należy zainstalować klienta programu Usługi zarządzania prawami dostępu (RMS). Klient programu RMS jest częścią systemu Windows Vista®.

Wiele organizacji chce kontrolować rozmieszczenie oprogramowania klienckiego. Do rozmieszczenia klienta programu RMS z dodatkiem Service Pack 2 (SP2) można wykorzystać program Systems Management Server (SMS) lub Zasady grupy.

Przed rozpoczęciem rozmieszczania zobacz [http://go.microsoft.com/fwlink/?LinkID=67736](http://go.microsoft.com/fwlink/?linkid=67736), aby pobrać klienta programu RMS.

| ![](images/Cc747749.Important(WS.10).gif)Ważne                                               |
|---------------------------------------------------------------------------------------------------------------------------|
| Klient programu RMS został zintegrowany z systemem Windows Vista. Dzięki temu oddzielna instalacja nie jest już wymagana. |

Wyodrębnianie plików instalacyjnych
-----------------------------------

Po pobraniu pliku WindowsRightsManagementServicesSP2-KB917275-Client-ENU.exe należy wyodrębnić pliki Instalatora Microsoft® Windows® z pakietu wykonywalnego.

W tym celu w wierszu polecenia można wpisać następujące polecenie:

`WindowsRightsManagementServicesSP2-KB917275-Client-ENU.exe /x <path>`

gdzie zmienna &lt;ścieżka&gt; jest katalogiem docelowym, w którym mają zostać zapisane wyodrębnione pliki.

Uruchomienie tego polecenia powoduje wyodrębnienie następujących plików do wybranego katalogu docelowego:

-   Bootstrap.exe
    Jest to plik interfejsu używany przez plik wykonywalny do instalacji innych plików pakietu. Nie jest używany podczas instalacji klienta programu RMS z dodatkiem SP2 za pomocą programu SMS lub Zasad grupy.
-   MSDrmClient.msi
    Jest to plik instalacyjny klienta programu RMS z dodatkiem SP2. Ta instalacja powoduje odinstalowanie wszystkich poprzednich wersji klienta programu RMS na komputerze. Program ten należy instalować najpierw na komputerach klienckich.
-   RMClientBackCompat.msi
    Jest to plik instalacyjny, w którym zdefiniowano nowego klienta programu RMS z dodatkiem SP2 dla aplikacji korzystających z programu RMS (np. Microsoft Office Professional 2003 lub 2007 Microsoft Office System) zależnych od poprzedniej wersji klienta programu RMS. Dzięki temu mogą one korzystać z klienta programu RMS z dodatkiem SP2. Program ten należy instalować na komputerach klienckich po pomyślnym zainstalowaniu pliku MSDrmClient.msi.

| ![](images/Cc747749.note(WS.10).gif)Uwaga                                                                                                                                                            |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Niezależnie od wybranej metody instalacji należy prawidłowo zainstalować oba pliki Instalatora Windows. Jeśli wystąpi błąd uniemożliwiający instalację pliku MSDrmClient.msi, nie należy instalować pliku RMClientBackCompat.msi. |

Rozmieszczanie klienta programu RMS za pomocą instalacji dyskretnej
-------------------------------------------------------------------

Wyodrębnianie plików w celu zainstalowania plików Instalatora Windows jest opcjonalne. Rozmieszczanie klienta programu RMS jest również możliwe za pomocą instalacji dyskretnej. W tym celu w wierszu polecenia można wpisać następujące polecenie:

`WindowsRightsManagementServicesSP2-KB917275-Client-ENU.exe -override 1 /I MsDrmClient.msi REBOOT=ReallySuppress /q -override 2 /I RmClientBackCompat.msi REBOOT=ReallySuppress /q`

To polecenie uruchamia instalację dyskretną klienta programu RMS.

| ![](images/Cc747749.note(WS.10).gif)Uwaga                                                                                                         |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Ponieważ jest to instalacja dyskretna, instalator nie informuje użytkownika o jej zakończeniu. Instalacje dyskretne są zwykle uruchamianie w pliku wsadowym lub pliku skryptu. |

Rozmieszczanie klienta programu RMS za pomocą programu SMS
----------------------------------------------------------

**Aby rozmieścić klienta programu RMS za pomocą programu SMS**
1.  Otwórz konsolę administracyjną programu SMS.

2.  Rozwiń bazę danych witryny, której chcesz użyć.

3.  W lewym okienku kliknij prawym przyciskiem myszy ikonę **Pakiety**, wybierz polecenie **Nowy**, a następnie kliknij polecenie **Pakiet z definicji**.

4.  Utwórz pakiety z plików MSDRMClient.msi i RMClientBackCompat.msi. Pakiety powinny mieć następujące właściwości:

    **Ogólne**:

    -   W **wierszu polecenia** wpisz:
        `msiexec.exe /q ALLUSERS=2 /m MSIDGHOG /i "<file_name>.msi"`
        | ![](images/Cc747749.note(WS.10).gif)Uwaga                                                                                |
        |-------------------------------------------------------------------------------------------------------------------------------------------------------|
        | MSIDGHOG jest wartością losową. Zastąp zmienną &lt;nazwa\_pliku&gt; nazwą pliku Instalatora Windows, za pomocą którego będzie instalowany ten pakiet. |

    -   W obszarze **Uruchom** zaznacz opcję **Ukryty**.
    -   W obszarze **Po uruchomieniu** zaznacz opcję **Nie jest wymagana żadna akcja**.
    -   W obszarze **Kategoria** zaznacz opcję **Oprogramowanie administracyjne**.

    **Wymagania:**

    -   W polu **Szacowane miejsce na dysku** wpisz **445 KB**.
    -   W obszarze **Maksymalny dopuszczalny czas uruchamiania** zaznacz opcję **Nieznany**.
    -   Zaznacz pole wyboru **Ten program można uruchamiać na dowolnej platformie**.

    **Środowisko:**

    -   W obszarze **Program może uruchomić** zaznacz opcję **Niezależnie od tego, czy użytkownik jest zalogowany**.
    -   W obszarze **Tryb uruchamiania** zaznacz opcję **Uruchom z prawami administratora**.
    -   W obszarze **Tryb dysku** zaznacz opcję **Działa z nazwą UNC**.

    **Zaawansowane:**

    -   Wyczyść pole wyboru **Uruchom najpierw inny program**.
    -   Wyczyść pole wyboru **Wyłącz powiadomienia programu** w obszarze **Gdy program jest przypisany do komputera**.
    -   Wyczyść pole wyboru **Wyłącz ten program na komputerach, na których jest anonsowany**.

5.  Ustaw **konta dostępu i punkty dystrybucji** odpowiednie dla organizacji.

6.  Utwórz anons dla odpowiedniego zestawu. Podczas rozmieszczania programu SMS zaleca się używanie programu **nienadzorowanego użytkownika**.

7.  Anonsowanie należy zaplanować zależnie od potrzeb organizacji.

Rozmieszczanie klienta programu RMS za pomocą Zasad grupy
---------------------------------------------------------

Aby rozmieścić klienta programu RMS na komputerach docelowych, można użyć funkcji Instalacja i konserwacja oprogramowania przystawki Zasady grupy.

Korzystanie z przystawki Zasady grupy jest zalecaną metodą w przypadku aktywnego zarządzania rozmieszczaniem klientów programu RMS w małych i średnich organizacjach, które jeszcze nie używają rozwiązań do zarządzania aktualizacjami w przedsiębiorstwach, np. Systems Management Server 2003.

Jeśli do dystrybucji programu jest używana przystawka Zasady grupy, można przypisać program do komputerów. Program jest instalowany po uruchomieniu komputera i jest dostępny dla wszystkich użytkowników logujących się do tego komputera. Aby uzyskać więcej informacji na temat przystawki Zasady grupy, zobacz Infrastruktura zasad grupy ([http://go.microsoft.com/fwlink/?LinkID=24328](http://go.microsoft.com/fwlink/?linkid=24328)). Na potrzeby tej procedury założono, że użytkownik korzysta z Konsoli zarządzania zasadami grupy (GPMC). Informacje na temat pobierania konsol GPMC znajdują się w temacie Konsola zarządzania zasadami grupy z dodatkiem Service Pack 1 ([hhttp://go.microsoft.com/fwlink/?LinkID=21813](http://go.microsoft.com/fwlink/?linkid=21813)).

Poniżej przedstawiono kilka wskazówek dla administratorów niezaznajomionych z dystrybucją oprogramowania opartą na zasadach grupy. Opisane czynności można odpowiednio dostosowywać, zależnie od potrzeb organizacji.

**Rozmieszczanie klienta programu RMS za pomocą przystawki Zasady grupy**
1.  Na kontrolerze domeny otwórz przystawkę **Użytkownicy i komputery usługi Active Directory** konsoli Microsoft Management Console (MMC).

2.  Utwórz nową jednostkę organizacyjną lub wybierz istniejącą jednostkę organizacyjną.

    Jeśli utworzono nową jednostkę, dodaj komputery, na których chcesz zainstalować klienta programu RMS.

3.  Kliknij prawym przyciskiem myszy odpowiednią jednostkę organizacyjną i wybierz polecenie **Właściwości**.

4.  Kliknij kartę **Zasady grupy**.

5.  Kliknij przycisk **Nowy**, aby utworzyć nowy obiekt zasad grupy.

6.  Kliknij przycisk **Edycja**, aby edytować nowy obiekt zasad grupy.

7.  W drzewie konsoli rozwiń węzeł **Konfiguracja komputera,Ustawienia oprogramowania**, a następnie wybierz opcję Instalacja oprogramowania.

8.  Kliknij prawym przyciskiem myszy okienko szczegółów, kliknij polecenie **Nowy**, a następnie kliknij polecenie **Pakiet**.

9.  Wprowadź ścieżkę do pliku MSDRMclient.msi w folderze udostępnionym w sieci, do którego mogą uzyskać dostęp komputery klienckie.

10. Kliknij przycisk **OK**, aby przypisać pakiet.

11. Ponownie wykonaj czynności opisane w punktach od 5 do 10, aby utworzyć obiekt zasad grupy, który zainstaluje plik RMClientBackCompat.msi.

| ![](images/Cc747749.note(WS.10).gif)Uwaga                                                                                                                                                                                                                                                                                                                                                       |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Powyższy opis zawiera jedynie wskazówki dla użytkowników, którzy nie mają doświadczenia w korzystaniu z przystawki Zasady grupy. Jeśli jesteś doświadczonym administratorem zasad grupy, możesz rozpowszechniać pakiet MSDrmClient.msi według własnych procedur. Ponadto czynności te należy wykonywać na kontrolerze domeny z systemem Windows Server 2003 — w domenie Windows 2000 procedura i terminologia mogą być inne. |

Uaktualnianie z poprzedniej wersji
----------------------------------

        ```
| ![](images/Cc747749.note(WS.10).gif)Uwaga                                          |
|-----------------------------------------------------------------------------------------------------------------|
| Ten skrypt nie działa w systemie Windows Vista, ponieważ klient programu RMS jest częścią systemu operacyjnego. |
