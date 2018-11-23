---
TOCTitle: Przygotowanie przywracania systemu
Title: Przygotowanie przywracania systemu
ms:assetid: '885c047f-1e3b-4bf5-8248-3a4505759cbb'
ms:contentKeyID: 18123373
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747659(v=WS.10)'
---

Przygotowanie przywracania systemu
==================================

Awaria dowolnego składnika systemu RMS, w tym połączenia internetowego i intranetowego używanego przez serwer programu RMS, serwer certyfikacji programu RMS, każdy z podrejestrowanych serwerów licencji programu RMS lub serwerów bazy danych, na których znajdują się bazy danych konfiguracji programu RMS, może spowodować nieoczekiwaną przerwę w świadczeniu usług. Podczas konfiguracji systemu RMS należy zastanowić się nad potencjalnym negatywnym wpływem, jaki przerwa w świadczeniu usług będzie miała na systemy informatyczne i istotne dane, oraz przygotować się do jak najskuteczniejszego przywrócenia zagrożonych składników.

Awarie serwerów baz danych, na których znajdują się bazy danych konfiguracji programu RMS, są jedną z przyczyn, które mogą uniemożliwić ciągły dostęp do informacji chronionych za pomocą technologii RMS. W tej sekcji omówiono ważne zagadnienia i czynniki związane z przygotowaniem przywracania systemu w wypadku systemu RMS, w tym:

