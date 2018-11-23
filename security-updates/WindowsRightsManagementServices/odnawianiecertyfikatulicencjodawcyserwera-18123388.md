---
TOCTitle: Odnawianie certyfikatu licencjodawcy serwera
Title: Odnawianie certyfikatu licencjodawcy serwera
ms:assetid: 'affce9cf-8b46-4293-8e1c-ee06f2ca6537'
ms:contentKeyID: 18123388
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747636(v=WS.10)'
---

Odnawianie certyfikatu licencjodawcy serwera
============================================

Aby wykonać tę procedurę, należy zalogować się lokalnie w administracyjnej witrynie sieci Web przy użyciu konta należącego do grupy Administratorzy na komputerze, do którego użytkownik uzyskuje dostęp. Członkowie grupy Administratorzy domeny również mogą wykonać tę procedurę. Ze względu na najważniejsze wskazówki dotyczące bezpieczeństwa należy rozważyć użycie trybu **Uruchom jako** w celu wykonania tej procedury.

Aby otworzyć stronę sieci Web **Administracja globalna**, należy kliknąć przycisk **Start**, wskazać polecenie **Wszystkie programy**, wskazać polecenie **Windows RMS**, a następnie kliknąć polecenie **Administracja programem Windows RMS**.

W przypadku odnawiania w trybie offline i korzystania z komputera z rozszerzoną konfiguracją zabezpieczeń przeglądarki, na przykład z komputera z systemem Windows Server 2003 lub Windows XP z dodatkiem Service Pack 2, aby połączyć się z Internetem i zażądać certyfikatu licencjodawcy serwera, należy dodać adres URL witryny sieci Web Enrollment Service do strefy Zaufane witryny w celu umożliwienia pobrania certyfikatu licencjodawcy serwera. Adresem tym jest https://activation.drm.microsoft.com.

W przypadku rejestracji w trybie offline należy sprawdzić, czy na komputerze używanym do wysyłania żądania rejestracji do usługi rejestrowania firmy Microsoft został zainstalowany certyfikat urzędu certyfikacji GTE Cyber Trust Root CA. Ten urząd certyfikacji jest domyślnie zaufanym urzędem certyfikacji na komputerach z systemem Windows Server 2003. W przypadku komputerów z inną wersją systemu Windows można dodać ten urząd certyfikacji do zaufanych, instalując najnowsze aktualizacje certyfikatów z witryny Windows Update.

Odnawianie certyfikatu licencjodawcy serwera
--------------------------------------------

#### Odnawianie certyfikatu licencjodawcy serwera

1.  Otwórz stronę **Administracja globalna**, a następnie obok witryny sieci Web, w której chcesz odnowić certyfikat, kliknij łącze **Administruj programem RMS w tej witrynie sieci Web**.

2.  Na stronie **Administracja** w obszarze **Zasoby klastra** kliknij przycisk **Odnów**. Zostanie wyświetlone okno dialogowe Odnów.

3.  Jeżeli serwer jest podłączony do Internetu wybierz opcję **Tryb online** i kliknij przycisk **Odnów**, aby automatycznie odnowić certyfikat licencjodawcy serwera.

4.  Jeżeli serwer nie jest podłączony do Internetu, wybierz opcję **Tryb offline**, a następnie kliknij przycisk **Eksportuj**. Zostanie wyświetlone okno dialogowe **Pobieranie pliku**.

5.  Kliknij przycisk **Zapisz**. Zostanie wyświetlone okno dialogowe **Zapisz jako**.

    > [!note]  
    > W oknie dialogowym **Pobieranie pliku** nie klikaj przycisku **Otwórz**. Jeżeli klikniesz przycisk **Otwórz**, zostanie wyświetlony komunikat o błędzie, a plik żądania rejestracji nie zostanie zapisany. 

6.  Kliknij przycisk **Zapisz**, aby wyeksportować żądanie odnowienia do pliku. Domyślnie plik zostanie zapisany na pulpicie i nazwany *Nazwa\_serwera*RenewalRequest.xml, gdzie *nazwa\_serwera* zostanie zastąpiona nazwą serwera systemu RMS. Plik można zapisać w innej lokalizacji, wybierając żądaną lokalizację z menu rozwijanego Zapisz w. Można także zmienić domyślną nazwę pliku, wpisując nową w polu **Nazwa pliku**.

7.  Po zapisaniu żądania odnowienia pliku zostanie wyświetlone okno dialogowe **Pobieranie ukończone**. Aby wyświetlić kod XML w pliku, można kliknąć przycisk **Otwórz**, jednak nie można wprowadzać żadnych zmian w pliku. Aby otworzyć folder, w którym znajduje się plik, kliknij przycisk **Otwórz folder**. Po zakończeniu przeglądania pliku i sprawdzeniu jego lokalizacji, kliknij przycisk **Zamknij**.

8.  Przenieś plik żądania odnowienia z serwera na komputer z dostępem do Internetu, a następnie przejdź do [witryny sieci Web usługi rejestrowania]() (https://go.microsoft.com/fwlink/?LinkId=25828).

9.  Wykonaj instrukcje znajdujące się w witrynie sieci Web, aby uzyskać certyfikat licencjodawcy serwera.

10. Przenieś certyfikat licencjodawcy serwera z powrotem na serwer głównej certyfikacji.

11. W obszarze **Zasoby klastra** kliknij przycisk **Odnów**. Zostanie wyświetlone okno dialogowe **Odnów**.

12. W oknie dialogowym **Odnów** kliknij przycisk **Przeglądaj** i zlokalizuj pobrany certyfikat licencjodawcy serwera, a następnie kliknij przycisk **Importuj**.

13. Kliknij przycisk **Tak**, aby potwierdzić, że chcesz zaimportować ten certyfikat.

14. Po pomyślnym odnowieniu certyfikatu licencjodawcy serwera obszar **Zasoby klastra** zostanie zaktualizowany i będzie wyświetlana nowa data wygaśnięcia certyfikatu licencjodawcy serwera.

Aby uzyskać więcej informacji dotyczących odnawiania certyfikatów licencjodawcy serwera, zobacz „[Zarządzanie certyfikatami licencjodawcy serwera](https://technet.microsoft.com/549979ad-13ee-4abc-8281-3e002a5a9561)” we wcześniejszej części tego tematu.
