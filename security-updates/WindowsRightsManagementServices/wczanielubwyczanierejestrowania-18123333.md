---
TOCTitle: Włączanie lub wyłączanie rejestrowania
Title: Włączanie lub wyłączanie rejestrowania
ms:assetid: '8e672f95-566f-4070-9a2a-2f70f087148f'
ms:contentKeyID: 18123333
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747674(v=WS.10)'
---

Włączanie lub wyłączanie rejestrowania
======================================

Aby wykonać tę procedurę, należy zalogować się lokalnie w administracyjnej witrynie sieci Web przy użyciu konta należącego do grupy Administratorzy na komputerze, do którego użytkownik uzyskuje dostęp. Członkowie grupy Administratorzy domeny również mogą wykonać tę procedurę. Ze względu na najważniejsze wskazówki dotyczące bezpieczeństwa należy rozważyć użycie trybu **Uruchom jako** w celu wykonania tej procedury.

Aby otworzyć stronę sieci Web **Administracja globalna**, należy kliknąć przycisk **Start**, wskazać polecenie **Wszystkie programy**, wskazać polecenie **Windows RMS**, a następnie kliknąć polecenie **Administracja programem Windows RMS**.

Należy upewnić się, że serwer programu RMS ma połączenie z bazą danych i że ta usługa bazy danych została uruchomiona przed włączeniem rejestrowania. Jeżeli usługa kolejkowania wiadomości nie może dostarczyć dzienników do bazy danych rejestrowania, dane zostaną umieszczone w kolejce na dysku twardym serwera programu RMS. Proces ten będzie trwał, aż do zapełnienia miejsca na przechowywanie danych na serwerze. W programie RMS nie zostanie wyświetlony błąd, ponieważ funkcja ta ma na celu obsługę rejestrowania w czasie, gdy połączenie z serwerem SQL zostanie przerwane.

Włączanie lub wyłączanie rejestrowania
--------------------------------------

#### Włączanie lub wyłączanie rejestrowania

1.  Otwórz stronę **Administracja globalna**, a następnie obok witryny sieci Web, w której chcesz włączyć lub wyłączyć rejestrowanie, kliknij łącze **Administruj programem RMS w tej witrynie sieci Web**.

2.  W obszarze **Łącza administracyjne** kliknij łącze **Ustawienia rejestrowania**.

3.  W obszarze **Serwer i baza danych rejestrowania** zaznacz pole wyboru **Włącz rejestrowanie**, a następnie kliknij przycisk **Aktualizuj**.

    Aby wyłączyć rejestrowanie, wyczyść pole wyboru, a następnie kliknij przycisk **Aktualizuj**.

Aby uzyskać więcej informacji dotyczących wykonywania tej procedury, zobacz „[Włączanie i wyłączanie rejestrowania](https://technet.microsoft.com/50ccd827-2d39-41e7-a395-3d5f5836869b)” we wcześniejszej części tego tematu.