-   [łączność z Internetem,](#bkmk_1)
-   [łączność z intranetem,](#bkmk_2)
-   [usługi certyfikacji i licencjonowania,](#bkmk_3)
-   [serwery baz danych,](#bkmk_4)
-   [usługę Active Directory.](#bkmk_5)

<span id="BKMK_1"></span>
Łączność z Internetem
---------------------

Jeśli użytkownik korzysta z funkcji rejestracji serwera w trybie online, podczas zastrzegania serwer programu RMS wymaga połączenia z Internetem, aby uzyskać certyfikat licencjodawcy serwera (SLC, Server Licensor Certificate) i odnowić go raz w roku. Gdy zbliża się ten czas, serwer certyfikacji powiadamia użytkownika o konieczności odnowienia certyfikatu, rejestrując zdarzenia w dzienniku zdarzeń systemowych. Zdarzenia są rejestrowane miesiąc przed datą wygaśnięcia certyfikatu SLC (identyfikator zdarzenia 16), tydzień przed datą wygaśnięcia certyfikatu SLC (identyfikator zdarzenia 17) oraz gdy certyfikat SLC wygaśnie (identyfikator zdarzenia 18). Na stronie sieci Web Administracja globalna w witrynie administracyjnej sieci Web programu RMS będzie także wyświetlane powiadomienie o zbliżającej się dacie wygaśnięcia certyfikatu SLC. Jeśli używany jest pakiet RMS Management Pack dla Microsoft Operations Manager (MOM), zdarzenia wygaśnięcia generują powiadomienie. Jeśli połączenie internetowe nie jest dostępne na serwerze programu RMS, certyfikatu licencjodawcy serwera nie można odnowić za pomocą przycisku **Odnów** w witrynie administracyjnej sieci Web programu RMS. Wówczas należy wykonać procedurę rejestracji offline w celu zażądania zaktualizowanego certyfikatu.

Najlepiej odnowić certyfikat SLC na długo przed datą jego wygaśnięcia, aby uniknąć komplikacji, jeśli połączenie internetowe miałoby być niedostępne w chwili wygaśnięcia certyfikatu. Serwer programu RMS nie może udostępniać usług RMS bez ważnego certyfikatu SLC. Oznacza to, że użytkownicy nie będą mogli publikować informacji chronionych za pomocą technologii RMS ani uzyskiwać licencji użytkowania oraz certyfikatów kont praw dostępu (RAC, Rights Account Certificate) wymaganych do odczytu informacji chronionych za pomocą technologii RMS. Użytkownicy, którzy wcześniej uzyskali licencje użytkowania i certyfikaty RAC na części zawartości chronionej za pomocą technologii RMS, mogą nadal mieć dostęp do informacji, dopóki nie wygasną ich licencje użytkowania lub certyfikaty RAC.

<span id="BKMK_2"></span>
Łączność z intranetem
---------------------

RMS jest technologią klient-serwer opartą na infrastrukturze sieciowej. Bez działającej sieci intranet serwery programu RMS nie mogą łączyć się z wymaganymi usługami w firmie lub z użytkownikami i udostępniać usług. Bez łączności z intranetem użytkownicy nie mogą uzyskiwać certyfikatów kont praw dostępu (RAC, Rights Account Certificate), certyfikatów licencjodawcy klienta (CLC, Client Licensor Certificate) i licencji użytkowania z serwerów RMS.

Zaleca się, aby organizacje rozważyły zastosowanie nadmiarowych architektur routingu i łączy używanych w wypadku awarii z lokacji zdalnych do lokacji serwerów programu RMS.

Po uzyskaniu certyfikatu CLC dla danego komputera użytkownik może opublikować informacje chronione za pomocą technologii RMS w trybie offline, jeśli nie ma dostępu do serwera programu RMS. Niektóre aplikacje e-mail oparte na technologii RMS są tak skonfigurowane, że automatycznie pobierają licencje użytkowania odpowiednich wiadomości e-mail chronionych za pomocą technologii RMS podczas synchronizacji skrzynki pocztowej. Dzięki temu użytkownik może czytać wiadomości e-mail chronione za pomocą technologii RMS, nawet jeśli połączenie z intranetem nie jest dostępne.

<span id="BKMK_3"></span>
Usługi certyfikacji i licencjonowania
-------------------------------------

System RMS jest oparty przede wszystkim na dwóch katalogach wirtualnych Internetowych usług informacyjnych (IIS) w wersji 6.0. Są to usługi certyfikacji i licencjonowania. Umożliwiają one użytkownikom i ich komputerom rejestrowanie się w środowisku RMS i aplikacjach obsługujących technologię RMS w celu dostępu do informacji chronionych za pomocą technologii RMS oraz ich publikowania. Jeśli te usługi nie są dostępne, użytkownicy mogą uzyskać odmowę korzystania z usług, dopóki usługi nie zostaną przywrócone.

Aby przygotować się na ewentualną niedostępność usługi, należy rozważyć utworzenie serwera certyfikacji oraz klastrów podrejestrowanych serwerów licencjonowania, tak by awaria któregokolwiek z węzłów w klastrze nie miała wpływu na dostępność usługi.

Zaleca się założenie nieco większej wydajności w klastrach, tak by awarie w węzłach nie miały wpływu na wydajność ogólną. Instalując pierwszy serwer certyfikacji i każdy podrejestrowany serwer licencji lub pierwszy podrejestrowany serwer licencji w klastrze, należy dokładnie zapisywać opcje konfiguracji i dane wprowadzone podczas zastrzegania.

<span id="BKMK_4"></span>
Serwery baz danych
------------------

Najważniejszymi składnikami systemu RMS są serwery baz danych, na których znajdują się bazy danych konfiguracji. Każdy serwer systemu RMS lub klaster serwerów wykorzystuje bazy danych do przechowywania informacji dotyczących konfiguracji i rejestracji. Informacje dotyczące konfiguracji są podstawą działania systemu RMS. W tych bazach danych znajduje się certyfikat licencjodawcy serwera, utworzone szablony zasad systemu RMS i lista użytkowników zarejestrowanych w systemie RMS. Jeśli na serwerze systemu RMS nie jest używany sprzętowy moduł zabezpieczeń, w tych bazach znajdują się także klucze publiczne i prywatne serwera systemu RMS. Dzięki kopiom zapasowym baz danych systemu RMS można przywrócić poprzednią instalację systemu RMS na nowym serwerze i odtworzyć system RMS. Negatywne skutki utraty bazy danych zależą od utraconej bazy. Poniżej przedstawiono listę skutków utraty określonych baz danych.

-   **Baza danych konfiguracji** Jeśli ta baza danych nie będzie dostępna podczas pracy serwera RMS, usługi RMS mogą być nadal dostępne, ponieważ system RMS lokalnie buforuje wymagane informacje. Jeśli jednak wystąpi zdarzenie wymagające współpracy usługi RMS z bazą danych konfiguracji, np. rejestracja nowego użytkownika, wystąpi błąd usługi RMS i nowy użytkownik nie będzie mógł pracować z zawartością chronioną za pomocą technologii RMS. Jeśli zostaną wykonane czynności powodujące odrzucenie buforowanych informacji przez serwer systemu RMS, np. ponowne uruchomienie usług IIS lub zaplanowane odświeżenie lokalnej pamięci podręcznej, usługa RMS przestanie działać. Serwer systemu RMS nie będzie mógł wznowić normalnej pracy, dopóki nie będzie dostępna baza danych konfiguracji.
    Jeśli baza danych konfiguracji zostanie uszkodzona lub będzie trwale niedostępna, serwery systemu RMS przestają działać.
-   **Baza danych usług katalogowych** W tej bazie danych znajdują się buforowane informacje dotyczące nazw grup i szczegóły dotyczące ich przynależności uzyskane z serwera wykazu globalnego. Jeśli ta tabela nie jest dostępna przez krótkie okresy czasu, jakość usług RMS nie ulega widocznemu pogorszeniu. Jej głównym zastosowaniem jest zapewnienie nadmiarowości i ograniczenie obciążenia serwera wykazu globalnego.
-   **Baza danych rejestrowania** Jeśli na serwerze systemu RMS włączono rejestrowanie, jest to baza danych, w której ma być przechowywany ten dziennik. Jeśli baza danych jest niedostępna, wpisy dziennika będą umieszczane w kolejce przez usługę kolejkowania wiadomości (MSMQ) na serwerze systemu RMS. W ten sposób może zostać wykorzystane całe wolne miejsce na dysku, o ile nie skonfigurowano inaczej odpowiednich ustawień.

Najlepiej podzielić serwery bazy danych na klastry, aby dostępna była ochrona przed awariami w trybie aktywnej gotowości oczekiwania. Należy także regularnie tworzyć kopie zapasowe baz danych serwerów i klastrów certyfikacji systemu RMS oraz serwerów i klastrów licencji.

Ponadto zaleca się utrzymywanie gotowej kopii zapasowej bazy danych, korzystając z funkcji dostarczania dziennika transakcji. Mimo że może to wymagać dodatkowego sprzętu, pozwala organizacjom na szybsze przywracanie baz danych. W Microsoft IT zaimplementowano tę metodę przywracania bazy danych konfiguracji systemu RMS. W tym celu należy wybrać wirtualną nazwę SQL podczas zastrzegania systemu RMS. Wirtualna nazwa SQL umożliwia mapowanie na rzeczywistą nazwę SQL za pomocą systemu nazw domen (DNS, Domain Name System). Jeśli główny serwer SQL przestanie działać, można łatwo przełączyć się na zapasowy serwer SQL, zmieniając mapowanie nazwy DNS serwera głównego na nazwę serwera zapasowego. Aby uzyskać więcej informacji na temat wewnętrznej implementacji tego rozwiązania w firmie Microsoft, zapoznaj się z przykładem dotyczącym firmy Microsoft Corporation w [witrynie firmy Microsoft w sieci Web](http://go.microsoft.com/fwlink/?linkid=42070) (http://go.microsoft.com/fwlink/?LinkId=42070).

<span id="BKMK_5"></span>
Usługa Active Directory
-----------------------

Na usłudze Active Directory są oparte dwie ważne usługi systemu RMS: uwierzytelnianie użytkowników i usługa wykazu globalnego. Jeśli usługa Active Directory nie jest dostępna, uwierzytelnianie użytkowników nie jest możliwe, a użytkownicy i ich komputery nie mogą rejestrować się w systemie RMS. Do uzyskania certyfikatu RAC niezbędny jest potok certyfikacji. Wymaga on uwierzytelniania. Gdy użytkownik uzyska certyfikat RAC, może uzyskiwać licencje użytkowania bez dalszego uwierzytelniania, ponieważ potok licencjonowania jest domyślnie anonimowy.

Ponieważ działy firmy mogą korzystać z członkostwa w grupach w usłudze Active Directory do definiowania osób, które mają dostęp do informacji chronionych za pomocą technologii RMS, utrata usługi Active Directory uniemożliwiłaby użytkownikom uzyskanie tych licencji. Informacje na temat członkostwa w grupach są domyślnie buforowane na serwerze RMS przez 15 minut, dzięki czemu może być tolerowana tymczasowa utrata usługi wykazu globalnego. Aby zwiększyć lub zmniejszyć czas między aktualizacjami pamięci podręcznej, należy zmodyfikować klucz rejestru kontrolujący czas ważności. Aby uzyskać więcej informacji, zobacz „Modyfikowanie ustawień pamięci podręcznej usługi Active Directory” w części „Obsługa serwerów programu RMS” w tym zestawie dokumentacji.
