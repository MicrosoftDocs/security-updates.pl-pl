---
TOCTitle: 'Appendix I: Database Maintenance'
Title: 'Appendix I: Database Maintenance'
ms:assetid: '0077e395-434d-4f60-85a0-ed3091449235'
ms:contentKeyID: 21798554
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Dd939795(v=WS.10)'
---

Appendix I: Database Maintenance
================================

In order to keep your WSUS server functioning correctly, you should have a maintenance plan that includes re-indexing the database on a regular basis, preferably at least once a month.

The [WsusDBMaintenance](http://go.microsoft.com/fwlink/?linkid=87027) script (http://go.microsoft.com/fwlink/?LinkId=87027) allows you to re-index any version of the WSUS database, either SQL Server or Wewnętrzna baza danych systemu Windows.

If you are using Wewnętrzna baza danych systemu Windows, you will need to use the **sqlcmd** utility. For more information about the **sqlcmd** utility, see [sqlcmd Utility](http://go.microsoft.com/fwlink/?linkid=81183) (http://go.microsoft.com/fwlink/?LinkId=81183).

        ```
where *&lt;scriptLocation&gt;* is the directory where you have copied the WsusDBMaintenance script.
