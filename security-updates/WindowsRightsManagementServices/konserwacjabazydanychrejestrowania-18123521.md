---
TOCTitle: Konserwacja bazy danych rejestrowania
Title: Konserwacja bazy danych rejestrowania
ms:assetid: 'de55058b-0d1a-4997-8a45-e14678ddd13f'
ms:contentKeyID: 18123521
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747691(v=WS.10)'
---

Konserwacja bazy danych rejestrowania
=====================================

Wpisy dziennika zawierają również kopie licencji wystawianych dla różnych operacji programu RMS, np. rejestrowania użytkowników i przypisywania licencji użytkowania. W najgorszym przypadku — gdy każdy wpis dziennika jest pomyślną rejestracją użytkownika lub pomyślnym uzyskaniem licencji użytkowania — każdy wpis zwiększy rozmiar bazy danych rejestrowania o około 200 KB.

Przykładowo wiadomość e-mail chroniona technologią RMS została wysłana do wszystkich pracowników przedsiębiorstwa zatrudniającego 50 tys. osób i każdy z nich otworzył ją. Jeżeli wszyscy pracownicy otworzą tę wiadomość w ciągu jednego dnia, to rozmiar bazy danych rejestrowania zwiększy się o 10 GB. Poprzez wyłączenie rejestrowania rzeczywistych danych XrML przez usługę odbiornika można zmniejszyć ilość rejestrowanych informacji.

