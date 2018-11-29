---
TOCTitle: Dodawanie zaufanej domeny publikacji
Title: Dodawanie zaufanej domeny publikacji
ms:assetid: '731416d8-ddf4-4d4a-9f1a-bbd1ea48fe3c'
ms:contentKeyID: 18123317
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747624(v=WS.10)'
---

Dodawanie zaufanej domeny publikacji
====================================

Aby wykonać tę procedurę, należy zalogować się lokalnie w administracyjnej witrynie sieci Web przy użyciu konta należącego do grupy Administratorzy na komputerze, do którego użytkownik uzyskuje dostęp. Członkowie grupy Administratorzy domeny również mogą wykonać tę procedurę. Ze względu na najważniejsze wskazówki dotyczące bezpieczeństwa należy rozważyć użycie trybu **Uruchom jako** w celu wykonania tej procedury.

Aby otworzyć stronę sieci Web **Administracja globalna**, należy kliknąć przycisk **Start**, wskazać polecenie **Wszystkie programy**, wskazać polecenie **Windows RMS**, a następnie kliknąć polecenie **Administracja programem Windows RMS**.

Jeśli klucz prywatny programu RMS jest chroniony przy użyciu sprzętowego modułu zabezpieczeń, a import certyfikatu licencjodawcy serwera odbywa się z instalacji programu RMS, w której stosowana jest programowa ochrona klucza prywatnego, przed zaimportowaniem certyfikatu należy określić hasło klucza prywatnego na stronie **Ustawienia zabezpieczeń** serwera każdego serwera programu RMS w klastrze.

Dodawanie zaufanej domeny publikacji
------------------------------------

#### Dodawanie zaufanej domeny publikacji

1.  Otwórz stronę **Administracja globalna**, a następnie obok witryny sieci Web, do której chcesz dodać zaufaną domenę publikacji, kliknij łącze **Administruj programem RMS w tej witrynie sieci Web**.

2.  W obszarze **Łącza administracyjne** kliknij łącze **Zasady zaufania**.

3.  W obszarze **Zaufane domeny publikacji** kliknij przycisk **Przeglądaj**. Zlokalizuj i kliknij dwukrotnie certyfikat domeny publikacji, którą chcesz dodać. W polu **Hasło do odszyfrowania importowanego pliku** wpisz hasło wymagane do odszyfrowania tego pliku, a następnie kliknij przycisk **Importuj**.

    Zaszyfrowany za pomocą hasła plik zawiera certyfikat licencjodawcy serwera, klucz prywatny (jeśli klucz jest przechowywany w oprogramowaniu) i szablony zasad praw dostępu.

4.  Nazwa domeny zostanie wyświetlona na liście **Zaufane domeny publikacji**.

Aby uzyskać więcej informacji dotyczących wykonywania tej procedury, zobacz [Dodawanie i usuwanie zaufanych domen publikacji](https://technet.microsoft.com/d87b502d-5497-4ccd-badf-f6807d587cee) we wcześniejszej części tego tematu.
