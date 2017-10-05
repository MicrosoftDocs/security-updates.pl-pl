---
TOCTitle: Odnajdowanie usługi licencjonowania
Title: Odnajdowanie usługi licencjonowania
ms:assetid: '4eabbb76-b359-443a-b737-098c5659e9c6'
ms:contentKeyID: 18123260
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720269(v=WS.10)'
---

Odnajdowanie usługi licencjonowania
===================================

Usługa licencjonowania programu RMS wystawia licencje użytkowania, które umożliwiają uwierzytelnionym użytkownikom korzystanie z zawartości chronionej.

Usługa działa na serwerach głównej certyfikacji i licencji lub w klastrach. W celu wysłania żądania licencji użytkowania klient najpierw pobiera z usługi Active Directory adres URL katalogu wirtualnego licencjonowania klastra głównej certyfikacji, w którym znajduje się usługa licencjonowania. Następnie dołącza ścieżkę do usługi licencjonowania.

Na przykład adres URL katalogu wirtualnego licencjonowania klastra głównej certyfikacji jest przechowywany w usłudze Active Directory w następującej postaci:

http://*nazwa\_serwera*/\_wmcs/Licensing

Gdy klient żąda licencji użytkowania, dodaje nazwę pliku usługi licencjonowania do adresu URL w następujący sposób:

http://*nazwa\_serwera*/\_wmcs/Licensing/License.asmx

Lokalizacją usługi jest serwer programu RMS lub konto .NET Passport, które wystawiło licencję publikacji. Adres URL jest uwzględniany w licencji publikacji.

| ![](images/Cc720269.note(WS.10).gif)Uwaga                                               |
|----------------------------------------------------------------------------------------------------------------------|
| Jeśli włączono protokół SSL dla serwera programu RMS, te adresy URL będą korzystały z protokołu połączenia https://. |
