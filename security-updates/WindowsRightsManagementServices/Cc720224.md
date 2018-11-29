---
TOCTitle: Odnajdowanie usługi certyfikacji kont
Title: Odnajdowanie usługi certyfikacji kont
ms:assetid: '293a2f91-4712-45ec-8b74-7533f4144cbd'
ms:contentKeyID: 18123210
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720224(v=WS.10)'
---

Odnajdowanie usługi certyfikacji kont
=====================================

Usługa certyfikacji kont programu RMS udziela użytkownikom certyfikatów kont praw. Każdy certyfikat konta praw (RAC) jest ważny tylko dla określonego komputera lub urządzenia. Wymaga on od użytkownika żądającego certyfikatu posiadania ważnego certyfikatu komputera.

Tylko serwer lub klaster głównej certyfikacji obsługuje usługę certyfikacji kont. W celu wysłania żądania certyfikacji konta klient najpierw pobiera z usługi Active Directory adres URL katalogu wirtualnego Certification na serwerze głównej certyfikacji, w którym znajduje się usługa certyfikacji kont. Następnie klient dołącza ścieżkę do usługi certyfikacji kont.

Na przykład adres URL katalogu wirtualnego Certification na serwerze głównej certyfikacji jest przechowywany w usłudze Active Directory w następującej postaci:

http://*nazwa\_serwera*/\_wmcs/Certification

Gdy klient żąda certyfikatu konta praw, dodaje nazwę pliku usługi certyfikacji kont do adresu URL w następujący sposób:

http://*nazwa\_serwera*/\_wmcs/Certification/Certification.asmx

> [!note]  
> Jeśli włączono protokół SSL dla serwera programu RMS, te adresy URL będą korzystały z protokołu połączenia https://. 
