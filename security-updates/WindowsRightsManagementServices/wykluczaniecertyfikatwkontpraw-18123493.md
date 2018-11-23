---
TOCTitle: Wykluczanie certyfikatów kont praw
Title: Wykluczanie certyfikatów kont praw
ms:assetid: 'e5cd9dec-ac29-437e-8515-dc697ec75edf'
ms:contentKeyID: 18123493
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747785(v=WS.10)'
---

Wykluczanie certyfikatów kont praw
==================================

Aby wykonać tę procedurę, należy zalogować się lokalnie w administracyjnej witrynie sieci Web przy użyciu konta należącego do grupy Administratorzy na komputerze, do którego użytkownik uzyskuje dostęp. Członkowie grupy Administratorzy domeny również mogą wykonać tę procedurę. Ze względu na najważniejsze wskazówki dotyczące bezpieczeństwa należy rozważyć użycie trybu **Uruchom jako** w celu wykonania tej procedury.

Aby otworzyć stronę sieci Web **Administracja globalna**, należy kliknąć przycisk **Start**, wskazać polecenie **Wszystkie programy**, wskazać polecenie **Windows RMS**, a następnie kliknąć polecenie **Administracja programem Windows RMS**.

Te warunki są wymuszane przez klienta, gdy licencja użytkowania jest ograniczona do chronionej zawartości.

Wykluczanie certyfikatów kont praw
----------------------------------

#### Wykluczanie certyfikatów kont praw

1.  Otwórz stronę **Administracja globalna**, a następnie obok witryny sieci Web, w której chcesz wykluczyć certyfikaty kont praw, kliknij łącze **Administruj programem RMS w tej witrynie sieci Web**.

2.  W obszarze **Łącza administracyjne** kliknij łącze **Zasady wykluczania**.

3.  W obszarze wykluczania certyfikatu konta praw kliknij przycisk **Włącz**, aby wykluczyć certyfikat konta praw użytkownika.

4.  Wybierz metodę określania certyfikatów kont do wykluczenia:

    -   Aby wykluczyć certyfikat konta według nazwy użytkownika, kliknij opcję **Nazwa użytkownika** certyfikatu konta praw, który ma zostać wykluczony, wpisz nazwę użytkownika, który ma być wykluczony (w formie *nazwa\_użytkownika*@*nazwa\_domeny*.com), a następnie kliknij przycisk **Dodaj**. Tej opcji należy użyć, aby wykluczyć certyfikaty kont użytkowników wewnętrznych, którzy mają konta użytkowników usługi Active Directory.
    -   Aby wykluczyć certyfikat konta według jego klucza publicznego, kliknij opcję **Ciąg klucza publicznego** dla certyfikatu konta praw, który ma zostać wykluczony, wpisz odpowiedni ciąg klucza publicznego certyfikatu konta praw, a następnie kliknij przycisk **Dodaj**. Tej opcji należy użyć, aby wykluczyć certyfikaty kont użytkowników zewnętrznych, którzy nie mają kont użytkowników usługi Active Directory.

    > [!note]  
    > Aby usunąć certyfikat konta z listy wykluczania, należy kliknąć na liście wykluczony certyfikat konta praw, a następnie kliknąć opcję **Usuń wybrane klucze publiczne z listy wykluczania**. Użytkownik mający taki charakterystyczny certyfikat konta będzie mógł od tej chwili uzyskiwać licencje zawartości chronionej technologią RMS z tego serwera. 

    > [!note]  
    > Aby wyłączyć wykluczanie certyfikatów kont praw, należy kliknąć przycisk **Wyłącz**. 

Aby uzyskać więcej informacji dotyczących wykonywania tej procedury, zobacz „[Wykluczanie certyfikatów kont praw](https://technet.microsoft.com/cba5e901-942c-4d06-9865-e6c4648c95e6)” we wcześniejszej części tego tematu.
