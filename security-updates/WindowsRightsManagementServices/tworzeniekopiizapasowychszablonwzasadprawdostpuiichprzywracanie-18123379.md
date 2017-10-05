---
TOCTitle: Tworzenie kopii zapasowych szablonów zasad praw dostępu i ich przywracanie
Title: Tworzenie kopii zapasowych szablonów zasad praw dostępu i ich przywracanie
ms:assetid: 'a6ed3328-4128-45e8-9236-3de484b460de'
ms:contentKeyID: 18123379
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747625(v=WS.10)'
---

Tworzenie kopii zapasowych szablonów zasad praw dostępu i ich przywracanie
==========================================================================

Aby zapewnić ochronę cennych szablonów zasad praw dostępu, należy regularnie tworzyć na nośniku kopie zapasowe danych szablonów przechowywanych w bazie danych konfiguracji i przechowywać ten nośnik w bezpiecznym miejscu. W ten sposób w razie ewentualnej awarii systemu będzie można przywrócić szablony zasad praw dostępu z kopii zapasowej.

Wykonaj jedną z następujących czynności:

-   Utworzyć kopię zapasową całej bazy danych konfiguracji, łącznie z danymi szablonów zasad praw dostępu. Aby uzyskać więcej informacji dotyczących tworzenia kopii zapasowej bazy danych programu SQL Server, zobacz dokumentację programu SQL Server.
    — lub —
-   Utworzyć kopię zapasową tylko danych szablonów zasad praw dostępu, które znajdują się w bazie danych konfiguracji. Czynność tę można wykonać przez wyeksportowanie informacji GUID i TemplateData z tabeli DRMS\_RightsTemplate do nowego pliku tekstowego. Aby uzyskać więcej informacji dotyczących eksportowania danych z bazy danych programu SQL Server, zobacz dokumentację programu SQL Server.

Jeśli zajdzie potrzeba przywrócenia danych szablonów zasad praw dostępu znajdujących się w bazie danych konfiguracji, można wyodrębnić informacje GUID i TemplateData z tabeli DRMS\_RightsTemplate w kopii zapasowej bazy danych konfiguracji lub po prostu zaimportować te dane z pliku tekstowego. Aby uzyskać więcej informacji dotyczących wykonywania tych zadań, zobacz dokumentację programu SQL Server.

| ![](images/Cc747625.note(WS.10).gif)Uwaga                                                                            |
|---------------------------------------------------------------------------------------------------------------------------------------------------|
| Aby określić plan tworzenia kopii zapasowych szablonów zasad praw dostępu, należy skonsultować się z administratorem serwera programu SQL Server. |