Należy rozważyć utworzenie skryptów archiwizujących starsze informacje z bazy danych rejestrowania w pomocniczej bazie danych. Przykładowe skrypty rejestrowania są dostępne w zestawie RMS Toolkit, który można bezpłatnie pobrać z [witryny sieci Web firmy Microsoft](http://go.microsoft.com/fwlink/?linkid=26724)(http://go.microsoft.com/fwlink/?LinkId=26724).

Zmienne decydujące o przyroście bazy danych rejestrowania
---------------------------------------------------------

Prognozowanie rozmiaru bazy danych rejestrowania jest uzależnione od danego środowiska. Można prognozować liczbę początkowych wpisów rejestru, w tym:

-   Rejestracje serwera programu RMS
-   Rejestracje użytkowników (unikatowe żądanie z każdego komputera użyte przez każdego użytkownika)
-   Automatyczne żądania użytkowników dotyczące certyfikatów publikowania w trybie offline

Liczba wpisów w bazie rejestrowania po zainicjowaniu jej wpisami początkowymi jest uzależniona od wystawiania licencji użytkowania dla zawartości chronionej. O przyroście tej bazy danych decyduje kilka warunków:

-   Każdorazowe wymaganie nowej licencji przy próbie dostępu do zawartości chronionej. Nie jest to domyślna metoda używana dla dokumentów chronionych, lecz ustawienie opcjonalne. W przypadku dokonania implementacji tego wymagania rozmiar baz danych będzie rósł w szybszym tempie.
-   Spodziewana liczba chronionych wiadomości e-mail codziennie wysyłanych do wszystkich osób.
-   Spodziewana liczba unikatowych użytkowników, którzy odczytają te wiadomości.
-   Spodziewana liczba chronionych dokumentów pakietu Microsoft Office 2003 (programów Word, PowerPoint i Excel), codziennie tworzonych przez wszystkich użytkowników.
-   Spodziewana liczba odbiorców tych dokumentów.

Początkowy rozmiar bazy danych rejestrowania będzie wynosił około 1,7 MB, co obejmuje żądanie certyfikatu od serwera programu RMS. Podczas każdej rejestracji nowego użytkownika otrzymuje on certyfikat konta praw (RAC) i certyfikat licencjodawcy klienta (CLC). Obie czynności są rejestrowane i każda z nich zwiększa rozmiar bazy danych o 0,06 MB. Każde pomyślne uzyskanie przez użytkownika licencji dla zawartości chronionej zwiększa rozmiar bazy danych o 0,19 MB.

Powyższe szacunki można zobrazować na przykładzie organizacji z 5 tys. użytkowników, w której wszyscy korzystają z programu RMS. Każdy użytkownik ma jeden komputer i używane są dwa serwery programu RMS. Po rozmieszczeniu każdy użytkownik tworzy dziennie średnio jedną wiadomość e-mail chronioną technologią RMS, która jest wysyłana do pięciu innych użytkowników. Każdy użytkownik tworzy również codziennie jeden dokument chroniony technologią RMS, z którego korzysta trzech innych użytkowników. Poniższa tabela przedstawia szacunkowe wartości zwiększenia rozmiaru bazy danych rejestrowania dla poszczególnych czynności.

 
<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Czynność</th>
<th style="border:1px solid black;" >Przyrost dziennika</th>
<th style="border:1px solid black;" >Skumulowany rozmiar dziennika</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Pomyślne zastrzeżenie serwera programu RMS</td>
<td style="border:1px solid black;">1,7 MB</td>
<td style="border:1px solid black;">1,7 MB</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Rejestracja 5 tys. pracowników (5000*0,06)</td>
<td style="border:1px solid black;">300 MB</td>
<td style="border:1px solid black;">301,7 MB</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Uzyskanie dostępu do chronionych wiadomości e-mail (25000*0,19)</td>
<td style="border:1px solid black;">4 750 MB</td>
<td style="border:1px solid black;">5 051,7 MB</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Uzyskanie dostępu do chronionych dokumentów (15000*0,19)</td>
<td style="border:1px solid black;">2 850 MB</td>
<td style="border:1px solid black;">7 901,7 MB</td>
</tr>
</tbody>
</table>
  
Po zarejestrowaniu pracowników statyczny rozmiar bazy danych rejestrowania wynosi około 300 MB. Jednak dzienny przyrost w powyższym przykładzie jest równy 7,6 GB — osiągając prawie 8 GB limit w domyślnej instalacji usługi kolejkowania wiadomości. Jeśli baza danych rejestrowania będzie niedostępna dłużej niż jeden dzień, wpisy dziennika zaczną być tracone.
  
Kontrolowanie rozmiaru bazy danych rejestrowania  
------------------------------------------------
  
W planie rozmieszczania należy uwzględnić metodę zarządzania bazą danych rejestrowania. Najczęściej stosowane są następujące metody.
  
-   **Odcięcie i archiwizacja**  
    Metoda ta polega na archiwizowaniu wybranych informacji z bazy danych rejestrowania w pomocniczej bazie danych za pomocą skryptów programu SQL Server, po osiągnięciu przez wpisy dziennika ustalonego wieku. Obejmuje ona także filtrowanie bazy danych pod kątem zbędnych informacji, co pozwala na zaoszczędzenie miejsca.  
-   **Ograniczenie rejestrowanych informacji**  
    Baza danych rejestrowania składa się z trzech głównych tabel. Jedną z nich jest tabela **DRMS\_Log\_Filter**, która określa pola z głównej tabeli rejestrowane przy włączonym filtrowaniu dziennika.  
    Wpisy tabeli w postaci przełączników „włącz/wyłącz” określają, które pola z głównej tabeli są faktycznie rejestrowane przez usługę odbiornika rejestrowania na serwerze programu RMS. W dwóch polach (powiązanych z XrML) zostały już ustawione wartości 0 w celu wyłączenia rejestrowania ze względu na prawie wyłączny udział tych pól (około 99%) w rozmiarze wiersza dla żądania licencji.  
    Tabela **DRMS\_ClusterPolicies** w bazie danych **DRMS\_Config\_ServerName\_Port** zawiera wpis **PolicyName** dla pola **LoggingFiltering**. Pole **LoggingFiltering** nie jest domyślnie włączone. Po zmianie wartości pola **LoggingFiltering** na 1 i zrestartowaniu usługi odbiornika rejestrowania dzienny przyrost bazy danych w powyższym przykładzie spadnie z 7,6 GB do około 160 MB.  
-   **Przeniesienie bazy danych rejestrowania**  
    Inną możliwością kontrolowania rosnącej bazy danych rejestrowania jest przeniesienie jej na serwer z większą ilością miejsca na dysku. Baza danych rejestrowania może znajdować się na innym serwerze bazy danych niż baza danych konfiguracji. Aby przenieść bazę danych na inny serwer, należy wykonać następujące czynności:  
    1.  Zatrzymaj usługę odbiornika rejestrowania na każdym z serwerów programu RMS.  
    2.  Skopiuj bazę danych (lub utwórz nową) na inny serwer.  
    3.  Zmodyfikuj bazę danych programu RMS **DRMS\_Config\_ServerName\_Port** zaznaczając tabelę **DRMS\_ClusterPolicies** i zmieniając wartości w polach **LoggingDatabaseName** (nazwa serwera bazy danych) i **LoggingDatabaseServer** (nazwa bazy danych).  
    4.  Ponownie uruchom usługi IIS za pomocą programu IISRESET.exe, uruchamianego z wiersza polecenia.
