---
TOCTitle: Zaufanie dla certyfikatów konta praw utworzonych na podstawie usługi Passport
Title: Zaufanie dla certyfikatów konta praw utworzonych na podstawie usługi Passport
ms:assetid: 'c096fa36-c40d-4b28-843c-e9cbbe8eef70'
ms:contentKeyID: 18123408
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747655(v=WS.10)'
---

Zaufanie dla certyfikatów konta praw utworzonych na podstawie usługi Passport
=============================================================================

Firma Microsoft udostępnia usługę certyfikacji kont, która korzysta z poświadczeń programu Microsoft .NET Passport w celu ustanowienia certyfikatu konta praw dostępu dla użytkownika. Aby użytkownicy z certyfikatami konta praw dostępu w ramach tej usługi mogli uzyskiwać licencje z klastra RMS, konieczne jest skonfigurowanie zaufanej domeny użytkowników, która będzie akceptować poświadczenia użytkowników z usługi certyfikacji konta firmy Microsoft.

Aby użyć tej funkcji, należy skonfigurować Internetowe usługi informacyjne do przyznania dostępu anonimowego do usługi licencjonowania programu RMS. Ten krok jest istotny dla użytkowników zewnętrznych, ponieważ usługa licencjonowania została skonfigurowana w taki sposób, aby domyślnie korzystała z uwierzytelniania zintegrowanego systemu Windows. Jeśli dostęp anonimowy nie został ustawiony, użytkownicy zewnętrzni z certyfikatami konta praw utworzonych na podstawie usługi Passport (RAC) nie będą mogli uzyskać licencji.

Zaufanie dla certyfikatów konta praw utworzonych na podstawie usługi Passport
-----------------------------------------------------------------------------

#### Aby włączyć dostęp anonimowy do usługi licencjonowania programu RMS

1.  Otwórz przystawkę **Menedżer internetowych usług informacyjnych (IIS)** i rozwiń serwer obsługujący program RMS.

2.  W drzewie konsoli rozwiń węzeł **Witryny sieci Web**, a następnie rozwiń witrynę sieci Web ze skonfigurowanym programem RMS. Domyślnie jest to **Domyślna witryna sieci Web**.

3.  W drzewie konsoli rozwiń witrynę sieci Web **\_wmcs**, a następnie wybierz katalog wirtualny **licensing**.

4.  Kliknij prawym przyciskiem myszy katalog wirtualny **licensing**i wybierz polecenie **Właściwości**.

5.  W oknie dialogowym **Właściwości licencjonowania** kliknij kartę **Zabezpieczenia katalogów**.

6.  Klikniij polecenie **Edytuj** w obszarze **Uwierzytelnianie i kontrola dostępu**.

7.  Zaznacz pole wyboru **Włącz dostęp anonimowy**.

#### Zaufanie dla certyfikatów konta praw utworzonych na podstawie usługi Passport

1.  Otwórz stronę **Administracja globalna**, a następnie obok witryny sieci Web, w której mają być zaufane certyfikaty kont praw utworzonych na podstawie usługi Passport, kliknij łącze **Administruj programem RMS w tej witrynie sieci Web**.

2.  W obszarze **Łącza administracyjne** kliknij łącze **Zasady zaufania**.

3.  W obszarze **Zaufane domeny użytkowników** kliknij opcję **Ufaj certyfikatom RAC usługi Passport**. Pozycja Microsoft RM Certification Service zostanie wyświetlona na liście **Zaufane domeny użytkowników**.

4.  Opcjonalnie można wykluczyć użytkowników na podstawie ich adresów e-mail. W tym celu kliknij opcję **Wykluczone tożsamości**, a następnie wpisz adres e-mail użytkownika, który nie jest zaufany.
