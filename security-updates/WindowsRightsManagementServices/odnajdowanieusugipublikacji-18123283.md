---
TOCTitle: Odnajdowanie usługi publikacji
Title: Odnajdowanie usługi publikacji
ms:assetid: '5d500841-a202-4865-b5d2-d0775d4e1bbc'
ms:contentKeyID: 18123283
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747580(v=WS.10)'
---

Odnajdowanie usługi publikacji
==============================

Usługa publikacji programu RMS wystawia licencje publikacji, które służą do ochrony zawartości. Usługa ta wystawia również certyfikaty licencjodawcy klienta, które umożliwiają użytkownikom publikowanie zawartości, gdy nie są podłączeni do sieci firmowej.

Usługa publikacji jest dostępna z poziomu klastra głównej certyfikacji lub z serwerów licencji. Aplikacja obsługująca technologię RMS żąda tej usługi, gdy autor publikuje zawartość chronioną technologią RMS. W celu wysłania żądania usługi publikacji aplikacja najpierw pobiera z usługi Active Directory adres URL katalogu wirtualnego Licensing serwera, na którym znajduje się usługa publikacji. Następnie aplikacja dołącza ścieżkę do usługi publikacji.

Na przykład adres URL katalogu wirtualnego Licensing serwera jest przechowywany w usłudze Active Directory w następującej postaci:

http://*nazwa\_serwera*/\_wmcs/Licensing

Gdy serwer żąda licencji publikacji, dodaje nazwę pliku usługi publikacji do adresu URL w następujący sposób:

http://*nazwa\_serwera*/\_wmcs/Licensing/Publish.asmx

Jeśli program RMS wykryje, że certyfikat konta praw jest oparty na uwierzytelnianiu systemu Windows, lokalizacja usługi publikacji zostanie określona na podstawie lasu Active Directory. Ma to zastosowanie do użytkowników wewnętrznych i zewnętrznych, którzy łączą się z siecią firmową za pomocą wirtualnych sieci prywatnych (VPN).

Jeśli program RMS wykryje, że certyfikat konta praw jest oparty na usłudze Microsoft® .NET Passport, lokalizacją usługi publikacji jest konto .NET Passport określone w zawartości chronionej technologią RMS.

> [!note]  
> Jeśli włączono protokół SSL dla serwera programu RMS, te adresy URL będą korzystały z protokołu połączenia https://. 
