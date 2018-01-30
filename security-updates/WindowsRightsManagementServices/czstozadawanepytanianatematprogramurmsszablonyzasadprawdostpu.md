---
TOCTitle: 'Często zadawane pytania na temat programu RMS: Szablony zasad praw dostępu'
Title: 'Często zadawane pytania na temat programu RMS: Szablony zasad praw dostępu'
ms:assetid: '01515f08-9844-4c1a-9ab5-a5a60a901b50'
ms:contentKeyID: 18123163
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720175(v=WS.10)'
---

Często zadawane pytania na temat programu RMS: Szablony zasad praw dostępu
==========================================================================

Pytania dotyczące szablonów programu RMS
----------------------------------------

-   [Czy da się narzucić domyślny szablon RMS na całą zawartość tworzoną w ramach organizacji, dzięki czemu dałoby się zapewnić minimalny zestaw uprawnień?](#bkmk_57)
-   [Gdzie są przechowywane szablony zasad programu RMS?](#bkmk_58)
-   [Po utworzeniu szablonów zostają z nimi związane aliasy użytkowników i listy rozpowszechniania. W jaki sposób organizacja o wielu oddziałach może przygotować szablony z jednakowym zestawem podstawowych praw, jednak przydzielać te prawa różnym grupom zależnie od zawartości?](#bkmk_59)
-   [Czy prawa przypisane do dokumentu są statyczne? Jeśli plik zostanie wysłany, a później zaistnieje potrzeba zmiany uprawnień, czy da się to zrobić, skoro licencja publikacji jest już osadzona w pliku, a nie na serwerze zasad RMS?](#bkmk_60)

<span id="BKMK_57"></span>
#### Czy da się narzucić domyślny szablon RMS na całą zawartość tworzoną w ramach organizacji, dzięki czemu dałoby się zapewnić minimalny zestaw uprawnień?

Tak Przy użyciu pakietu programistycznego (SDK) dla programu RMS można opracować własną aplikację, która będzie wymuszała dowolnie wybrane szablony. Jednak implementacja technologii RMS w pakiecie Office 2003 i nowszych wersjach nie obsługuje wymuszania szablonów zawartości.

<span id="BKMK_58"></span>
#### Gdzie są przechowywane szablony zasad programu RMS?

Położenie szablonów jest uzależnione od aplikacji obsługującej technologię RMS. W przypadku pakietu Office 2003 i nowszych wersji jest to ustawienie użytkownika w rejestrze, w następującej lokalizacji:

**HKEY\_CURRENT\_USER\\Software\\Microsoft\\Office\\11,0\\Common\\DRM\\AdminTemplatePath**

lub

**HKEY\_CURRENT\_USER\\Software\\Microsoft\\Office\\12.0\\Common\\DRM\\AdminTemplatePath** dla Microsoft Office 2007.

> [!note]  
> Jeśli ten wpis wskazuje lokalny folder na komputerze klienta, pliki szablonów muszą zostać skopiowane na klienta. Jeśli wpis wskazuje na folder udostępniony w sieci, szablon nie będzie dostępny, jeśli użytkownik jest w trybie offline. 

<span id="BKMK_59"></span>
#### Po utworzeniu szablonów zostają z nimi związane aliasy użytkowników i listy rozpowszechniania. W jaki sposób organizacja o wielu oddziałach może przygotować szablony z jednakowym zestawem podstawowych praw, jednak przydzielać te prawa różnym grupom zależnie od zawartości?

Taki efekt można osiągnąć na dwa sposoby:

-   Utworzyć pojedynczy szablon o nazwie „Informacje poufne”, który będzie licencjonowany dla wszystkich pracowników w danym dziale firmy, a następnie użyć tego szablonu w poczcie elektronicznej adresowanej do konkretnych osób. Zaletą tego rozwiązania jest posiadanie pojedynczego szablonu poczty dla każdego oddziału firmy, przy czym szablon ten otrzymają tylko użytkownicy, do których go wyślemy. Wadą jest zaś to, że każdy użytkownik spoza grupy pierwotnych adresatów może odczytać wiadomość.
-   Innym rozwiązaniem jest utworzenie wielu szablonów, także po jednym na każdą listę rozpowszechniania. Ten sposób zapewnia wyższy poziom szczegółowej kontroli, jednak wymaga przy tym opracowania i obsługi wielu szablonów.

<span id="BKMK_60"></span>
#### Czy prawa przypisane do dokumentu są statyczne? Jeśli plik zostanie wysłany, a później zaistnieje potrzeba zmiany uprawnień, czy da się to zrobić, skoro licencja publikacji jest już osadzona w pliku, a nie na serwerze zasad RMS?

Tak, jest to możliwe, jeśli używany jest szablon zasad programu RMS. Kiedy zawartość jest publikowana przy użyciu szablonu zasad programu RMS, definicja zasad pozostaje na serwerze i może być zmieniana przez administratora także po opublikowaniu zawartości. Gdy użytkownik zwraca się z żądaniem dostępu do zawartości, licencja będzie udzielać uprawnień zgodnie z aktualnymi zasadami zdefiniowanymi na serwerze. W przypadku modyfikacji uprawnień już po wydaniu licencji użytkowania, użytkownik nadal będzie uzyskiwał prawa obowiązujące w momencie wydania licencji. Aby umożliwić stosowanie nowego szablonu praw dostępu po opublikowaniu zawartości, należy włączyć zasady wygasania szablonu i zaznaczyć opcję **Licencje użytkowania dla zawartości muszą być odnawiane co: n dni**. W miejscu parametru n należy określić liczbę dni, po upływie których użytkownik musi wystąpić z żądaniem nowej licencji użytkowania.
