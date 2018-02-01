---
TOCTitle: 'Aktualizacja wdrożonego rozwiązania przy użyciu usługi RMS z dodatkiem Service Pack 1 (SP1)'
Title: 'Aktualizacja wdrożonego rozwiązania przy użyciu usługi RMS z dodatkiem Service Pack 1 (SP1)'
ms:assetid: 'a562c4b0-15df-46db-9d61-24db74871cfa'
ms:contentKeyID: 18123419
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747714(v=WS.10)'
---

Aktualizacja wdrożonego rozwiązania przy użyciu usługi RMS z dodatkiem Service Pack 1 (SP1)
===========================================================================================

Poniższa sekcja zawiera informacje pomocne w instalacji usługi Microsoft® Windows® Rights Management Services (RMS) z dodatkiem Service Pack 1 (SP1) w organizacji, w której wdrożono już usługi RMS. Konieczność aktualizacji RMS do wersji z dodatkiem SP1 dotyczy tylko organizacji, w których wdrożono już usługi RMS. Organizacje, w których usługi RMS wdrażane są po raz pierwszy, mogą zainstalować usługi RMS z dodatkiem SP1 , postępując zgodnie ze wskazówkami zawartymi w artykułach Planowanie rozmieszczenia programu RMS i Rozmieszczanie systemu RMS należących do niniejszego zestawu dokumentacji.

Instalacja usług RMS z dodatkiem SP1 nie wymaga usuwania istniejącej instalacji RMS. Instalator usług RMS z dodatkiem SP1 wykrywa instalację usług RMS i w miarę potrzeb dodaje odpowiednie funkcje i ustawienia.

**W tym temacie**

