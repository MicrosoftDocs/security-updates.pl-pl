---
TOCTitle: Zmienianie ustawień serwera proxy programu RMS
Title: Zmienianie ustawień serwera proxy programu RMS
ms:assetid: '8f50bd4d-26b1-4996-b361-722ee21607f3'
ms:contentKeyID: 18123340
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747594(v=WS.10)'
---

Zmienianie ustawień serwera proxy programu RMS
==============================================

Aby wykonać tę procedurę, należy zalogować się lokalnie w administracyjnej witrynie sieci Web przy użyciu konta należącego do grupy Administratorzy na komputerze, do którego użytkownik uzyskuje dostęp. Członkowie grupy Administratorzy domeny również mogą wykonać tę procedurę. Ze względu na najważniejsze wskazówki dotyczące bezpieczeństwa należy rozważyć użycie trybu **Uruchom jako** w celu wykonania tej procedury.

Więcej informacji na temat metod uwierzytelniania serwera proxy oraz sposobów ich działania w systemie Windows Server 2003 można znaleźć w Pomocy programu Internetowe usługi informacyjne.

Zmienianie ustawień serwera proxy programu RMS
----------------------------------------------

#### Zmienianie ustawień serwera proxy programu RMS

1.  Otwórz stronę **Administracja globalna**, a następnie kliknij łącze **Administruj programem RMS w tej witrynie sieci Web**.

2.  W obszarze **Administrowanie klastrem** kliknij pozycję **Ustawienia zabezpieczeń**.

3.  Jeśli wcześniej z programem RMS nie był stosowany serwer proxy, zaznacz pole wyboru **Ten komputer używa serwera proxy do łączenia się z Internetem**. Na stronie zostaną wyświetlone dodatkowe ustawienia, które trzeba będzie uzupełnić.

4.  W polu **Adres** wpisz adres IP lub nazwę DNS serwera proxy, z którego chcesz korzystać.

5.  W polu **Port** wpisz numer portu, za pośrednictwem którego serwer proxy łączy się z Internetem.

6.  Jeśli serwer proxy nie służy do łączenia się z zasobami lokalnymi, zaznacz pole wyboru **Nie używaj serwera proxy dla adresów lokalnych**.

7.  W razie potrzeby zaznacz pole wyboru **Ten serwer proxy wymaga uwierzytelnienia**.

    -   Wybierz z listy typ uwierzytelniania: **Podstawowe**, **Porządkowanie** lub **Zintegrowane systemu Windows**.
    -   W polu **Nazwa użytkownika** wpisz nazwę użytkownika, która ma być podawana na żądanie serwera proxy.
    -   W polu **Hasło** wpisz hasło, które ma być podawane na żądanie serwera proxy.
    -   W polu **Potwierdź hasło** wpisz ponownie poprzednio wprowadzone hasło, aby potwierdzić jego poprawne wpisanie.
    -   Jeśli serwer proxy korzysta ze zintegrowanego uwierzytelniania systemu Windows, w polu **Domena** wpisz domenę, do której należy użytkownik.

8.  Kliknij przycisk **Wyślij**.
