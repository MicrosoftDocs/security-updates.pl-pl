---
TOCTitle: Rozmieszczanie list odwołania
Title: Rozmieszczanie list odwołania
ms:assetid: 'e331338b-66d4-45e4-8d3f-acccf2302ac4'
ms:contentKeyID: 18123465
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747702(v=WS.10)'
---

Rozmieszczanie list odwołania
=============================

Do implementacji odwołania konieczne jest rozmieszczenie list odwołania. Listy odwołania określają zawartość, aplikacje, użytkowników lub inne podmioty, które zostały odwołane. Rozmieszczać można zarówno organizacyjne listy odwołania, jak i listy odwołania od firmy Microsoft.

Rozmieszczanie organizacyjnych list odwołania
---------------------------------------------

Aby móc używać szablonu zasad praw dostępu wraz z listą odwołania, należy udostępnić tę listę odwołania komputerom klienckim w organizacji. Aby uzyskać informacje dotyczące tworzenia list odwołania, zobacz „Implementowanie odwołania” we wcześniejszej części tego tematu.

Organizacyjną listę odwołania można rozmieścić, wykonując następujące kroki:

1.  Skopiuj plik listy odwołania na publicznie dostępny serwer sieci Web. Ponieważ użytkownicy korzystający z chronionej zawartości mogą pochodzić spoza organizacji, określona lokalizacja powinna być dostępna dla wszystkich użytkowników, zarówno wewnątrz sieci, jak i znajdujących się poza nią.  
    Rozpowszechnianie pliku listy odwołania wśród komputerów klienckich może trochę potrwać. Dlatego możliwe jest, że w momencie, gdy użytkownicy spróbują otworzyć dokument wymagający listy odwołania, nie będą mieć na swoich komputerach klienckich dostępu do takiej listy. Jeśli na komputerze klienckim nie ma listy odwołania, aplikacja obsługująca technologię RMS może pobrać tę listę z lokalizacji określonej w licencji użytkowania.
    Najlepszym rozwiązaniem jest utworzenie skryptu, który co dzień automatycznie podpisuje i kopiuje listę odwołania do witryny sieci Web. Daje to gwarancję, że nie powstanie sytuacja, w której użytkownicy nie będą mogli korzystać z zawartości z powodu dysponowania nieaktualną listą odwołania. Aby zapoznać się z przykładowym skryptem, zobacz „Korzystanie z narzędzia Podpisywanie listy odwołania” we wcześniejszej części tego tematu.
2.  W szablonie zasad praw dostępu określ interwał odświeżania organizacyjnej listy odwołania o wartości większej od zera. Daje to gwarancję, że lista odwołania nie będzie opcjonalna. Jeśli lista będzie aktualizowana rzadko, na przykład tylko w razie naruszenia zabezpieczeń, można ustawić długi interwał odświeżania, a następnie do rozprowadzenia listy odwołania wśród komputerów klienckich stosownie do potrzeb stosować skrypty lub ustawienia zasad. Aby uzyskać informacje dotyczące ustawiania interwałów odświeżania, zobacz „Definiowanie zasad odwołania” we wcześniejszej części tego tematu. Aby uzyskać więcej informacji dotyczących konfigurowania szablonów zasad praw dostępu, zobacz „Tworzenie i modyfikowanie szablonów zasad praw dostępu” w dalszej części tego tematu.
3.  W szablonie zasad praw dostępu określ adres URL, z którego można pobrać listę odwołań.
4.  Możesz opcjonalnie rozmieścić listę odwołania na komputerach klienckich przez użycie automatycznej metody, na przykład zasad grup lub programu Systems Management Server (SMS).

Rozmieszczanie list odwołania od firmy Microsoft
------------------------------------------------

Aby klient Usług zarządzania prawami dostępu (RMS) mógł korzystać z listy odwołania od firmy Microsoft, listę tę należy rozmieścić na komputerach klienckich. W tym temacie opisano sposoby rozmieszczania listy odwołania od firmy Microsoft z uwzględnieniem następujących scenariuszy:

-   Organizacja chce rozmieścić własną listę odwołania oraz listę odwołania od firmy Microsoft.
-   Organizacja chce rozmieścić tylko listę odwołania od firmy Microsoft.

Po opublikowaniu listy odwołań przez firmę Microsoft można ją pobrać z następujących lokalizacji:

-   Serwery programu RMS będą mogły pobrać listę odwołań za pomocą usługi Windows Update.
-   Jeżeli serwer programu RMS nie jest podłączony do Internetu, lista odwołań opublikowana przez firmę Microsoft będzie dostępna do pobrania także w Centrum pobierania firmy Microsoft.

