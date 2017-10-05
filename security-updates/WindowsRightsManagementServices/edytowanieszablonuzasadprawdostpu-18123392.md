---
TOCTitle: Edytowanie szablonu zasad praw dostępu
Title: Edytowanie szablonu zasad praw dostępu
ms:assetid: '9580b934-bd6f-4097-9d3c-4fc14a3147fa'
ms:contentKeyID: 18123392
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747684(v=WS.10)'
---

Edytowanie szablonu zasad praw dostępu
======================================

Aby wykonać tę procedurę, należy zalogować się lokalnie w administracyjnej witrynie sieci Web przy użyciu konta należącego do grupy Administratorzy na komputerze, do którego użytkownik uzyskuje dostęp. Członkowie grupy Administratorzy domeny również mogą wykonać tę procedurę. Ze względu na najważniejsze wskazówki dotyczące bezpieczeństwa należy rozważyć użycie trybu **Uruchom jako** w celu wykonania tej procedury.

Aby otworzyć stronę sieci Web **Administracja globalna**, należy kliknąć przycisk **Start**, wskazać polecenie **Wszystkie programy**, wskazać polecenie **Windows RMS**, a następnie kliknąć polecenie **Administracja programem Windows RMS**.

Edytowanie szablonu zasad praw dostępu
--------------------------------------

#### Edytowanie szablonu zasad praw dostępu

1.  Otwórz stronę **Administracja globalna**, a następnie obok witryny sieci Web, w której chcesz edytować szablon zasad praw dostępu, kliknij łącze **Administruj programem RMS w tej witrynie sieci Web**.

2.  W obszarze **Łącza administracyjne** kliknij łącze **Szablony zasad praw dostępu**.

3.  W obszarze **Nazwa szablonu** kliknij nazwę szablonu, który ma być edytowany.

4.  W obszarze **Identyfikacja szablonu** zmodyfikuj informacje w obszarach **Nazwa szablonu**, **Opis szablonu** i **Adres URL żądania praw**.

5.  W obszarze **Użytkownicy i grupy** wykonaj jedną lub kilka następujących czynności:

    -   Aby dodać użytkownika lub grupę, w polu **Dodaj użytkowników lub grupy** wpisz prawidłowy adres e-mail określonego użytkownika lub grupy, która ma zostać dodana, kliknij przycisk **Dodaj**, a następnie na liście **Bieżący użytkownicy lub grupy** wybierz odpowiednią nazwę. W obszarze **Prawa** zaznacz wszystkie prawa, które mają zostać udzielone wybranemu użytkownikowi lub grupie.
    -   Aby zmodyfikować prawa istniejącego użytkownika lub grupy, wybierz odpowiednią nazwę na liście **Bieżący użytkownicy lub grupy**, a następnie zaznacz lub wyczyść odpowiednie pola wyboru.
    -   Aby usunąć użytkownika lub grupę, wybierz odpowiednią nazwę na liście **Bieżący użytkownicy lub grupy**, a następnie kliknij przycisk **Usuń**.

6.  W obszarze **Zasady wygasania** edytuj odpowiednio informacje, aby zmienić datę wygaśnięcia licencji zawartości lub datę odnowienia licencji.

7.  W obszarze **Zasady rozszerzone** edytuj odpowiednio informacje, aby zmienić sposób implementowania licencji zawartości (w tym trwałość praw autorskich), określić, czy są obsługiwane zaufane przeglądarki, określić trwałość licencji w obrębie zawartości lub wymusić dane charakterystyczne dla aplikacji.

8.  W obszarze **Zasady odwołania** określ, czy lista odwołania będzie wymagana dla zawartości utworzonej przy użyciu tego szablonu. Jeśli zostanie wybrana opcja **Wymagane odwołanie**, wypełnij odpowiednio następujące ustawienia:

    -   W polu **Adres URL** wpisz adres URL lokalizacji, w której opublikowany jest plik z listą odwołania. Jeśli konieczna jest obsługa odłączonych użytkowników lub użytkowników zewnętrznych, ten adres URL powinien być dostępny w sieci Internet i w sieci korporacyjnej. Aby uzyskać więcej informacji, zobacz „[Implementowanie odwołania](https://technet.microsoft.com/4735f060-7197-4ae2-830a-f91bcc4de30a)” we wcześniejszej części tego tematu.
    -   W polu **Interwał odświeżania listy odwołania** wpisz liczbę dni ważności listy odwołania. Jeśli użytkownik ma kopię listy odwołania starszą niż dopuszczalna, pobranie zawartości, wymaga uzyskania zaktualizowanej listy odwołania.
    -   W polu **Plik klucza publicznego** wpisz ścieżkę i nazwę pliku klucza publicznego dla tej listy odwołania. Aby uzyskać więcej informacji dotyczących tego pliku, zobacz „Wstawianie podpisu do listy odwołania” we wcześniejszej części tego tematu.

    | ![](images/Cc747684.Caution(WS.10).gif)Przestroga                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
    |--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Podczas implementowania odwołania należy zachować ostrożność. Na podstawie określonego interwału odświeżania należy okresowo odnawiać listę odwołania, ponieważ w przeciwnym przypadku wygaśnie ona automatycznie, co uniemożliwi użytkownikom pobieranie zawartości wymagającej użycia tej listy. Aby zapewnić, że nie nastąpi przypadkowe uniemożliwienie użytkownikom pobierania zawartości, należy dokładnie oszacować interwał wymagany do odświeżania listy odwołania. Aby uzyskać więcej informacji, zobacz „[Zarządzanie odwołaniem](https://technet.microsoft.com/df732a7d-1fb0-4845-87ca-fab4bc5f98a0)” we wcześniejszej części tego tematu. |

9.  Kliknij przycisk **Wyślij**. 

Aby uzyskać więcej informacji dotyczących wykonywania tej procedury, zobacz „[Tworzenie i modyfikowanie szablonów zasad praw dostępu](https://technet.microsoft.com/6014176f-ef71-4d29-b3e3-da129c18563d)” we wcześniejszej części tego tematu.
