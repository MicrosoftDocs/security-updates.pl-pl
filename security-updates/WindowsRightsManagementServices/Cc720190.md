---
TOCTitle: Planowanie dotyczące zewnętrznych użytkowników programu RMS
Title: Planowanie dotyczące zewnętrznych użytkowników programu RMS
ms:assetid: '107e1338-4dcf-4ed5-a49d-e875cc883db1'
ms:contentKeyID: 18123182
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720190(v=WS.10)'
---

Planowanie dotyczące zewnętrznych użytkowników programu RMS
===========================================================

W tej części topologie, które można zaimplementować, aby umożliwić organizacji i użytkownikom zewnętrznym współużytkowanie zawartości chronionej technologią RMS w Internecie.

Klastry programu RMS dla użytkowników wewnętrznych i zewnętrznych można rozmieszczać za pomocą jednej z następujących opcji:

-   Ustawienie adresu URL klastra głównej certyfikacji na adres URL, który będzie dostępny w Internecie. Należy zapewnić rozpoznawanie adresu URL w sieci intranet przez serwery programu RMS danego klastra. Po wykonaniu tych czynności adres URL licencji publikacji używany przez komputery użytkowników końcowych w celu pobierania licencji będzie dostępny w sieci intranet i Internet.
-   Skonfigurowanie odrębnego klastra programu RMS służącego specjalnie do publikowania w Internecie. W tym klastrze należy publikować zawartość, która ma być licencjonowana w sieci Internet. Jeśli zawartość powinna być dostępna zewnętrznie i wewnętrznie, należy opublikować ją w obu tych lokalizacjach. W innym przypadku użytkownicy muszą mieć możliwość kontaktowania się z serwerem sieci Internet.

Zezwalanie na dostęp użytkownikom zewnętrznym
---------------------------------------------

W instalacji programu RMS można uwzględnić użytkowników zewnętrznych, jeśli zostaną dla nich utworzone konta wewnętrzne, które umożliwią tym użytkownikom uzyskanie dostępu do sieci korporacyjnej za pośrednictwem wirtualnej sieci prywatnej (VPN). Konto może mieć wewnętrzną skrzynkę pocztową lub adres e-mail wskazujący zewnętrzną skrzynkę pocztową.

Jeśli będzie używana wewnętrzna skrzynka pocztowa, podczas publikowania zawartości chronionej technologią RMS autorzy wewnętrzni będą musieli określić adres e-mail skojarzony z wewnętrzną skrzynką pocztową (a nie dowolny adres e-mail, jaki użytkownik zewnętrzny ma poza daną organizacją). Jeśli będzie używana zewnętrzna skrzynka pocztowa, podczas publikowania zawartości chronionej technologią RMS autorzy wewnętrzni będą musieli określać zewnętrzny adres e-mail konta.

Aby zapewnić zabezpieczenia sieci, gdy obsługiwany jest dostęp do sieci użytkowników zewnętrznych, można utworzyć na potrzeby kont partnerów odrębny las usługi Active Directory. Dzięki tej topologii można utworzyć odrębny klaster głównej certyfikacji na potrzeby części systemu RMS dostępnej w Internecie. Umożliwia to użytkownikom zewnętrznym odebranie certyfikatu komputera RMS i certyfikatu konta praw z części klastra głównej certyfikacji dostępnej w Internecie, gdy po raz pierwszy uzyskują dostęp do zawartości chronionej technologią RMS.

Jeśli użytkownik zdecyduje się na zaimplementowanie odrębnego lasu dla partnerów zewnętrznych, który będzie zawierać konta partnerów, w lesie tym musi być zainstalowany program RMS. Następnie można użyć funkcji zaufanej domeny publikacji programu RMS, aby ustanowić relację zaufania między dwoma serwerami programu RMS. Zewnętrzne rekordy DNS muszą także określać adres URL klastra zewnętrznego instalacji programu RMS w lesie utworzonym dla partnerów zewnętrznych. Utworzenie tej relacji zaufania pozwala zewnętrznemu serwerowi programu RMS na wystawianie licencji użytkowania dla całej zawartości wystawionej przez wewnętrzny system RMS i odwrotnie.

Zamiast konfigurowania serwera programu RMS w lesie zewnętrznym można użyć serwera, np. ISA, i za jego pomocą filtrować ruch przychodzący oraz zwracać żądania licencji programu RMS z serwera proxy do wewnętrznego serwera RMS.

Używanie certyfikatów zewnętrznych
----------------------------------

Użytkownikom zewnętrznym można zezwolić na dostęp do zawartości chronionej technologią RMS, jeśli skonfigurowano odrębny serwer RMS jako serwer licencji dostępny w Internecie, opublikowano zawartość z tego serwera licencji, a następnie określono relacje zaufania na tym serwerze.

Dostępna w Internecie część rozmieszczenia programu RMS jest odrębnym serwerem licencji przeznaczonym do użycia w Internecie. Jest to część tego samego klastra co instalacja licencji wewnętrznych i używa tej samej bazy danych i tego samego adresu URL co instalacja licencji wewnętrznych. Jest to jedyny serwer, który może akceptować ruch przychodzący z Internetu.

Gdy użytkownicy zewnętrzni żądają licencji użytkowania z tego serwera licencji RMS, będą używać certyfikatu konta praw z innej usługi certyfikacji RMS, któremu musi zaufać ten serwer licencji.

#### Zaufanie w przypadku certyfikatów kont praw utworzonych na podstawie usługi Passport

W organizacji można określić zaufanie dla certyfikatów kont praw utworzonych na podstawie poświadczeń usługi Microsoft .NET Passport. Te certyfikaty kont wymagają, aby użytkownicy uzyskali certyfikaty kont praw bezpośrednio z usługi certyfikacji firmy Microsoft dostępnej w Internecie.

W tym modelu użytkownicy zewnętrzni odbierają certyfikaty komputerów RMS i certyfikaty kont praw z firmy Microsoft. Po opublikowaniu zawartości konta usługi Microsoft .NET Passport użytkowników zewnętrznych muszą mieć nazwy odbiorców w licencji publikacji.

Konto usługi Microsoft® .NET Passport musi być zgodne z kontem usługi.NET Passport użytym przez użytkownika podczas pobierania certyfikatu konta praw z firmy Microsoft. Autor musi określić to konto podczas dodawania odbiorców w aplikacji obsługującej technologię RMS. Jeśli konta nie pasują, nie można korzystać z zawartości.

#### Zaufanie w przypadku innych certyfikatów zewnętrznych

Jeśli firma użytkownika zewnętrznego również dysponuje rozmieszczeniem programu RMS, można skonfigurować relację zaufania z taką firmą. W tym celu należy poprosić tę firmę, aby wyeksportowała swój certyfikat licencjodawcy serwera programu RMS i przesłała go użytkownikowi. Następnie można zaimportować ten certyfikat za pomocą konsoli administracyjnej programu RMS do serwera licencji dostępnego w Internecie.
