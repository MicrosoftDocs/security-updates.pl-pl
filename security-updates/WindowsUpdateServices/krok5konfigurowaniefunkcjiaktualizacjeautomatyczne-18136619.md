---
TOCTitle: 'Krok 5. Konfigurowanie funkcji Aktualizacje automatyczne'
Title: 'Krok 5. Konfigurowanie funkcji Aktualizacje automatyczne'
ms:assetid: '5da6d10a-6ff1-4de8-b53a-4893bf8bd9fa'
ms:contentKeyID: 18136619
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720532(v=WS.10)'
---

Krok 5. Konfigurowanie funkcji Aktualizacje automatyczne
========================================================

Komputery klienckie WSUS wymagają zgodnej wersji funkcji Aktualizacje automatyczne. Instalator programu WSUS automatycznie konfiguruje program IIS w taki sposób, aby najnowsza wersja funkcji Aktualizacje automatyczne była dystrybuowana na wszystkie komputery klienckie połączone z serwerem WSUS.

Najlepszy sposób skonfigurowania funkcji Aktualizacje automatyczne zależy od używanego środowiska sieciowego. W środowisku usługi Active Directory można skorzystać z obiektu zasad grupy opartego na domenie. W środowisku bez usługi Active Directory należy użyć lokalnego obiektu zasad grupy. W przypadku korzystania z lokalnego obiektu zasad grupy lub obiektu zasad grupy opartych na domenie należy wskazać komputery klienckie serwerowi WSUS, a następnie skonfigurować funkcję Aktualizacje automatyczne.

W poniższych instrukcjach założono, że używane jest środowisko sieciowe usługi Active Directory. W tych procedurach przyjęto również, że użytkownik zna sposób korzystania z zasad grupy oraz używa ich do zarządzania siecią. Dla ustawień programu WSUS należy utworzyć nowy obiekt zasad grupy, a następnie połączyć go z domeną.

