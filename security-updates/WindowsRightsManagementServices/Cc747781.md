---
TOCTitle: Określanie lokalizacji szablonów zasad praw dostępu
Title: Określanie lokalizacji szablonów zasad praw dostępu
ms:assetid: 'e1bee46d-33db-424f-ba45-1dcedcb883ab'
ms:contentKeyID: 18123487
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747781(v=WS.10)'
---

Określanie lokalizacji szablonów zasad praw dostępu
===================================================

Aby wykonać tę procedurę, należy zalogować się lokalnie w administracyjnej witrynie sieci Web przy użyciu konta należącego do grupy Administratorzy na komputerze, do którego użytkownik uzyskuje dostęp. Członkowie grupy Administratorzy domeny również mogą wykonać tę procedurę. Ze względu na najważniejsze wskazówki dotyczące bezpieczeństwa należy rozważyć użycie trybu **Uruchom jako** w celu wykonania tej procedury.

Aby otworzyć stronę sieci Web **Administracja globalna**, należy kliknąć przycisk **Start**, wskazać polecenie **Wszystkie programy**, wskazać polecenie **Windows RMS**, a następnie kliknąć polecenie **Administracja programem Windows RMS**.

Jeśli szablony zasad praw dostępu są przechowywane w folderze udostępnionym, którego lokalizacja zostanie następnie zmieniona, należy ręcznie skopiować szablony zasad praw dostępu z poprzedniej lokalizacji do nowej.

Szablony zasad praw dostępu są również przechowywane w bazie danych konfiguracji. Aby uzyskać więcej informacji dotyczących rozpowszechniania szablonów zasad praw dostępu, zobacz „[Rozpowszechnianie szablonów zasad praw dostępu](https://technet.microsoft.com/ae6fa26f-d744-4ac9-9eb1-728ffab87bfe)” we wcześniejszej części tego tematu.

Jeśli jako aplikacja obsługująca technologię RMS wykorzystywana jest aplikacja pakietu Microsoft Office 2003, lokalizacja szablonów zasad praw dostępu jest określona kluczem rejestru `AdminTemplatePath`, a klient RMS będzie ich poszukiwał właśnie w takiej lokalizacji.

Określanie lokalizacji szablonów zasad praw dostępu
---------------------------------------------------

#### Określanie lokalizacji szablonów zasad praw dostępu

1.  Otwórz stronę **Administracja globalna**, a następnie obok witryny sieci Web, w której chcesz określić lokalizację szablonów zasad praw dostępu, kliknij łącze **Administruj programem RMS w tej witrynie sieci Web**.

2.  W obszarze **Łącza administracyjne** kliknij łącze **Szablony zasad praw dostępu**.

3.  W obszarze **Lokalizacja szablonu** określ nazwę UNC (Universal Naming Convention) udostępnionego folderu (w formie \\\\*nazwa\_serwera*\\*nazwa\_udziału*), w którym będą przechowywane szablony zasad praw dostępu dla tego klastra. Konto, na którym jest uruchamiana pula aplikacji administracyjnych (**Admin**), musi mieć uprawnienia do zapisu w tym udostępnionym folderze. Należy upewnić się, że szablony są przechowywane w dostępnej lokalizacji sieciowej spełniającej wymagania dotyczące bezpieczeństwa obowiązujące w organizacji. Udostępnionych folderów szablonów nie należy tworzyć w podstawowych folderach używanych przez program RMS, takich jak folder Program Files lub foldery IISRoot.

4.  Kliknij przycisk **Zapisz**.

5.  Po utworzeniu szablonów zasad praw dostępu i zapisaniu ich w tej lokalizacji należy udostępnić je użytkownikom. Domyślnie klient technologii RMS będzie wyszukiwać szablony zasad praw dostępu w następującej lokalizacji na komputerze lokalnym:

    %HOMEPATH%\\Ustawienia lokalne\\Dane aplikacji\\Microsoft\\DRM\\templates

    Szablony zasad praw dostępu należy skopiować do tej lokalizacji z lokalizacji określonej w kroku 3, aby były dostępne dla wszystkich użytkowników w organizacji korzystających z technologii RMS.
