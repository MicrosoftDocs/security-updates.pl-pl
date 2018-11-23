---
TOCTitle: Konfigurowanie grupy administratorów
Title: Konfigurowanie grupy administratorów
ms:assetid: 'f2ef847e-2824-471f-9079-5c343094aba8'
ms:contentKeyID: 18123515
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747798(v=WS.10)'
---

Konfigurowanie grupy administratorów
====================================

Aby wykonać tę procedurę, należy zalogować się lokalnie w administracyjnej witrynie sieci Web przy użyciu konta należącego do grupy Administratorzy na komputerze, do którego użytkownik uzyskuje dostęp. Członkowie grupy Administratorzy domeny również mogą wykonać tę procedurę. Ze względu na najważniejsze wskazówki dotyczące bezpieczeństwa należy rozważyć użycie trybu **Uruchom jako** w celu wykonania tej procedury.

Aby otworzyć stronę sieci Web **Administracja globalna**, należy kliknąć przycisk **Start**, wskazać polecenie **Wszystkie programy**, wskazać polecenie **Windows RMS**, a następnie kliknąć polecenie **Administracja programem Windows RMS**.

Aby grupę można było wyznaczyć jako grupę administratorów programu RMS, musi ona istnieć w usłudze Active Directory, a właściwości tej grupy muszą zawierać adres e-mail (określony jako pełna kwalifikowana nazwa domeny), który jest taki sam jak nazwa konta.

Konfigurowanie grupy administratorów
------------------------------------

#### Konfigurowanie grupy administratorów

1.  Otwórz stronę **Administracja globalna**, a następnie obok witryny sieci Web, w której chcesz skonfigurować grupę administratorów, kliknij łącze **Administruj programem RMS w tej witrynie sieci Web**.

2.  W obszarze **Łącza administracyjne** kliknij łącze **Ustawienia zabezpieczeń**.

3.  W obszarze **Administratorzy** kliknij przycisk **Włącz**, aby dodać grupę administratorów.

4.  W polu **Nazwa grupy administratorów** wpisz pełną kwalifikowaną nazwę domeny (w formie *nazwa\_grupy*@*nazwa\_domeny.com*) istniejącej grupy w tym lesie usługi Active Directory, której członkowie otrzymają prawa właścicieli wszystkich dokumentów chronionych przez program RMS, a następnie kliknij przycisk **Zapisz**.

    Aby wyłączyć prawa dostępu grupy administratorów, kliknij przycisk **Wyłącz**.

Aby uzyskać więcej informacji dotyczących wykonywania tej procedury, zobacz „[Używanie grupy administratorów](https://technet.microsoft.com/0febcb3e-7124-4e51-971a-1013b928d33b)” we wcześniejszej części tego tematu.
