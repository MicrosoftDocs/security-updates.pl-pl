---
TOCTitle: 'Usuwanie usługi sieci Web (usuwanie zastrzeżenia programu RMS)'
Title: 'Usuwanie usługi sieci Web (usuwanie zastrzeżenia programu RMS)'
ms:assetid: '68b4e2b0-b1b7-4b0a-8c1a-82ac27c1f12e'
ms:contentKeyID: 18123295
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747602(v=WS.10)'
---

Usuwanie usługi sieci Web (usuwanie zastrzeżenia programu RMS)
==============================================================

Po zlikwidowaniu serwera programu RMS i usunięciu wszystkich zabezpieczeń RMS można usunąć usługę sieci Web, wykonując następujące czynności:

-   Na stronie **Administracja globalna** kliknij łącze **Usuń program RMS z tej witryny sieci Web**.

Następny krok zależy od typu usuwanego serwera, mimo że we wszystkich przypadkach program RMS będzie usuwany z Internetowych usług informacyjnych (IIS).

-   Jeśli serwer jest częścią klastra (ale nie może być ostatnim serwerem w klastrze), nie trzeba wykonywać dodatkowych czynności.
-   Jeśli serwer jest tylko serwerem licencji, należy usunąć bazę danych usług katalogowych, ale zachować bazę danych konfiguracji i rejestrowania (jest ona używana przez nadal działający serwer certyfikacji).
-   Jeśli serwer jest ostatnim serwerem programu RMS w organizacji, należy zachować bazę danych konfiguracji i rejestrowania, ale usunąć punkt połączenia usługi (SCP) w usłudze Active Directory.
