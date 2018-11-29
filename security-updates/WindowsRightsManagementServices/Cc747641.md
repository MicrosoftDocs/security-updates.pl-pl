---
TOCTitle: Odnajdowanie usługi podrejestrowywania
Title: Odnajdowanie usługi podrejestrowywania
ms:assetid: 'b159953a-af38-4a9e-8c87-1aff5fb4e366'
ms:contentKeyID: 18123390
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747641(v=WS.10)'
---

Odnajdowanie usługi podrejestrowywania
======================================

Pojedynczy serwer licencji lub pierwszy serwer licencji w klastrze musi wysłać żądanie podrejestrowywania do serwera głównej certyfikacji programu RMS oraz uzyskać certyfikat licencjodawcy serwera. W tym celu serwer licencji uzyskuje adres URL usługi podrejestrowywania głównej certyfikacji w następujący sposób.

Podczas zastrzegania serwera licencji Instalator programu RMS wysyła kwerendę do usługi Active Directory, a następnie wykrywa punkt połączenia usługi dla klastra głównej certyfikacji. Program RMS używa adresu URL przechowywanego w tym punkcie połączenia usługi do zlokalizowania klastra głównej certyfikacji, a następnie wysyła żądanie certyfikatu licencjodawcy serwera do usługi podrejestrowywania serwera głównej certyfikacji.

W celu wysłania żądania usługi podrejestrowywania serwer licencji najpierw pobiera z usługi Active Directory adres URL katalogu wirtualnego Certification serwera głównej certyfikacji, w którym znajduje się usługa podrejestrowywania. Następnie dołącza ścieżkę do usługi podrejestrowywania.

Na przykład adres URL katalogu wirtualnego Certification na serwerze głównej certyfikacji jest przechowywany w usłudze Active Directory w następującej postaci:

http://*nazwa\_serwera*/\_wmcs/Certification

Gdy serwer licencji żąda usługi podrejestrowywania, dołącza nazwę pliku usługi do adresu URL w następujący sposób:

http://nazwa\_serwera/\_wmcs/Certification/SubEnrollService.asmx

> [!note]  
> Jeśli włączono protokół SSL dla serwera programu RMS, te adresy URL będą korzystały z protokołu połączenia https://. 
