---
TOCTitle: 'Często zadawane pytania na temat programu RMS: Wdrażanie'
Title: 'Często zadawane pytania na temat programu RMS: Wdrażanie'
ms:assetid: '5559ae65-77ae-4e0b-bfd8-3512409ed29b'
ms:contentKeyID: 18123266
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720274(v=WS.10)'
---

Często zadawane pytania na temat programu RMS: Wdrażanie
========================================================

Pytania dotyczące rozmieszczania programu RMS
---------------------------------------------

-   [Jeśli podmiotami zabezpieczeń w kontekście RMS są członkowie globalnej listy adresów, czy istnieje jakaś zależność od wersji programu Exchange?](#bkmk_20)
-   [Jaką rolę w systemie RMS odgrywa serwer SQL Server?](#bkmk_21)
-   [Czy komputer użytkownika musi być przyłączony do tej samej domeny, co klaster główny RMS, aby móc korzystać z usług RMS?](#bkmk_22)
-   [Jeśli klient chce umieścić serwer RMS w sieci obwodowej, które porty muszą być otwarte na zaporze od strony Internetu i od strony intranetu, aby umożliwić komunikację z RMS?](#bkmk_23)
-   [W jaki sposób rejestrowane są serwery podrzędne w klastrze przeznaczonym tylko do licencjonowania i czy trzeba wykonywać jakiekolwiek zabiegi na klientach, aby ich konfiguracja uwzględniała obecność klastra?](#bkmk_24)
-   [Jakie korzyści płyną z używania klastra przeznaczonego tylko do licencjonowania?](#bkmk_25)
-   [Co jest potrzebne, aby całkowicie wycofać instalację RMS?](#bkmk_26)
-   [Czy po odinstalowaniu klienta RMS za pomocą funkcji Dodaj lub usuń programy, zostają jeszcze jakieś pliki, które trzeba usunąć ręcznie?](#bkmk_27)
-   [Czy program RMS współpracuje z systemem plików FAT?](#bkmk_28)
-   [Jakie są typowe wymagania sprzętowe dotyczące serwera bazy danych używanego przez program RMS?](#bkmk_29)
-   [W jaki sposób stopień wykorzystania wykazu globalnego przez RMS w celu rozszerzania grup wpływa na wydajność serwera wykazu globalnego?](#bkmk_30)
-   [Czy program RMS wymaga jakichkolwiek zmian schematu w usłudze Active Directory?](#bkmk_31)
-   [Czy punkt połączenia usługi (SCP) będzie automatycznie replikowany między różnymi kontrolerami domen w domenie, w której jest zainstalowany klaster RMS?](#bkmk_32)
-   [Jeśli użytkownicy nie mają uprawnień administracyjnych na swoich komputerach, w jaki sposób mogą zainstalować i skonfigurować klienta RMS?](#bkmk_33)
-   [W jakim stopniu system RMS jest skalowalny?](#bkmk_35)
-   [Czy program RMS pozwala na stosowanie sprzętowych modułów zabezpieczeń do zabezpieczania kluczy RMS w sprzęcie?](#bkmk_36)

<span id="BKMK_20"></span>
#### Jeśli podmiotami zabezpieczeń w kontekście RMS są członkowie globalnej listy adresów, czy istnieje jakaś zależność od wersji programu Exchange?

Program RMS współpracuje z usługą Active Directory, a nie z serwerem Exchange. Tymczasem serwer Exchange 5.5 prowadzi własny katalog i nie korzysta z usługi Active Directory. Należy zadbać o to, by wszystkie obiekty użytkowników i grup w katalogu Active Directory miały poprawny atrybut e-mail, obejmujący pełną nazwę domeny. Jest to wykonywane automatycznie w przypadku serwera Exchange 2000 lub jego nowszej wersji.

<span id="BKMK_21"></span>
#### Jaką rolę w systemie RMS odgrywa serwer SQL Server?

Program RMS korzysta z bazy danych do przechowywania wszystkich danych konfiguracyjnych usługi, informacji o podmiotach zabezpieczeń w systemie, wszystkich danych logowania oraz do tymczasowego przechowywania wyników wyszukiwań podczas rozszerzania nazw na podstawie katalogu Active Directory i list rozpowszechniania. Program RMS został dokładnie przetestowany pod kątem pracy z programami SQL Server 2000 i SQL Server 2005.

<span id="BKMK_22"></span>
#### Czy komputer użytkownika musi być przyłączony do tej samej domeny, co serwer RMS, aby móc korzystać z usług RMS?

Komputer użytkownika nie musi być członkiem tej samej domeny co klaster RMS, ale komputer musi być w stanie odnaleźć klaster RMS. Najłatwiejszym sposobem zagwarantowania, że komputery klienckie będą mogły odnaleźć klaster RMS, jest użycie funkcji wyszukiwania w katalogu Active Directory za pośrednictwem punktu połączenia usługi. Niemniej jednak ustawienia rejestru na komputerze klienta mogą zostać skonfigurowane w taki sposób, by umożliwiać odnajdywanie klastra RMS bez odwoływania się do katalogu Active Directory. Szczegóły ustawień rejestru są uzależnione od aplikacji obsługującej technologię RMS.

<span id="BKMK_23"></span>
#### Jeśli klient chce umieścić serwer RMS w sieci obwodowej, które porty muszą być otwarte na zaporze od strony Internetu i od strony intranetu, aby umożliwić komunikację z RMS?

Użytkownicy wewnętrzni będą potrzebowali dostępu do serwerów RMS wydających certyfikaty kont praw dostępu oraz licencje użytkowania. Serwer RMS domyślnie oczekuje na żądania na porcie HTTP (port TCP o numerze 80) lub HTTPS (port TCP o numerze 443), zależnie od tego, czy konfiguracja serwera przewiduje stosowanie protokołu SSL, tak więc te właśnie porty muszą być otwarte na zaporze od strony Internetu. Od strony intranetu na zaporze należy otworzyć dodatkowe porty, wykorzystywane przez serwery należące do domeny.

<span id="BKMK_24"></span>
#### W jaki sposób rejestrowane są serwery podrzędne w klastrze przeznaczonym tylko do licencjonowania i czy trzeba wykonywać jakiekolwiek zabiegi na klientach, aby ich konfiguracja uwzględniała obecność klastra?

Pierwszy serwer RMS w klastrze głównym tworzony w przedsiębiorstwie otrzymuje certyfikat licencjodawcy serwera od usługi rejestrowania firmy Microsoft. Po zainstalowaniu i zastrzeżeniu kolejnego serwera RMS można przyłączy go do klastra głównego lub zarejestrować jako serwer w podrzędnym klastrze przeznaczonym tylko do licencjonowania. W przypadku decyzji o zarejestrowaniu go jako serwera w podrzędnym klastrze przeznaczonym tylko do licencjonowania serwer wysyła żądanie rejestrowania do klastra głównego RMS. Aplikacje obsługujące technologię RMS określają, czy aplikacja klienta ma szukać klastra przeznaczonego tylko do licencjonowania. Pakiet Office 2003 jest przykładem aplikacji obsługującej technologię RMS, która domyślnie poszukuje klastra głównego. Ten tryb działania można zmienić za pomocą ustawień rejestru, tak aby aplikacja poszukiwała nowego podrzędnego klastra przeznaczonego tylko do licencjonowania.

<span id="BKMK_25"></span>
#### Jakie korzyści płyną z używania podrzędnego klastra przeznaczonego tylko do licencjonowania?

Jedna z korzyści polega na wydzielaniu odrębnych działów organizacji. Jeśli nie ustanowiono zaufanej domeny publikowania między klastrami RMS, z zawartości mogą korzystać jedynie użytkownicy mający dostęp do danego serwera licencjonowania. Tym sposobem dział prawny może zabronić pracownikom wszystkich innych działów odczytywania swoich wiadomości szyfrowanych przez program RMS. Ponadto w klastrze przeznaczonym tylko do licencjonowania można określić kilka dodatkowych opcji, takich jak szablony praw, przynależność do grupy użytkowników uprzywilejowanych oraz zasady wykluczania.

<span id="BKMK_26"></span>
#### Co jest potrzebne, aby całkowicie wycofać instalację RMS?

Poniższa procedura pozwala całkowicie usunąć instalację programu RMS.

**Aby wycofać instalację programu RMS**
1.  Usuń punkt połączenia usługi klastra RMS za pomocą administracyjnej witryny sieci Web.

2.  Na stronie **Administracja globalna** kliknij opcję **Usuń program RMS z tej witryny sieci Web**, aby usunąć zastrzeżenie programu RMS na serwerze. Należy w pierwszej kolejności usunąć zastrzeżenie zarejestrowanych podrzędnie serwerów w klastrach przeznaczonych tylko do licencjonowania, a następnie usunąć zastrzeżenie serwerów klastra głównego.

3.  W **Panelu sterowania** kliknij opcję **Dodaj lub usuń programy** i usuń składnik **Usługi zarządzania prawami dostępu**.

4.  Na serwerze bazy danych usuń wszelkie pozostałe bazy danych RMS.

5.  Usuń konto usługi RMS z listy autoryzowanych poświadczeń logowania na serwerach baz danych, a następnie usuń konto z samego katalogu Active Directory.

6.  Jeśli na komputerach klienckich RMS działa system Windows XP lub Windows 2000, usuń klienta RMS z tych komputerów.

> [!Important]  
> Po wykonaniu tej procedury otwarcie zawartości chronionej prawami dostępu przestaje być możliwe. Jeśli program RMS służył do ochrony cennych danych, przed usunięciem instalacji należy wykonać procedurę likwidowania programu RMS. 

<span id="BKMK_27"></span>
#### Czy po odinstalowaniu klienta RMS za pomocą funkcji Dodaj lub usuń programy, zostają jeszcze jakieś pliki, które trzeba usunąć ręcznie?

Chociaż nie jest to konieczne, można usunąć skrytkę z katalogu %systemroot%\\system32.

<span id="BKMK_28"></span>
#### Czy program RMS współpracuje z systemem plików FAT?

Tak, program RMS może działać na komputerze z systemem plików FAT, chociaż zaleca się stosowanie systemu plików NTFS.

<span id="BKMK_29"></span>
#### Jakie są typowe wymagania sprzętowe dotyczące serwera bazy danych używanego przez program RMS?

Baza danych rejestrowania rośnie w szybkim tempie, zwłaszcza w środowiskach, w których program RMS jest intensywnie używany. Jeśli jako serwer bazy danych ma być używany program SQL Server, najkorzystniej jest użyć wersji SQL Server 2000 Enterprise Edition lub SQL Server 2005 Enterprise Edition w systemie Windows 2000 Advanced Server lub Windows Server 2003, Enterprise Edition skonfigurowanym w klastrze w konfiguracji aktywnej gotowości. W takim przypadku zalecana konfiguracja to dyski rejestrowania macierzy RAID-1 i dyski danych w macierzy RAID-5 oraz przynajmniej 512 MB pamięci RAM. Minimalna zalecana moc procesora w takiej konfiguracji to Pentium III z zegarem 1,4 GHz. Na dedykowanych serwerach baz danych stosowanie systemów wieloprocesorowych nie jest konieczne.

<span id="BKMK_30"></span>
#### W jaki sposób stopień wykorzystania wykazu globalnego przez RMS w celu rozszerzania grup wpływa na wydajność serwera wykazu globalnego?

Serwer RMS zapisuje listy rozszerzeń grup w pamięci podręcznej, więc ta operacja nie powinna w nadmierny sposób obciążać globalnego serwera usług katalogowych. Częste modyfikowanie przynależności do grup zwiększa zależność od serwera katalogowego, chociaż czas realizacji tej usługi można konfigurować za pośrednictwem rejestru. Często wykonywane rozszerzanie dużych grup spowoduje spadek sprawności. Aby uzyskać więcej informacji, zobacz punkt „Zmiana ustawień pamięci podręcznej usługi Active Directory” w części poświęconej działaniu programu RMS w niniejszym zestawie dokumentów.

<span id="BKMK_31"></span>
#### Czy program RMS wymaga jakichkolwiek zmian schematu w usłudze Active Directory?

Aby program RMS mógł pomyślnie rozszerzyć członkostwo w grupie określonej w licencji publikacji poza granice lasu, w lokalnym lesie usługi Active Directory musi istnieć obiekt kontaktowy przedstawiający grupę w lesie zdalnym. Program RMS może odczytać atrybuty obiektu kontaktowego i uzyskać informację, że ten obiekt reprezentuje grupę w innym lesie.

Aby możliwe było takie działanie programu RMS, usługa Active Directory wymaga atrybutu schematu serwera Exchange Server 2003 lub nowszego o nazwie msExchOriginatingForest. Atrybut ten jest instalowany domyślnie w schemacie usługi Active Directory, jeśli w lesie działa jeden serwer z systemem Exchange Server 2003. Atrybut ten musi znajdować się w lesie każdego schematu usługi Active Directory, który będzie współpracować z programem RMS. Jeśli program Exchange Server 2003 nie jest używany, można zainstalować schemat osobno w strukturze usługi Active Directory przy użyciu administracyjnego zestawu narzędzi programu RMS.

<span id="BKMK_32"></span>
#### Czy punkt połączenia usługi (SCP) będzie automatycznie replikowany między różnymi kontrolerami domen w domenie, w której jest zainstalowany serwer RMS?

Po zastrzeżeniu pierwszego serwera RMS w lesie musi on zostać zarejestrowany w katalogu Active Directory przy użyciu konta domeny mającego poziom uprawnień wystarczający do utworzenia obiektu kontenera poniżej kontenera Usługi w kontenerze Konfiguracja w katalogu Active Directory. Wbudowana grupa zabezpieczeń — Enterprise Admins — jest przykładem konta mającego wymagane uprawnienia. W rezultacie powstaje punkt połączenia usługi. Ponieważ ma to miejsce w kontenerze Usługi, w wyniku replikacji katalogu Active Directory informacje te są kopiowane na wszystkie kontrolery domeny w lesie.

<span id="BKMK_33"></span>
#### Jeśli użytkownicy nie mają uprawnień administracyjnych na swoich komputerach, w jaki sposób mogą zainstalować i skonfigurować klienta RMS?

Klient RMS jest rozprowadzany w postaci pliku instalatora systemu Windows za pomocą infrastruktury dystrybucji oprogramowania, takiej jak Systems Management Server 2003. Klienta RMS można także rozprowadzać za pomocą obiektu zasad grupy, korzystającego z konta usługi mającego uprawnienia administracyjne. Jeśli na komputerze klienckim RMS działa system Windows Vista, osobna instalacja klienta programu RMS nie jest potrzebna, ponieważ jest on zintegrowany z systemem operacyjnym.

<span id="BKMK_35"></span>
#### W jakim stopniu system RMS jest skalowalny?

RMS jest bezstanową usługą sieci Web, a więc może być łączony w klastry i objęty równoważeniem obciążenia podobnie jak każda inna witryna lub usługa sieci Web. Wydajność programu RMS zależy w głównej mierze od dostępności procesora, a więc wprowadzanie dodatkowych procesorów może poprawić wydajność.

<span id="BKMK_36"></span>
#### Czy program RMS pozwala na stosowanie sprzętowych modułów zabezpieczeń do zabezpieczania kluczy RMS w sprzęcie?

Tak, program RMS współpracuje ze sprzętowymi modułami zabezpieczeń, które są zgodne ze standardem CAPI, np. modułem nCipher.
