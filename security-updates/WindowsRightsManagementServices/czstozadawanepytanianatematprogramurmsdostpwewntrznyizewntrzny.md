---
TOCTitle: 'Często zadawane pytania na temat programu RMS: Dostęp wewnętrzny i zewnętrzny'
Title: 'Często zadawane pytania na temat programu RMS: Dostęp wewnętrzny i zewnętrzny'
ms:assetid: '59c2c51f-6c20-450c-a334-0e1486292074'
ms:contentKeyID: 18123281
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747577(v=WS.10)'
---

Często zadawane pytania na temat programu RMS: Dostęp wewnętrzny i zewnętrzny
=============================================================================

Pytania dotyczące wewnętrznego i zewnętrznego dostępu do programu RMS
---------------------------------------------------------------------

-   [Jakie zmiany należy wprowadzić w konfiguracji zapory połączenia internetowego, aby klienci spoza zapory mogli komunikować się z serwerami RMS?](#bkmk_37)
-   [W jaki sposób wykonuje się instalację z ekstranetem?](#bkmk_38)
-   [Jeśli użytkownik utworzy zawartość chronioną prawami dostępu, a następnie przekaże ją komuś, kto nie ma dostępu do instalacji RMS, czy odbiorca będzie mógł korzystać z tej zawartości?](#bkmk_39)
-   [Jeśli wysyłam wiadomość chronioną prawami dostępu do jednego z moich klientów za pomocą programu Outlook 2003 lub Outlook 2007, czego adresat potrzebuje, by odczytać wiadomość?](#bkmk_40)
-   [Jeśli każda organizacja ma własny serwer RMS, jak mogą one wymieniać zawartość chronioną prawami dostępu?](#bkmk_41)
-   [Czy po wysyłaniu wiadomości elektronicznej chronionej przez program RMS do organizacji zewnętrznej, w której program Outlook nie jest używany, odbiorca może odpowiedzieć na adres odczytany przy użyciu dodatku zarządzania prawami dostępu w programie Internet Explorer?](#bkmk_42)

<span id="BKMK_37"></span>
#### Jakie zmiany należy wprowadzić w konfiguracji zapory połączenia internetowego, aby klienci spoza zapory mogli komunikować się z serwerami RMS?

Zapora musi umożliwiać komputerom zewnętrznym zgłaszanie żądań typu SOAP na serwerze RMS za pomocą protokołu HTTP (port TCP o numerze 80) lub HTTPS (port TCP o numerze 443).

<span id="BKMK_38"></span>
#### W jaki sposób wykonuje się instalację z ekstranetem?

Z zawartością związana jest licencja publikacji z dwoma adresami. Jeden to adres intranetowy, wysyłany przy zastrzeganiu klastra RMS. Drugi to adres ekstranetowy konfigurowany przez administratora RMS. Adres ekstranetowy pozwala klientom uzyskiwać licencje użytkowania z serwera poza zaporą. Adres URL w sieci ekstranet nie może posłużyć do tworzenia nowej zawartości chronionej prawami dostępu. W takim przypadku wymagane jest zastąpienie ustawień rejestru klienta RMS.

<span id="BKMK_39"></span>
#### Jeśli użytkownik utworzy zawartość chronioną prawami dostępu, a następnie przekaże ją komuś, kto nie ma dostępu do instalacji RMS, czy odbiorca będzie mógł korzystać z tej zawartości?

Jeśli użytkownik nie ma połączenia z instalacją RMS przy pierwszym otwarciu chronionej zawartości, użycie tej zawartości nie będzie możliwe.

Należy zaznaczyć, że aplikacje pakietu Office 2003 i nowsze automatycznie uzyskują licencje użytkowania na wiadomości pocztowe chronione prawami dostępu podczas synchronizacji, dzięki czemu pocztę można odczytywać bez połączenia z siecią. Jednak podczas gdy program Outlook 2003 lub nowszy automatycznie zachowuje licencje użytkowania w pamięci podręcznej, ewentualne dokumenty programów Excel 2007, Excel 2003, Word 2007, Word 2003 i PowerPoint 2003 załączone do wiadomości będą miały przypisane te same prawa, co zawierająca je wiadomość. Dokumenty nie są automatycznie synchronizowane przy pobieraniu poczty i muszą być otwierane indywidualnie w czasie, gdy komputer nawiązuje połączenie z siecią w celu uzyskania licencji.

<span id="BKMK_40"></span>
#### Jeśli wysyłam chronioną wiadomość e-mail do jednego z moich klientów za pomocą programu Outlook 2003 lub Outlook 2007, czego adresat potrzebuje, by odczytać wiadomość?

Adresat musi korzystać z programu Outlook 2003 lub 2007 albo modułu dodatkowego do zarządzania prawami dostępu w programie Internet Explorer. Jeśli w organizacji adresata ustanowiono relację zaufania między posiadanymi instalacjami RMS a instalacjami w organizacji nadawcy, odbiorca może odczytać wiadomość bez żadnych dodatkowych zabiegów. Relację zaufania między serwerami RMS ustanawia się przez wymianę certyfikatów licencjodawcy serwera, zawierających ich klucze publiczne.

Jeśli organizacja adresata nie ma infrastruktury RMS albo nie ustanowiono relacji zaufania, można prosić klientów o założenie konta Windows Live™ ID i wysyłanie poczty do adresata przy użyciu uprawnień przypisanych do poświadczeń Windows Live™ ID klienta. Przy takim trybie postępowania licencja użytkowania jest uzyskiwana przy użyciu usługi Microsoft IRM, oferowanej w Internecie. Usługa IRM jest świadczona bezpłatnie, aby umożliwić każdemu skorzystanie z technologii RMS w celach testowych. Decydując się na ochronę zawartości przy użyciu tej usługi, należy mieć na uwadze fakt, że w przyszłości operator może zawiesić jej świadczenie bez uprzedzenia.

<span id="BKMK_41"></span>
#### Jeśli każda organizacja ma własny serwer RMS, jak mogą one wymieniać zawartość chronioną prawami dostępu?

Program RMS korzysta z systemu zaufanych domen użytkowników, w którym certyfikaty użytkowników generowane w jednej instalacji RMS są traktowane jako zaufane w drugiej organizacji.

<span id="BKMK_42"></span>
#### Czy po wysyłaniu wiadomości elektronicznej chronionej przez program RMS do organizacji zewnętrznej, w której program Outlook nie jest używany, odbiorca może odpowiedzieć na adres odczytany przy użyciu dodatku zarządzania prawami dostępu w programie Internet Explorer?

Odbiorca wiadomości pocztowej może odpowiedzieć na wiadomość chronioną prawami dostępu tak samo jak w przypadku zwykłej wiadomości, ale oryginalna treść odebranej wiadomości pozostanie zabezpieczona prawami dostępu w stosunku do odbiorcy pierwotnego. To, w jaki sposób wiadomość e-mail jest pakowana, zależy od aplikacji klienckiej. Oryginalna wiadomość pocztowa może być załączona do odpowiedzi jako zaszyfrowany załącznik albo całkowicie usunięta (ustawienie domyślne w programie Outlook 2003 i Outlook 2007).