Jeśli pakiet listy odwołania pobierany jest na serwer programu RMS, zostanie zapisany w folderze %systemdrive%\\Program Files\\Windows Rights Management Services Revocation List. Jeśli pakiet listy odwołania pobierany jest na komputer innego typu, można wybrać lokalizację pobierania. Ten pakiet zawiera plik wykonywalny CRL\_Update.exe, który można uruchomić w celu zainstalowania wszystkich klienckich list odwołania w magazynie licencji klienta, a także plik listy odwołania Msrl.xml, który można skopiować do witryny sieci Web lub do udostępnionego foldera publicznego.

**Aby rozmieścić listę odwołania własnej organizacji i listę odwołania od firmy Microsoft**
1.  Aby rozmieścić listę odwołania własnej organizacji, wykonaj instrukcje zawarte we wcześniejszej części tego tematu „[Rozmieszczanie list odwołania](https://technet.microsoft.com/e331338b-66d4-45e4-8d3f-acccf2302ac4)”.

2.  Pobierz pakiet listy odwołania firmy Microsoft i rozmieść go na wszystkich komputerach klienckich w organizacji przy użyciu odpowiedniej metody, na przykład zasad grup lub programu Systems Management Server (SMS). Można także skopiować wpisy z listy odwołania firmy Microsoft do organizacyjnej listy odwołania i rozmieścić tylko organizacyjną listę odwołania.

> [!Caution]  
> Firma Microsoft występuje jako podmiot w łańcuchu zaufania we wszystkich certyfikatach i licencjach wystawianych przez program RMS. Dlatego też lista odwołania wystawiona przez firmę Microsoft obowiązuje we wszystkich żądaniach powiązania, dla których uzyskiwana jest licencja użytkowania, zgodnie z szablonem zasad praw dostępu, który wymaga organizacyjnej listy odwołania. Ponadto lista odwołania firmy Microsoft jest rejestrowana na komputerze klienckim. 

**Aby rozmieścić tylko listę odwołania firmy Microsoft**
1.  Pobierz pakiet listy odwołania firmy Microsoft.

2.  Zmodyfikuj istniejące szablony zasad praw dostępu, tak aby wymagały odwołania, a jeśli szablony zasad praw dostępu nie istnieją, utwórz szablon wymagający odwołania. Użyj klucza publicznego firmy Microsoft przy określaniu warunku odwołania.

3.  Podaj jako interwał odświeżania bardzo dużą liczbę, na przykład 50 000. Taka liczba daje gwarancję, że lista odwołania opublikowana przez firmę Microsoft nigdy nie wygaśnie. Z tego względu rozprowadzane licencje użytkowania nie będą wymagały nowej wersji listy odwołania firmy Microsoft, jeśli nie będzie ona dostępna.

4.  Skopiuj plik listy odwołania na publicznie dostępny serwer sieci Web. Ponieważ użytkownicy korzystający z chronionej zawartości mogą pochodzić spoza organizacji, określona lokalizacja powinna być dostępna dla wszystkich użytkowników, zarówno wewnątrz sieci, jak i znajdujących się poza nią.

5.  Udostępnienie listy odwołania jest konieczne, ponieważ rozpowszechnianie pliku tej listy wśród komputerów klienckich może zająć dużo czasu. Dlatego możliwe jest, że w momencie, gdy użytkownik spróbuje otworzyć dokument z licencją publikacji wymagającą odwołania, nie będzie mieć na swoim komputerze lokalnego dostępu do listy odwołania. Jeśli na komputerze klienckim nie ma listy odwołania, aplikacja obsługująca technologię RMS może pobrać tę listę z określonej lokalizacji.

6.  W szablonie zasad praw dostępu określ adres URL, z którego można pobrać listę odwołań. Aby uzyskać więcej informacji dotyczących konfigurowania szablonów zasad praw dostępu, zobacz „[Tworzenie i modyfikowanie szablonów zasad praw dostępu](https://technet.microsoft.com/6014176f-ef71-4d29-b3e3-da129c18563d)” w dalszej części tego tematu.

7.  Można opcjonalnie rozmieścić pakiet listy odwołania na komputerach klienckich, używając odpowiedniej metody, na przykład zasad grup lub programu SMS. Dzięki temu użytkownicy będą mogli otwierać zawartość chronioną technologią RMS, która wymaga list odwołania, nawet jeśli nie będą podłączeni do sieci.
