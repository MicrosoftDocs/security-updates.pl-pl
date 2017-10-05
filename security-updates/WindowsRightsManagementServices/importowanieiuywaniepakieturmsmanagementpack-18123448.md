---
TOCTitle: Importowanie i używanie pakietu RMS Management Pack
Title: Importowanie i używanie pakietu RMS Management Pack
ms:assetid: 'd9a73ef0-2f81-48c2-97cc-deb7bf477389'
ms:contentKeyID: 18123448
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747688(v=WS.10)'
---

Importowanie i używanie pakietu RMS Management Pack
===================================================

Importowanie i używanie pakietu RMS Management Pack
---------------------------------------------------

#### Importowanie i używanie pakietu RMS Management Pack

1.  Skopiuj pakiet RMS Management Pack (RMS\_MOMPack.akm) z folderu %ProgramFiles%\\Windows Rights Management Services\\Tools na serwer pakietu Microsoft Operations Manager (MOM).

2.  Otwórz konsolę administracyjną programu MOM, a następnie zaimportuj pakiet RMS Management Pack, wykonując następujące czynności:

    1.  W drzewie konsoli administracyjnej programu MOM rozwiń pozycję **Rules (Reguły)**, a następnie prawym przyciskiem myszy kliknij pozycję **Processing Rule Groups (Grupy reguł przetwarzania)**.
    2.  W menu skrótów kliknij polecenie **Import Management Pack (Importuj pakiet Management Pack)**. Zostanie wyświetlone okno dialogowe **Import Management Pack (Importowanie pakietu Management Pack)**.
    3.  Kliknij przycisk **Browse (Przeglądaj)**, a następnie wybierz plik RMS\_MOMPack.akm.

3.  Określ opcje scalania lub zamieniania. Aby uzyskać więcej informacji dotyczących opcji scalania i zamieniania, zobacz dokument „Eksportowanie i importowanie pakietów Management Pack” w witrynie sieci Web firmy Microsoft (http://www.microsoft.com/).

    Kliknij przycisk **Replace (Zamień)**. Użycie opcji zamieniania spowoduje, że zaimportowany pakiet zarządzania zastąpi istniejące grupy reguł przetwarzania; komentarze użytkowników nie będą zachowywane. Jeśli chcesz scalić ten pakiet zarządzania z istniejącym pakietem zarządzania, wykonaj tę czynność w środowisku testowym, a następnie użyj opcji **Replace (Zamień)** podczas wdrażania pakietu zarządzania w środowisku produkcyjnym.

4.  Kliknij przycisk **Import (Importuj)**, aby zaimportować pakiet zarządzania.

5.  W **konsoli administracyjnej programu MOM** zaznacz pozycję **Configuration (Konfiguracja)**, a następnie kliknij folder **Agent Managers (Menedżerowie agenta)**.

6.  Prawym przyciskiem myszy kliknij nazwę serwera, na który zaimportowano pakiet RMS Management Pack, a następnie wybierz polecenie **Scan Managed Computers Now (Skanuj teraz zarządzane komputery)**.
