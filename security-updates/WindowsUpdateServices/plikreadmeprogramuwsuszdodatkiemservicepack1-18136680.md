---
TOCTitle: Plik Readme programu WSUS z dodatkiem Service Pack 1
Title: Plik Readme programu WSUS z dodatkiem Service Pack 1
ms:assetid: '937ecfe9-e8e0-41ac-85f7-4b65956f3d1e'
ms:contentKeyID: 18136680
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc708486(v=WS.10)'
---

Plik Readme programu WSUS z dodatkiem Service Pack 1
====================================================

W tym dokumencie zamieszczono opis znanych błędów związanych z programem Windows Server Update Services z dodatkiem Service Pack 1 (WSUS z dodatkiem SP1). Bezpośrednio po informacjach na temat programu WSUS z dodatkiem SP1 można znaleźć pełne informacje, które zostały poprzednio zamieszczone w uwagach w oryginalnym pliku Readme programu WSUS. Te informacje dotyczą także zaleceń oraz wymagań instalacji programu WSUS. Aby pobrać program WSUS z dodatkiem SP1, zobacz [Centrum pobierania firmy Microsoft](http://go.microsoft.com/fwlink/?linkid=67516).

Co nowego w programie WSUS z dodatkiem SP1
------------------------------------------

Program WSUS z dodatkiem SP1 jest wersją dodatku Service Pack poprawiającego bezpieczeństwo, niezawodność, skalowalność, zgodność oraz wydajność programu WSUS. Poniżej przedstawiono nowe funkcje i ulepszenia:

-   Obsługa klientów w systemie Windows Vista: Komputery z systemem Windows Vista można zaktualizować za pośrednictwem serwera WSUS z dodatkiem SP1.
-   Obsługa większej liczby języków na kliencie: Obsługa wszystkich języków pakietu Office i systemu Windows Vista.
-   Nowa wersja programu WMSDE: Instalacja programu WMSDE zostanie uaktualniona do programu WMSDE z dodatkiem SP4 za pośrednictwem programu WSUS z dodatkiem SP1 (WSUS RTM korzysta z programu WMSDE z dodatkiem SP3).
-   Poprawa wydajności Program WSUS z dodatkiem SP1 zawiera różne ulepszenia w zakresie wydajności, które skracają czas odpowiedzi interfejsu użytkownika.
-   Wszystkie poprawki: Program WSUS z dodatkiem SP1 zawiera wszystkie zmiany i poprawki, które zostały wydane od momentu opracowania wersji programu WSUS RTM.
-   Obsługa programu SQL Server 2005.

Przed rozpoczęciem uaktualniania programu WSUS z dodatkiem SP1
--------------------------------------------------------------

Poniżej przedstawiono problemy związane z uaktualnianiem programu WSUS z dodatkiem SP1. Problemy i wymagania opisane w sekcji „Zanim rozpoczniesz” w oryginalnej wersji tego tematu nie zostały zamieszczone w tej sekcji, ale nadal obowiązują. Przykładowo nadal obowiązują wymagania dotyczące instalacji opisane w oryginalnej sekcji „Zanim rozpoczniesz”.

**Uwaga**   Po zastosowaniu dodatku SP1 dla programu WSUS 2.0 nie jest możliwe jego odinstalowanie. Odinstalowanie dodatku SP1 spowoduje odinstalowanie całego produktu.

**Ważne**   Ten dokument zawiera informacje dotyczące sposobu modyfikowania rejestru. Przed zmodyfikowaniem rejestru należy utworzyć jego kopię zapasową. Należy zapoznać się ze sposobem przywracania rejestru w razie wystąpienia problemu. Aby uzyskać więcej informacji na temat sposobu tworzenia kopii zapasowej, przywracania i modyfikowania rejestru, zobacz poniższy artykuł w bazie wiedzy Microsoft Knowledge Base:

[Opis rejestru systemu Microsoft Windows](http://support.microsoft.com/kb/256986) (http://support.microsoft.com/kb/256986/)

#### Problem 1: Należy upewnić się, że na dysku jest dostępna odpowiednia ilość wolnego miejsca dla kopii zapasowej bazy danych

Podczas uaktualniania programu WSUS RTM Instalator programu WSUS z dodatkiem SP1 automatycznie tworzy kopię zapasową bazy danych WSUS. Należy upewnić się, że ilość wolnego miejsca w systemie plików serwera WSUS jest odpowiednia do zapisania kopii zapasowej bazy danych WSUS; w przeciwnym razie instalacja programu WSUS z dodatkiem SP1 nie powiedzie się.

**Aby sprawdzić, czy ilość wolnego miejsca na dysku jest odpowiednia**
1.  Otwórz Eksploratora Windows i przejdź do folderu zawierającego bazę danych WSUS. Domyślnie w ramach instalacji programu WSUS baza danych jest instalowana w następującym folderze:

    
        ```
2.  Naciśnij i przytrzymaj klawisz **CTRL**, zaznacz pliki **SUSDB.MDF** i **SUSDB\_log.LDF**, a następnie kliknij prawym przyciskiem myszy i wybierz polecenie **Właściwości**.

3.  W oknie dialogowym **Pliki** odczytaj wartość w polu **Rozmiar na dysku**. Na dysku musi znajdować się co najmniej taka ilość wolnego miejsca, aby możliwa była instalacja programu WSUS z dodatkiem SP1.

4.  W menu **Start** kliknij polecenie **Mój komputer**. Upewnij się, że na dysku, na którym jest zainstalowany program WSUS, znajduje się wymagana ilość wolnego miejsca.

Jeśli z jakiegoś powodu instalacja programu WSUS z dodatkiem SP1 nie powiedzie się, ręcznie przywróć kopię bazy danych. Aby uzyskać instrukcje na temat przywracania bazy danych WSUS, zobacz [WSUS Operations Guide (Przewodnik po obsłudze programu WSUS)](http://technet2.microsoft.com/windowsserver/en/library/05f2e884-ae62-4c90-9681-6c9f2f3c9fd91033.mspx).

#### Problem 2: Program WSUS z dodatkiem SP1 uaktualnia tylko program WSUS RTM

Program WSUS RTM można uaktualnić wyłącznie za pomocą programu WSUS z dodatkiem SP1. Obecnie uaktualnianie z kandydata do wydania programu WSUS nie jest obsługiwane. W przypadku zainstalowania kandydata do wydania programu WSUS lub wcześniejszych kompilacji programu WSUS należy je odinstalować, a następnie uruchomić program WSUS z dodatkiem SP1.

#### Problem 3: Usługa IIS na serwerze zostanie zatrzymana podczas uaktualniania programu WSUS z dodatkiem SP1

Instalator uaktualnienia programu WSUS z dodatkiem SP1 zatrzyma działanie Internetowych usług informacyjnych (IIS) na serwerze w trakcie procesu uaktualniania. Oznacza to, że wszystkie witryny sieci Web udostępnione w ramach instalacji Internetowych usług informacyjnych nie będą dostępne podczas uaktualniania. Internetowe usługi informacyjne zostaną automatycznie uruchomione po zakończeniu uaktualniania.

#### Problem 4: Podczas uaktualniania nie należy uruchamiać aplikacji, które wywołują interfejsy API programu WSUS

Wywołania interfejsu aplikacji (API) programu WSUS powodują powstanie konfliktów z instalatorem programu WSUS z dodatkiem SP1, a w konsekwencji niepowodzenie uaktualnienia (zostanie wyświetlony komunikat z prośbą o ponowne uruchomienie serwera w celu zakończenia procesu uaktualnienia).

#### Problem 5: Przed uaktualnieniem do programu WSUS z dodatkiem SP1 należy wyłączyć programy antywirusowe

W przypadku uaktualnienia programu WSUS za pośrednictwem programu WSUS z dodatkiem SP1 konieczne może okazać się wyłączenie programów antywirusowych, aby możliwe było pomyślne wykonanie uaktualnienia lub zastosowanie dodatku Service Pack. Po wyłączeniu programów antywirusowych należy ponownie uruchomić komputer z systemem Windows Server zanim zostanie zastosowane uaktualnienie lub dodatek Service Pack. Ta procedura zapobiega blokowaniu plików, do których proces uaktualnienia wymaga dostępu. Po zakończeniu instalacji należy uruchomić program antywirusowy. Informacje dotyczące sposobu wyłączania i ponownego włączania programu antywirusowego oraz jego wersji można znaleźć w witrynie dostawcy programu antywirusowego w sieci Web.

| ![](images/Cc708486.Caution(WS.10).gif)Przestroga                                                                                                                                                                                                                                                                                    |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| W wyniku tego obejścia komputer lub sieć stają się bardziej narażone na ataki ze strony użytkowników złośliwych lub oprogramowania złośliwego, takiego jak wirusy. Nie zalecamy stosowania tego obejścia, jednak podaliśmy te informacje, aby użytkownik mógł je zaimplementować według własnego uznania. To obejście należy stosować na własną odpowiedzialność. |

| ![](images/Cc708486.note(WS.10).gif)Uwaga                                                                                                                                                                                   |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Program antywirusowy pomaga chronić komputer przed wirusami. Nie należy pobierać ani otwierać plików z niezaufanych źródeł, odwiedzać niezaufanych witryn sieci Web ani otwierać załączników wiadomości e-mail, gdy program antywirusowy jest wyłączony. |

#### Problem 6: W przypadku korzystania z serwera proxy uaktualnienie dodatku SP1 może spowodować skasowanie nazwy użytkownika i hasła konfiguracji proxy

W niektórych przypadkach przy korzystaniu z serwera proxy uaktualnienie dodatku SP1 może spowodować skasowanie nazwy użytkownika i hasła konfiguracji proxy. Na skutek tego podczas synchronizacji uaktualnień z serwerów Microsoft Server może zostać wygenerowany błąd dotyczący „nieprawidłowego parametru”. W celu usunięcia tego problemu należy zresetować nazwę użytkownika i hasło konfiguracji proxy oraz ponownie zsynchronizować serwer.

#### Problem 7: W jaki sposób odzyskać sprawność po nieudanym uaktualnieniu, aby przywrócić spójny stan serwera WSUS, a następnie ponowić próbę uaktualnienia.

W przypadku niepowodzenia uaktualnienia do programu WSUS z dodatkiem SP1 stan instalacji programu WSUS może być niespójny lub bezużyteczny. Aby ponowić próbę uaktualnienia do programu WSUS z dodatkiem SP1, należy uzyskać spójny stan instalacji programu WSUS. W tym celu można użyć kopii zapasowej bazy danych utworzonej na początku procesu uaktualnienia i przywrócić stan serwera WSUS sprzed uaktualnienia.

W razie niepowodzenia uaktualnienia ponów próbę uaktualnienia do programu WSUS z dodatkiem SP1, wykonując następujące czynności:

**Aby ponowić próbę uaktualnienia do programu WSUS z dodatkiem SP1**
1.  Określ lokalizację kopii zapasowej bazy danych, przeglądając zawartość pliku WSUSSetup\_%timestamp%.log. Ten plik znajduje się w następującym folderze:

    -   %programfiles%\\Update Services\\LogFiles

2.  Przywróć kopię zapasową bazy danych na komputerze WSUS za pomocą następującego polecenia:

    -   osql.exe -S &lt;instancja\_bazy\_danych&gt; -E -Q "USE master ALTER DATABASE SUSDB SET SINGLE\_USER WITH ROLLBACK IMMEDIATE RESTORE DATABASE SUSDB FROM DISK=N'&lt;ścieżka\_kopii\_zapasowej\_bazy\_danych&gt;' WITH REPLACE ALTER DATABASE SUSDB SET MULTI\_USER"
    -   Pamiętaj o zastąpieniu wartości &lt;instancja\_bazy\_danych&gt; i &lt;ścieżka\_kopii\_zapasowej\_bazy\_danych&gt; wartościami z instalacji.
    -   Dla parametru &lt;instancja\_bazy\_danych&gt; użyj wartości z następującego klucza rejestru:
    -   HKLM\\Software\\Microsoft\\Update Services\\Server\\Setup\\SqlServerName
    -   Dla parametru &lt;ścieżka\_kopii\_zapasowej\_bazy\_danych&gt; użyj wartości określonej w kroku 1

3.  Odinstaluj program WSUS, zachowując bazę danych WSUS, pliki dzienników oraz pliki aktualizacji, gdy pojawi się pytanie o ich usunięcie. (Usuń zaznaczenia wszystkich opcji w obszarze **Usuwanie programu Microsoft Windows Server Update Services**.)

4.  Ponownie zainstaluj program (oryginalna wersja inna niż WSUS z dodatkiem SP1). Użyj istniejącej bazy danych po wyświetleniu odpowiedniego monitu. Spowoduje to przywrócenie spójnego stanu systemu WSUS.

5.  Zainstaluj program WSUS z dodatkiem SP1.

**Uwaga**    Nie można użyć kopii zapasowej bazy danych utworzonej z kroku 1 bezpośrednio w instalacji czystej programu WSUS z dodatkiem SP1. Schemat bazy danych został zmieniony, w wyniku czego ta baza danych nie będzie zgodna bez uaktualnienia do programu WSUS z dodatkiem SP1.

#### Problem 8: W niektórych przypadkach po przeprowadzeniu migracji bazy danych programu WMSDE uaktualnienie programu WSUS z dodatkiem SP1 może się nie powieść

Sposób rozwiązania tego problemu zależy od tego, czy migracja została przeprowadzona na lokalny czy na zdalny serwer SQL.

#### Baza danych programu WMSDE zmigrowana na lokalny serwer SQL 2000

Aby pakiet instalacyjny programu WSUS z dodatkiem SP1 rozpoznał, że baza danych programu WMSDE do uaktualnienia nie istnieje, należy zmienić wartość klucza rejestru.

W przypadku przeprowadzenia migracji programu WMSDE na lokalny serwer SQL 2000 przed podjęciem próby uaktualnienia do programu WSUS z dodatkiem SP1 wprowadź poniższe zmiany w rejestrze:

-   Zmień wartość następującego klucza rejestru z „1” na „0”:
    -   HKLM\\Software\\Microsoft\\Update Services\\Server\\Setup\\WmsdeInstalled  

#### Baza danych programu WMSDE zmigrowana na zdalny serwer SQL 2000

Aby pakiet instalacyjny programu WSUS z dodatkiem SP1 rozpoznał, że baza danych programu WMSDE do aktualizacji nie istnieje, należy zmienić dwie wartości klucza rejestru. Aktualizacja musi zostać zainicjowane na serwerze typu back end, a następnie na serwerze frontonu.  

W przypadku przeprowadzenia migracji programu WMSDE na zdalny serwer SQL przed podjęciem próby uaktualnienia do programu WSUS z dodatkiem SP1 wprowadź poniższe zmiany w rejestrze:

1.  Zmień wartość następującego klucza rejestru z „1” na „0”:
    -   HKLM\\Software\\Microsoft\\Update Services\\Server\\Setup\\WmsdeInstalled 
2.  Zmień wartość następującego klucza rejestru z „0x80” na „0x20”
    -   HKLM\\Software\\Microsoft\\Update Services\\Server\\Setup\\InstallType 

Po uaktualnieniu tych wartości klucza rejestru zainicjuj uaktualnienie na serwerach typu back end, a następnie na serwerach frontonu.

#### Problem 9: Program WSUS z dodatkiem SP1 nie uaktualnia serwerów WSUS, które są instalowane za pośrednictwem zdalnych wdrożeń SQL

Pakiet instalacyjny programu WSUS z dodatkiem SP1 należy uruchomić zarówno na serwerach frontonu, jak i serwerach typu back end.

**Aby uaktualnić do programu WSUS z dodatkiem SP1, gdy jest używany zdalny serwer SQL**
1.  Uruchom pakiet instalacyjny serwera frontonu bez przełączników i wybierz opcję uaktualnienia.

2.  Uruchom pakiet instalacyjny serwera typu back end bez przełączników i wybierz opcję uaktualnienia.

#### Problem 10: Zmiana nazwy komputera przed uaktualnieniem do programu WSUS z dodatkiem SP1 może być przyczyną niepowodzenia uaktualnienia

W przypadku zmiany nazwy komputera po zainstalowaniu programu WSUS RTM, ale przed uaktualnieniem do programu WSUS z dodatkiem SP1 uaktualnienie programu WSUS z dodatkiem SP1 może się nie powieść.

Za pomocą poniższego skryptu usuń i ponownie dodaj grupy Administratorów ASPNET i WSUS. Następnie ponownie uruchom uaktualnienie.

        ```
| ![](images/Cc708486.note(WS.10).gif)Uwaga                                                                       |
|----------------------------------------------------------------------------------------------------------------------------------------------|
| Konieczne może być zastąpienie wartości &lt;ContentDirectory&gt; w ostatnim wierszu ścieżką do aktualnego miejsca przechowywania zawartości. |

Oryginalna zawartość pliku Readme programu WSUS
-----------------------------------------------

Poniżej przedstawiono oryginalną zawartość pliku Readme programu WSUS. W programie WSUS z dodatkiem SP1 *nie* rozwiązano żadnych z następujących problemów. Poniższe informacje zamieszczono tylko dla wygody użytkowników.

Przed rozpoczęciem
------------------

#### Problem 1: Wymagane jest zainstalowanie Internetowych usług informacyjnych

Program Microsoft® Windows Server™ Update Services (WSUS) wymaga zainstalowania Internetowych usług informacyjnych (IIS). W przypadku systemów Microsoft Windows Server 2003 i Microsoft Windows® 2000 Server Internetowe usługi informacyjne nie są instalowane domyślnie, w wyniku czego działanie Instalatora programu Windows Server Update Services może zostać przerwane i może zostać wyświetlony komunikat o błędzie, informujący o braku zainstalowanych Internetowych usług informacyjnych.

Aby zainstalować program IIS:

1.  Otwórz Panel sterowania.
2.  Kliknij dwukrotnie opcję **Dodaj lub usuń programy**.
3.  Kliknij przycisk **Dodaj/Usuń składniki systemu Windows**.
4.  Na liście **Składniki** kliknij opcję **Serwer aplikacji**.
5.  Kliknij polecenie **Szczegóły**.
6.  Zaznacz pole wyboru **ASP.NET**. Pola wyboru **Włącz dostęp sieciowy modelu COM+** i Internetowe usługi informacyjne (IIS) zostaną zaznaczone automatycznie.
7.  Wybierz opcję **Internetowe usługi informacyjne (IIS)**, a następnie kliknij polecenie **Szczegóły**, aby wyświetlić listę opcjonalnych składników Internetowych usług informacyjnych.
8.  Wybierz wszystkie składniki opcjonalne, które mają zostać zainstalowane. Składnik opcjonalny Usługa World Wide Web zawiera ważne składniki dodatkowe, takie jak Strony ASP i Administracja zdalna (HTML). Aby wyświetlić i wybrać te składniki dodatkowe, kliknij opcję Usługa World Wide Web, a następnie kliknij polecenie Szczegóły. Klikaj przycisk OK, aż do powrócenia do Kreatora składników systemu Windows.
9.  Kliknij przycisk **Dalej** i zakończ pracę z Kreatorem składników systemu Windows.
10. Po zainstalowaniu Internetowych usług informacyjnych uruchom Instalatora programu Windows Server Update Services.

#### Problem 2: W przypadku serwerów z systemem Windows 2000 Server przed zainstalowaniem programu WSUS w ramach Internetowych usług informacyjnych musi być dostępna co najmniej jedna witryna sieci Web

Jeśli po uruchomieniu Instalatora programu Windows Server Update Services w ramach Internetowych usług informacyjnych nie są dostępne żadne witryny, utworzenie witryny sieci Web przez Instalatora może się nie powieść. Taka sytuacja może wystąpić na przykład wtedy, gdy w ramach Internetowych usług informacyjnych dostępna była jedynie witryna Software Update Services (SUS) 1.0 i została ona usunięta przed zainstalowaniem programu WSUS.

W takim przypadku konieczne jest utworzenie nowej witryny sieci Web za pośrednictwem przystawki Menedżer internetowych usług informacyjnych (IIS). Po wykonaniu tej czynności można wybrać tę witrynę lub określić nową witrynę w trakcie pracy Instalatora programu WSUS.

Jeśli już podjęto próbę zainstalowania programu WSUS i instalacja nie powiodła się z powodu braku witryn, otwórz przystawkę Menedżer internetowych usług informacyjnych (IIS) i usuń witrynę sieci Web nr 1. Następnie wykonaj czynności opisane wcześniej i ponownie uruchom Instalatora.

#### Problem 3: Instalowanie wstępnie wymaganych składników

#### Wymagania programowe

W poniższej tabeli przedstawiono oprogramowanie wymagane dla poszczególnych obsługiwanych systemów operacyjnych. Przed uruchomieniem Instalatora programu WSUS należy upewnić się, czy serwer WSUS spełnia wymagania wymienione na tej liście. Jeśli jakiekolwiek z tych uaktualnień wymagają ponownego uruchomienia komputera po zakończeniu aktualizacji, komputera należy ponownie uruchomić przed zainstalowaniem programu WSUS.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >System operacyjny</th>
<th style="border:1px solid black;" >Wymagania</th>
<th style="border:1px solid black;" >Pliki pobieralne</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Wszystkie systemy operacyjne</td>
<td style="border:1px solid black;">Microsoft Internet Information Services (IIS) 5.0</td>
<td style="border:1px solid black;">Zainstaluj z systemu operacyjnego.
Patrz Problem 1: Wymagane jest zainstalowanie Internetowych usług informacyjnych.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Wszystkie systemy operacyjne</td>
<td style="border:1px solid black;">Background Intelligent Transfer Service (BITS) 2.0</td>
<td style="border:1px solid black;">W przypadku systemów Windows Server 2003 — zobacz aktualizację usługi Background Intelligent Transfer Service (BITS) 2.0 i WinHTTP 5.1 Windows Server 2003 (KB842773) w Centrum pobierania (<a href="http://go.microsoft.com/fwlink/?linkid=47251">http://go.microsoft.com/fwlink/?LinkId=47251</a>).
W przypadku systemów operacyjnych Windows Server 2000 — zobacz aktualizację usługi Background Intelligent Transfer Service (BITS) 2.0 i WinHTTP 5.1 Windows 2000 (KB842773) w Centrum pobierania (<a href="http://go.microsoft.com/fwlink/?linkid=46794">http://go.microsoft.com/fwlink/?LinkId=46794</a>).</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Server 2003</td>
<td style="border:1px solid black;">Microsoft .NET Framework 1.1 z dodatkiem Service Pack 1 dla systemu Windows Server 2003</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=47358">Microsoft .NET Framework 1.1 z dodatkiem Service Pack 1 dla systemu Windows Server 2003</a>
Alternatywnie, przejdź do witryny <a href="http://go.microsoft.com/fwlink/?linkid=47370">Windows Update</a> i sprawdź dostępność krytycznych aktualizacji i dodatków Service Pack; zainstaluj pakiet Microsoft .NET Framework 1.1 z dodatkiem Service Pack 1 dla systemu Windows Server 2003.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows Server 2003</td>
<td style="border:1px solid black;">Oprogramowanie bazy danych w pełni zgodne z językiem Microsoft SQL</td>
<td style="border:1px solid black;">N/D</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows 2000 Server</td>
<td style="border:1px solid black;">Oprogramowanie bazy danych w pełni zgodne z językiem Microsoft SQL</td>
<td style="border:1px solid black;">Jeśli nie jest używany program Microsoft SQL Server 2000, można zainstalować program Microsoft SQL Server 2000 Desktop Engine (MSDE 2000). Wymaga to wykonania kilku czynności. Aby uzyskać więcej informacji, zobacz punkt Instalowanie programu MSDE w systemie Windows 2000 (poniżej).</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows 2000 Server</td>
<td style="border:1px solid black;">Program Microsoft Internet Explorer 6.0 z dodatkiem Service Pack 1</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=47359">Program Internet Explorer 6 z dodatkiem Service Pack 1</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows 2000 Server</td>
<td style="border:1px solid black;">Microsoft .NET Framework w wersji 1.1 do dystrybucji</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=47369">Microsoft .NET Framework w wersji 1.1 do dystrybucji</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows 2000 Server</td>
<td style="border:1px solid black;">Microsoft .NET Framework 1.1 z dodatkiem Service Pack 1</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=47368">Microsoft .NET Framework 1.1 z dodatkiem Service Pack 1</a>
Alternatywnie, przejdź do witryny <a href="http://go.microsoft.com/fwlink/?linkid=47370">Windows Update</a> i sprawdź dostępność krytycznych aktualizacji i dodatków Service Pack; zainstaluj pakiet Microsoft .NET Framework 1.1 z dodatkiem Service Pack 1 dla systemu Windows Server 2000.</td>
</tr>
</tbody>
</table>
 

Oprócz tych wymagań program WSUS może w razie potrzeby zainstalować lub skonfigurować na serwerze funkcję ASP.NET w wersji 1.1. (Funkcję ASP.NET konfiguruje instalator WSUS).

#### Instalowanie programu MSDE 2000 w systemie Windows 2000

W przypadku używania systemu Windows 2000 dla programu WSUS i braku dostępu do programu Microsoft SQL Server 2000 przed uruchomieniem Instalatora programu WSUS należy zainstalować program Microsoft SQL Server 2000 Desktop Engine (MSDE). Jeśli na serwerze WSUS jest już zainstalowany program MSDE, nie ma potrzeby instalowania jego specjalnej instancji dla programu WSUS. Można po prostu wskazać istniejącą nazwę instancji w trakcie procesu instalacji programu WSUS.

Instalowanie programu MSDE w systemie Windows 2000 Server jest procesem składającym się z czterech etapów. Najpierw należy pobrać i rozwinąć archiwum programu MSDE do folderu znajdującego się na serwerze WSUS. Następnie za pomocą wiersza polecenia i jego opcji należy uruchomić Instalatora programu MSDE, określić hasło administratora systemu i przypisać WSUS jako nazwę instancji. Następnie po zakończeniu instalacji programu MSDE należy sprawdzić, czy instancja programu WSUS jest uruchomiona jako usługa systemu NT. W końcowym etapie należy dodać poprawkę zabezpieczeń do programu MSDE w celu zabezpieczenia serwera WSUS.

#### Krok 1: Pobranie i rozwinięcie archiwum programu MSDE

Pobierz i rozwiń archiwum programu MSDE do folderu znajdującego się na serwerze WSUS. Zobacz [Microsoft SQL Server Desktop Engine (MSDE 2000) wydanie A](http://go.microsoft.com/fwlink/?linkid=47366).

#### Krok 2: Instalacja programu MSDE

Za pomocą wiersza polecenia i jego opcji uruchom Instalatora programu MSDE, określ hasło i przypisz WSUS jako nazwę instancji. Po zakończeniu instalacji programu MSDE sprawdź, czy instancja programu WSUS jest uruchomiona jako usługa NT.

Aby zainstalować program MSDE, określ hasło administratora systemu i przypisz nazwę instancji:

1.  W wierszu polecenia przejdź do folderu instalacji programu MSDE podanego w „Kroku 1: Pobranie i rozwinięcie archiwum programu MSDE”.
2.  Wpisz następujące polecenie: **setup sapwd="***hasło***" nazwa\_instancji=WSUS***,*
    gdzie zmienna *hasło* jest silnym hasłem do konta administratora systemu w tej instancji programu MSDE, natomiast zmienna **nazwa\_instancji** jest nazwą instancji bazy danych. Alternatywnie, dla bazy danych WSUS można użyć domyślnej nazwy instancji (zamiast „WSUS”). W przypadku wybrania tego rozwiązania nie ma potrzeby wpisywania polecenia **instancename=WSUS** jako parametru w wierszu polecenia. To polecenie umożliwia uruchomienie programu instalacyjnego MSDE, podanie wartości dla hasła administratora systemu oraz nazw instancji programu MSDE.

#### Krok 3: Sprawdzenie instalacji instancji WSUS programu MSDE

1.  Kliknij przycisk **Start**, a następnie polecenie **Uruchom**.
2.  W polu **Otwórz** wpisz **services.msc**, a następnie kliknij przycisk **OK**.

Przewiń listę usług i sprawdź, czy usługa SSQL$WSUS (jeśli nazwa instancji to „WSUS”) lub MSSQLSERVER (jeśli użyto domyślnej nazwy instancji) istnieje.

#### Krok 4: Uruchomienie instancji programu MSDE

Na końcu procesu instalacji programu MSDE należy uruchomić instancję. Jeśli jako nazwę instancji została podana wartość „WSUS”, uruchom usługę „MSSQL$WSUS”. W przypadku użycia domyślnej nazwy instancji uruchom usługę MSSQLSERVER. Dopóki te usługa nie zostanie uruchomiona, program nie będzie mógł korzystać z instancji bazy danych.

#### Krok 5: Uaktualnienie programu MSDE

Wymagane jest pobranie i zainstalowanie poprawki zabezpieczeń opisanej w biuletynie [MS03-031: Cumulative Security Patch for SQL Server (Skumulowany pakiet zabezpieczeń dla programu SQL Server)](http://go.microsoft.com/fwlink/?linkid=47364).

Aby pobrać pakiet zabezpieczeń, zobacz artykuł dotyczący [pakietu poprawek dla programu SQL Server 2000 (32-bitowy) MS03-031](http://go.microsoft.com/fwlink/?linkid=47363).

#### Problem 4: Wymagania dotyczące minimalnego miejsca na dysku

Poniżej przedstawiono wymagania dotyczące minimalnego miejsca na dysku dla instalacji programu Windows Server Update Services:

-   1 gigabajt (GB) w partycji systemowej
-   2 GB dla woluminu, na którym będą przechowywane pliki bazy danych
-   6 GB, co jest wartością oszacowaną na podstawie przewidywanej objętości zawartości

#### Problem 5: Przed zainstalowaniem najnowszej wersji programu WSUS należy odinstalować wcześniejsze wersje tego programu za pomocą apletu Dodaj lub usuń programy

W przypadku zamiaru zainstalowania programu Windows Server Update Services na serwerze, na którym jest zainstalowany program Windows Update Services w wersji beta 1 lub beta 2 należy najpierw odinstalować wcześniejszą wersję programu za pomocą apletu Dodaj lub usuń programy w Panelu sterowania.

#### Problem 6: Program WSUS wymaga włączenia opcji zagnieżdżonych wyzwalaczy w programie SQL Server

Ta opcja jest domyślnie włączona; jednak może zostać wyłączona przez administratora programu SQL Server.

W przypadku zamiaru używania bazy danych programu SQL Server jako magazynu danych programu Windows Server Update Services administrator serwera SQL powinien sprawdzić, czy opcja zagnieżdżonych wyzwalaczy na serwerze jest włączona zanim administrator WSUS zainstaluje program WSUS i wskaże bazę danych w trakcie instalacji.

Instalator programu WSUS powoduje włączenie opcji RECURSIVE\_TRIGGERS właściwej dla bazy danych; jednak nie powoduje włączenia opcji zagnieżdżonych wyzwalaczy będącej globalną opcją serwera.

Aby sprawdzić, czy opcja wyzwalaczy zagnieżdżonych jest włączona, użyj następującego polecenia:

**sp\_configure 'nested triggers'**

Aby włączyć opcję zagnieżdżonych wyzwalaczy na serwerze SQL, uruchom poniższe polecenie z pliku wsadowego na komputerze z zainstalowanym programem SQL Server:

**sp\_configure 'nested triggers', 1**

**GO**

**RECONFIGURE**

**GO**

#### Problem 7: Parametry wiersza polecenia Instalatora programu WSUS

Istnieje możliwość wykonania instalacji nienadzorowanej programu WSUS. Aby uzyskać więcej informacji oraz parametry wiersza polecenia, zobacz „Dodatek A: Instalacja nienadzorowana” w części dotyczącej [wdrażania programu Microsoft Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=41777).

Znane problemy
--------------

#### Problem 1: Kreator IIS Lockdown

W przypadku uruchamiania Internetowych usług informacyjnych (IIS) na komputerze z zainstalowanym systemem Windows 2000 Server zainstaluj najnowszą wersję Kreatora IIS Lockdown (zawierającej narzędzie URLScan) ze strony IIS Lockdown Tool (Narzędzie IIS Lockdown) w bazie informacji technicznych Microsoft TechNet. Firma Microsoft zdecydowanie zaleca zainstalowanie tego narzędzia w celu zabezpieczenia serwerów Internetowych usług informacyjnych. Działanie Kreatora IIS Lockdown polega na wyłączeniu zbędnych funkcji Internetowych usług informacyjnych, co ogranicza zagrożenie dla bezpieczeństwa.

| ![](images/Cc708486.note(WS.10).gif)Uwaga                                                                                                                                                                                     |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Instalator programu WSUS nie instaluje tych składników. Te składniki muszą zostać zainstalowane ręcznie. Nie ma potrzeby instalowania narzędzia IIS Lockdown na komputerach z systemem Windows Server 2003, ponieważ ta funkcja jest częścią tego systemu. |

#### Problem 2: Zmiana konfiguracji programu WSUS bezpośrednio w bazie danych nie jest obsługiwana

Dane konfiguracji programu Windows Server Update Services są przechowywane w bazie danych (programu MSDE lub SQL Server). Jednak zmiana danych konfiguracji przez bezpośredni dostęp do bazy danych nie jest obsługiwana. Administratorzy nie powinni podejmować prób modyfikacji konfiguracji programu WSUS w ten sposób. Konfigurację programu WSUS można zmieniać za pośrednictwem konsoli WSUS lub przez wywoływanie interfejsów API programu WSUS.

#### Problem 3: Aby można było uzyskać dostęp do witryny administracyjnej programu WSUS, należy włączyć opcję wykonywania skryptów aktywnych

Aby można było uzyskać dostęp do witryny administracyjnej programu WSUS za pośrednictwem programu Internet Explorer, na stacji roboczej administratora należy skonfigurować program Internet Explorer w taki sposób, aby zezwalał na wykonywanie skryptów aktywnych.

#### Problem 4: Usługa IIS zostanie ponownie uruchomiona podczas instalacji programu WSUS

Instalator programu Windows Server Update Services ponownie uruchomi usługę IIS bez powiadomienia. Może to mieć wpływ na istniejące witryny sieci Web w danej organizacji.

#### Problem 5: Zmiana dostępu do katalogu wirtualnego punktów zarządzania programem WSUS lub SMS

Domyślnie dostęp do zawartości katalogu wirtualnego programu Windows Server Update Services jest możliwy w trybie anonimowym. W przypadku zmiany tego ustawienia i żądania uwierzytelniania klienci będą otrzymywać błędy dotyczące uwierzytelniania oraz nie będą mogli pobierać aktualizacji. Jest to znany problem wynikający z faktu, że biblioteka Winhttp.dll używa niewłaściwego kontekstu uwierzytelniania, gdy wymagane jest uwierzytelnianie niejawne, a w konsekwencji wezwanie do uwierzytelnienia kończy się niepowodzeniem. Aby uniknąć tego problemu, upewnij się, że dla serwera WSUS oraz punktów zarządzania (MP) programem SMS został skonfigurowany dostęp anonimowy do katalogów wirtualnych usług IIS.

#### Problem 6: W przypadku instalowania programu WSUS w systemie Windows Small Business Server 2003 należy zmodyfikować domyślne ustawienia dostępu do wirtualnych katalogów głównych programu WSUS w witrynie sieci Web w taki sposób, aby klienci WSUS mogli dokonywać autoaktualizacji z serwera

W trakcie instalacji serwera WSUS są instalowane dwa wirtualne katalogi główne, SelfUpdate i ClientWebService, oraz określone pliki w katalogu głównym domyślnej witryny sieci Web (na porcie 80). Dzięki temu klienci mogą dokonywać autoaktualizacji za pośrednictwem domyślnej witryny sieci Web. Domyślnie w systemie Windows Small Business Server 2003 konfiguracja domyślnej witryny sieci Web zezwala tylko na dostęp do adresu IP i hosta lokalnego tego serwera. Oznacza to odmowę dostępu do wirtualnych katalogów głównych SelfUpdate i ClientWebService oraz brak możliwości wykonywania autoaktualizacji przez klientów. Aby zezwolić klientom na wykonywanie autoaktualizacji, wykonaj poniższe czynności w wirtualnych katalogach głównych SelfUpdate i ClientWebService w domyślnej witrynie sieci Web.

1.  W wirtualnym katalogu głównym kliknij polecenie **Właściwości**, kliknij polecenie **Zabezpieczenia katalogów**, kliknij polecenie **Ograniczenia adresów IP i nazw domen**, a następnie kliknij polecenie **Edytuj**.
2.  Wybierz opcję **Udzielony dostęp**, a następnie kliknij przycisk **OK**. Zamknij wszystkie strony właściwości.

#### Problem 7: Instalowanie programu WSUS w systemie Small Business Server — problemy z integracją

-   Jeśli system Windows Small Business Server 2003 uzyskuje dostęp do Internetu za pośrednictwem serwera proxy ISA, w interfejsie użytkownika **Ustawienia** należy ręcznie wprowadzić następujące ustawienia: ustawienia serwera proxy, nazwę serwera proxy oraz port.
-   Jeśli program ISA korzysta z uwierzytelniania systemu Windows, poświadczenia serwera proxy muszą zostać wprowadzone w postaci „DOMENA\\użytkownik” (użytkownik należący do grupy „Użytkownicy Internetu”).

#### Problem 8: W przypadku przenoszenia komputera z jednej grupy komputerów do drugiej opóźnienie przeniesienia komputera do nowej grupy widoczne z konsoli administracyjnej może wynosić maksymalnie godzinę

Gdy komputer zostanie po raz pierwszy przypisany do grupy docelowej, dane na komputerze są modyfikowane informacjami o grupie. Te dane są odświeżane systematycznie lub co godzinę. W związku z tym przy przenoszeniu komputera z jednej grupy komputerów do drugiej opóźnienie odświeżenia tych informacji na kliencie i wyświetlenie zmian na konsoli administracyjnej programu WSUS może wynosić maksymalnie godzinę.

#### Problem 9: W przypadku instalowania programu WSUS na serwerze członkowskim i zamiaru podwyższenia poziomu serwera członkowskiego do kontrolera domeny należy najpierw odinstalować program WSUS

W przypadku instalowania programu WSUS na serwerze członkowskim i zamiaru podwyższenia poziomu serwera członkowskiego do kontrolera domeny należy wykonać następujące czynności:

1.  Odinstaluj program WSUS.
2.  Podwyższ poziom serwera do kontrolera domeny.
3.  Ponownie zainstaluj program WSUS.

#### Problem 10: Aby obniżyć poziom serwera WSUS z kontrolera domeny na serwer członkowski, należy najpierw odinstalować program WSUS

W przypadku uruchomienia serwera WSUS na kontrolerze domeny i zamiaru obniżenia poziomu kontrolera domeny do serwera członkowskiego, należy wykonać następujące czynności:

1.  Odinstaluj program WSUS i zachowaj bazę danych.
2.  Utwórz konto użytkownika ASPNET.
3.  W wierszu polecenia wpisz polecenie **aspnet\_regiis -i**.
4.  Ponownie zainstaluj program WSUS i użyj zachowanej bazy danych.

#### Problem 11: Jeśli platforma .NET Framework 1.0 lub 2.0 została zainstalowana po zainstalowaniu programu WSUS, konsola administracyjna programu WSUS nie będzie wyświetlana

Wynika to z tego, że platforma .NET Framework 1.0 jest rejestrowana za pośrednictwem usług IIS, a serwer WSUS wymaga platformy .NET Framework 1.1. Aby rozwiązać ten problem, otwórz plik aspnet\_regiis.exe i uruchom poniższe polecenia, w których zmienna *id\_witryny\_sieci\_Web* jest wartością znajdującą się w następującym kluczu rejestru:

HKLM\\Software\\Microsoft\\WindowsUpdateServices\\Server\\Setup\\IISTargetWebsiteIndex

-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*id\_witryny\_sieci\_Web*&gt;\\ROOT\\ReportingWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*id\_witryny\_sieci\_Web*&gt;\\ROOT\\ClientWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*id\_witryny\_sieci\_Web*&gt;\\ROOT\\SimpleAuthWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*id\_witryny\_sieci\_Web*&gt;\\ROOT\\WSUSAdmin
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*id\_witryny\_sieci\_Web*&gt;\\ROOT\\AdministrationWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*id\_witryny\_sieci\_Web*&gt;\\ROOT\\ServrSyncWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*id\_witryny\_sieci\_Web*&gt;\\ROOT\\DssAuthWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*id\_witryny\_sieci\_Web*&gt;\\ROOT\\Content

#### Problem 12: Ograniczenia zdalnego serwera SQL

Program WSUS oferuje ograniczoną obsługę uruchamiania oprogramowania baz danych na komputerze innym niż komputer zawierający pozostałe aplikacje WSUS.

-   Nie można używać serwera Windows 2000 Server jako komputera frontonu w zdalnej parze SQL.
-   Nie można używać serwera skonfigurowanego jako kontroler domeny jako serwera frontonu lub serwera typu back-end zdalnej pary SQL.
-   Nie można używać programu WMSDE ani MSDE dla oprogramowania bazy danych na komputerach typu back-end.
-   Instalacja zdalnego serwera SQL (który ma być używany jako baza danych WSUS) nie powiedzie się, jeśli usługi terminalowe są zainstalowane na serwerze zdalnym i działają w trybie aplikacji. Podczas instalowania programu SQL Server na serwerze usług terminalowych należy wykonać następujące czynności:
    1.  Przed uruchomieniem instalatora otwórz wiersz polecenia i wpisz polecenie: „change user /install”
    2.  Uruchom Instalatora programu SQL Server.
    3.  Po uruchomieniu instalatora w wierszu polecenia wpisz polecenie: "change user /execute"
-   Aby można było zainstalować bazę danych WSUS na serwerze zdalnym SQL, użytkownik musi należeć do lokalnej grupy zabezpieczeń Administratorzy zarówno na komputerze frontonu, jak i komputerze typu back-end.
-   Aby uzyskać więcej informacji na temat problemów ze zdalnym serwerem SQL, zobacz „Dodatek C: Zdalny serwer SQL” w części dotyczącej [wdrażania programu Microsoft Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=41777).

#### Problem 13: Następny serwer replik może mieć mniej zatwierdzeń niż poprzedni serwer nadrzędny.

Następny serwer replik może mieć mniej zatwierdzeń niż poprzedni serwer nadrzędny. Wynika to z faktu, że zatwierdzenia instalacji nie przepływają do następnego serwera, dopóki pobieranie zawartości nie zakończy się na poprzednim serwerze.

#### Problem 14: W razie niepowodzenia synchronizacji wstępnej należy ponowić próbę synchronizacji

Jeśli synchronizacja nie powiedzie się, pierwszym etapem rozwiązywania problemów jest ponowienie próby synchronizacji serwera. Jeśli kolejna próba synchronizacji nie powiedzie się, skorzystaj z informacji dotyczących rozwiązywania problemów znajdujących się w dokumencie WSUS Operations Guide (Przewodnik po obsłudze programu WSUS).

#### Problem 15: Przy próbie uzyskania dostępu do konsoli administracyjnej programu WSUS jest wyświetlany komunikat o błędzie System.IO.FileNotFoundException

W przypadku wyświetlenia poniższego komunikatu o błędzie konieczna może być zmiana uprawnień na kontach usługi sieciowej lub ASP.NET:

System.IO.FileNotFoundException: File or Assembly name *xxxxxx*.dll, or one of its dependencies, was not found

Zmienna *xxxx* jest nazwą losową.

Aby rozwiązać ten problem w systemach operacyjnych Windows Server 2003, nadaj dla konta usługi sieciowej uprawnienie odczytu/zapisu do folderu to %systemroot%\\Temp. W systemie Windows 2000 Server nadaj dla konta ASP.NET uprawnienie odczytu/zapisu dla folderu %systemroot%\\Temp.

#### Problem 16: Aktualizacja zabezpieczeń SQL MS03-031 (KB815495)

Ta aktualizacja może być wskazywana jako zainstalowana na serwerze WSUS, nawet wtedy, gdy instalacja na kliencie nie powiodła się. Z tego powodu pakiet może być ponownie oferowany klientowi. Ten problem można obejść, cofając zatwierdzenie aktualizacji na serwerze.

#### Problem 17: Utrata ustawień usług IIS podczas uaktualniania wersji RTM.

W przypadku instalacji programu WSUS RTM na serwerze z zainstalowaną poprzednią wersją programu WSUS (na przykład RC) program WSUS RTM spowoduje odinstalowanie wcześniejszej wersji, a następnie zainstalowanie nowej wersji. Oznacza to, że wirtualne katalogi główne i pliki skojarzone z programem WSUS w ramach Internetowych usług informacyjnych zostaną usunięte.

W przypadku zainstalowania programu WSUS w domyślnej witrynie sieci Web ustawienia katalogów wirtualnych programu WSUS charakterystyczne dla tego programu zostaną utracone. Na przykład, jeśli wirtualne katalogi główne programu WSUS zostały skonfigurowane dla protokołu SSL w celu zabezpieczenia programu WSUS, konieczne będzie ich ponowne skonfigurowanie po zainstalowaniu wersji RTM programu WSUS. Uwaga: w konsoli programu WSUS zostanie wyświetlone powiadomienie o włączeniu obsługi protokołu SSL.

Jeśli program WSUS nie został zainstalowany w domyślnej witrynie sieci Web, wszystkie ustawienia dodatkowe na poziomie witryny sieci Web programu WSUS zostaną utracone.

#### Problem 18: Korzystanie z nagłówków hosta

Aby przypisać wartości nagłówków hosta do domyślnej witryny sieci Web (witryna sieci Web programu WSUS) w ramach Internetowych usług informacyjnych, należy dodać „wszystkie nieprzypisane” lub przypisany adres IP do listy adresów IP bez wartości nagłówka hosta w domyślnej witrynie sieci Web. Informacje te należy także dodać do witryny sieci Web innej niż domyślna.

**Ostrzeżenie**: Może to spowodować zakłócenia pracy programu Microsoft SharePoint i Exchange.

#### Problem 19: Konieczne jest dodanie adresu URL konsoli programu WSUS do listy stref zawartości sieci Web Zaufane witryny lub Lokalny intranet na komputerach z włączoną opcją ograniczenia funkcjonalności programu Internet Explorer

Jeśli opcja ograniczenia funkcjonalności programu Internet Explorer (znana także jako składnik Konfiguracja zwiększonych zabezpieczeń programu Internet Explorer w systemie Microsoft Windows Server 2003 Internet Explorer) jest włączona na komputerze i konsola programu WSUS nie zostanie dodana do stref zawartości sieci Web Zaufane witryny lub Lokalny intranet, przy każdej próbie otwarcia strony w konsoli programu WSUS będzie wyświetlany monit z prośbą o podanie poświadczeń użytkownika.

Aby dodać konsolę programu WSUS do stref zawartości sieci Web **Lokalny intranet** oraz **Zaufane witryny**:

1.  Otwórz aplet **Opcje internetowe** (na przykład kliknij przycisk **Start**, wskaż polecenie **Panel sterowania**, a następnie kliknij polecenie **Opcje internetowe**).
2.  Na karcie **Zabezpieczenia** kliknij polecenie **Lokalny intranet**, kliknij polecenie **Witryny**, kliknij opcję **Zaawansowane**, dodaj adres URL (http://*nazwa\_serwera\_WSUS*/WSUSAdmin), a następnie kliknij przycisk **OK**.
3.  Kliknij polecenie **Zaufane witryny**, kliknij polecenie **Witryny**, dodaj adres URL konsoli programu WSUS, kliknij przycisk **OK**, a następnie ponownie kliknij przycisk **OK**, aby zamknąć aplet **Opcje internetowe**.

#### Prawa autorskie

Informacje zawarte w niniejszym dokumencie odpowiadają aktualnemu w dniu publikacji poglądowi firmy Microsoft Corporation na omawiane zagadnienia. Ponieważ firma Microsoft musi reagować na zmieniające się uwarunkowania rynkowe, niniejszego materiału nie należy traktować jako zobowiązania ze strony firmy Microsoft, a firma Microsoft nie może zagwarantować poprawności jakichkolwiek informacji zamieszczonych w niniejszych dokumencie po dacie publikacji.

Niniejszy dokument ma charakter wyłącznie informacyjny. FIRMA MICROSOFT NIE UDZIELA ŻADNYCH GWARANCJI, JAWNYCH, DOMNIEMANYCH ANI USTAWOWYCH, W ZAKRESIE ZAMIESZCZONYCH W NINIEJSZYM DOKUMENCIE INFORMACJI.

Za przestrzeganie wszelkich odpowiednich praw autorskich odpowiada użytkownik. Niezależnie od praw wchodzących w zakres praw autorskich, żadnej części tego dokumentu nie można powielać, przechowywać lub wprowadzać do systemów wyszukiwania informacji ani też przekazywać w żadnej formie lub za pomocą jakichkolwiek urządzeń (elektronicznych, mechanicznych, fotokopiujących, rejestrujących lub innych) w jakimkolwiek celu, bez pisemnej zgody firmy Microsoft Corporation.

Firma Microsoft może posiadać patenty, zgłoszenia patentowe, znaki towarowe, prawa autorskie lub inne prawa własności intelektualnej dotyczące treści tego dokumentu. Z wyjątkiem przypadków wyraźnie określonych w jakiejkolwiek pisemnej umowie licencyjnej firmy Microsoft, udostępnienie tego dokumentu nie jest równoznaczne z udzieleniem użytkownikowi jakichkolwiek licencji na wymienione patenty, znaki towarowe, prawa autorskie lub inną własność intelektualną.

Wszystkie firmy, organizacje, produkty, nazwy domen, adresy e-mail, logo, osoby, miejsca i zdarzenia używane w przykładach są fikcyjne i nie mają żadnego związku z jakimikolwiek rzeczywistymi firmami, organizacjami, produktami, nazwami domen, adresami e-mail, logo, osobami, miejscami lub zdarzeniami, o ile nie zaznaczono, że jest inaczej.

© 2006 Microsoft Corporation. Wszelkie prawa zastrzeżone.

Microsoft, SQL Server, Windows, i Windows Server są zastrzeżonymi znakami towarowymi lub znakami towarowymi firmy Microsoft Corporation w Stanach Zjednoczonych i/lub innych krajach.

Nazwy rzeczywistych firm i produktów wymienionych w tym dokumencie mogą być znakami towarowymi ich prawnych właścicieli.