-   [Przygotowanie do aktualizacji do wersji RMS z dodatkiem SP1](#bkmk_1)
-   [Przeprowadzenie aktualizacji do wersji RMS z dodatkiem SP1](#bkmk_2)
-   [Aktualizacja klastrów](#bkmk_3)
-   [Aktualizacja klientów RMS](#bkmk_4)
-   [Współdziałanie z RMS w wersji 1.0](#bkmk_5)
-   [Usuwanie usług RMS z dodatkiem SP1](#bkmk_6)

<span id="BKMK_1"></span>
Przygotowanie do aktualizacji do wersji RMS z dodatkiem SP1
-----------------------------------------------------------

Aktualizacja RMS do wersji z dodatkiem SP1 została przygotowana w sposób umożliwiający uniknięcie przerywania działania usług RMS. Przed uaktualnianiem serwerów usług RMS zaleca się jednak wykonanie następujących czynności:

-   Utwórz kopię zapasową bazy danych konfiguracji i klucza prywatnego RMS. Więcej informacji można znaleźć w artykule poświęconym kopiom zapasowym systemu dla usług RMS, który znajduje się w sekcji „Planowanie rozmieszczenia programu RMS” niniejszego zestawu dokumentacji.
-   Upewnij się, że posiadasz hasło klucza prywatnego RMS.
-   Wykonaj kopię zapasową bazy danych rejestrowania, aby zachować zarejestrowane wcześniej statystyki.
-   Upewnij się, że zostały zainstalowane najnowsze aktualizacje krytyczne oraz aktualizacje zabezpieczeń dla systemu operacyjnego klientów i serwerów. Aby sprawdzić, czy zostały zainstalowane wszystkie aktualizacje krytyczne oraz aktualizacje zabezpieczeń, kliknij przycisk **Start**, kliknij **Windows Update**, a następnie wykonaj instrukcje wyświetlane na ekranie.

<span id="BKMK_2"></span>
Przeprowadzenie aktualizacji do wersji RMS z dodatkiem SP1
----------------------------------------------------------

Gdy kreator instalacji usług RMS z dodatkiem SP1 wykryje zainstalowane usługi RMS, dodaje tylko nowe pliki lub zastępuje istniejące, jeśli wymaga tego wersja RMS z dodatkiem SP1. Jeśli na komputerach działają już usługi RMS, po instalacji usług RMS z dodatkiem SP1 nie ma potrzeby ponownego zastrzegania oprogramowania ani przeprowadzania dodatkowych prac konfiguracyjnych, aby ich działanie było kontynuowane.

<span id="BKMK_3"></span>
Aktualizacja klastrów
---------------------

Jeśli usługi RMS zostały zainstalowane w konfiguracji klastra, należy tak planować aktualizację klastrów, aby zmniejszyć do minimum jej wpływ na instalację. Określając najlepszy sposób wdrożenia w organizacji usług RMS z dodatkiem SP1, należy wziąć pod uwagę następujące zalecenia:

-   Zaleca się instalowanie usług RMS z dodatkiem SP1 na jednej części klastra naraz, co pozwala zwiększyć przewidywalność procesu uaktualniania klastra i zmniejszyć prawdopodobieństwo, że pociągnie on za sobą pogorszenie jakości świadczenia tych usług.
-   W przypadku wielu klastrów RMS należy najpierw uaktualniać klastry głównej certyfikacji, a następnie zarejestrowane podrzędnie klastry licencjonowania.
-   Użytkownicy korzystający z przechodzenia grup między lasami mogą niezależnie uaktualniać klastry w lasach, nie wpływając na zdolność serwerów RMS do rozwinięcia przynależności do grupy między lasami.
-   Usługi RMS z dodatkiem SP1 i serwer RMS w wersji 1.0 mogą współistnieć i współpracować.
-   Pakiet instalacyjny usług RMS z dodatkiem SP1 może także posłużyć do zainstalowania na serwerze nowej wersji usług RMS z dodatkiem SP1. Oprogramowanie serwera RMS w wersji 1.0 nie musi być zainstalowane.

<span id="BKMK_4"></span>
Aktualizacja klientów RMS
-------------------------

Wersja RMS z dodatkiem SP1 zawiera nowego klienta RMS. Pakiet instalacyjny klienta usług RMS z dodatkiem SP1 może także posłużyć do zainstalowania na komputerze nowej wersji klienta RMS z dodatkiem SP1. Klient RMS w wersji 1.0 nie musi być zainstalowany. Klient RMS z dodatkiem SP1 wyposażony został w funkcję zgodności wstecznej, dzięki której możliwe jest wykorzystanie go z aplikacjami obsługującymi RMS, które wymagają RMS w wersji 1.0.

Nowy klient RMS oferuje następujące funkcje:

-   Klient nie musi już łączyć się przez Internet z firmą Microsoft i pobierać skrytki.
-   Instalacja klienta RMS nie wymaga uprawnień administratora, jeśli przeprowadzana jest przy użyciu programu SMS lub zasad grupy.
-   Klient RMS z dodatkiem SP1 zawiera nową skrytkę serwera (znaną również pod nazwą procesora zabezpieczeń serwera), która może być wykorzystywana do zapewnienia obsługi RMS w usługach sieci Web lub aplikacjach wykonywanych po stronie serwera, takich jak programy Windows SharePoint® Services i Exchange Server 2003, dzięki czemu mogą one przyjmować i rozpowszechniać zawartość chronioną technologią RMS. Zastosowana skrytka została zaprojektowana w sposób zapewniający wysoką wydajność i skalowalność podczas używania w zaufanych aplikacjach serwera
-   Klient RMS wykorzystuje certyfikowane algorytmy kryptograficzne FIPS 140-2. Umożliwia to wdrażanie w organizacjach zachowujących zgodność ze standardem FIPS.

<span id="BKMK_5"></span>
Współdziałanie z RMS w wersji 1.0
---------------------------------

Ze względu na liczne udoskonalenia i rozszerzenia funkcjonalności zaleca się zainstalowanie RMS z dodatkiem SP1 po ukończeniu testów. Pomimo pełnej współpracy serwerów i klientów RMS z oprogramowaniem RMS z dodatkiem SP1 z serwerami i klientami RMS, na których nie zainstalowano tego oprogramowania, należy zdawać sobie sprawę z następujących różnic w ich działaniu w środowisku mieszanym:

-   Tylko serwery z oprogramowaniem RMS z dodatkiem SP1 oferują możliwość rejestrowania w trybie offline.
-   Tylko klienci z oprogramowaniem RMS z dodatkiem SP1 mają funkcję automatycznej aktywacji.
-   W poniższej tabeli ukazano funkcjonalność obsługiwaną w środowiskach mieszanych:

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Wersja serwera RMS</th>
<th style="border:1px solid black;" >Funkcje obsługiwane przy klientach z wersją 1</th>
<th style="border:1px solid black;" >Funkcje obsługiwane przy klientach z dodatkiem SP1</th>
<th style="border:1px solid black;" >Funkcje obsługiwane w środowiskach z różnymi klientami (wersja 1 i SP1)</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">1.0</td>
<td style="border:1px solid black;">Wszystkie starsze funkcje.
Brak rejestrowania serwera w trybie offline. Serwer musi być rejestrowany przez Internet.
Brak klientów z funkcją automatycznej aktywacji.</td>
<td style="border:1px solid black;">Wszystkie starsze funkcje.
Brak rejestrowania serwera w trybie offline.
Klienci z funkcją automatycznej aktywacji.</td>
<td style="border:1px solid black;">Wszystkie starsze funkcje.
Klienci z oprogramowaniem w wersji z dodatkiem SP1 mają funkcję automatycznej aktywacji.
W przypadku wersji 1 aktywacja klienta musi przebiegać za pośrednictwem Internetu.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">SP1</td>
<td style="border:1px solid black;">Wszystkie starsze funkcje.
Rejestrowanie serwera w trybie offline.
Brak klientów z funkcją automatycznej aktywacji.</td>
<td style="border:1px solid black;">Wszystkie funkcje SP1.
Rejestrowanie serwera w trybie offline.
Klienci z funkcją automatycznej aktywacji.
Skrytka serwera.</td>
<td style="border:1px solid black;">Wszystkie starsze funkcje i funkcje wersji z dodatkiem SP1.
Rejestrowanie serwera w trybie offline.
Klienci z oprogramowaniem w wersji z dodatkiem SP1 mają funkcję automatycznej aktywacji.
W przypadku wersji 1 aktywacja klienta musi przebiegać za pośrednictwem Internetu.</td>
</tr>
</tbody>
</table>
 

<span id="BKMK_6"></span>
Usuwanie usług RMS z dodatkiem SP1
----------------------------------

Aby po instalacji usług RMS z dodatkiem SP1 przywrócić poprzednią konfiguracje serwera RMS, można usunąć usługi RMS z dodatkiem SP1 przy użyciu apletu **Dodaj lub usuń programy** w **Panelu sterowania**.

**Uwaga**   Jeśli dostępna jest kopia zapasowa bazy danych konfiguracji, którą wykonano przez zainstalowaniem RMS z dodatkiem SP1, można przywrócić zawarte w niej dane, usuwając w ten sposób całkowicie wszystkie zmiany wprowadzone przez RMS z dodatkiem SP1. Jeśli nie wykonano kopii zapasowej bazy danych konfiguracji, może być możliwe wykorzystanie takiej bazy z instalacji RMS z dodatkiem SP1 z przywróconą instalacją RMS. Przywrócona instalacja RMS zignoruje dodatkowe pola dodane do bazy danych konfiguracji podczas instalacji RMS z dodatkiem SP1, ponieważ nie będzie ich używać.
