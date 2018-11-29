---
TOCTitle: Rozmieszczanie programu RMS w wielu lasach
Title: Rozmieszczanie programu RMS w wielu lasach
ms:assetid: 'd531dfdc-efff-4eb0-8d99-f1fd19d7a963'
ms:contentKeyID: 18123437
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747685(v=WS.10)'
---

Rozmieszczanie programu RMS w wielu lasach
==========================================

Jeśli organizacja ma wiele lasów Active Directory i użytkownik chce umożliwić korzystanie z programu RMS w całej organizacji, należy upewnić się, że skonfigurowano sieć w sposób umożliwiający programowi RMS identyfikowanie i uwierzytelnianie kont użytkowników oraz grup dystrybucyjnych pochodzących z różnych lasów.

Program RMS korzysta z usługi Active Directory przy identyfikacji użytkowników i grup dystrybucyjnych. Jeśli rozmieszczenie usługi Active Directory w organizacji obejmuje wiele lasów, program RMS wykorzystuje obiekty kontaktowe do uzyskania informacji o tożsamościach użytkowników i grup należących do innego lasu niż serwer programu RMS. W tym celu muszą zostać spełnione trzy warunki:

1.  W innych lasach muszą istnieć serwery certyfikacji RMS; dla każdej grupy zdalnej muszą być zdefiniowane obiekty kontaktowe.
2.  W lasach zawierających obiekty kontaktowe muszą istnieć rozszerzenia schematu, dzięki którym będzie możliwe odwoływanie się tych obiektów do lasów zawierających obiekty rzeczywiste.
3.  Atrybuty obiektów kontaktowych muszą być zsynchronizowane, aby obiekty odwoływały się do lasów zawierających obiekty rzeczywiste.

Przykładowa konfiguracja lasów zakłada definiowanie grup i zarządzanie nimi w jednym lesie, a definiowanie użytkowników i zarządzanie nimi w innym. Użytkownik chce przypisać prawa do zawartości w oparciu o członkostwo w pewnej grupie. W tym scenariuszu *RMS\_Server\_U* jest serwerem w lesie zawierającym konta użytkowników, a *RMS\_Server\_G* jest serwerem w lesie zawierającym konta grup. Między tymi dwoma serwerami programu RMS utworzono zaufaną domenę użytkownika. Aby serwer *RMS\_Server\_U* mógł pomyślnie rozszerzyć członkostwo w grupie określonej w licencji publikacji poza granice lasu, w lokalnym lesie usługi Active Directory musi istnieć obiekt kontaktowy przedstawiający grupę w lesie zdalnym. Program RMS może odczytać atrybuty obiektu kontaktowego i uzyskać informację, że ten obiekt reprezentuje grupę w innym lesie. Następnie może wyszukać serwer programu RMS w tym lesie i określić, czy między nim a innym serwerem programu RMS istnieje relacja zaufania. Gdy serwer *RMS\_Server\_U* wyśle kwerendę do usługi Active Directory dotyczącą grupy zdefiniowanej w licencji publikacji, obiekt kontaktowy rozpozna, że grupa należy do innego lasu. Gdy serwer *RMS\_Server\_U* przekazuje żądanie do serwera programu RMS wymienionego na liście w punkcie połączenia usługi (SCP) tej domeny. Punkt połączenia usługi rozpoznaje serwer *RMS\_Server\_G* jako serwer certyfikacji programu RMS domeny. Następnie serwer *RMS\_Server\_U* wysyła kwerendę do serwera *RMS\_Server\_G*, aby uzyskać członkostwo grupy.

Atrybutem, do którego skierowana jest kwerenda programu RMS z prośbą o informacje, jest **msExchOriginatingForest**. Ten atrybut jest instalowany domyślnie w schemacie usługi Active Directory, jeśli w lesie jest zainstalowany program Exchange Server 2003. Atrybut ten musi znajdować się w lesie każdego schematu usługi Active Directory, który będzie współpracować z programem RMS. Jeśli użytkownik nie korzysta z programu Exchange Server 2003, może dodać te rozszerzenia schematu, pobierając zestaw RMS Administration Toolkit. Zestaw ten zawiera plik schematu i instrukcje dotyczące dodawania tego schematu do usługi Active Directory.

Atrybuty te muszą być zsynchronizowane, tak by obiekt kontaktowy odwoływał się do obiektu rzeczywistego w innych lasach. Po dodaniu tego atrybutu do schematu usługi Active Directory należy skonfigurować jego wartość, aby był w pełni kwalifikowaną nazwą domeny (FQDN) lasu, w którym znajduje się grupa, na przykład corp.fabrikam.com.

W tym celu można użyć programu Microsoft Identity Integration Server (MIIS) 2003 lub Identity Integration Feature Pack (IIFP) i agenta zarządzania dla globalnej listy adresów (GAL) usługi Active Directory.

Należy przyznać lokalnemu serwerowi programu RMS odpowiednie prawa do przeszukiwania zdalnej usługi Active Directory oraz do wywołania interfejsów .NET Remoting w zdalnej instalacji programu RMS.

