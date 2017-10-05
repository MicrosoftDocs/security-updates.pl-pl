---
TOCTitle: Konserwacja bazy danych usług katalogowych
Title: Konserwacja bazy danych usług katalogowych
ms:assetid: '911a62f2-c1d6-4091-99b0-b53211be27a7'
ms:contentKeyID: 18123385
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747680(v=WS.10)'
---

Konserwacja bazy danych usług katalogowych
==========================================

Program RMS zawiera bazę danych usług katalogowych, która znajduje się na serwerze bazy danych. Zawiera ona informacje na temat użytkowników, identyfikatorów (np. adresy e-mail), identyfikatorów zabezpieczeń (SID), członkostwa w grupach i identyfikatory alternatywne. Te informacje są pobierane z kwerend LDAP wysyłanych do wykazu globalnego usługi Active Directory przez usługę licencjonowania programu RMS, a następnie buforowane lokalnie w tej bazie danych w celu skrócenia czasu odpowiedzi serwera, gdy użytkownicy żądają licencji użytkowania.

Ponieważ dane przechowywane w tej bazie danych są często wstawiane i usuwane, baza ta może być często fragmentowana. Co pewien czas (codziennie lub raz w tygodniu) należy wykonywać reorganizację bazy danych na podstawie indeksów wszystkich tabel bazy danych DRMS\_DirectoryServices. W ten sposób indeksy są przebudowywane w taki sposób, że fragmentacja danych nie jest konieczna. Fragmentacja danych może być przyczyną niskiej wydajności, a nawet awarii serwera, jeśli będzie wykonywana bez interwencji administratora.

Jeśli jako serwer bazy danych używany jest program SQL Server, reorganizację bazy danych można wykonać za pomocą kreatora konserwacji lub za pomocą własnego skryptu niestandardowego, używając programu SQL Server Agent.

Jeśli podczas reindeksowania bazy danych okaże się, że rozmiar dziennika transakcji jest zbyt duży, można go ograniczyć, zmieniając tryb z Pełnego przywracania na Bulk-Logged przed rozpoczęciem reindeksowania.
