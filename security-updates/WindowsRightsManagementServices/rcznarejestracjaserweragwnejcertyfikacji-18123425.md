---
TOCTitle: Ręczna rejestracja serwera głównej certyfikacji
Title: Ręczna rejestracja serwera głównej certyfikacji
ms:assetid: 'aecdebb5-b28b-4b58-937a-392bb6ce9643'
ms:contentKeyID: 18123425
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747727(v=WS.10)'
---

Ręczna rejestracja serwera głównej certyfikacji
===============================================

Aby wykonać tę procedurę, należy zalogować się lokalnie w witrynie sieci Web Administracja przy użyciu konta należącego do grupy Administratorzy na komputerze, do którego użytkownik uzyskuje dostęp. Członkowie grupy Administratorzy domeny również mogą wykonać tę procedurę. Ze względu na najważniejsze wskazówki dotyczące bezpieczeństwa należy rozważyć użycie trybu Uruchom jako w celu wykonania tej procedury.

Aby otworzyć stronę sieci Web **Administracja globalna**, należy kliknąć przycisk **Start**, wskazać polecenie **Wszystkie programy**, wskazać polecenie **Windows RMS**, a następnie kliknąć polecenie **Administracja programem Windows RMS**.

W przypadku procesu rejestracji w trybie offline należy dopilnować, aby klienci RMS nie próbowali łączyć się z serwerem programu RMS w celu uzyskania licencji do czasu ukończenia procesu rejestracji. Jeżeli klienci będą próbować łączyć się z niezarejestrowanym serwerem programu RMS, wystąpi błąd usług sieci Web, który uniemożliwi korzystanie z nich. Jeżeli nie można zagwarantować, że klienci nie będą łączyć się z serwerem programu RMS, najlepszym sposobem jest zresetowanie usługi IIS po ukończeniu rejestracji, aby wyczyścić wszystkie utworzone stany błędu.

W przypadku wyboru opcji rejestrowania w trybie offline i korzystania z komputera z konfiguracją zwiększonych zabezpieczeń przeglądarki, na przykład z komputera z systemem Windows Server 2003 lub Windows XP z dodatkiem Service Pack 2, aby połączyć się z Internetem i zażądać certyfikatu licencjodawcy serwera, do strefy Zaufane witryny należy dodać adres URL witryny sieci Web usługi rejestracji w celu umożliwienia pobrania certyfikatu licencjodawcy serwera. Adresem tym jest https://activation.drm.microsoft.com.

W przypadku rejestracji w trybie offline należy sprawdzić, czy na komputerze używanym do wysyłania żądania rejestracji do usługi rejestrowania firmy Microsoft został zainstalowany certyfikat urzędu certyfikacji GTE Cyber Trust Root CA. Ten urząd certyfikacji jest domyślnie zaufanym urzędem certyfikacji na komputerach z systemem Windows Server 2003. W przypadku komputerów z inną wersją systemu Windows można dodać ten urząd certyfikacji do zaufanych, instalując najnowsze aktualizacje certyfikatów z witryny Windows Update.

Ręczna rejestracja serwera głównej certyfikacji
-----------------------------------------------

#### Ręczna rejestracja serwera głównej certyfikacji

1.  Po zainstalowaniu programu RMS na serwerze, który ma być serwerem głównej certyfikacji, otwórz stronę **Administracja globalna**, a następnie obok witryny sieci Web, do której chcesz zaimportować główny certyfikat licencjodawcy serwera, kliknij łącze **Administruj programem RMS w tej witrynie sieci Web**.

2.  W obszarze **Zasoby klastra** kliknij przycisk **Zarejestruj**. Zostanie wyświetlone okno dialogowe **Rejestracja**.

3.  Wybierz opcję **Offline**, a następnie kliknij przycisk **Eksportuj**. Zostanie wyświetlone okno dialogowe **Pobieranie pliku**.

4.  Kliknij przycisk **Zapisz**. Zostanie wyświetlone okno dialogowe **Zapisz jako**.

    > [!note]  
    > W oknie dialogowym **Pobieranie pliku** nie klikaj przycisku **Otwórz**. Jeżeli klikniesz przycisk **Otwórz**, zostanie wyświetlony komunikat o błędzie, a plik żądania rejestracji nie zostanie zapisany. 

5.  Kliknij przycisk **Zapisz**, aby wyeksportować żądanie rejestrowania do pliku. Domyślnie plik zostanie zapisany na pulpicie i nazwany *Nazwa\_serwera*EnrollRequest.xml, gdzie *nazwa\_serwera* zostanie zastąpiona nazwą serwera systemu RMS. Plik można zapisać w innej lokalizacji, wybierając żądaną lokalizację z menu rozwijanego **Zapisz w**. Można także zmienić domyślną nazwę pliku, wpisując nową w polu **Nazwa pliku**.

6.  Po zapisaniu żądania rejestracji pliku zostanie wyświetlone okno dialogowe **Pobieranie ukończone**. Aby wyświetlić kod XML w pliku, można kliknąć przycisk **Otwórz**, jednak nie można wprowadzać żadnych zmian w pliku. Aby otworzyć folder, w którym znajduje się plik, kliknij przycisk **Otwórz folder**. Po zakończeniu przeglądania pliku i sprawdzeniu jego lokalizacji, kliknij przycisk **Zamknij**.

7.  Przenieś plik żądania rejestracji z serwera na komputer z dostępem do Internetu, a następnie przejdź do [witryny sieci Web usługi rejestrowania]()

8.  Wykonaj instrukcje znajdujące się w witrynie sieci Web, aby uzyskać certyfikat licencjodawcy serwera.

9.  Przenieś certyfikat licencjodawcy serwera z powrotem na serwer głównej certyfikacji.

10. W obszarze **Zasoby klastra** kliknij przycisk **Zarejestruj**. Zostanie wyświetlone okno dialogowe **Rejestracja**.

11. W oknie dialogowym **Rejestracja** kliknij przycisk **Przeglądaj** i wskaż pobrany certyfikat licencjodawcy serwera, a następnie kliknij przycisk **Importuj**.

12. Kliknij przycisk **Tak**, aby potwierdzić, że chcesz zaimportować ten certyfikat.

13. W obszarze **Zasoby klastra** zostaną wyświetlone zaktualizowane informacje o certyfikacie licencjodawcy serwera.