Więcej informacji o zasadach grupy można znaleźć w witrynie sieci Web dotyczącej zasad grupy ([http://go.microsoft.com/fwlink/?LinkID=47375](http://go.microsoft.com/fwlink/?linkid=47375), strona może być w języku angielskim).

**Krok 5 obejmuje następujące procedury**:

-   Dodawanie szablonu administracyjnego WSUS
-   Konfigurowanie funkcji Aktualizacje automatyczne
-   Wskazywanie komputera klienckiego serwerowi WSUS
-   Ręczne inicjowanie wykrywania przez serwer WSUS

Pierwsze trzy procedury należy wykonać przy użyciu obiektu zasad grupy opartego na domenie. Konieczne jest utworzenie nowego obiektu zasad grupy lub użycie już istniejącego obiektu. Jeśli do zarządzania obiektami zasad grupy używana jest Konsola zarządzania zasadami grupy (GPMC), przejdź do obiektu zasad grupy, który chcesz zmodyfikować, a następnie kliknij przycisk **Edytuj**.

Aby wyświetlić ustawienia zasad służące do zarządzania programem WSUS, należy upewnić się, że plik szablonu administracyjnego programu WSUS o nazwie wuau.adm został dodany do Edytora obiektów zasad grupy. Plik wuau.adm jest instalowany domyślnie w systemie operacyjnym, więc powinien on być już obecny w Edytorze obiektów zasad grupy.

**Aby dodać szablon administracyjny WSUS**
1.  W Edytorze obiektów zasad grupy kliknij dowolny węzeł **Szablony administracyjne**.

2.  W menu **Akcja** kliknij polecenie **Dodaj/Usuń szablony**, a następnie kliknij przycisk **Dodaj**.

3.  W oknie dialogowym **Szablony zasad** kliknij pozycję **wuau.adm**, a następnie kliknij przycisk **Otwórz**.

4.  W oknie dialogowym **Dodawanie/usuwanie szablonów** kliknij przycisk **Zamknij**.

**Aby skonfigurować funkcję Aktualizacje automatyczne**
1.  W Edytorze obiektów zasad grupy rozwiń węzeł **Konfiguracja komputera**, rozwiń węzeł **Szablony administracyjne**, rozwiń węzeł **Składniki systemu Windows**, a następnie kliknij pozycję **Windows Update**.

2.  W okienku szczegółów kliknij dwukrotnie pozycję **Konfigurowanie aktualizacji automatycznych**.

3.  Kliknij pozycję **Włączona**, a następnie kliknij jedną z następujących opcji:

    -   **Powiadom o pobieraniu i powiadom o instalacji**: W przypadku tej opcji zalogowany użytkownik administracyjny jest powiadamiany o zamiarze pobierania i zainstalowania aktualizacji.
    -   **Pobierz automatycznie i powiadom o instalacji**: W przypadku tej opcji pobieranie aktualizacji rozpoczyna się automatycznie, a następnie zalogowany użytkownik administracyjny jest powiadamiany o zamiarze ich zainstalowania.
    -   **Pobierz automatycznie i zaplanuj instalację**: Jeśli funkcja Aktualizacje automatyczne zostanie skonfigurowana pod kątem przeprowadzenia zaplanowanej instalacji, należy również ustawić datę i godzinę instalacji zaplanowanej jako cykliczna.
    -   **Zezwalaj lokalnemu administratorowi na wybranie ustawienia**: W przypadku tej opcji lokalni administratorzy mogą użyć funkcji Aktualizacje automatyczne w Panelu sterowania do wybierania opcji konfiguracji. Na przykład mogą oni wybrać własną planowaną godzinę instalacji. Lokalni administratorzy nie są uprawnieni do wyłączania funkcji Aktualizacje automatyczne.

4.  Kliknij przycisk **OK**.

| ![](images/Cc720532.note(WS.10).gif)Uwaga                                                                                                                           |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Ustawienie **Zezwalaj lokalnemu administratorowi na wybranie ustawienia** pojawia się tylko wtedy, gdy program Aktualizacje automatyczne jest zaktualizowany do wersji zgodnej z programem WSUS. |

**Aby wskazać komputer kliencki serwerowi WSUS**
1.  W Edytorze obiektów zasad grupy rozwiń węzeł **Konfiguracja komputera**, rozwiń węzeł **Szablony administracyjne**, rozwiń węzeł **Składniki systemu Windows**, a następnie kliknij pozycję **Windows Update**.

2.  W okienku szczegółów kliknij dwukrotnie pozycję **Określ lokalizację intranetową usługi aktualizującej firmy Microsoft**.

3.  Kliknij pozycję **Włączona**, a następnie w polach **Ustaw intranetową usługę aktualizacji do wykrywania aktualizacji** oraz **Ustaw serwer statystyk intranetowych** wpisz adres URL tego samego serwera WSUS. Na przykład w obydwu polach wpisz *http://nazwa\_serwera*, a następnie kliknij przycisk **OK**.

| ![](images/Cc720532.note(WS.10).gif)Uwaga                                                                                                                                                                                                                                     |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Jeśli do wskazania tego komputera serwerowi WSUS jest używany lokalny obiekt zasad grupy, to ustawienie zostanie uwzględnione bezzwłocznie, a komputer powinien pojawić się na ekranie konsoli administracyjnej WSUS po krótkim czasie. Ręcznie inicjując cykl wykrywania, możesz przyspieszyć ten proces. |

Po skonfigurowaniu komputera klienckiego i upływie kilku minut pojawi się on na stronie **Komputery** na konsoli WSUS. W przypadku komputerów klienckich skonfigurowanych przy użyciu obiektu zasad grupy opartych na domenie nowe ustawienia dotyczące komputera klienckiego zostaną zastosowane po upływie około 20 minut po odświeżeniu tego obiektu. Domyślnie obiekt zasad grupy jest odświeżany w tle co 90 minut z losowym przesunięciem z przedziału od 0 do 30 minut. Aby szybciej odświeżyć obiekt zasad grupy, można przejść do wiersza polecenia na komputerze klienckim i wpisać polecenie: **gpupdate /force**.

W przypadku komputerów klienckich skonfigurowanych przy użyciu lokalnego obiektu zasad grupy zasady grupy są stosowane natychmiast, a ich wprowadzanie trwa około 20 minut.

Po zastosowaniu zasad grupy można ręcznie zainicjować wykrywanie. Po wykonaniu tego kroku nie trzeba czekać 20 minut na nawiązanie połączenia między komputerem klienckim a programem WSUS.

**Aby ręcznie zainicjować wykrywanie przez serwer WSUS**
1.  Na komputerze klienckim kliknij przycisk **Start**, a następnie kliknij polecenie **Uruchom**.

2.  W polu **Otwórz** wpisz polecenie **cmd**, a następnie kliknij przycisk **OK**.

3.  W wierszu polecenia wpisz **wuauclt.exe /detectnow**. Ta opcja wiersza polecenia instruuje funkcję Aktualizacje automatyczne o konieczności natychmiastowego nawiązania połączenia z serwerem WSUS.
