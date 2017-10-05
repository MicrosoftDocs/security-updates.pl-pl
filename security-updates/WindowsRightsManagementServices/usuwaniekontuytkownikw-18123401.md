---
TOCTitle: Usuwanie kont użytkowników
Title: Usuwanie kont użytkowników
ms:assetid: 'bf73b141-d4d1-4807-a773-3aaff58b0db6'
ms:contentKeyID: 18123401
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747653(v=WS.10)'
---

Usuwanie kont użytkowników
==========================

Gdy z usługi Active Directory zostanie usunięte konto użytkownika, nie powoduje to automatycznego usunięcia wpisu odpowiadającego certyfikatowi konta praw tego użytkownika, który znajduje się w tabeli kluczy użytkowników w bazie danych konfiguracji klastra głównej certyfikacji. Z tego powodu, w wyniku dodawania nowych kluczy bez usuwania starych, tabela kluczy użytkowników może rozrastać się bez ograniczeń.

W celu obsługi bazy danych konfiguracji można uruchomić procedurę przechowywaną, która usunie odpowiedni klucz użytkownika na podstawie jego identyfikatora zabezpieczeń (SID) w momencie, gdy w usłudze Active Directory nastąpi usunięcie skojarzonego z nim konta użytkownika. Inne rozwiązanie to okresowe uruchamianie skryptu, który usuwa z bazy danych konfiguracji wszystkie klucze użytkowników, z którymi w usłudze Active Directory nie są skojarzone identyfikatory SID. Należy pamiętać, że ta czynność powoduje znaczące obciążenie zarówno serwera programu SQL Server, jak i usługi Active Directory.
