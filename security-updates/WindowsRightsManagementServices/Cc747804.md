---
TOCTitle: Praca z szablonami zasad praw dostępu
Title: Praca z szablonami zasad praw dostępu
ms:assetid: 'ff4f1143-f6b9-4dd8-aa4c-c2cbbf6fdf06'
ms:contentKeyID: 18123519
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747804(v=WS.10)'
---

Praca z szablonami zasad praw dostępu
=====================================

Po utworzeniu szablonu zasad praw dostępu można zarządzać sposobem jego stosowania w organizacji, kontrolując jego rozpowszechnianie wśród autorów.

W programie RMS szablony zasad praw dostępu są przechowywane w bazie danych konfiguracji. Ponadto w określonym udostępnionym folderze przechowywana jest kopia wszystkich szablonów zasad praw dostępu, tak jak opisano w części „[Określanie lokalizacji szablonów zasad praw dostępu](https://technet.microsoft.com/e1bee46d-33db-424f-ba45-1dcedcb883ab)” w dalszej części tego tematu. Należy upewnić się, że szablony są przechowywane w dostępnej lokalizacji sieciowej spełniającej wymagania dotyczące bezpieczeństwa obowiązujące w organizacji. Udostępnianych folderów na szablony nie należy tworzyć w folderach głównych, z których korzysta program RMS, takich jak folder Program Files czy foldery IISRoot.

Podczas publikowania chronionej zawartości autor wybiera szablon zasad praw dostępu do zastosowania spośród szablonów dostępnych na komputerze lokalnym. Aby udostępnić szablony zasad praw dostępu do użytku, administrator musi rozmieścić je na komputerach użytkowników z sieciowego udostępnionego folderu.

Kiedy użytkownik próbuje użyć chronionej zawartości, aplikacja obsługująca technologię RMS uzyskuje z bazy danych konfiguracji najnowszą wersję szablonu zasad praw dostępu, którego użyto do opublikowania zawartości. Następnie aplikacja obsługujące technologię RMS zastosuje ustawienia z szablonu do zawartości. Jeśli szablon zasad praw dostępu zostanie zmodyfikowany na serwerze programu RMS, program RMS odpowiednio zaktualizuje ten szablon zarówno w bazie danych konfiguracji, jak i w udostępnionym folderze (o ile serwer programu RMS jest skonfigurowany tak, aby określał miejsce przechowywania plików kopii szablonów zasad praw dostępu). Zmodyfikowany szablon zasad praw dostępu należy rozmieścić ponownie w systemach klienckich, tak aby użytkownicy mieli na swoich komputerach dostęp do jego najbardziej aktualnej wersji.

Usunięcie szablonu zasad praw dostępu powoduje jego usunięcie z bazy danych konfiguracji, a także z udostępnionego folderu, który określono jako lokalizację, w której są przechowywane kopie szablonów. Nie jest on jednak usuwany z komputerów użytkowników. Z tej lokalizacji trzeba go usunąć ręcznie. Usunięte szablony zasad praw dostępu należy usunąć ze wszystkich komputerów użytkowników. Jeśli się tego nie zrobi, a usunięty szablon zasad praw dostępu zostanie użyty do opublikowania zawartości, program RMS nie będzie mógł wystawić licencji użytkowania na tę zawartość, ponieważ nie będzie mógł w bazie danych konfiguracji odszukać określonego szablonu.

Praca z szablonami zasad praw dostępu obejmuje następujące zadania:

-   **Określanie udostępnionego folderu**. Przed utworzeniem pierwszego szablonu zasad praw dostępu należy określić udostępniony folder, w którym przechowywane będą wszystkie szablony zasad praw dostępu. Aby uzyskać więcej informacji, zobacz „[Określanie lokalizacji szablonów zasad praw dostępu](https://technet.microsoft.com/e1bee46d-33db-424f-ba45-1dcedcb883ab)” w dalszej części tego tematu.
-   **Tworzenie i edytowanie szablonów zasad praw dostępu**. Można utworzyć dowolną liczbę szablonów zasad praw dostępu, jakiej wymaga zarządzanie prawami dostępu w organizacji. Tworząc szablon zasad praw dostępu, definiuje się użytkowników i dotyczące ich prawa. Można także określić sposób zastosowania szablonu zasad praw dostępu do zawartości. Jeśli w późniejszym czasie wystąpi potrzeba zaktualizowania szablonów zasad praw dostępu, będzie można je edytować. Aby uzyskać więcej informacji, zobacz „[Tworzenie i modyfikowanie szablonów zasad praw dostępu](https://technet.microsoft.com/6014176f-ef71-4d29-b3e3-da129c18563d)” w dalszej części tego tematu.
-   **Rozpowszechnianie szablonów zasad praw dostępu**. Aby autor mógł zastosować dany szablon zasad praw dostępu do zawartości, na komputerze autora musi istnieć kopia tego szablonu. Przez zarządzanie rozpowszechnianiem szablonów można określić, którzy autorzy mogą stosować poszczególne szablony zasad praw dostępu. Aby uzyskać więcej informacji, zobacz „[Rozpowszechnianie szablonów zasad praw dostępu](https://technet.microsoft.com/ae6fa26f-d744-4ac9-9eb1-728ffab87bfe)” w dalszej części tego tematu.
-   **Wycofywanie szablonów zasad praw dostępu**. Jeśli szablon zasad praw dostępu stanie się nieodpowiedni do potrzeb, można go usunąć. W takim przypadku należy także usunąć go z komputerów użytkowników, tak aby użytkownicy nie napotykali na problemy przy próbie korzystania z zawartości, która została opublikowana przy użyciu wycofanego szablonu zasad praw dostępu. Aby uzyskać więcej informacji, zobacz „[Wycofywanie szablonów zasad praw dostępu](https://technet.microsoft.com/32bf98c7-edda-4507-a4b8-4c11bddd6e60)” w dalszej części tego tematu.
