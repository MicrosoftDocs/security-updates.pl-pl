---
TOCTitle: Dodawanie szablonu zasad praw dostępu
Title: Dodawanie szablonu zasad praw dostępu
ms:assetid: '1a5555cd-6d39-4078-a879-4106864674be'
ms:contentKeyID: 18123191
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720206(v=WS.10)'
---

Dodawanie szablonu zasad praw dostępu
=====================================

Aby wykonać tę procedurę, należy zalogować się lokalnie w administracyjnej witrynie sieci Web przy użyciu konta należącego do grupy Administratorzy na komputerze, do którego użytkownik uzyskuje dostęp. Członkowie grupy Administratorzy domeny również mogą wykonać tę procedurę. Ze względu na najważniejsze wskazówki dotyczące bezpieczeństwa należy rozważyć użycie trybu **Uruchom jako** w celu wykonania tej procedury.

Aby otworzyć stronę sieci Web **Administracja globalna**, należy kliknąć przycisk **Start**, wskazać polecenie **Wszystkie programy**, wskazać polecenie **Windows RMS**, a następnie kliknąć polecenie **Administracja programem Windows RMS**.

Dodawanie szablonu zasad praw dostępu
-------------------------------------

#### Dodawanie szablonu zasad praw dostępu

1.  Otwórz stronę **Administracja globalna**, a następnie obok witryny sieci Web, do której chcesz dodać szablon zasad praw dostępu, kliknij łącze **Administruj programem RMS w tej witrynie sieci Web**.

2.  W obszarze **Łącza administracyjne** kliknij łącze **Szablony zasad praw dostępu**.

3.  W obszarze **Język** kliknij, aby wybrać język szablonu.

4.  Kliknij opcję **Dodaj szablon zasad praw dostępu**.

5.  W obszarze **Identyfikacja szablonu** określ nazwę, opis i adres URL żądania praw dla tego szablonu.

6.  W obszarze **Użytkownicy i grupy** w polu **Dodaj użytkowników lub grupy** wpisz prawidłowy adres e-mail użytkownika lub grupy, które ma zostać dodana, a następnie kliknij przycisk **Dodaj**. Powtórz tę czynność, jeśli konieczne jest dodanie kolejnych użytkowników lub grup.

7.  Na liście **Bieżący użytkownicy lub grupy** zaznacz adres e-mail użytkownika lub grupy, do której zostaną przypisane prawa.

8.  Zaznacz pola wyboru obok wszystkich praw, które mają zostać udzielone wybranemu użytkownikowi lub grupie. Powtórz te czynności, aby udzielić uprawnień pozostałym użytkownikom i grupom.

9.  W obszarze **Zasady wygasania** wybierz jedną z trzech opcji wygasania, a następnie określ odpowiednio datę lub godzinę wygaśnięcia. W razie potrzeby zaznacz opcję **Licencje użytkowania dla zawartości muszą być odnawiane co** i określ liczbę dni, po upływie której nastąpi odnowienie.

10. W obszarze **Zasady rozszerzone** zaznacz jedną lub więcej spośród czterech dostępnych opcji. Jeśli zostanie wybrana opcja **Wymuszaj dane charakterystyczne dla aplikacji**, określ nazwę i wartość danych, które będą wymuszane, a następnie kliknij przycisk **Dodaj**.

11. Aby zaimplementować odwołanie, w obszarze **Zasady odwołania** zaznacz pole wyboru **Wymagane odwołanie**, a następnie wykonaj następujące czynności:

    1.  W polu **Adres URL lub UNC** wpisz adres URL lokalizacji, w której opublikowany jest plik z listą odwołania. Jeśli konieczna jest obsługa odłączonych użytkowników lub użytkowników zewnętrznych, ten adres URL powinien być dostępny w sieci Internet i w sieci korporacyjnej.
    2.  W polu **Interwał odświeżania listy odwołania** wpisz liczbę dni ważności listy odwołania. Jeśli użytkownik ma kopię listy odwołania starszą niż dopuszczalna, pobranie zawartości, wymaga uzyskania zaktualizowanej listy odwołania.
    3.  W polu **Plik klucza publicznego** wpisz ścieżkę i nazwę pliku lub kliknij przycisk **Przeglądaj**, aby zlokalizować plik klucza publicznego dla tej listy odwołania. Aby uzyskać więcej informacji dotyczących tego pliku, zobacz „Wstawianie podpisu do listy odwołania” we wcześniejszej części tego tematu.

    > [!Caution]  
    > Podczas implementowania odwołania należy zachować ostrożność. Na podstawie określonego interwału odświeżania należy okresowo odnawiać listę odwołania, ponieważ w przeciwnym przypadku wygaśnie ona automatycznie, co uniemożliwi użytkownikom pobieranie zawartości wymagającej użycia tej listy. Aby zapewnić, że nie nastąpi przypadkowe uniemożliwienie użytkownikom pobierania zawartości, należy dokładnie oszacować interwał wymagany do odświeżania listy odwołania. Aby uzyskać więcej informacji, zobacz „[Zarządzanie odwołaniem](https://technet.microsoft.com/df732a7d-1fb0-4845-87ca-fab4bc5f98a0)” we wcześniejszej części tego tematu. 

12. Kliknij przycisk **Wyślij**. 

Aby uzyskać więcej informacji dotyczących odwoływania, zobacz „[Zarządzanie odwołaniem](https://technet.microsoft.com/df732a7d-1fb0-4845-87ca-fab4bc5f98a0)” we wcześniejszej części tego tematu.

Aby uzyskać informacje dotyczące określania opcji odwołania, zobacz „[Definiowanie zasad odwołania](https://technet.microsoft.com/e2fffe9f-def7-439b-a8aa-43f8a065813d)” we wcześniejszej części tego tematu.

Aby uzyskać więcej informacji dotyczących wykonywania tej procedury, zobacz „[Tworzenie i modyfikowanie szablonów zasad praw dostępu](https://technet.microsoft.com/6014176f-ef71-4d29-b3e3-da129c18563d)” we wcześniejszej części tego tematu.
