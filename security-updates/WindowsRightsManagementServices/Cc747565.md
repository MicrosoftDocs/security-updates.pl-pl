---
TOCTitle: Włączanie i wyłączanie rejestrowania
Title: Włączanie i wyłączanie rejestrowania
ms:assetid: '50ccd827-2d39-41e7-a395-3d5f5836869b'
ms:contentKeyID: 18123269
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747565(v=WS.10)'
---

Włączanie i wyłączanie rejestrowania
====================================

Rejestrowanie dotyczące bieżącego klastra lub serwera włącza się i wyłącza na stronie **Ustawienia rejestrowania**. Wyłączenie rejestrowania powoduje, że usługi sieci Web programu RMS przestają wysyłać rejestrowane dane do kolejki wiadomości rejestrowania. Powoduje to również zatrzymanie usługi odbiornika rejestrowania. Wyłączanie rejestrowania przy użyciu narzędzia do administrowania usługami systemu Windows Serwer 2003 nie jest obsługiwane.

Dzienniki programu RMS są wysyłane do serwera bazy danych za pomocą usługi kolejkowania wiadomości. W przypadku braku połączenia z serwerem bazy danych usługa kolejkowania wiadomości zapisze dzienniki w lokalnej pamięci podręcznej, gdzie będą one przechowywane aż do przywrócenia połączenia. Przy pierwszym włączaniu rejestrowania należy się upewnić, że serwer programu RMS ma połączenie z serwerem bazy danych i że usługa bazy danych została uruchomiona. W przypadku gdy funkcję serwera baz danych pełni SQL Server można sprawdzić, czy dzienniki są zapisywane w bazie danych. W tym celu należy wykonać poniższe kroki:

-   W przystawce SQL Server Enterprise Manager przejdź do bazy danych rejestrowania, rozwiń element **Databases** (Bazy danych), a następnie rozwiń bazę danych, która zawiera bazę danych rejestrowania programu RMS.
-   Kliknij bazę danych rejestrowania, kliknij pozycję **Tables** (Tabele), kliknij prawym przyciskiem myszy tabelę **DRMS\_log\_master**, a następnie kliknij polecenie **Open table return all rows** (Otwórz tabelę – zwróć wszystkie wiersze). Jeśli pliki dzienników są tworzone, będzie widoczny jeden lub kilka plików dzienników.
