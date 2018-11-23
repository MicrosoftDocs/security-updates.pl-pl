---
TOCTitle: Wprowadzanie zmian w bazie danych konfiguracji
Title: Wprowadzanie zmian w bazie danych konfiguracji
ms:assetid: '6a7bec73-09e4-4060-b551-5990836df4bc'
ms:contentKeyID: 18123297
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747606(v=WS.10)'
---

Wprowadzanie zmian w bazie danych konfiguracji
==============================================

Zmiany konfiguracji wprowadzane przy użyciu administracyjnej witryny sieci Web są odzwierciedlane w bazie danych konfiguracji danego serwera lub klastra. Zdecydowanie zaleca się zmianę ustawień konfiguracyjnych z poziomu administracyjnej witryny sieci Web, a nie przez ręczne zmienianie danych w bazie danych konfiguracji. Istnieją jednak dwie sytuacje, w których może być wymagane ręczne wprowadzenie zmian w bazie danych:

-   **Przenoszenie bazy danych rejestrowania na inny serwer.**Domyślnie baza danych rejestrowania jest instalowana na tym samym serwerze, co baza danych konfiguracji. Jeśli zostanie podjęta decyzja o przeniesieniu bazy danych rejestrowania na inny serwer, należy zmodyfikować bazę danych konfiguracji, tak aby odnosiła się do nowej lokalizacji. Aby uzyskać więcej informacji dotyczących przenoszenia bazy danych rejestrowania, w tym aktualizowania bazy danych konfiguracji w nowej lokalizacji, zobacz temat „[Zmienianie lokalizacji bazy danych rejestrowania](https://technet.microsoft.com/34ea8045-dc94-422e-9601-29927cfc1534)”.
-   **Usuwanie kluczy użytkownika skojarzonych z certyfikatami konta praw**. Jeśli ma miejsce usunięcie konta użytkownika z usługi Active Directory lub wykluczenie albo odwołanie certyfikatu konta praw za pomocą administracyjnej witryny sieci Web, klucze użytkownika skojarzone z certyfikatem konta praw z bazy danych konfiguracji nie są usuwane. Należy ręcznie usunąć nieaktywne klucze użytkownika z bazy danych konfiguracji, po części ze względów bezpieczeństwa, a po części po to, aby ułatwić śledzenie liczby licencji dostępu klienta (CAL). Aby uzyskać więcej informacji dotyczących usuwania kluczy użytkownika z bazy danych konfiguracji, zobacz sekcję „[Usuwanie kont użytkowników](https://technet.microsoft.com/bf73b141-d4d1-4807-a773-3aaff58b0db6)” we wcześniejszej części tego tematu. Aby uzyskać więcej informacji dotyczących śledzenia licencji CAL, zobacz sekcję „[Śledzenie certyfikatów konta praw](https://technet.microsoft.com/5bb0f3cf-fc44-4e60-a93f-c789d6f8a902)” we wcześniejszej części tego tematu.

Jeśli wymagane jest wprowadzenie zmian bezpośrednio w bazie danych konfiguracji, należy skontaktować się z administratorem bazy danych serwera.
