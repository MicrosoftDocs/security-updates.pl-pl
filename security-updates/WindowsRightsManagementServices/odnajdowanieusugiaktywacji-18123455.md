---
TOCTitle: Odnajdowanie usługi aktywacji
Title: Odnajdowanie usługi aktywacji
ms:assetid: 'e178d81b-b35c-4958-87ef-e077e2204b32'
ms:contentKeyID: 18123455
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747697(v=WS.10)'
---

Odnajdowanie usługi aktywacji
=============================

Usługa aktywacji wystawia skrytki i certyfikaty komputerów RMS dla klientów RMS w wersji 1.0. Jest ona obsługiwana ze względu na wymóg zachowania zgodności wstecz z programem RMS w wersji 1.0. Klaster głównej certyfikacji programu RMS dostarcza usługę serwera proxy aktywacji, która przekazuje żądania aktywacji komputerów RMS do usługi aktywacji z komputerów klienckich działających w sieci firmowej.

Aby wysłać żądanie aktywacji komputera RMS, klient RMS w wersji 1.0 najpierw pobiera z katalogu Active Directory adres URL do wirtualnego katalogu certyfikacji na serwerze głównej certyfikacji, gdzie znajduje się usługa serwera proxy aktywacji. Następnie klient dołącza ścieżkę do usługi serwera proxy aktywacji.

Na przykład adres URL katalogu wirtualnego certyfikacji na serwerze głównej certyfikacji jest przechowywany w usłudze Active Directory w następującej postaci:

http://*nazwa\_serwera*/\_wmcs/Certification

Gdy klient żąda aktywacji komputera RMS, dodaje nazwę pliku usługi serwera proxy aktywacji do adresu URL w następujący sposób:

http://*nazwa\_serwera*/\_wmcs/Certification/Activation.asmx

Klienci działający poza siecią firmową korzystają z rejestru usług UDDI w celu odnajdowania usługi aktywacji. Aby uzyskać więcej informacji, zobacz „[Publikowanie usług obsługiwanych przez firmę Microsoft](https://technet.microsoft.com/7ee8cb4d-1b46-48be-8a4c-5ff6a458231a)” we wcześniejszej części tematu.

| ![](images/Cc747697.note(WS.10).gif)Uwaga                                               |
|----------------------------------------------------------------------------------------------------------------------|
| Jeśli włączono protokół SSL dla serwera programu RMS, te adresy URL będą korzystały z protokołu połączenia https://. |
