---
TOCTitle: 'Krok 5. Aktualizowanie i konfigurowanie funkcji Aktualizacje automatyczne'
Title: 'Krok 5. Aktualizowanie i konfigurowanie funkcji Aktualizacje automatyczne'
ms:assetid: '4ac8d574-f48e-4d9d-86c9-9aeb0f57e750'
ms:contentKeyID: 18136606
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720533(v=WS.10)'
---

Krok 5. Aktualizowanie i konfigurowanie funkcji Aktualizacje automatyczne
=========================================================================

Komputery klienckie WSUS wymagają zgodnej wersji funkcji Aktualizacje automatyczne. Instalator programu WSUS automatycznie konfiguruje program IIS w taki sposób, aby najnowsza wersja funkcji Aktualizacje automatyczne była dystrybuowana na wszystkie komputery klienckie połączone z serwerem WSUS.

> [!note]  
> Chociaż większość wersji funkcji Aktualizacje automatyczne można wskazać serwerowi WSUS (dzięki czemu zostaną one automatycznie zaktualizowane do wersji zgodnej z programem WSUS), wersja funkcji Aktualizacje automatyczne używana w systemie Windows XP nie może być automatycznie aktualizowana bez zainstalowanych dodatków Service Pack. Instrukcje dotyczące programu Software Update Services (SUS) w przypadku pracy w środowisku systemu Windows XP bez zainstalowanych dodatków Service Pack można znaleźć w oficjalnym dokumencie „Deploying Microsoft Windows Server Update Services” (dokument dostępny w języku angielskim). 

Najlepszy sposób skonfigurowania funkcji Aktualizacje automatyczne zależy od używanego środowiska sieciowego. W środowisku usługi Active Directory można skorzystać z obiektu zasad grupy. W środowisku innym niż środowisko usługi Active Directory należy użyć lokalnego obiektu zasad grupy. W przypadku korzystania z lokalnego obiektu zasad grupy lub obiektu zasad grupy przechowywanego w kontrolerze domeny należy wskazać komputery klienckie serwerowi WSUS, a następnie skonfigurować funkcję Aktualizacje automatyczne.

W poniższych instrukcjach założono, że używane jest środowisko sieciowe usługi Active Directory. W tych procedurach przyjęto również, że użytkownik skonfigurował już obiekt zasad grupy oraz używa go do zarządzania siecią. Dla ustawień WSUS należy utworzyć nowy obiekt zasad grupy, a następnie połączyć go na poziomie domeny.

