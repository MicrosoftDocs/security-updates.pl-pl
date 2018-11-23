---
TOCTitle: Wykluczanie aplikacji
Title: Wykluczanie aplikacji
ms:assetid: '422f2ddd-bcf4-45f1-905a-b8bad30fd7dd'
ms:contentKeyID: 18123245
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720262(v=WS.10)'
---

Wykluczanie aplikacji
=====================

Aby wykonać tę procedurę, należy zalogować się lokalnie w administracyjnej witrynie sieci Web przy użyciu konta należącego do grupy Administratorzy na komputerze, do którego użytkownik uzyskuje dostęp. Członkowie grupy Administratorzy domeny również mogą wykonać tę procedurę. Ze względu na najważniejsze wskazówki dotyczące bezpieczeństwa należy rozważyć użycie trybu **Uruchom jako** w celu wykonania tej procedury.

Aby otworzyć stronę sieci Web **Administracja globalna**, należy kliknąć przycisk **Start**, wskazać polecenie **Wszystkie programy**, wskazać polecenie **Windows RMS**, a następnie kliknąć polecenie **Administracja programem Windows RMS**.

Zasady wykluczamoa są wymuszane przez klienta, gdy licencja użytkowania jest ograniczona do chronionej zawartości.

Wykluczanie aplikacji lub zatrzymywanie wykluczania aplikacji
-------------------------------------------------------------

#### Wykluczanie aplikacji

1.  Otwórz stronę **Administracja globalna**, a następnie obok witryny sieci Web, w której chcesz kontrolować, które wersje aplikacji mogą być używane z zawartością chronioną technologią praw dostępu, kliknij łącze **Administruj programem RMS w tej witrynie sieci Web**.

2.  W obszarze **Łączaadministracyjne** kliknij łącze **Zasady wykluczania**.

3.  W obszarze **Wykluczanie aplikacji** kliknij przycisk **Włącz**, aby wykluczyć aplikację lub składnik obsługujący technologię RMS.

    Aby wyłączyć wykluczanie aplikacji, należy kliknąć przycisk **Wyłącz**.

4.  Wpisz nazwę pliku aplikacji lub składnika, która ma zostać wykluczona, wpisz najniższą i najwyższą wersję, które mają zostać wykluczone (w formacie *x*.*x*.*x*.*x*), a następnie kliknij przycisk **Wyklucz tę aplikację**.

    Aby usunąć aplikację lub składnik z listy wykluczania, zaznacz nazwę pliku, a następnie kliknij opcję **Usuń zaznaczone aplikacje z listy wykluczania**.

    > [!note]  
    > Program RMS wymaga określenia wersji aplikacji w formacie 4-cyfrowym z separatorem w postaci kropki (\#.\#.\#.\# ). Jednak oznaczenia wersji niektórych aplikacji składają się z 2 lub 3 cyfr rozdzielonych kropkami. W takim przypadku należy odpowiednio dopisać .0, aby format numeru wersji był zgodny z formatem wymaganym przez program RMS. 

#### Zatrzymywanie wykluczania aplikacji

1.  Otwórz stronę **Administracja globalna**, a następnie obok witryny sieci Web, w której chcesz kontrolować, które wersje aplikacji mogą być używane z zawartością chronioną technologią praw dostępu, kliknij łącze **Administruj programem RMS w tej witrynie sieci Web**.

2.  W obszarze **Łączaadministracyjne** kliknij łącze **Zasady wykluczania**.

3.  W obszarze **Wykluczanie aplikacji** kliknij opcję **Wyłącz**.

Aby uzyskać więcej informacji dotyczących wykonywania tej procedury, zobacz „[Wykluczanie aplikacji](https://technet.microsoft.com/b68ae4b2-b9ba-44ae-90cb-c88df600ec86)” we wcześniejszej części tego tematu.
