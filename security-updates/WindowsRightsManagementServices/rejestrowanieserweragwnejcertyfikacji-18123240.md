---
TOCTitle: Rejestrowanie serwera głównej certyfikacji
Title: Rejestrowanie serwera głównej certyfikacji
ms:assetid: '3f69d25e-ecae-447f-b741-a819c8cf6227'
ms:contentKeyID: 18123240
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720250(v=WS.10)'
---

Rejestrowanie serwera głównej certyfikacji
==========================================

Każda instalacja programu RMS musi zawierać co najmniej jeden serwer głównej certyfikacji, a opcjonalnie również dodatkowe serwery głównej certyfikacji w klastrze. Pierwszy instalowany serwer głównej certyfikacji należy zarejestrować w usłudze rejestracji firmy Microsoft, aby uzyskać główny certyfikat licencjodawcy serwera. W certyfikacie tym są zapisane podstawowe informacje na temat hierarchii zaufania w implementacji programu RMS.

Główny certyfikat licencjodawcy serwera można uzyskać za pomocą jednej z poniższych metod. Można wybrać certyfikat, który ma być używany, po wprowadzeniu informacji na temat zastrzegania serwera programu RMS:

-   **Rejestracja w trybie online**. Jeżeli serwer głównej certyfikacji może łączyć się z Internetem, certyfikat licencjodawcy serwera można uzyskać automatycznie podczas zastrzegania. Jest to metoda domyślna.
-   **Rejestracja w trybie offline**. Jeżeli serwer głównej certyfikacji nie jest podłączony do Internetu, rejestrację można przeprowadzić ręcznie po zakończeniu procesu zastrzegania. W tym celu należy wyeksportować żądanie rejestracji z serwera do pliku, który można przenieść na inny komputer podłączony do Internetu, a następnie wysłać do usługi rejestrowania firmy Microsoft w celu uzyskania certyfikatu licencjodawcy serwera. W przypadku wybrania rejestracji w trybie offline podczas zastrzegania program RMS ukończy proces zastrzegania, jednak programu tego nie będzie można używać do chwili zaimportowania certyfikatu licencjodawcy serwera uzyskanego przez inny komputer. Aby uzyskać więcej informacji, zobacz [Ręczna rejestracja serwera głównej certyfikacji](https://technet.microsoft.com/aecdebb5-b28b-4b58-937a-392bb6ce9643) w dalszej części tego tematu.

Żądanie rejestrowania zawiera następujące informacje:

-   Revocation information — informacje określające, czy instalacja programu RMS będzie stosować odwoływanie standardowe, czy też niestandardowe (przez niezależny podmiot). W przypadku zastosowania odwoływania przez niezależny podmiot dołączony zostaje klucz publiczny urzędu odwołującego.
-   Certificate Public Key — klucz publiczny certyfikatu licencjodawcy serwera. Taki klucz publiczny jest generowany na serwerze programu RMS i przesyłany do usługi rejestrowania firmy Microsoft w celu uzyskania certyfikatu licencjodawcy serwera.
-   SKU — oficjalna nazwa SKU programu RMS.
-   Version — numer wersji programu RMS.
-   URL — bazowy adres URL klastra serwerów programu RMS.

W odpowiedzi na żądanie rejestrowania usługa rejestrowania firmy Microsoft zwraca serwerowi programu RMS następujące informacje w formacie XML:

-   Certyfikat licencjodawcy serwera
-   Łańcuch certyfikatów urzędów podpisujących.

Identyczne informacje są przekazywane bez względu na to, czy serwer głównej certyfikacji programu RMS jest rejestrowany w trybie online czy offline. Przy korzystaniu z każdej z tych metod nie są zbierane żadne dodatkowe informacje.

> [!note]  
> W przypadku wyboru opcji rejestrowania w trybie offline i korzystania z komputera z konfiguracją zwiększonych zabezpieczeń przeglądarki, na przykład z komputera z systemem Windows Server 2003 lub Windows XP z dodatkiem Service Pack 2, aby połączyć się z Internetem i zażądać certyfikatu licencjodawcy serwera, do strefy Zaufane witryny należy dodać adres URL witryny sieci Web usługi rejestracji w celu umożliwienia pobrania certyfikatu licencjodawcy serwera. Adresem tym jest https://activation.drm.microsoft.com. W przypadku rejestracji w trybie offline należy sprawdzić, czy na komputerze używanym do wysyłania żądania rejestracji do usługi rejestrowania firmy Microsoft zostały zainstalowane wszystkie najnowsze aktualizacje certyfikatów. Certyfikatem SSL usług rejestrowania firmy Microsoft jest certyfikat GTE Cyber Trust Root CA, który jest domyślnie zaufanym certyfikatem na wszystkich komputerach z systemem Windows Server 2003. W przypadku procesu rejestracji w trybie offline należy dopilnować, aby klienci RMS nie próbowali łączyć się z serwerem programu RMS w celu uzyskania licencji do czasu ukończenia procesu rejestracji. Jeżeli klienci będą próbować łączyć się z niezarejestrowanym serwerem programu RMS, wystąpi błąd usług sieci Web, który uniemożliwi korzystanie z nich. Jeżeli nie można zagwarantować, że klienci nie będą łączyć się z serwerem programu RMS, najlepszym sposobem jest zresetowanie usługi IIS po ukończeniu rejestracji, aby wyczyścić wszystkie utworzone stany błędu. 