Obsługa rozszerzania grup między lasami wymaga, aby konto używane dla konta usługi programu RMS w każdym lesie miało uprawnienia do odczytu i wykonywania dla usługi Active Directory. Program RMS automatycznie udziela uprawnień do odczytu usługi Active Directory wszystkim uwierzytelnionym użytkownikom, którzy posiadają poświadczenia domeny. Aby zwiększyć poziom zabezpieczeń, można usunąć ten dostęp ze swobodnej listy kontroli dostępu (DACL) i zastąpić go indywidualnymi kontami usługi występującymi w różnych lasach.

W zależności od relacji zaufania usługi Active Directory pomiędzy lasem lokalnym i lasami zdalnymi uprawnienia wymagane dla konta usługi programu RMS mogą się różnić. Poniższa lista przedstawia modele zaufania i wymagane uprawnienia:

-   **Istnieje dwustronna relacja zaufania**. Lokalny las programu RMS ufa i jest zaufany w lesie, z którego pochodzi grupa. Konto usługi programu RMS dla serwera programu RMS w każdym z lasów może być dowolnym prawidłowym kontem domeny w lesie. Należy upewnić się, że lokalne konto usługi programu RMS zostanie dodane do listy DACL folderu \\Inetpub\\wwwroot\\\_wmcs\\drmRemote na wszystkich serwerach programu RMS w lesie, z którego pochodzi grupa.
-   **Istnieje jednostronna relacja zaufania**. Lokalny las programu RMS ufa lasowi, z którego pochodzi grupa, ale nie jest zaufany w tym lesie. Konto usługi programu RMS dla wszystkich serwerów programu RMS w organizacji powinno pochodzić z prawidłowego konta domeny w zaufanym lesie. To konto należy dodać do listy DACL folderu \\Inetpub\\wwwroot\\\_wmcs\\drmRemote na wszystkich serwerach programu RMS w lesie, z którego pochodzi grupa.
-   **Brak relacji zaufania**. Lasy w organizacji nie mogą uwierzytelniać użytkowników i grup z innych lasów. Nie zaleca się używania rozszerzania grupowego na wiele lasów, jeśli między odpowiednimi lasami nie ma relacji zaufania. Jeśli jednak jest to konieczne, można zastosować ten scenariusz, konfigurując konto usługi programu RMS jako prawidłowe konto domeny w obu lasach. W obu lasach należy używać tej samej nazwy użytkownika i hasła. Ponadto na każdym serwerze frontonu programu RMS musi być utworzone lokalne konto komputera, który musi mieć dokładnie taką samą nazwę użytkownika i hasło, jak konta domeny używane dla konta usługi programu RMS w obu lasach. Dzięki temu lokalna usługa automatycznie uzyska odpowiednie uprawnienia do uwierzytelniania zdalnej usługi Active Directory i zdalnego programu RMS.

Korzystanie z zasad zaufania programu RMS
-----------------------------------------

Jeśli program RMS jest rozmieszczany w organizacji z wieloma lasami, serwer certyfikacji programu RMS należy rozmieścić w każdym lesie, w którym znajdują się konta użytkowników, którzy będą należeć do systemu RMS. Jeśli użytkownicy z różnych lasów mają mieć możliwość współużytkowania zawartości chronionej technologią RMS, trzeba skonfigurować zasady zaufania programu RMS, tak by można było ufać certyfikatom i licencjom generowanym przez inny serwer programu RMS. Istnieją dwie zasady zaufania, których można używać z programem RMS, zaufane domeny użytkowników i zaufane domeny publikacji. Zaufane domeny użytkowników umożliwiają serwerowi programu RMS zaufanie certyfikatom kont praw dostępu generowanym przez inny serwer certyfikacji programu RMS i wystawianie licencji użytkowania użytkownikom posiadającym certyfikaty kont praw dostępu z innych serwerów. Zaufane domeny publikacji umożliwiają serwerowi programu RMS generowanie licencji użytkowania na podstawie licencji publikacji definiujących inny serwer licencji.

Oto niektóre opcje umożliwiające używanie zasad zaufania w wielu lasach:

-   Klaster certyfikacji programu RMS w każdym lesie z jednym klastrem licencjonowania współużytkowanym przez wszystkich użytkowników. Klaster licencjonowania programu RMS zostanie skonfigurowany za pomocą zaufanej domeny użytkownika obejmującej wszystkie klastry certyfikacji programu RMS. Klientów programu RMS konfiguruje się za pomocą klucza rejestru w celu nawiązania połączenia z klastrem licencjonowania w celu uzyskania licencji użytkowania.
-   Klaster certyfikacji i licencjonowania programu RMS w każdym lesie przy zaufanej domenie użytkowników skonfigurowanej w każdym klastrze, tak by ustanowić relację zaufania z serwerami programu RMS w innych lasach. Każdy użytkownik będzie używać serwera programu RMS we własnym lesie w celu uzyskania licencji użytkowania i może wykrywać serwer licencji za pomocą punktu połączenia usługi w usłudze Active Directory.
-   Jeśli użytkownicy zawartości chronionej technologią RMS należą do lasu, który nie ma dostępu do lasu, w którym opublikowano tę zawartość, można utworzyć zaufaną domenę publikacji, aby możliwe było licencjonowanie i używanie zawartości. Zaufane domeny publikacji wymagają zaimportowania klucza prywatnego serwera programu RMS do publikacji zawartości.

Aby uzyskać więcej informacji dotyczących konfigurowania zasad zaufania, zobacz „Zarządzanie zaufaniem i zasady zaufania” w części „Obsługa serwerów programu RMS” w tym zestawie dokumentacji.