Więcej informacji o zasadach grupy można znaleźć na stronie [Group Policy](http://go.microsoft.com/fwlink/?linkid=47375) pod adresem http://go.microsoft.com/fwlink/?LinkID=47375.

Krok 5 obejmuje następujące procedury:

-   Ładowanie szablonu administracyjnego WSUS
-   Konfigurowanie funkcji Aktualizacje automatyczne
-   Wskazywanie komputerów klienckich serwerowi WSUS
-   Ręczne inicjowanie wykrywania na komputerze klienckim

Następne trzy procedury należy wykonać przy użyciu obiektu zasad grupy (w środowisku usługi Active Directory).

**Aby dodać szablon administracyjny WSUS:**
1.  W Edytorze obiektów zasad grupy kliknij dowolny węzeł **Szablony administracyjne**.

2.  W menu **Akcja** kliknij polecenie **Dodaj/Usuń szablony**.

3.  Kliknij przycisk **Dodaj**.

4.  W oknie dialogowym **Szablony zasad** kliknij pozycję **wuau.adm**, a następnie kliknij przycisk **Otwórz**.

5.  W oknie dialogowym **Dodawanie/usuwanie szablonów** kliknij przycisk **Zamknij**.

**Aby skonfigurować zachowanie funkcji Aktualizacje automatyczne:**
1.  W Edytorze obiektów zasad grupy rozwiń węzeł **Konfiguracja komputera**, rozwiń węzeł **Szablony administracyjne**, rozwiń węzeł **Składniki systemu Windows**, a następnie kliknij pozycję **Windows Update**.

2.  W okienku szczegółów kliknij dwukrotnie pozycję **Konfigurowanie aktualizacji automatycznych**.

3.  Kliknij pozycję **Włączona**, a następnie kliknij jedną z następujących opcji:

    -   **Powiadom o pobieraniu i powiadom o instalacji.** W przypadku tej opcji zalogowany użytkownik administracyjny jest powiadamiany o zamiarze pobierania i zainstalowania aktualizacji.
    -   **Pobierz automatycznie i powiadom o instalacji.** W przypadku tej opcji pobieranie aktualizacji rozpoczyna się automatycznie, a następnie zalogowany użytkownik administracyjny jest powiadamiany o zamiarze ich zainstalowania.
    -   **Pobierz automatycznie i zaplanuj instalację.** Jeśli funkcja Aktualizacje automatyczne została skonfigurowana pod kątem przeprowadzania zaplanowanej instalacji, musisz również ustawić datę i godzinę instalacji zaplanowanej jako cykliczna.
    -   **Zezwalaj lokalnemu administratorowi na wybranie ustawienia.** W przypadku tej opcji lokalni administratorzy mogą użyć funkcji Aktualizacje automatyczne w Panelu sterowania do wybierania opcji konfiguracji. Na przykład mogą wybrać własną planowaną godzinę instalacji. Lokalni administratorzy nie są uprawnieni do wyłączania funkcji Aktualizacje automatyczne.

4.  Kliknij przycisk **OK**.

> [!note]  
> Ustawienie **Zezwalaj lokalnemu administratorowi na wybranie ustawienia** pojawia się tylko wtedy, gdy program Aktualizacje automatyczne jest zaktualizowany do wersji zgodnej z programem WSUS. 

**Aby wskazać komputery klienckie serwerowi WSUS:**
1.  W Edytorze obiektów zasad grupy rozwiń węzeł **Konfiguracja komputera**, rozwiń węzeł **Szablony administracyjne**, rozwiń węzeł **Składniki systemu Windows**, a następnie kliknij pozycję **Windows Update**.

2.  W okienku szczegółów kliknij dwukrotnie pozycję **Określ lokalizację intranetową usługi aktualizującej firmy Microsoft**.

3.  Kliknij pozycję **Włączona**, a następnie w polach **Ustaw intranetową usługę aktualizującą do wykrywania aktualizacji** oraz **Ustaw serwer statystyk intranetowych** wpisz adres URL tego samego serwera WSUS. Na przykład w obydwu polach wpisz **http://***nazwa\_serwera*.

4.  Kliknij przycisk **OK**.

> [!note]  
> Jeśli do wskazania tego komputera serwerowi WSUS jest używany lokalny obiekt zasad grupy, to ustawienie zostanie uwzględnione bezzwłocznie, a komputer powinien pojawić się na konsoli administracyjnej WSUS w ciągu 20 minut. Ręcznie inicjując cykl wykrywania, możesz przyspieszyć ten proces. 

Po skonfigurowaniu komputera klienckiego i upływie kilku minut pojawi się on na stronie **Komputery** na konsoli WSUS. W przypadku komputerów klienckich skonfigurowanych przy użyciu obiektu zasad grupy (w środowisku usługi Active Directory) nowe ustawienia dotyczące komputera klienckiego zostaną zastosowane po upływie około 20 minut po odświeżeniu tego obiektu. Domyślnie obiekt zasad grupy jest odświeżany w tle co 90 minut, z losowym przesunięciem z przedziału od 0 do 30 minut. Aby szybciej odświeżyć obiekt zasad grupy, można przejść do wiersza polecenia na komputerze klienckim i wpisać polecenie: **gpupdate /force**.

W przypadku komputerów klienckich skonfigurowanych przy użyciu lokalnego obiektu zasad grupy, zasady grupy są stosowane natychmiast, a ich uwzględnianie trwa około 20 minut.

Po zastosowaniu zasad grupy można ręcznie zainicjować wykrywanie. Po wykonaniu tego kroku nie trzeba czekać 20 minut na nawiązanie połączenia między komputerem klienckim a programem WSUS.

**Aby ręcznie zainicjować wykrywanie przez serwer WSUS:**
1.  Na komputerze klienckim kliknij przycisk **Start**, a następnie kliknij polecenie **Uruchom**.

2.  Wpisz polecenie **cmd**, a następnie kliknij przycisk **OK**.

3.  W wierszu polecenia wpisz **wuauclt.exe /detectnow**. Ta opcja wiersza polecenia instruuje funkcję Aktualizacje automatyczne o konieczności natychmiastowego nawiązania połączenia z serwerem WSUS.
