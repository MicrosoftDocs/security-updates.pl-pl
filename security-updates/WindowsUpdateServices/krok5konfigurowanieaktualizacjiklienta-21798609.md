---
TOCTitle: 'Krok 5. Konfigurowanie aktualizacji klienta'
Title: 'Krok 5. Konfigurowanie aktualizacji klienta'
ms:assetid: '5ae60ead-3e94-456c-a692-c0f193ea5d5a'
ms:contentKeyID: 21798609
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Dd939830(v=WS.10)'
---

Krok 5. Konfigurowanie aktualizacji klienta
===========================================

W programie Windows Server Update Services 3.0 z dodatkiem SP2 (WSUS 3.0 z dodatkiem SP2) Instalator programu WSUS automatycznie konfiguruje usługi IIS do rozpowszechniania najnowszej wersji Aktualizacji automatycznych na wszystkich komputerach klienckich nawiązujących połączenia z serwerem WSUS.

Wybór najlepszego sposobu skonfigurowania Aktualizacji automatycznych zależy od używanego środowiska sieciowego. W środowisku, w którym jest używana usługa katalogowa Active Directory®, można użyć istniejącego obiektu zasad grupy (GPO, Group Policy Object) opartego na domenie lub utworzyć nowy obiekt GPO. W środowisku bez usługi Active Directory należy użyć lokalnego obiektu zasad grupy. W tym kroku zostaną skonfigurowane Aktualizacje automatyczne. Następnie komputerom klienckim zostanie wskazany serwer WSUS.

W poniższych procedurach założono, że w sieci działa usługa Active Directory. W tych procedurach założono również, że użytkownik wie, jak korzystać z zasad grupy, oraz używa ich do zarządzania siecią.

Więcej informacji o zasadach grupy można znaleźć w witrynie dotyczącej zasad grupy w witrynie Tech Center w sieci Web [http://go.microsoft.com/fwlink/?LinkID=47375](http://go.microsoft.com/fwlink/?linkid=47375) (strona może zostać wyświetlona w języku angielskim).

Procedury kroku 5
-----------------

W kroku 4 ukończono konfigurację aktualizacji do pobrania. Poniżej przedstawiono zestaw procedur konfigurowania aktualizacji automatycznych dla komputerów klienckich.

1.  Konfigurowanie Aktualizacji automatycznych w zasadach grupy
2.  Wskazywanie serwera WSUS komputerowi klienckiemu
3.  Ręczne inicjowanie wykrywania przez serwer WSUS

Dwie pierwsze procedury należy wykonać w wybranym obiekcie zasad grupy opartym na domenie, a trzecią procedurę w wierszu polecenia na komputerze klienckim.

**Aby skonfigurować funkcję Aktualizacje automatyczne**
1.  W konsoli zarządzania zasadami grupy przejdź do obiektu zasad grupy, w którym chcesz skonfigurować program WSUS, a następnie kliknij przycisk **Edytuj**.

2.  W konsoli zarządzania zasadami grupy rozwiń węzeł **Konfiguracja komputera**, rozwiń węzeł **Szablony administracyjne**, rozwiń węzeł **Składniki systemu Windows**, a następnie kliknij pozycję **Windows Update**.

3.  W okienku szczegółów kliknij dwukrotnie pozycję **Konfigurowanie aktualizacji automatycznych**.

4.  Kliknij pozycję **Włączona**, a następnie kliknij jedną z następujących opcji:

    -   **Powiadom o pobieraniu i powiadom o instalacji**. Ta opcja służy do powiadamiania zalogowanego użytkownika administracyjnego przed pobraniem i przed zainstalowaniem aktualizacji.
    -   **Pobierz automatycznie i powiadom o instalacji**. W przypadku tej opcji pobieranie aktualizacji rozpoczyna się automatycznie, a następnie zalogowany użytkownik administracyjny jest powiadamiany o zamiarze ich zainstalowania.
    -   **Pobierz automatycznie i zaplanuj instalację**. W przypadku tej opcji aktualizacje są pobierane automatycznie, po czym są instalowane w określonym dniu i o określonej godzinie.
    -   **Zezwalaj lokalnemu administratorowi na wybranie ustawienia**. W przypadku tej opcji administratorzy lokalni mogą wybierać opcje konfiguracji za pomocą apletu Aktualizacje automatyczne w Panelu sterowania. Na przykład mogą oni wybrać własną planowaną godzinę instalacji. Administratorzy lokalni nie mogą wyłączać Aktualizacji automatycznych.

5.  Kliknij przycisk **OK**.

**Aby wskazać serwer WSUS komputerom klienckim**
1.  W okienku szczegółów **Windows Update** kliknij dwukrotnie pozycję **Określ lokalizację intranetowej usługi aktualizującej firmy Microsoft**.

2.  Kliknij pozycję **Włączona**, a następnie w polach **Ustaw intranetową usługę aktualizacji do wykrywania aktualizacji** oraz **Ustaw serwer statystyk intranetowych** wpisz adres URL tego samego serwera WSUS. Na przykład w obydwu polach wpisz *http://nazwa\_serwera*, a następnie kliknij przycisk **OK**.
 
> [!note]  
> Jeśli do wskazywania komputerowi serwera WSUS jest używany lokalny obiekt zasad grupy, to ustawienie jest stosowane natychmiast i wkrótce nazwa tego komputera jest wyświetlana w konsoli administracyjnej programu WSUS. Ręcznie inicjując cykl wykrywania, możesz przyspieszyć ten proces. 

Po skonfigurowaniu komputera klienckiego i upływie kilku minut jego nazwa zostanie wyświetlona na stronie **Komputery** w konsoli administracyjnej programu WSUS. W przypadku komputerów klienckich skonfigurowanych przy użyciu zasad grupy opartych na domenie odświeżenie zasad grupy (czyli zastosowanie nowych ustawień zasad do komputera klienckiego) może potrwać około 20 minut. Domyślnie zasady grupy są aktualizowane w tle co 90 minut z losowym przesunięciem od 0 do 30 minut. Aby szybciej zaktualizować zasady grupy, można przejść do wiersza polecenia na komputerze klienckim i wpisać polecenie **gpupdate /force**.

W przypadku komputerów klienckich skonfigurowanych za pomocą lokalnego obiektu zasad grupy zasady grupy są stosowane natychmiast, a aktualizowanie trwa około 20 minut.

W przypadku ręcznego zainicjowania wykrywania nie trzeba czekać 20 minut na nawiązanie przez komputer kliencki połączenia z programem WSUS.

**Aby ręcznie zainicjować wykrywanie przez serwer WSUS**
1.  Na komputerze klienckim kliknij przycisk **Start**, a następnie kliknij polecenie **Uruchom**.

2.  W polu **Otwórz** wpisz polecenie **cmd**, a następnie kliknij przycisk **OK**.

3.  W wierszu polecenia wpisz polecenie **wuauclt.exe /detectnow**. Ta opcja wiersza polecenia instruuje funkcję Aktualizacje automatyczne o konieczności natychmiastowego nawiązania połączenia z serwerem WSUS.

Następny krok
-------------

[Krok 6. Konfigurowanie grup komputerów](https://technet.microsoft.com/70518732-2179-4e41-9609-7f9999867f41)

Materiały dodatkowe
-------------------

[Program Windows Server Update Services 3.0 z dodatkiem SP2 — przewodnik krok po kroku](https://technet.microsoft.com/4b504edc-93b3-45b0-a7e8-d0107f1a4442)
