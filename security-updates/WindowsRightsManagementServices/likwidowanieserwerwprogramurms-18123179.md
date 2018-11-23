---
TOCTitle: Likwidowanie serwerów programu RMS
Title: Likwidowanie serwerów programu RMS
ms:assetid: '11badb02-62c1-455c-96b7-935bbcb496bc'
ms:contentKeyID: 18123179
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720200(v=WS.10)'
---

Likwidowanie serwerów programu RMS
==================================

Likwidacja serwera programu RMS powoduje zmianę jego zachowania, dzięki czemu serwer ten może udostępnić klucz służący do odszyfrowania zawartości chronionej technologią RMS, którą wcześniej opublikował. Ten klucz umożliwia zapisanie zawartości bez ochrony technologią RMS. Może to być użyteczne, jeśli podjęto decyzję o zaprzestaniu używania ochrony technologią RMS w organizacji.

Serwer w stanie likwidacji powinien działać na tyle długo, aby użytkownicy mogli zapisać swoją zawartość bez ochrony technologią RMS oraz aby administratorzy sieci i systemu mogli wyłączyć korzystanie z usługi w ewentualnych klientach obsługujących technologię RMS.

Likwidowanie można włączyć na stronie sieci Web **Ustawienia zabezpieczeń** w administracyjnej witrynie sieci Web. Po włączeniu likwidowania nie można przywrócić na serwerze standardowej konfiguracji serwera programu RMS. Jeśli instalacja obejmowała zaufane domeny publikacji, również one są likwidowane.

Po włączeniu likwidowania witryna administracyjna sieci Web będzie zawierać tylko stronę **Informacje o zlikwidowanym serwerze**; dalsza administracja nie będzie obsługiwana. Aby ukończyć proces likwidowania serwera, należy wykonać następujące kroki:

1.  Nadaj **grupie usługi programu RMS** uprawnienia do odczytu i wykonywania dotyczące głównego katalogu wirtualnego likwidacji.
2.  Dodaj grupę **Wszyscy** do listy DACL pliku decommissioning.asmx z uprawnieniami do odczytu.
3.  Poinformuj użytkowników o likwidowaniu instalacji programu RMS i poradź im, aby połączyli się z serwerem i zapisali zawartość bez ochrony technologią RMS.
4.  Skonfiguruj wszystkie aplikacje obsługujące technologię RMS w przedsiębiorstwie tak, aby łączyły się ze stroną decommissioning.asmx. W zależności od aplikacji obsługującej technologię RMS tą funkcją może sterować klucz rejestru lub ustawienie Zasady grupy.
5.  Jeśli organizacja korzysta z aplikacji obsługujących technologię RMS, które automatycznie używają danej instalacji w celu publikacji, należy za pomocą zasad grupy tak ustawić wpis rejestru na odpowiednich komputerach, aby aplikacje te korzystały z usługi likwidowania.
6.  Jeśli istnieje przekonanie co do tego, że usunięto ochronę całej zawartości, należy utworzyć kopię zapasową klucza prywatnego serwera, a następnie odinstalować program RMS z tego serwera.
