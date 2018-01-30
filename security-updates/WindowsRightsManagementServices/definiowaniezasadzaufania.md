---
TOCTitle: Definiowanie zasad zaufania
Title: Definiowanie zasad zaufania
ms:assetid: 'e8d78300-4b26-4f15-9e4f-5ae9eb827ef9'
ms:contentKeyID: 18123472
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747711(v=WS.10)'
---

Definiowanie zasad zaufania
===========================

Zaufane domeny użytkowników i publikacji można definiować w następujący sposób:

-   **Zaufane domeny użytkowników**. W wyniku dodania domeny użytkowników program RMS może przetwarzać żądania licencji użytkowania pochodzące od użytkowników, których certyfikaty konta praw zostały wystawione przez instalację programu RMS istniejącą w innym drzewie usługi Active Directory, a więc innymi słowy przez inny klaster głównej certyfikacji. Zaufaną domenę użytkowników dodaje się przez zaimportowanie certyfikatu licencjodawcy serwera z instalacji, której ma dotyczyć zaufanie.
-   **Zaufane domeny publikacji**. W wyniku dodania domeny publikacji jeden serwer programu RMS może wystawiać licencje użytkowania na podstawie licencji publikacji wystawionych przez inny serwer programu RMS. Zaufaną domenę publikacji dodaje się przez zaimportowanie certyfikatu licencjodawcy serwera i klucza prywatnego serwera, którego ma dotyczyć zaufanie.

Aby uzyskać więcej informacji, zobacz sekcje „[Dodawanie i usuwanie zaufanych domen użytkowników](https://technet.microsoft.com/7c440b15-01c4-49f1-b43c-00f67f3388c1)”i „[Dodawanie i usuwanie zaufanych domen publikacji](https://technet.microsoft.com/d87b502d-5497-4ccd-badf-f6807d587cee)” w dalszej części tego tematu. Aby uzyskać instrukcje krok po kroku, zobacz „[Ustanawianie zasad zaufania](https://technet.microsoft.com/6c2be3c2-1837-4de4-a72e-3ba3eec3321d)” w dalszej części tego tematu.
