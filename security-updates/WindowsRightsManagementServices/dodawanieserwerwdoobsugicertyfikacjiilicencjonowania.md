---
TOCTitle: Dodawanie serwerów do obsługi certyfikacji i licencjonowania
Title: Dodawanie serwerów do obsługi certyfikacji i licencjonowania
ms:assetid: '089ceb62-2a96-444f-ab42-1d5deaabd0c3'
ms:contentKeyID: 18123170
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720189(v=WS.10)'
---

Dodawanie serwerów do obsługi certyfikacji i licencjonowania
============================================================

Po zainstalowaniu i zastrzeżeniu pierwszego serwera i ustanowieniu głównej instalacji programu RMS można skonfigurować dodatkowe serwery w celu uzyskania rozbudowanej obsługi usług licencjonowania i certyfikacji. Na przykład:

-   Można dodać serwer jako członka klastra głównej certyfikacji w celu uzyskania dodatkowej obsługi certyfikacji i licencjonowania. Serwer dodany do tego klastra korzysta z tej samej konfiguracji i z tych samych baz danych, co serwer głównej certyfikacji.
-   Można skonfigurować osobny serwer licencji lub uczynić go członkiem klastra serwerów licencji. W takim wypadku jest on podrejestrowany w klastrze głównej certyfikacji i przypisywany jest mu unikatowy certyfikat licencjodawcy serwera (SLC) za pomocą usług certyfikacji serwera głównej certyfikacji. Wszystkie żądania usług certyfikacji kierowane do serwera licencji są przekazywane do serwera certyfikacji. Serwer licencji może wystawiać licencje użytkowania i licencje publikacji bez wysyłania żądań do serwera głównej certyfikacji.

Stosowana opcja zależy od rozmiaru organizacji i pożądanego sposobu implementowania nadmiarowości, skalowalności, zabezpieczeń oraz obsługi równoważenia obciążenia. Jeśli dodatkowe serwery programu RMS są rozmieszczane w celu obsługi narastających potrzeb certyfikacji, licencjonowania i publikowania, należy rozmieścić serwery programu RMS jako część serwera głównej certyfikacji, tak aby możliwe było skonfigurowanie nadmiarowości i równoważenia obciążenia na wszystkich serwerach. Można dodawać serwery certyfikacji w klastrze i odciążać usługi licencjonowania i publikowania poprzez podrejestrowanie serwerów licencji (które mogą także tworzyć klaster w celu równoważenia obciążenia), ale nie można równoważyć obciążenia w podrejestrowanym klastrze licencji, używając klastra głównej certyfikacji.

Wskazówki dotyczące tego zadania można znaleźć w następujących tematach:

-   [Role, uprawnienia oraz prawa wymagane do instalacji i zastrzegania](#bkmk_1)
-   [Proces zastrzegania dla dodatkowych serwerów certyfikacji i licencjonowania](#bkmk_2)
-   [Konfigurowanie klastrów i równoważenia obciążenia](#bkmk_3)

<span id="BKMK_1"></span>
Role, uprawnienia oraz prawa wymagane do instalacji i zastrzegania
------------------------------------------------------------------

Do zainstalowania i zastrzeżenia dodatkowych serwerów potrzebne są te same role, uprawnienia i prawa co do skonfigurowania serwera początkowego. Ponadto wymagane są także też uprawnienia od serwera głównej certyfikacji do konfigurowania osobnego serwera licencji, noszące nazwę podrejestrowywania. Serwer głównej certyfikacji jest kontrolowany za pomocą listy DACL z pliku SubEnrollService.asmx. Członkowie grupy RMS Service Group, w tym konto usługi programu RMS zdefiniowane podczas zastrzegania serwera głównej certyfikacji, mają uprawnienia do podrejestrowania. Aby uzyskać więcej informacji, zobacz [Konfigurowanie usług certyfikacji i licencjonowania na pierwszym serwerze](https://technet.microsoft.com/cce29a2f-984f-48ed-9187-0eb68286ec5b) we wcześniejszej części tego tematu.

<span id="BKMK_2"></span>
Proces zastrzegania dla dodatkowych serwerów certyfikacji i licencjonowania
---------------------------------------------------------------------------

Dodawanie serwerów do klastrów certyfikacji i licencji wymaga ukończenia przez serwer procesu zastrzegania. Proces zastrzegania różni się w zależności od rodzaju zastrzeganego serwera.

-   W przypadku zastrzegania osobnego serwera licencji należy określić bazę danych konfiguracji, konto usługi programu RMS, adres URL klastra oraz informacje dotyczące ochrony klucza prywatnego, w ten sam sposób, w jaki podano te informacje dla serwera głównej certyfikacji. Nie należy jednak określać zasad odwołania certyfikatu licencjodawcy serwera, ponieważ zasady te są kontrolowane przez serwer głównej certyfikacji.
-   W przypadku zastrzegania serwera jako członka klastra jedynymi informacjami wymaganymi podczas zastrzegania są: konto usługi programu RMS, baza danych konfiguracji oraz hasło do ochrony klucza prywatnego (lub określenie tego samego dostawcy CSP i klucza prywatnego, co w przypadku istniejącego klastra). Wszystkie serwery w klastrze współdzielą ten sam certyfikat licencjodawcy serwera oraz parę kluczy serwera.

> [!Important]  
> Nie należy rozpoczynać instalowania programu RMS na innych serwerach przed ukończeniem konfigurowania programu RMS na pierwszym serwerze, w tym procesów instalowania i zastrzegania serwera. 

Po zainstalowaniu i zastrzeżeniu dodatkowego serwera, serwer jest automatycznie konfigurowany jako członek klastra. Jednak w przypadku gdy zaimplementowano równoważenie obciążenia, należy skonfigurować oprogramowanie równoważenia obciążenia do pracy z nowym serwerem.

<span id="BKMK_3"></span>
Konfigurowanie klastrów i równoważenia obciążenia
-------------------------------------------------

Program RMS został zaprojektowany z myślą o obsłudze klastrów serwerów. Tworzenie klastrów serwerów programu RMS zapewnia większą skalowalność, niezawodność i równoważenie obciążenia w rozmieszczeniu programu RMS.

**Tworzenie klastrów**

Aby skonfigurować klaster, należy utworzyć serwer głównej certyfikacji lub serwer licencji. W przypadku drugiego i kolejnych serwerów w każdym klastrze należy zainstalować program RMS na nowym serwerze, przejść do strony **Administracja globalna**, a następnie kliknąć łącze **Dodaj ten serwer do klastra**, aby zastrzec wymagane zasoby i dołączyć serwer do klastra głównej certyfikacji lub klastra licencji.

Wprowadź nazwę bazy danych klastra, do którego chcesz się przyłączyć.

**Klastry równoważenia obciążenia**

Program RMS nie implementuje automatycznie równoważenia obciążenia. Do równoważenia obciążenia wszystkich serwerów programu RMS można wykorzystać sprzęt lub oprogramowanie równoważące obciążenie, w tym usługę równoważenia obciążenia sieci.

Następujące tematy zawierają dodatkowe informacje dotyczące tego zagadnienia:

-   Aby uzyskać więcej informacji dotyczących różnic między usługami certyfikacji i licencjonowania, zobacz „Omówienie systemu RMS” w części „Informacje techniczne dotyczące programu RMS” w tym zestawie dokumentacji.
-   Aby uzyskać więcej informacji dotyczących mapowania rozmieszczeń serwerów zgodnie z wymaganiami organizacji dotyczącymi dostępności i wydajności, zobacz „Zapewnianie nadmiarowości i równoważenie obciążenia” w części „Planowanie rozmieszczenia programu RMS” w tym zestawie dokumentacji.
-   Aby uzyskać więcej informacji dotyczących określania liczby serwerów wymaganych do obsługi rozmieszczenia programu RMS w organizacji, zobacz „Ocenianie wymagań dotyczących skalowalności” w części „Planowanie rozmieszczenia programu RMS” w tym zestawie dokumentacji.
-   Aby uzyskać więcej informacji dotyczących implementowania zabezpieczeń informatycznych podczas rozmieszczania programu RMS, zobacz „[Zabezpieczanie rozmieszczania programu RMS](https://technet.microsoft.com/6de8b636-a824-4844-aefc-f26347abfc14)” w dalszej części tego tematu.
-   Aby uzyskać informacje dotyczące instalowania programu RMS, zobacz „Instalowanie programu RMS z dodatkiem Service Pack 1” w części „Obsługa serwerów programu RMS” w tym zestawie dokumentacji.
    Program RMS można również zainstalować z poziomu wiersza polecenia. Aby uzyskać więcej informacji, zobacz „Instalacja programu RMS z wiersza polecenia” w części „Obsługa serwerów programu RMS” w tym zestawie dokumentacji.
-   Aby uzyskać informacje dotyczące zastrzegania serwera licencji, zobacz „Zastrzeganie serwera licencji” w części „Obsługa serwerów programu RMS” w tym zestawie dokumentacji.
-   Aby uzyskać informacje dotyczące zastrzegania dodatkowych serwerów w klastrze, zobacz „Dodawanie serwera do klastra” w części „Obsługa serwerów programu RMS” w tym zestawie dokumentacji.
