---
TOCTitle: Zabezpieczenia podczas instalacji programu RMS
Title: Zabezpieczenia podczas instalacji programu RMS
ms:assetid: '0a3d40b2-f27e-4e63-baff-a9c8433f5f91'
ms:contentKeyID: 18123168
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720192(v=WS.10)'
---

Zabezpieczenia podczas instalacji programu RMS
==============================================

W celu zainstalowania i skonfigurowania plików programu RMS Instalator programu RMS używa poświadczeń zalogowanego użytkownika. Z tego powodu administrator wykonujący procedurę instalacyjną musi zalogować się za pomocą konta użytkownika będącego członkiem lokalnej grupy administratorów. Dla wszystkich instalacji z wyjątkiem instalacji na pojedynczym komputerze musi to być także konto użytkownika domeny.

Podczas procedury instalacji uruchamiana jest usługa instalatora systemu Windows (Msiexec.exe). Ta usługa dziedziczy token użytkownika nadrzędnego. W późniejszej części procedury, jeśli wystąpią niestandardowe czynności, usługa Msiexec.exe korzysta z tożsamości zalogowanego użytkownika. Dzieje się tak niezależnie od tego, czy proces został uruchomiony z poziomu przeglądarki czy z poziomu wiersza polecenia.

Instalator programu RMS wykonuje następujące zadania:

-   Kopiuje pliki do folderu C:\\Program Files\\RMS. Do tego folderu zwykle mają dostęp administratorzy i użytkownicy zaawansowani. Podczas instalacji można skonfigurować dysk i lokalizację plików.
-   Tworzy witrynę sieci Web zastrzegania, administracyjną witrynę sieci Web programu RMS, domyślnie na porcie 5720. Ta witryna sieci Web wskazuje zainstalowane pliki.
-   Tworzy pulę aplikacji WMCSProvisioningAppPool i kojarzy ją z administracyjną witryną sieci Web programu RMS. Konto usługi używane przez tę pulę aplikacji to konto Usługi sieciowe.
-   Instaluje liczniki wydajności.
-   Udziela grupie RMS Service Group uprawnień do odczytu i zapisu dla następujących kluczy rejestru.
    W komputerach z 32-bitową wersją systemu Windows Server 2003:
    `HKEY_LOCAL_MACHINE\Software\Microsoft\DRMS\1.0`
    W komputerach z 64-bitową wersją systemu Windows Server 2003:
    `HKEY_LOCAL_MACHINE\Software\WOW6432Node\Microsoft\DRMS\1.0`
