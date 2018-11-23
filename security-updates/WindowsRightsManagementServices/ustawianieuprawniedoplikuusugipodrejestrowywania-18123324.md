---
TOCTitle: Ustawianie uprawnień do pliku usługi podrejestrowywania
Title: Ustawianie uprawnień do pliku usługi podrejestrowywania
ms:assetid: '737bb69b-fe26-4057-9569-e632f7bbf295'
ms:contentKeyID: 18123324
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747627(v=WS.10)'
---

Ustawianie uprawnień do pliku usługi podrejestrowywania
=======================================================

Usługa podrejestrowywania działa na serwerze głównej certyfikacji i podczas zastrzegania rejestruje serwer licencji. Domyślnie usługa podrejestrowywania zezwala na dostęp wyłącznie z lokalnego konta systemowego znajdującego się na serwerze głównej certyfikacji. Aby zastrzec serwer licencji, należy zalogować się do tego serwera za pomocą takiego konta. Istnieje też inne rozwiązanie, które wymaga, aby lokalny administrator serwera głównej certyfikacji zmienił listę DACL w pliku usługi podrejestrowywania pod nazwą SubEnrollService.asmx, udzielając w ten sposób dostępu kontu użytkownika, który ma przeprowadzić zastrzeganie na serwerze licencji. Plik SubEnrollService.asmx znajduje się w katalogu wirtualnym Certification na serwerze głównej certyfikacji.
