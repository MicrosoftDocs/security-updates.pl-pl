---
TOCTitle: Szablony zasad praw dostępu
Title: Szablony zasad praw dostępu
ms:assetid: 'eee931c8-7c98-48e9-9e2c-d0b7bd4f2b96'
ms:contentKeyID: 18123495
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747732(v=WS.10)'
---

Szablony zasad praw dostępu
===========================

Szablony zasad praw dostępu określają standardowy zestaw użytkowników, praw i warunków, które można zastosować do zawartości chronionej technologią RMS. Kiedy użytkownik zastosuje szablon zasad praw dostępu do elementu zawartości, prawa dostępu określone w tym szablonie stają się elementem licencji publikacji. 

W witrynie sieci Web Administracja programem RMS można tworzyć szablony zasad praw dostępu, a także usuwać lub modyfikować istniejące szablony. Szablony zasad praw dostępu mogą zawierać różne warunki, takie jak określone grupy odbiorców lub grupy usługi Active Directory, okres ważności licencji użytkowania dla zawartości, okres czasu, przez jaki zawartość może być używana, licząc od momentu publikacji, a nawet wartości niestandardowe, mające znaczenie dla danej aplikacji obsługującej technologię RMS. Szablon może wymagać listy odwołania. Szablon określa adres URL pliku listy oraz liczbę dni, przez jaką lista jest ważna. Gdy użytkownik żąda licencji użytkowania opartej na szablonie, system sprawdza listę odwołania, zanim użytkownik będzie mógł używać zawartości chronionej technologią RMS. Aby uzyskać więcej informacji, zobacz „[Odwoływanie w programie RMS](https://technet.microsoft.com/72689f90-f3c5-4b61-94ea-d825f3199b3b)” w dalszej części tego tematu.

Przykłady praw umieszczanych w szablonach zasad praw dostępu przedstawiono poniżej:

-   Każdy użytkownik może przeglądać zawartość, ale tylko autor może ją modyfikować.
-   Każdy użytkownik w firmie może przeglądać zawartość, ale tylko przez miesiąc od momentu jej publikacji.
-   Każdy członek przedsiębiorstwa może przeglądać zawartość, ale nie mogą jej przeglądać partnerzy zewnętrzni ani klienci.
-   Tylko określeni odbiorcy mogą przeglądać zawartość.
-   Tylko określony odbiorca może przeglądać lub modyfikować zawartość.

Szablony mogą zawierać różne warunki, na przykład:

-   Określone grupy odbiorców lub grupy usługi Active Directory mające prawa dostępu do zawartości.
-   Okres ważności licencji użytkowania dla zawartości.
-   Okres czasu od momentu publikacji, przez który można używać zawartości.
-   Wymaganie listy odwołania dla licencji użytkowania oraz częstotliwość odświeżania tej listy.
-   Wartości niestandardowe, mające znaczenie dla określonej aplikacji obsługującej technologię RMS.

Szablony zasad praw dostępu są przechowywane w bazie danych konfiguracji oraz w folderze udostępnionym. Administrator programu RMS jest odpowiedzialny za rozpowszechnianie szablonów zasad praw dostępu z folderu udostępnionego do komputerów klienckich, tak aby autorzy mogli z nich korzystać. Aby uzyskać więcej informacji, zobacz „Rozpowszechnianie szablonów zasad praw dostępu” w sekcji „Obsługa serwerów programu RMS” w tym zestawie dokumentacji.

W aplikacji obsługującej technologię RMS autorzy mogą wybrać szablon zasad praw dostępu określający zwykle grupy, których członkowie mogą korzystać z zawartości. Gdy użytkownik żąda licencji użytkowania, serwer stosuje szablon zasad praw dostępu z bazy danych. Dzięki temu warunki licencji użytkowania zawsze odpowiadają aktualnej wersji szablonu.
