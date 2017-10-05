---
TOCTitle: Wycofywanie serwerów
Title: Wycofywanie serwerów
ms:assetid: '52005e2e-9563-4ba0-906c-3cc76f9c378f'
ms:contentKeyID: 18123272
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747568(v=WS.10)'
---

Wycofywanie serwerów
====================

Potrzebę wycofania serwera programu RMS mogą spowodować różne czynniki, między innymi:

-   Problemy ze sprzętem lub jego modernizacja, w wyniku czego dochodzi do wymiany określonych serwerów.
-   Zmniejszenie ruchu związanego z licencjonowaniem i publikacją, powodujące likwidację niektórych serwerów.
-   Prawnie narzucony obowiązek usunięcia serwerów z pewnych miejsc, skutkujący likwidacją całego klastra.
-   Fuzja lub sprzedaż działów lub innych jednostek organizacji, która powoduje przeniesienie aktywów.
-   Fuzja całej organizacji z inną organizacją, która również korzysta z programu RMS, w wyniku czego obie instalacje programu RMS stają się nadmiarowe.

Przed wycofaniem serwera należy utworzyć kopię zapasową wszystkich używanych przez niego baz danych programu RMS, a w szczególności bazy danych konfiguracji. Aby uzyskać więcej informacji dotyczących tworzenia kopii zapasowych baz danych, zobacz „Tworzenie kopii zapasowych systemu RMS i jego przywracanie” w części „Planowanie rozmieszczenia programu RMS” w tym zestawie dokumentacji. .

Po utworzeniu kopii zapasowej baz danych można usunąć serwer. Wymagania związane z usuwaniem serwera programu RMS zależą od roli tego serwera i topologii instalacji programu RMS:

-   **Usuwanie jednego serwera z klastra**. Jeśli serwer programu RMS przeznaczony do wycofania znajduje się w klastrze, w którym wciąż działają i wymagane są inne serwery tego programu, to w celu usunięcia pojedynczego serwera programu RMS z tego klastra należy usunąć zastrzeżenie i odinstalować program RMS na wycofywanym serwerze, usunąć jego sprzęt z klastra oraz zarchiwizować bazy danych.
    | ![](images/Cc747568.note(WS.10).gif)Uwaga                                                                                                               |
    |--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Przed odinstalowaniem programu RMS konieczne jest usunięcie zastrzeżenia serwerów tylko w klastrze głównej certyfikacji. Proces ten nie jest wymagany w przypadku serwerów licencji. |

-   **Wycofywanie serwera autonomicznego**. Jeśli serwer programu RMS przeznaczony do wycofania jest autonomicznym serwerem tego programu (niewchodzącym w skład wieloserwerowego klastra) i ma być zastąpiony nowym serwerem, należy wykonać następujące kroki: usunąć zastrzeżenie i odinstalować istniejący serwer programu RMS, usunąć go z sieci, a następnie niezwłocznie zainstalować i zastrzec program RMS na nowym serwerze. Nowy serwer programu RMS należy skonfigurować do korzystania z tego samego adresu URL i bazy danych konfiguracji, z których korzystał wycofany serwer programu RMS. Należy pamiętać, że do momentu zainstalowania i zastrzeżenia nowego serwera użytkownicy nie będą mogli użytkować zawartości opublikowanej przez serwer wycofany.
    | ![](images/Cc747568.Important(WS.10).gif)Ważne                                                                                                                                                                                                                           |
    |-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Jeśli zastępowany serwer programu RMS używa sprzętowego modułu zabezpieczeń, wszystkie ustawienia zabezpieczeń należy przenieść na nowy serwer przed zainstalowaniem i zastrzeżeniem na nim programu RMS. Aby uzyskać instrukcje, zobacz dokumentację dostarczoną ze sprzętowym modułem zabezpieczeń. |

-   **Zastępowanie instalacji programu RMS inną, istniejącą instalacją tego programu**. W pewnych okolicznościach może wystąpić potrzeba wycofania instalacji programu RMS i zastąpienia jej inną, istniejącą instalacją tego programu, na przykład w przypadku fuzji dwóch firm, z których każda korzysta z programu RMS.

Usunięcie zastrzeżenia i odinstalowanie serwera powoduje usunięcie tego serwera z tabeli ClusterServer w bazie danych konfiguracji oraz usunięcie bazy danych usług katalogowych z serwera programu SQL Server. Aby uzyskać instrukcje dotyczące usuwania zastrzeżenia i odinstalowywania programu RMS, zobacz „[Usuwanie zastrzeżenia programu RMS](https://technet.microsoft.com/9fa63daa-5fb9-4afd-8371-b38248619857)” i „[Odinstalowywanie programu RMS](https://technet.microsoft.com/885e3b4f-ea32-466f-9f7f-d8440b0f7c28)” w dalszej części tego tematu.
