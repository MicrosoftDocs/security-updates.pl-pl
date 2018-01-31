---
TOCTitle: Dodawanie i usuwanie zaufanych domen użytkowników
Title: Dodawanie i usuwanie zaufanych domen użytkowników
ms:assetid: '7c440b15-01c4-49f1-b43c-00f67f3388c1'
ms:contentKeyID: 18123328
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747571(v=WS.10)'
---

Dodawanie i usuwanie zaufanych domen użytkowników
=================================================

Domyślnie program RMS nie obsługuje żądań pochodzących od użytkowników, których certyfikaty konta praw zostały wystawione przez inną instalację programu RMS. Można jednak dodać nowe domeny użytkowników do listy zaufanych domen, umożliwiając przetwarzanie takich żądań przez program RMS.

W każdej zaufanej domenie można także dodawać i usuwać określonych użytkowników lub grupy użytkowników. Można również usunąć zaufaną domenę użytkowników, ale nie można z zaufanych domen użytkowników usunąć klastra głównej certyfikacji odpowiadającego danemu lasowi usługi Active Directory. Każdy serwer programu RMS w rozmieszczeniu, w tym serwer głównej certyfikacji, ufa klastrowi głównej certyfikacji znajdującemu się w jego własnym lesie.

Zaufanymi domenami użytkowników można zarządzać w następujący sposób:

-   Aby umożliwić ogólną obsługę zewnętrznych użytkowników, można do listy zaufanych domen dodać usługę Microsoft® .NET Passport. Dzięki temu serwer RMS znajdujący się w firmie może przetwarzać żądania licencji, które zawierają certyfikat konta praw wystawiony przez usługę Microsoft .NET Passport.
-   Aby ufać zewnętrznym użytkownikom z instalacji programu RMS w innej organizacji, można dodać tę organizację do listy zaufanych domen użytkowników. Dzięki temu serwer RMS może przetwarzać żądania licencji, które obejmują certyfikat konta praw wystawiony przez serwer RMS znajdujący się w innej organizacji.
-   Analogicznie, aby umożliwić przetwarzanie żądań licencji pochodzących od użytkowników z własnej organizacji, którzy znajdują się w innym lesie usługi Active Directory, można dodać instalację programu RMS działającą w tym lesie do listy zaufanych domen użytkowników. Dzięki temu serwer RMS znajdujący się w bieżącym lesie może przetwarzać żądanie licencji obejmujące certyfikat konta praw wystawiony przez serwer RMS znajdujący się w innym lesie.
-   Dla każdej zaufanej domeny użytkownika można określić, które domeny e-mail są zaufane. Dla zaufanych domen usługi Passport można określić, których użytkowników i/lub domen poczty e-mail zaufanie nie obejmuje.

Aby dodać instalację programu RMS do listy zaufanych domen użytkowników, należy zaimportować certyfikat licencjodawcy serwera dla instalacji programu RMS, która ma zostać dodana. Administrator musi najpierw wyeksportować certyfikat licencjodawcy serwera z serwera lub klastra, który ma być objęty zaufaniem, a następnie wysłać ten certyfikat do danego użytkownika. Następnie można zaimportować ten plik, określając jego lokalizację. Aby zapisać plik, zalogowany użytkownik musi mieć uprawnienia do danego udostępnionego folderu. Podczas konfigurowania zaufanej domeny użytkowników nie są przenoszone informacje klucza prywatnego.

Aby uzyskać instrukcje krok po kroku dotyczące ustanawiania zaufanych domen użytkowników, zobacz „[Dodawanie zaufanej domeny użytkownika](https://technet.microsoft.com/ed672e58-6272-4ac0-a434-d1d938037e93)” w dalszej części tego tematu.
