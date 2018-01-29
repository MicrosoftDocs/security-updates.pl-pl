---
TOCTitle: Zabezpieczanie rozmieszczania programu RMS
Title: Zabezpieczanie rozmieszczania programu RMS
ms:assetid: '6de8b636-a824-4844-aefc-f26347abfc14'
ms:contentKeyID: 18123307
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720291(v=WS.10)'
---

Zabezpieczanie rozmieszczania programu RMS
==========================================

Rozmieszczenie programu RMS jest zasobem organizacji, który wymaga takich samych zabezpieczeń fizycznych i zabezpieczeń sieci jak inne krytyczne serwery w infrastrukturze. W ramach rozmieszczania należy zdefiniować zagrożenia i środki zapobiegawcze, które mają dotyczyć serwerów programu RMS.

Program RMS implementuje się jako usługę sieci Web. Dlatego można kontrolować dostęp do niego w taki sam sposób jak w wypadku innych usług sieci Web — korzystając z list kontroli dostępu i protokołu SSL (Secure Sockets Layer).

**Ograniczanie dostępu do usług sieci Web programu RMS za pomocą list kontroli dostępu**

Dostęp do usług programu RMS można ograniczyć za pomocą list kontroli dostępu. Każdy z głównych katalogów wirtualnych, tworzonych, gdy program RMS jest zastrzegany w witrynie sieci Web, ma odpowiednią strukturę folderów, którą można zabezpieczyć. Domyślnie struktura folderów znajduje się w następującej lokalizacji: &lt;dysk\_systemowy&gt;:\\&lt;*folder\_główny\_sieci\_Web*&gt;\\\_wmcs. Zmienna *folder\_główny\_sieci\_Web* jest nazwą folderu przypisaną do witryny sieci Web, na której zastrzeżono program RMS. Niektóre usługi sieci Web, np. usługa podrejestrowywania, usługa certyfikacji urządzeń przenośnych i certyfikacji usług serwera, są domyślnie zastrzeżone i użytkownicy lub grupy, które mają mieć możliwość korzystania z usługi, muszą zostać jawnie dodani do listy kontroli dostępu.

Usługa certyfikacji usług serwera umożliwia tworzenie certyfikatów kont praw dostępu (RAC, Rights Account Certificate), za pomocą których można uzyskiwać dostęp do usług chronionych za pomocą programu RMS, np. usług współpracy w sieci Web, serwerów poczty i serwerów zarządzania dokumentami, w celu obsługi rozszerzenia systemu RMS, np.:

-   Serwera współpracy nad dokumentami, gdzie użytkownicy mogą załadować dokumenty, które nie są chronione, ale pobrane dokumenty są automatycznie chronione przez program RMS zgodnie z zasadami praw dla danego typu zawartości. Przykładem tego może być program Microsoft Office SharePoint Server 2007.
-   Systemu zarządzania dokumentami, który spełnia rolę głównego repozytorium i archiwum dokumentów, zarówno chronionych, jak i niechronionych. System może indeksować dokumenty chronione na podstawie praw na potrzeby wyszukiwania przy jednoczesnym zachowaniu zasad praw zdefiniowanych przez twórcę zawartości.
-   Włącz serwer poczty, aby szybko otworzyć zawartość chronią na podstawie praw w celu skanowania w poszukiwaniu wirusów, spamu lub w ramach postępowania według przepisów albo zasad dotyczących poczty obowiązujących w firmie.

Ponieważ te scenariusze wymagają licencji w imieniu użytkowników, wymagane jest, aby możliwość uzyskania certyfikatów kont praw dostępu do usługi była ograniczona tylko do tych serwerów w danej organizacji, które zostały zatwierdzone pod kątem realizacji takiej funkcji, i były one odpowiednio zabezpieczone.

**Ograniczanie dostępu do usług sieci Web programu RMS za pomocą protokołu SSL**

Zaleca się włączenie i wymaganie stosowania protokołu SSL (Secure Sockets Layer) ze 128-bitowym szyfrowaniem dla wszystkich plików usług sieci Web programu RMS. Pliki te mają rozszerzenie .asmx i znajdują się w katalogach wirtualnych Licensing, Certification oraz Admin. Protokół SSL wymaga, aby na serwerze był zainstalowany ważny certyfikat SSL dla danej witryny sieci Web. Jeśli protokół SSL zostanie zastosowany dla folderu instalacji programu RMS \_wmcs, podfoldery i pliki dziedziczą to ustawienie. Aby uzyskać więcej informacji na temat plików usług sieci Web i katalogów wirtualnych, zobacz „Internetowe usługi informacyjne (IIS)” w części „Informacje techniczne dotyczące programu RMS” w tym zestawie dokumentacji.

> [!note]  
> Jeśli administracyjne strony sieci Web programu Windows RMS mają być otwierane w przeglądarce na komputerze zdalnym, to konieczne jest włączenie protokołu SSL. Jednak nawet po włączeniu protokołu SSL nie będzie możliwe otwieranie strony **Administracja globalna** na komputerze zdalnym. Aby uzyskać więcej informacji na temat zdalnego administrowania programem RMS, zobacz „Korzystanie ze strony głównej administracji” w części dotyczącej operacji w programie RMS w tym zestawie dokumentacji. 

**Ustawianie silnego hasła klucza prywatnego**

Hasło klucza prywatnego służy do generowania i bezpiecznego przechowywania klucza prywatnego w bazie danych konfiguracji programu RMS. Silne hasło jest zalecane w celu zapewnienia maksymalnego poziomu zabezpieczeń. Jeśli konieczne jest zapisanie hasła, należy go umieścić w fizycznie zabezpieczonym obszarze.

> [!Caution]  
> Jeśli hasło klucza prywatnego zostało zgubione lub jest nieznane, a serwer programu RMS nieoczekiwanie przejdzie w tryb offline, konieczne będzie odszyfrowanie wszystkich dokumentów programu RMS, odtworzenie środowiska programu RMS oraz ponowne zaszyfrowanie wszystkich danych za pomocą nowego klucza prywatnego. 
