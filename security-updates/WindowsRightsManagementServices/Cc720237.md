---
TOCTitle: Określanie kontaktu administracyjnego
Title: Określanie kontaktu administracyjnego
ms:assetid: '31777458-5530-4ae0-ac1f-131b3d98dd35'
ms:contentKeyID: 18123220
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720237(v=WS.10)'
---

Określanie kontaktu administracyjnego
=====================================

Aby wykonać tę procedurę, należy zalogować się lokalnie w administracyjnej witrynie sieci Web przy użyciu konta należącego do grupy Administratorzy na komputerze, do którego użytkownik uzyskuje dostęp. Członkowie grupy Administratorzy domeny również mogą wykonać tę procedurę. Ze względu na najważniejsze wskazówki dotyczące bezpieczeństwa należy rozważyć użycie trybu **Uruchom jako** w celu wykonania tej procedury.

Administrator określony w tej procedurze powinien być lokalnym administratorem na serwerze głównej certyfikacji, ponieważ zalogowany użytkownik musi mieć uprawnienia do pliku SubEnrollService.asmx file na głównym serwerze certyfikacji, aby zastrzec serwer licencji. Jeśli użytkownik próbujący zastrzec serwer licencji nie ma uprawnień do tego pliku, może on wysłać do administratora określonego w tej operacji żądanie udzielenia kontu użytkownika wymaganych uprawnień. Aby uzyskać więcej informacji, zobacz „[Ustawianie uprawnień do pliku usługi podrejestrowywania](https://technet.microsoft.com/737bb69b-fe26-4057-9569-e632f7bbf295)” we wcześniejszej części tego tematu.

Aby otworzyć stronę sieci Web **Administracja globalna**, należy kliknąć przycisk **Start**, wskazać polecenie **Wszystkie programy**, wskazać polecenie **Windows RMS**, a następnie kliknąć polecenie **Administracja programem Windows RMS**.

Określanie kontaktu administracyjnego
-------------------------------------

#### Określanie kontaktu administracyjnego

1.  Otwórz stronę **Administracja globalna**, a następnie obok witryny sieci Web, w której chcesz określić kontakt administracyjny, kliknij łącze **Administruj programem RMS w tej witrynie sieci Web**.

2.  W obszarze **Łącza administracyjne** kliknij łącze **Ustawienia certyfikacji**.

3.  W obszarze **Kontakt administracyjny** wpisz adres e-mail administratora (w formie *nazwa\_użytkownika*@*nazwa\_domeny*.com), z którym można będzie skontaktować się w przypadku problemów z podrejestrowywaniem podczas zastrzegania serwera licencji.

4.  U dołu strony kliknij przycisk **Wyślij**.
