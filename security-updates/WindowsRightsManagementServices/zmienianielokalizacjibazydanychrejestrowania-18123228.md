---
TOCTitle: Zmienianie lokalizacji bazy danych rejestrowania
Title: Zmienianie lokalizacji bazy danych rejestrowania
ms:assetid: '34ea8045-dc94-422e-9601-29927cfc1534'
ms:contentKeyID: 18123228
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720238(v=WS.10)'
---

Zmienianie lokalizacji bazy danych rejestrowania
================================================

W domyślnej konfiguracji programu RMS baza danych konfiguracji i baza danych rejestrowania znajdują się na tym samym serwerze. Należy regularnie sprawdzać, czy na serwerze programu SQL Server istnieje wystarczająca ilość miejsca zarówno na bazę danych rejestrowania, jak i konfiguracji.

Jeśli baza danych rejestrowania zrobi się zbyt duża, można w dowolnej chwili przenieść ją na inny serwer. Bazy danych rejestrowania nie można przenieść przy użyciu administracyjnej witryny w sieci Web. Trzeba to zrobić ręcznie, wykonując następujące kroki:

1.  Wyłącz rejestrowanie w sposób opisany w „[Włączanie lub wyłączanie rejestrowania](https://technet.microsoft.com/8e672f95-566f-4070-9a2a-2f70f087148f)” w dalszej części tego tematu.
2.  Skopiuj bazę danych rejestrowania z serwera źródłowego na docelowy za pomocą programu SQL Server Enterprise Manager. Upewnij się, że w nowej bazie danych zostały utworzone tabele i procedury przechowywane. Jednym z możliwych sposobów wykonania tej czynności jest użycie Kreatora kopiowania bazy danych w programie SQL Server Enterprise Manager.
3.  Wprowadź zmiany w bazie danych konfiguracji, tak aby uwzględniała nowe nazwy serwera i bazy danych. W tabeli DRMS\_ClusterPolicies w bazie danych konfiguracji klastra, w którym przenoszona jest baza danych, wykonaj następujące czynności:
    -   Zmień wartość zasad LoggingDatabaseServer, tak aby odzwierciedlały nową nazwę serwera bazy danych.
    -   Zmień wartość zasad LoggingDatabaseName, tak aby odzwierciedlały nową nazwę bazy danych.

    | ![](images/Cc720238.note(WS.10).gif)Uwaga                                                                                                                                                                                                              |
    |-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Program SQL Server Enterprise Manager nie współpracuje z polami db\_variant, tak więc nie można użyć go do wykonania tego zadania. Zamiast niego można skorzystać z programu Query Analyzer, dostarczanego z programem SQL Server, lub z innego narzędzia do edytowania baz danych. |

4.  Uruchom ponownie usługi IIS na wszystkich serwerach wchodzących w skład klastra.
5.  Ponownie włącz rejestrowanie.
