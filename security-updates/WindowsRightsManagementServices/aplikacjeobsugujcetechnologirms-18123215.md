---
TOCTitle: Aplikacje obsługujące technologię RMS
Title: Aplikacje obsługujące technologię RMS
ms:assetid: '30bb5565-81d3-43d9-a64d-cf0c5b990712'
ms:contentKeyID: 18123215
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720231(v=WS.10)'
---

Aplikacje obsługujące technologię RMS
=====================================

W celu tworzenia lub korzystania z zawartości chronionej technologią RMS użytkownicy muszą mieć zainstalowaną aplikację obsługującą technologię RMS, tak jak opisano w tym temacie. Ponadto musi być zainstalowany klient programu RMS, a komputery z niego korzystające muszą być aktywowane. Aby uzyskać więcej informacji, zobacz „[Klient programu RMS](https://technet.microsoft.com/03294fa2-8350-430d-b4b0-03d5169937c2)” i „[Aktywacja komputera RMS](https://technet.microsoft.com/09a0d631-9860-477f-9d10-df61b3bfe125)” w dalszej części tego tematu.

Aplikacje obsługujące technologię RMS umożliwiają autorom zawartości załączanie praw użytkowania, w postaci licencji publikacji, do tworzonych plików w celu kontrolowania sposobu wykorzystywania zawartości. Aplikacje obsługujące technologię RMS przetwarzają również zaszyfrowane informacje o pliku i umożliwiają użytkownikom wykorzystywanie zawartości zgodnie z uprawnieniami zdefiniowanymi w licencji publikacji.

Za pomocą pakietu Rights Management Services Client SDK projektanci mogą tworzyć aplikacje obsługujące technologię RMS, które będą licencjonowały, publikowały i wykorzystywały zawartość chronioną technologią RMS. Aplikacje obsługujące technologię RMS mogą być tworzone dla komputerów działających pod kontrolą systemu operacyjnego Microsoft® Windows® 98 Wydanie drugie lub nowszego.

Projektanci mogą też tworzyć aplikacje serwerowe obsługujące technologię RMS, korzystając z pakietu Rights Management Services Client SDK. Te aplikacje mogą publikować zawartość, ale nie mogą jej wykorzystywać.

Użytkownicy, którzy nie mają innej aplikacji obsługującej technologię RMS do korzystania z zawartości chronionej technologią RMS w poczcie e-mail i na stronach sieci Web, mogą uzyskać i korzystać z dodatku zarządzania prawami dostępu dla programu Microsoft® Internet Explorer. Na przykład użytkownicy usługi Outlook Web Access (OWA) mogą za pomocą dodatku zarządzania prawami dostępu dla programu Internet Explorer korzystać z wiadomości e-mail chronionych technologią RMS.

Dodatek zarządzania prawami dostępu dla programu Internet Explorer można pobrać z [witryny sieci Web firmy Microsoft](http://go.microsoft.com/fwlink/?linkid=14450)(http://go.microsoft.com/fwlink/?LinkId=14450).

| ![](images/Cc720231.note(WS.10).gif)Uwaga                                                                                                                                                                           |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Jeżeli dodatek zarządzania prawami dostępu dla programu Internet Explorer jest używany w systemie Windows XP z dodatkiem Service Pack 2, mogą pojawić się problemy ze zgodnością aplikacji, wynikające z rozszerzonej konfiguracji zabezpieczeń. |

Jeżeli adres URL połączenia z siecią ekstranet dla wszystkich domen w organizacji nie zostanie dodany do listy witryn lokalnego intranetu w programie Internet Explorer, użytkownicy korzystający z dodatku zarządzania prawami dostępu dla programu Internet Explorer będą stale otrzymywali komunikaty z pytaniem o pozwolenie na połączenie z witrynami sieci Web. Niewłaściwa odpowiedź na pytanie komunikatu może spowodować, że klient programu RMS będzie uzyskiwać nowy certyfikat konta praw dla konta użytkownika.

Aby poprawnie skonfigurować te witryny sieci Web w całej organizacji, należy wprowadzić wymagane adresy URL do rejestru jako należące do strefy lokalnego intranetu, za pomocą odpowiedniego skryptu. Strefa lokalnego intranetu domyślnie zapewnia odpowiednio wysoki poziom zabezpieczeń, aby uniknąć pojawiania się tych komunikatów.
