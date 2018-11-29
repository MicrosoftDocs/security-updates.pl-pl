---
TOCTitle: Włączanie certyfikacji urządzeń przenośnych
Title: Włączanie certyfikacji urządzeń przenośnych
ms:assetid: '93ec088e-9056-4c3c-bd97-1173fb194578'
ms:contentKeyID: 18123349
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747603(v=WS.10)'
---

Włączanie certyfikacji urządzeń przenośnych
===========================================

Aby wykonać tę procedurę, należy zalogować się lokalnie w witrynie sieci Web Administracja przy użyciu konta należącego do grupy Administratorzy na komputerze, do którego użytkownik uzyskuje dostęp. Członkowie grupy Administratorzy domeny również mogą wykonać tę procedurę. Ze względu na najważniejsze wskazówki dotyczące bezpieczeństwa należy rozważyć użycie trybu **Uruchom jako** w celu wykonania tej procedury.

Ta procedura ma zastosowanie wyłącznie na klastrze głównej certyfikacji.

W tej procedurze założono, że użytkownik utworzył grupę użytkowników, która zawiera konta użytkowników urządzeń przenośnych korzystających z zawartości chronionej technologią RMS.

Włączanie certyfikacji urządzeń przenośnych
-------------------------------------------

#### Włączanie certyfikacji urządzeń przenośnych

1.  Na serwerze głównej certyfikacji otwórz przeglądarkę systemu plików i przejdź do folderu &lt;dysk systemowy&gt;:\\Inetpub\\wwwroot\\\_wmcs\\Certification.

2.  Aby umożliwić urządzeniom przenośnym odbieranie certyfikatów kont praw (RAC), kliknij prawym przyciskiem myszy plik MobileDeviceCertification.asmx, a następnie kliknij polecenie **Właściwości**.

3.  Na karcie **Zabezpieczenia** kliknij przycisk **Dodaj** i dodaj grupę utworzoną dla tej kategorii użytkowników oraz grupę **RMS Service Group**.

4.  Na liście **Uprawnienia** dla tych grup zaznacz pole wyboru **Zezwalaj** zarówno dla uprawnień **do odczytu**, jak i **do odczytu &i wykonywania**, a następnie kliknij przycisk **OK**.
