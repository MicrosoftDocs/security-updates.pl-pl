---
TOCTitle: Określanie wymagań dostępu
Title: Określanie wymagań dostępu
ms:assetid: 'eb2ce9a5-0430-4811-bd40-4a94a84426a8'
ms:contentKeyID: 18123504
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747790(v=WS.10)'
---

Określanie wymagań dostępu
==========================

Na tym etapie planowania powinien być już zidentyfikowany zakres implementacji programu RMS. Przy ocenie zabezpieczeń systemu RMS należy rozważyć metody umożliwiające ograniczenie zakresu do określonych użytkowników oraz zapewnienie ochrony ich danych również za pomocą najlepszych tradycyjnych metod ochrony informacji. Należy także ograniczyć dostęp do serwera programu RMS dla celów administracyjnych i konfiguracyjnych wyłącznie do zaufanych administratorów. W programie RMS można użyć następujących metod zabezpieczeń dostępu:

-   **Listy kontroli dostępu (ACL)**. Wszystkie usługi sieci Web programu RMS oraz administracyjna witryna sieci Web mogą być chronione za pomocą list kontroli dostępu. Aby z usługi programu RMS korzystali wyłącznie autoryzowani do tego użytkownicy, za pomocą list kontroli dostępu można ograniczyć użytkownikom możliwości łączenia się z usługami certyfikacji i licencjonowania programu RMS. Jest to dobre rozwiązanie, jeżeli możliwości tworzenia zawartości chronionej lub uzyskiwania licencji do tej zawartości mają mieć tylko określone grupy.
-   **Uwierzytelnianie klienta**. Przy próbie uzyskania licencji użytkowania lub certyfikatu można również wymagać od użytkownika uwierzytelniania klienta za pomocą kart inteligentnych lub innych metod. Dzięki temu można wyeliminować ryzyko otwarcia zawartości przez nieautoryzowanego użytkownika za pomocą sesji autoryzowanego użytkownika.
-   **Secure Sockets Layer**. W celu zapewnienia dodatkowej warstwy ochrony można wymagać połączenia SSL pomiędzy klientami programu RMS a serwerem programu RMS. Zaleca się włączenie i wymaganie stosowania protokołu SSL ze 128-bitowym szyfrowaniem dla wszystkich plików usług sieci Web programu RMS. Pliki te mają rozszerzenie .asmx i znajdują się w katalogach wirtualnych Licensing, Certification oraz Admin. Jeśli **administracyjne strony sieci Web programu RMS** mają być otwierane w przeglądarce na komputerze zdalnym, to konieczne jest włączenie protokołu SSL. Jednak nawet po włączeniu protokołu SSL nie będzie możliwe otwieranie strony **Administracja globalna** na komputerze zdalnym.
    Aby uzyskać informacje na temat konfigurowania protokołu SSL na serwerach, zobacz Pomoc programu IIS.

W niektórych organizacjach istnieje potrzeba funkcjonowania wydziałowego systemu licencjonowania, który będzie bezpieczny i odizolowany od innych wydziałów. Serwer programu RMS użyty w tym przypadku udostępnia narzędzia do ustanowienia zasad zarządzania prawami dostępu do informacji. W przypadku posiadania wydziału lub innej gałęzi organizacji, która zajmuje się wyjątkowo cenną zawartością, należy rozważyć skonfigurowanie osobnego serwera licencji lub klastra licencji, aby umożliwić zarządzanie licencjonowaniem i publikowaniem zawartości niezależnie od reszty organizacji. Serwer licencji jest podrejestrowywany w serwerze głównej certyfikacji (lub klastrze), który dostarcza certyfikację i inne usługi dla każdego serwera licencji. Jednak serwery licencji dostarczają własne usługi licencjonowania i publikacji.

Konta użytkowników, listy kontroli dostępu oraz zabezpieczenia fizyczne są kluczowymi elementami rozmieszczenia. Przed zaimplementowaniem programu RMS w środowisku produkcyjnym należy ocenić i według potrzeb zaimplementować wszystkie najważniejsze wskazówki dotyczące zabezpieczeń oraz model zabezpieczeń.
