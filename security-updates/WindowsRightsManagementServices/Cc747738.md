---
TOCTitle: Zaufane domeny publikacji
Title: Zaufane domeny publikacji
ms:assetid: 'bca1c33a-d3ef-42b5-adbe-6e104979a71f'
ms:contentKeyID: 18123435
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747738(v=WS.10)'
---

Zaufane domeny publikacji
=========================

Domyślnie serwery programu RMS nie wystawiają licencji użytkowania dla licencji publikacji wystawionych przez serwer programu RMS znajdujący się w innym klastrze. Jednak w niektórych sytuacjach ten sam serwer lub klaster nie może wystawiać licencji publikacji i licencji użytkowania dla chronionej zawartości. Może tak się stać, gdy dany klaster programu RMS zostanie wycofany i jego miejsce zajmie inny, na przykład gdy dwie firmy się połączą. W takiej sytuacji klaster programu RMS musi mieć możliwość wystawiania licencji użytkowania dla licencji publikacji utworzonych przez inny klaster programu RMS.

Można skonfigurować klaster programu RMS, tak aby ufał licencjom publikacji wystawionym przez inny klaster programu RMS i wystawiał dla nich licencje użytkowania. Aby to zrobić, można zaimplementować zaufaną domenę publikacji. W tym celu należy zaimportować certyfikat licencjodawcy serwera oraz klucz prywatny z innego serwera, a następnie dodać go do listy zaufanych domen publikacji. Zaimportowane klucze prywatne są używane tylko do deszyfrowania podpisanych licencji publikacji, a nie do podpisywania nowych licencji.

Aby uzyskać więcej informacji o zaufanych domenach użytkowników i instrukcjach krok po kroku, zobacz „Dodawanie i usuwanie zaufanych domen publikacji” i „Ustanawianie zasad zaufania” w części „Obsługa serwerów programu RMS” w tym zestawie dokumentacji.
