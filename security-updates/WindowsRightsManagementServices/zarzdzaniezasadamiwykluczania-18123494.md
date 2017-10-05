---
TOCTitle: Zarządzanie zasadami wykluczania
Title: Zarządzanie zasadami wykluczania
ms:assetid: 'ee31e099-e095-4648-95da-0009fbeb48cb'
ms:contentKeyID: 18123494
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747730(v=WS.10)'
---

Zarządzanie zasadami wykluczania
================================

Przez implementację zasad wykluczania po stronie serwera można odmawiać spełnienia żądań certyfikatów i licencji opartych o certyfikat konta praw lub wersję skrytki. Zasady wykluczania powodują odmowę nowych żądań certyfikatów i licencji zgłoszonych przez podmioty o naruszonym bezpieczeństwie, ale w odróżnieniu od odwołania, zasady wykluczania nie unieważniają podmiotów. Administratorzy mogą także wykluczać aplikacje potencjalnie szkodliwe lub o naruszonym bezpieczeństwie, skutkiem czego nie mogą one odszyfrowywać zawartości chronionej technologią RMS. Ponadto administratorzy mogą wykluczać określone wersje systemu operacyjnego Windows, co powoduje, że na komputerach klienckich wyposażonych w te wersje systemu Windows nie można korzystać z zawartości chronionej prawami.

Wykluczenie jednostki powoduje, że wymieniana jest ona na liście wykluczania w licencjach użytkowania tworzonych przez dany serwer programu RMS. Jeśli po jakimś czasie wystąpi potrzeba usunięcia jednostki umieszczonej wcześniej w zasadach wykluczania, jednostkę tę można usunąć za pomocą strony Zasady wykluczania w administracyjnej witrynie sieci Web. Spowoduje to usunięcie tej jednostki z listy wykluczania. W nowych żądaniach certyfikacji i licencji jednostka ta nie będzie uważana za wykluczoną.

Jeśli wykluczenie jednostki nie nastąpiło nieumyślnie, zaleca się, aby nie usuwać takiej jednostki z zasad wykluczania dopóki nie ma pewności, że wygasły wszystkie certyfikaty wystawione przed utworzeniem zasad wykluczania. W przeciwnym razie zarówno stare, jak i nowe certyfikaty będą pozwalały na odszyfrowanie zawartości, co dla organizacji może być sytuacją niepożądaną.

W tym temacie dostępne są informacje dotyczące zarządzania zasadami wykluczania. Aby uzyskać instrukcje krok po kroku dotyczące wykluczania jednostek, zobacz „[Włączanie zasad wykluczania](https://technet.microsoft.com/bbb1ce50-bc11-41cf-b75b-a6756141908f)” w dalszej części tego tematu.

W tej części omówiono następujące zagadnienia:

-   [Wykluczanie wersji skrytek](https://technet.microsoft.com/e287f026-aab2-43ab-93bc-48087da82f36)
-   [Wykluczanie certyfikatów kont praw](https://technet.microsoft.com/cba5e901-942c-4d06-9865-e6c4648c95e6)
-   [Wykluczanie wersji systemu Windows](https://technet.microsoft.com/8b8a184d-ac0e-4a43-822c-d2fae2faf484)
-   [Wykluczanie aplikacji](https://technet.microsoft.com/b68ae4b2-b9ba-44ae-90cb-c88df600ec86)
