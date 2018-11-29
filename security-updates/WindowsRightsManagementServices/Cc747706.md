---
TOCTitle: Usuwanie zastrzeżenia programu RMS
Title: Usuwanie zastrzeżenia programu RMS
ms:assetid: '9fa63daa-5fb9-4afd-8371-b38248619857'
ms:contentKeyID: 18123404
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747706(v=WS.10)'
---

Usuwanie zastrzeżenia programu RMS
==================================

Aby wykonać tę procedurę, należy zalogować się lokalnie w administracyjnej witrynie sieci Web przy użyciu konta należącego do grupy Administratorzy na komputerze, do którego użytkownik uzyskuje dostęp. Członkowie grupy Administratorzy domeny również mogą wykonać tę procedurę. Ze względu na najważniejsze wskazówki dotyczące bezpieczeństwa należy rozważyć użycie trybu **Uruchom jako** w celu wykonania tej procedury.

Aby otworzyć stronę sieci Web **Administracja globalna**, należy kliknąć przycisk **Start**, wskazać polecenie **Wszystkie programy**, wskazać polecenie **Windows RMS**, a następnie kliknąć polecenie **Administracja programem Windows RMS**.

Gdy usuwane jest zastrzeżenie serwera, serwer jest usuwany z tabeli ClusterServer w bazie danych konfiguracji. Gdy usuwane jest zastrzeżenie ostatniego serwera w klastrze, baza danych usług katalogowych jest usuwana z serwera SQL Server. Przy usuwaniu zastrzeżenia ostatniego serwera głównej certyfikacji w klastrze należy ręcznie wyrejestrować punkt połączenia usługi certyfikacji (SCP). Usuniecie zastrzeżenia i odinstalowanie nie spowoduje usunięcia punktu SCP z usługi Active Directory.

W przypadku odinstalowywania serwera głównej certyfikacji przed jego zastrzeżeniem zostanie wyświetlone ostrzeżenie informujące, że nie usunięto jeszcze zastrzeżenia witryny i że punkt połączenia usługi nie zostanie usunięty z usługi Active Directory. Jeśli jednak użytkownik wybierze opcję **Tak** w celu kontynuacji, zastrzeżenie witryny zostanie usunięte. Proces odinstalowywania nie spowoduje usunięcia punktu połączenia usługi z usługi Active Directory.

Usuwanie zastrzeżenia programu RMS
----------------------------------

#### Usuwanie zastrzeżenia programu RMS

1.  Zaloguj się na serwerze, na którym chcesz usunąć zastrzeżenie programu RMS.

2.  Otwórz stronę **Administracja globalna**.

3.  Obok witryny sieci Web, w której zastrzeżono program RMS, kliknij opcję **Usuń program RMS z tej witryny sieci Web**, a następnie kliknij przycisk **OK**.

4.  Na stronie sieci Web punktu połączenia usługi kliknij przycisk **Wyrejestruj URL**, aby wyrejestrować połączenie usługi certyfikacji z usługi Active Directory.
