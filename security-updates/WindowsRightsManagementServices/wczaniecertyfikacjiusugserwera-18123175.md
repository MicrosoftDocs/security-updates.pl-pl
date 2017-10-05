---
TOCTitle: Włączanie certyfikacji usług serwera
Title: Włączanie certyfikacji usług serwera
ms:assetid: '0ed78c85-7acb-4e3b-a594-613f8ccb5b14'
ms:contentKeyID: 18123175
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720196(v=WS.10)'
---

Włączanie certyfikacji usług serwera
====================================

Aby wykonać tę procedurę, należy zalogować się lokalnie w witrynie sieci Web Administracja przy użyciu konta użytkownika domeny należącego do grupy Administratorzy. Ze względu na najważniejsze wskazówki dotyczące bezpieczeństwa należy rozważyć użycie trybu **Uruchom jako** w celu wykonania tej procedury.

Ta procedura ma zastosowanie wyłącznie na klastrze głównym.

W tej procedurze założono, że użytkownik utworzył grupę użytkowników zwierającą konta użytkowników, które usług serwera będą personifikować podczas korzystania z zawartości chronionej na podstawie praw.

Włączanie certyfikacji usług serwera
------------------------------------

#### Włączanie certyfikacji usług serwera

1.  Zaloguj się na komputerze jako członek lokalnej grupy Administratorzy.

2.  Otwórz przeglądarkę systemu plików i przejdź do folderu &lt;dysk systemowy&gt;:\\Inetpub\\wwwroot\\\_wmcs\\Certification.

3.  Aby umożliwić odbieranie certyfikatów kont praw (RAC) przez usługi serwera, kliknij prawym przyciskiem myszy plik ServerCertification.asmx, a następnie kliknij polecenie **Właściwości**.

4.  Na karcie **Zabezpieczenia** kliknij przycisk **Dodaj** i dodaj grupę utworzoną dla tej kategorii użytkowników oraz grupę **RMS Service Group**.

5.  Na liście **Uprawnienia** dla tych grup zaznacz pole wyboru **Zezwalaj** dla uprawnień **Odczyt & Wykonywanie**, a następnie kliknij przycisk **OK**.

6.  Kroki 1 - 4 należy powtórzyć dla wszystkich serwerów w klastrze.

| ![](images/Cc720196.note(WS.10).gif)Uwaga                                                                                                                                                                                                                                                                                                                                                                                                                             |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| W przypadku programu Microsoft Exchange Server 2007 należy dodać każdy obiekt komputera usługi Active Directory serwera czołowego do listy arbitralnej kontroli dostępu (DACL) pliku ServerCertification.asmx. Podobnie w przypadku programu Microsoft Office SharePoint Server 2007 do tej listy DACL należy dodać obiekt komputera usługi Active Directory serwera Office SharePoint Server 2007. Do tej listy DACL zaleca się dodanie grupy zabezpieczeń oraz odpowiednich obiektów komputerów. |
