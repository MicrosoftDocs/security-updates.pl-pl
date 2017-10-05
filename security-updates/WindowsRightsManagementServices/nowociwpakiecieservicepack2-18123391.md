---
TOCTitle: Nowości w pakiecie Service Pack 2
Title: Nowości w pakiecie Service Pack 2
ms:assetid: 'a944cb73-d900-42bb-b7aa-92916dead408'
ms:contentKeyID: 18123391
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747629(v=WS.10)'
---

Nowości w pakiecie Service Pack 2
=================================

Program Rights Management Services (RMS) z dodatkiem Service Pack 2 (SP2) oferuje obsługę następujących funkcji:

-   **Macierzysta obsługa programu Microsoft® SQL Server™ 2005**. W poprzednich wersjach programu RMS do korzystania z programu SQL Server 2005 wymagane było zastosowanie obejścia. Aby uzyskać więcej informacji o tym obejściu, zobacz artykuł 913372 w bazie wiedzy Microsoft Knowledge Base ([http://go.microsoft.com/fwlink/?LinkId=68638](http://go.microsoft.com/fwlink/?linkid=68638)). Problem ten usunięto w wersji RMS z dodatkiem SP2.
-   **Microsoft Office SharePoint® Server 2007**. W tej wersji zapewniono obsługę programu Office SharePoint Server 2007. Biblioteka dokumentów programu Office SharePoint Server 2007 automatycznie stosuje uprawnienia RMS do pobieranych dokumentów, bazując na prawach programu Office SharePoint Server 2007. Jest to możliwe dzięki instalacji klienta RMS z dodatkiem SP2 na serwerze Office SharePoint Server 2007. Nie zaleca się instalowania na tym samym komputerze serwera RMS z dodatkiem SP2 i programu Office SharePoint Server 2007.
-   **Lepsze zabezpieczenie wiadomości przeznaczonych do bazy danych rejestrowania**. W tej wersji wszystkie wiadomości usługi kolejkowania z serwerów RMS do bazy danych rejestrowania RMS są podpisane cyfrowo.
-   **Większe rozmiary żądań wsadowych serwerów**. W obecnej wersji aplikacje obsługujące RMS mogą pobierać wiele licencji użytkowania dla różnych kont użytkownika poprzez pojedyncze żądanie licencji skierowane do serwera RMS. Zwiększa to wydajność dzięki redukcji obciążenia wieloma żądaniami licencji dla tej samej porcji zawartości chronionej prawami dostępu.
-   **Rozszerzone przechodzenie grup między lasami**. W tej wersji przechodzenie grup RMS między lasami odbywa się przy użyciu żądań protokołu SOAP (Simple Object Access Protocol) przesyłanych do nowej usługi sieci Web ASP.NET, która pracuje na serwerze RMS.
