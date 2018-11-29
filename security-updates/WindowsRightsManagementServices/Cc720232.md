---
TOCTitle: Hierarchia zaufania w programie RMS
Title: Hierarchia zaufania w programie RMS
ms:assetid: '2d44182f-a653-4383-aba1-dade53f7cf9a'
ms:contentKeyID: 18123211
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720232(v=WS.10)'
---

Hierarchia zaufania w programie RMS
===================================

Na składniki systemu RMS składają się: usługa rejestrowania firmy Microsoft, serwery programu RMS w organizacji, komputery klienckie oraz użytkownicy systemu. Każdy składnik otrzymuje certyfikat określający jego tożsamość w systemie. Hierarchia zaufania określa relację zaufania między tymi certyfikatami oraz jednostkami, do których certyfikaty należą. Określa również relacje zaufania między jednostkami zaufanymi i licencjami, które wystawiają one innym jednostkom zaufanym.

Hierarchia zaufania łączy certyfikaty i licencje w łańcuch zaufania, który program RMS może zawsze prześledzić od danego certyfikatu lub licencji aż do zaufanej pary kluczy. Łańcuch zaufania zawiera aktualny certyfikat, certyfikat jednostki, która go wystawiła, certyfikat jednostki, która wystawiła certyfikat tej jednostki, itd., aż do głównego poziomu zaufania.

Dla programu RMS głównym poziomem zaufania, czyli „kotwicą zaufania”, jest para kluczy firmy Microsoft. Ten wspólny główny poziom zaufania umożliwia organizacji stworzenie ekosystemu zaufania, który zawiera jednostki zaufane, takie jak użytkownicy i partnerzy, zarówno wewnątrz, jak i na zewnątrz organizacji.

Poniższy diagram przedstawia hierarchię zaufania w organizacji. Łańcuch zaufania prowadzi do usług firmy Microsoft wystawiających podstawowe certyfikaty.

![](images/Cc720232.6c169175-94fb-4ec0-93bc-12748aae3ac4(WS.10).gif)
1.  Każdy komputer kliencki otrzymuje unikatową skrytkę zawierającą główny klucz publiczny firmy Microsoft.
2.  Po otrzymaniu żądania licencji program RMS sprawdza obiekty główne, przechodząc ścieżkę w hierarchii zaufania aż do głównego poziomu zaufania.
3.  Program RMS sprawdza autentyczność jednostki zaufanej wymienionej w licencji.
4.  Program RMS sprawdza, czy certyfikat jednostki zaufanej został wystawiony przez serwer znajdujący się w hierarchii zaufania.

Na każdym z poziomów łańcucha certyfikatów program RMS sprawdza licencję lub certyfikat, a następnie sprawdza, czy certyfikat lub licencja ma połączenie w ramach łańcucha zaufania ze znanym głównym poziomem zaufania. Każda licencja lub certyfikat w łańcuchu są weryfikowane przez program RMS w celu sprawdzenia poniższych warunków:

-   Czy dane XrML są prawidłowe?
-   Czy podpis obiektu wystawiającego jest prawidłowy?
-   Czy semantyka licencji jest odpowiednia dla zamierzonego użycia?
-   Czy warunki (takie jak daty ważności) są spełnione?
-   Czy licencja nie została odwołana?
-   Czy klucz podpisu licencji oraz certyfikowany klucz obiektu wystawiającego pasują do siebie?
