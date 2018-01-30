---
TOCTitle: Dodawanie zaufanej domeny użytkownika
Title: Dodawanie zaufanej domeny użytkownika
ms:assetid: 'ed672e58-6272-4ac0-a434-d1d938037e93'
ms:contentKeyID: 18123510
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747793(v=WS.10)'
---

Dodawanie zaufanej domeny użytkownika
=====================================

Aby wykonać tę procedurę, należy zalogować się lokalnie w administracyjnej witrynie sieci Web przy użyciu konta należącego do grupy Administratorzy na komputerze, do którego użytkownik uzyskuje dostęp. Członkowie grupy Administratorzy domeny również mogą wykonać tę procedurę. Ze względu na najważniejsze wskazówki dotyczące bezpieczeństwa należy rozważyć użycie trybu **Uruchom jako** w celu wykonania tej procedury.

Aby otworzyć stronę sieci Web **Administracja globalna**, należy kliknąć przycisk **Start**, wskazać polecenie **Wszystkie programy**, wskazać polecenie **Windows RMS**, a następnie kliknąć polecenie **Administracja programem Windows RMS**.

Dodawanie zaufanej domeny użytkownika
-------------------------------------

#### Dodawanie zaufanej domeny użytkownika

1.  Otwórz stronę **Administracja globalna**, a następnie obok witryny sieci Web, do której chcesz dodać zaufaną domenę użytkowników, kliknij łącze **Administruj programem RMS w tej witrynie sieci Web**.

2.  W obszarze **Łącza administracyjne** kliknij łącze **Zasady zaufania**.

3.  W obszarze **Zaufane domeny użytkowników** kliknij przycisk **Przeglądaj**, zlokalizuj i kliknij dwukrotnie certyfikat licencjodawcy serwera odpowiadający domenie użytkowników, którą chcesz zaimportować w celu ustanowienia relacji zaufania, a następnie kliknij przycisk **Dodaj**.

    Nazwa domeny zostanie wyświetlona na liście **Zaufane domeny użytkowników**.

4.  Aby określić, które domeny e-mail w obrębie zaufanej domeny użytkowników są zaufane, kliknij opcję **Zaufane domeny** obok nazwy certyfikatu na liście, aby otworzyć okno **Zaufane domeny e-mail**.

5.  Wybierz jedną z następujących opcji zaufania:

    -   Wybierz opcję **Ufaj wszystkim domenom e-mail**, aby ufać wszystkim kontom użytkowników będących członkami domeny.
        — lub —
    -   Wybierz opcję **Ufaj tylko określonym domenom e-mail**, wpisz nazwę domeny, której ma dotyczyć zaufanie (np. przyklad.com), a następnie kliknij przycisk **Dodaj**. Spowoduje to dodanie domeny do listy Zaufane domeny e-mail. Aby usunąć nazwę z tej listy, zaznacz nazwę, a następnie kliknij przycisk **Usuń**. Umieszczenie domeny na liście obejmuje jej wszystkie poddomeny.

6.  Jeśli program RMS jest używany w środowisku, w którym należy rozszerzać członkostwo w grupach na wiele lasów, zaznacz pole wyboru **Ufaj licencjonowaniu RM do identyfikatorów zabezpieczeń (SID) dla tej domeny użytkownika**.

7.  Po zakończeniu kliknij łącze **Zamknij okno i wróć do części dotyczącej zasad zaufania**.

Aby uzyskać więcej informacji dotyczących wykonywania tej procedury, zobacz „[Dodawanie i usuwanie zaufanych domen użytkowników](https://technet.microsoft.com/7c440b15-01c4-49f1-b43c-00f67f3388c1)” we wcześniejszej części tego tematu.
