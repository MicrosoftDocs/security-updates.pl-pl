---
TOCTitle: Włączanie administracji zdalnej programu RMS
Title: Włączanie administracji zdalnej programu RMS
ms:assetid: '00f17054-5f5d-47e2-89c1-7a593b930bb3'
ms:contentKeyID: 18123172
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720181(v=WS.10)'
---

Włączanie administracji zdalnej programu RMS
============================================

Na komputerze używanym do zdalnego administrowania programem RMS należy zainstalować program Internet Explorer 6.0 lub nowszy.

Włączanie administracji zdalnej programu RMS
--------------------------------------------

#### Włączanie administracji zdalnej programu RMS

1.  Zaloguj się na serwerze, z którego chcesz realizować administrację zdalną.

2.  Z poziomu okna **Narzędzia administracyjne** otwórz przystawkę **Menedżer internetowych usług informacyjnych (IIS)**.

3.  Rozwiń pozycję reprezentującą witrynę sieci Web, w której zastrzeżono program RMS.

4.  Prawym przyciskiem myszy kliknij folder **\_wmcs**, a następnie kliknij polecenie **Właściwości**. Na karcie **Zabezpieczenia katalogów** w obszarze **Bezpieczna komunikacja** kliknij przycisk **Edytuj**, kliknij opcję **Wymagaj bezpiecznego kanału**, a następnie kliknij przycisk **OK**. Spowoduje to ochronę usług sieci Web programu RMS za pomocą protokołu SSL (Secure Sockets Layer). Aby uzyskać więcej informacji dotyczących zarządzania witrynami sieci Web przy użyciu programu IIS, zobacz Pomoc programu IIS.

    | ![](images/Cc720181.Important(WS.10).gif)Ważne                                                                                                                                                                                                                                                                                                     |
    |---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Usługi sieci Web programu RMS można zabezpieczyć za pomocą protokołu SSL, dzięki czemu można uzyskać dodatkowe zabezpieczenia i zdalny dostęp do administracyjnych stron sieci Web programu RMS za pośrednictwem protokołu HTTP. Jeśli planowane jest używanie protokołu SSL z usługami sieci Web programu RMS, należy uzyskać i zainstalować certyfikat SSL serwera sieci Web. |

5.  Prawym przyciskiem myszy kliknij folder **Admin**, a następnie kliknij polecenie **Właściwości**. Na karcie **Zabezpieczenia katalogów** w obszarze **Ograniczenia adresów IP i nazw domen** kliknij przycisk **Edytuj**, a następnie w obszarze **Ograniczenia dostępu do adresów IP** kliknij opcję **Udzielony dostęp**, aby zezwolić wszystkim komputerom na żądanie połączenia z tą witryną sieci Web.
