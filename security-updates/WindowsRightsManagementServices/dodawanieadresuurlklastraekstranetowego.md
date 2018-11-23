---
TOCTitle: Dodawanie adresu URL klastra ekstranetowego
Title: Dodawanie adresu URL klastra ekstranetowego
ms:assetid: '12c83186-ce9e-4100-bbd1-d87a885331c7'
ms:contentKeyID: 18123188
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720193(v=WS.10)'
---

Dodawanie adresu URL klastra ekstranetowego
===========================================

Aby wykonać tę procedurę, należy zalogować się lokalnie w administracyjnej witrynie sieci Web przy użyciu konta należącego do grupy Administratorzy na komputerze, do którego użytkownik uzyskuje dostęp. Członkowie grupy Administratorzy domeny również mogą wykonać tę procedurę. Ze względu na najważniejsze wskazówki dotyczące bezpieczeństwa należy rozważyć użycie trybu **Uruchom jako** w celu wykonania tej procedury.

Aby otworzyć stronę sieci Web **Administracja globalna**, należy kliknąć przycisk **Start**, wskazać polecenie **Wszystkie programy**, wskazać polecenie **Windows RMS**, a następnie kliknąć polecenie **Administracja programem Windows RMS**.

Adres URL należy zarejestrować w systemie nazw domen (DNS) i należy sprawdzić, czy ten adres działa i czy jest dostępny w sieci ekstranet w Internecie. Jeśli dla plików usług sieci Web włączono protokół SSL, należy określić protokół HTTPS dla adresu URL klastra.

W przypadku dodawania adresu URL klastra ekstranetowego do działającego serwera programu RMS bieżący klienci programu RMS muszą uzyskać nowe certyfikaty licencjodawców klienta, aby uzyskać dostęp do klastra ekstranetowego w celu obsługi licencjonowania.

Dodawanie adresów URL w sieci ekstranet
---------------------------------------

#### Dodawanie adresu URL klastra ekstranetowego

1.  Otwórz stronę **Administracja globalna**, a następnie obok witryny sieci Web, do której chcesz dodać adres URL klastra ekstranetowego, kliknij łącze **Administruj programem RMS w tej witrynie sieci Web**.

2.  W obszarze **Łącza administracyjne** kliknij łącze **Ustawienia adresu URL klastra ekstranetowego**.

3.  W obszarze **Adres URL klastra ekstranetowego** określ adres URL, pod którym użytkownicy zewnętrzni będą mogli uzyskiwać licencje. Można także wybrać protokół HTTP lub HTTPS.

4.  Kliknij przycisk **Wyślij**.
