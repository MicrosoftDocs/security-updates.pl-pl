---
TOCTitle: Monitorowanie kolejkowania wiadomości
Title: Monitorowanie kolejkowania wiadomości
ms:assetid: 'a7109399-3a84-4681-874b-f6ea1646b0a0'
ms:contentKeyID: 18123417
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747716(v=WS.10)'
---

Monitorowanie kolejkowania wiadomości
=====================================

Rejestrowanie w programie RMS wysyła zdarzenia do bazy danych rejestrowania za pomocą Usługi kolejkowania wiadomości (nazywanej także MSMQ). Każdy serwer frontonu programu RMS wysyła wiadomości do usługi kolejkowania wiadomości, natomiast usługa odbiornika rejestrowania na każdym serwerze frontonu pobiera wiadomości rejestrowania z kolejki usługi kolejkowania wiadomości i zapisuje je w bazie danych rejestrowania. Jeśli baza danych rejestrowania lub serwer bazy danych stanie się niedostępny lub jeśli usługa odbiornika rejestrowania zostanie zatrzymana, usługa kolejkowania wiadomości będzie przechowywać wiadomości w kolejce. Jeśli planowane jest zamknięcie bazy danych rejestrowania lub serwera bazy danych, zaleca się najpierw zamknąć usługę odbiornika rejestrowania na każdym serwerze frontonu, a następnie ponownie uruchomić usługę odbiornika rejestrowania na każdym serwerze frontonu po ponownym uruchomieniu bazy danych lub serwera bazy danych.

Jeśli w bazie danych wystąpi błąd, a usługa odbiornika rejestrowania będzie wciąż działać, usługa ta nie będzie mogła zapisywać wiadomości rejestrowania w bazie danych. Usługa odbiornika rejestrowania będzie przenosić wiadomości do kolejki „martwych wiadomości” usługi kolejkowania wiadomości do momentu, aż baza danych stanie się dostępna, po czym w bazie danych będą zapisywane nowe wiadomości rejestrowania. Wiadomości znajdujące się w kolejce martwych wiadomości nie zostaną automatycznie zapisane w bazie danych rejestrowania. Aby wyświetlić i usunąć wiadomości znajdujące się w kolejce martwych wiadomości, należy wykonać następujące kroki:

1.  Otwórz przystawkę Zarządzanie komputerem programu Microsoft Management Console (MMC). W tym celu kliknij przycisk **Start**, wskaż polecenie **Wszystkie programy**, wskaż polecenie **Narzędzia administracyjne**, a następnie kliknij polecenie **Zarządzanie komputerem**.
2.  W węźle Usługi i aplikacje w drzewie konsoli kliknij element Kolejkowanie wiadomości, a następnie kliknij element Kolejki prywatne.
3.  Zostaną wyświetlone dwie kolejki. Nazwy obu będą zaczynać się od ciągu „**drms\_logging**”, po którym będzie następować nazwa klastra. Jedna z kolejek będzie mieć nazwę „**drms\_logging\_***&lt;nazwa\_klastra&gt;***\_deadletter**”. Jest to kolejka martwych wiadomości. Kliknij nazwę kolejki, a następnie kliknij kolejkę Wiadomości w kolejce.
4.  Kliknij dwukrotnie każdą wiadomość, aby wyświetlić jej właściwości.
5.  Aby usunąć kolejkę, kliknij prawym przyciskiem myszy kolejkę **Wiadomości w kolejce**, wybierz polecenie **Wszystkie zadania**, a następnie kliknij polecenie **Przeczyść**.

W domyślnej konfiguracji usługa kolejkowania wiadomości przechowuje wszystkie kolejkowane wiadomości, a jedynym ograniczeniem jest wolne miejsce na przechowywanie danych na serwerze. Jeśli kolejka usługi kolejkowania wiadomości zużyje całe dostępne miejsce na dysku twardym, serwer programu RMS nie będzie mógł obsługiwać żądań klientów. Aby temu zapobiec, należy wykonać następujące czynności w celu ograniczenia ilości miejsca na dysku, którego usługa kolejkowania wiadomości używa na potrzeby kolejkowania:

1.  Otwórz przystawkę Zarządzanie komputerem programu Microsoft Management Console (MMC). W tym celu kliknij przycisk Start, wskaż polecenie Wszystkie programy, wskaż polecenie Narzędzia administracyjne, a następnie kliknij polecenie Zarządzanie komputerem.
2.  W węźle Usługi i aplikacje w drzewie konsoli kliknij element Kolejkowanie wiadomości, a następnie kliknij element Kolejki prywatne.
3.  Zostaną wyświetlone dwie kolejki. Nazwy obu będą zaczynać się od ciągu „drms\_logging”. W każdej kolejce wykonaj następujące czynności:
    -   Kliknij przycisk Właściwości.
    -   Zaznacz pole wyboru Ogranicz składowanie wiadomości do (KB), a następnie wpisz wyrażony w kilobajtach całkowity rozmiar wszystkich wiadomości, które mogą być przechowywane w kolejce.

Jeśli kolejka się zapełni, wiadomości przychodzące z programu RMS zostaną odrzucone, a do dziennika zdarzeń systemowych zostanie wysłany poniższy komunikat o zdarzeniu, skojarzony z identyfikatorem zdarzenia 48:

Sending the Property Bag to Message Queuing failed. (Wysłanie zbioru właściwości do Usługi kolejkowania wiadomości nie powiodło się).

Zalecane jest skonfigurowanie narzędzi monitorowania systemu w taki sposób, aby w razie wystąpienia tego zdarzenia generowały stosowne powiadomienie, ponieważ zdarzenie to wskazuje na istnienie problemu związanego z bazą danych rejestrowania.
