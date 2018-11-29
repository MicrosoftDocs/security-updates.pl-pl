---
TOCTitle: Szacowanie rozbudowy bazy danych
Title: Szacowanie rozbudowy bazy danych
ms:assetid: '87652cc2-b886-4797-8d40-356669768089'
ms:contentKeyID: 18123338
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747585(v=WS.10)'
---

Szacowanie rozbudowy bazy danych
================================

Szacując ilość pamięci niezbędnej do przechowywania baz danych programu RMS, należy założyć minimalnie 10 megabajtów (MB), a następnie dodatkowy 1 MB na każdych 500 użytkowników bazy danych konfiguracji programu RMS. Baza danych rejestrowania może istnieć na innym serwerze bazy danych niż baza danych konfiguracji.

Jeśli używana jest funkcja rejestrowania programu RMS, musi być możliwa rozbudowa bazy danych rejestrowania o ok. 1 MB dla każdego użytkownika w pierwszej fazie certyfikacji użytkownika, gdy rejestracja odbywa się bardzo często. Na przykład jeśli rozmieszczenie obejmuje 1000 użytkowników, baza danych rejestrowania będzie mieć rozmiar 1 gigabajta (GB), ponieważ każdy z tych użytkowników jest uaktywniony na serwerze certyfikacji programu RMS i ma na nim certyfikat. Podczas wykonywania rutynowych czynności baza danych rejestrowania może rozrastać się w tempie 200 kilobajtów (KB) dla każdego użytkownika dziennie (w przypadku wdrożenia podzielonego na fazy należy założyć dodatkowy 1 MB dla każdego nowego użytkownika dodawanego do systemu).
