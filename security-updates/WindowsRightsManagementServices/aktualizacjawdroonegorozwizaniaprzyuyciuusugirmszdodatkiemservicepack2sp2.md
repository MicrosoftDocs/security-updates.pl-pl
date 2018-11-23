---
TOCTitle: 'Aktualizacja wdrożonego rozwiązania przy użyciu usługi RMS z dodatkiem Service Pack 2 (SP2)'
Title: 'Aktualizacja wdrożonego rozwiązania przy użyciu usługi RMS z dodatkiem Service Pack 2 (SP2)'
ms:assetid: '27ee06a1-f467-4a6c-b662-45ddb5f8c13e'
ms:contentKeyID: 18123203
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720225(v=WS.10)'
---

Aktualizacja wdrożonego rozwiązania przy użyciu usługi RMS z dodatkiem Service Pack 2 (SP2)
===========================================================================================

Poniższa sekcja zawiera informacje pomocne w instalacji usługi Microsoft® Windows® Rights Management Services (RMS) z dodatkiem Service Pack 2 (SP2) w organizacji, w której wdrożono już usługi RMS. Konieczność aktualizacji RMS do wersji z dodatkiem SP2 dotyczy tylko organizacji, w których wdrożono już usługi RMS. Organizacje, w których usługi RMS wdrażane są po raz pierwszy, mogą zainstalować usługi RMS z dodatkiem SP2, postępując zgodnie ze wskazówkami zawartymi w artykułach Planowanie rozmieszczenia programu RMS ([http://go.microsoft.com/fwlink/?LinkId=74999](http://go.microsoft.com/fwlink/?linkid=74999)) i Rozmieszczanie systemu RMS ([http://go.microsoft.com/fwlink/?LinkID=75000](http://go.microsoft.com/fwlink/?linkid=75000)) należących do niniejszego zestawu dokumentacji.

Instalacja usług RMS z dodatkiem SP2 nie wymaga usuwania istniejącej instalacji RMS z dodatkiem SP1. Instalator usług RMS z dodatkiem SP2 wykrywa instalację usług RMS z dodatkiem SP1 i w miarę potrzeb dodaje odpowiednie funkcje i ustawienia.

> [!note]  
> Nie jest obsługiwana ścieżka uaktualnienia od serwera RMS bez dodatku Service Pack do wersji RMS z dodatkiem SP2. Użytkownicy korzystający z serwera RMS bez dodatku Service Pack muszą uaktualnić zainstalowane oprogramowanie do wersji RMS z dodatkiem SP1, a dopiero następnie do wersji z dodatkiem SP2. W przypadku klientów RMS uaktualnienie możliwe jest od dowolnej starszej wersji. 

**W tym temacie**

-   [Przygotowanie do aktualizacji do wersji RMS z dodatkiem SP2](#bkmk_preparingforsp2update)
-   [Przeprowadzenie aktualizacji do wersji RMS z dodatkiem SP2](#bkmk_performingsp2update)
-   [Aktualizacja klastrów](#bkmk_updateclusters)
-   [Aktualizacja klientów RMS](#bkmk_updateclients)
-   [Współdziałanie z RMS w wersji 1.0](#bkmk_interop)
-   [Usuwanie usług RMS z dodatkiem SP2](#bkmk_removingrms)

<span id="bkmk_PreparingForSP2Update"></span>
Przygotowanie do aktualizacji do wersji RMS z dodatkiem SP2
-----------------------------------------------------------

Aktualizacja RMS do wersji z dodatkiem SP2 została przygotowana w sposób umożliwiający uniknięcie przerywania działania usług RMS. Przed uaktualnianiem klastra RMS zaleca się jednak wykonanie następujących czynności:

-   Utwórz kopię zapasową bazy danych konfiguracji i klucza prywatnego RMS. Więcej informacji można znaleźć w artykule poświęconym kopiom zapasowym systemu dla usług RMS ([http://go.microsoft.com/fwlink/?LinkId=75001](http://go.microsoft.com/fwlink/?linkid=75001)) należącym do niniejszego zestawu dokumentacji..
-   Użytkownicy korzystający z programowego klucza prywatnego powinni upewnić się, że posiadają hasło klucza prywatnego RMS.
-   Wykonaj kopię zapasową bazy danych rejestrowania, aby zachować zarejestrowane wcześniej statystyki.
-   Upewnij się, że zostały zainstalowane najnowsze aktualizacje krytyczne oraz aktualizacje zabezpieczeń dla systemu operacyjnego klientów i serwerów. Aby sprawdzić, czy zostały zainstalowane wszystkie aktualizacje krytyczne oraz aktualizacje zabezpieczeń, kliknij przycisk **Start**, kliknij **Windows Update**, a następnie wykonaj instrukcje wyświetlane na ekranie.

<span id="bkmk_PerformingSP2Update"></span>
Przeprowadzenie aktualizacji do wersji RMS z dodatkiem SP2
----------------------------------------------------------

Gdy kreator instalacji usług Windows Rights Management Services z dodatkiem Service Pack 2 wykryje zainstalowane usługi RMS, sprawdza bieżącą instalację RMS z dodatkiem SP1 i dodaje tylko nowe pliki lub zastępuje istniejące, jeśli wymaga tego wersja RMS z dodatkiem SP2. Jeśli na komputerach działają już usługi RMS, po instalacji usług RMS z dodatkiem SP2 nie ma potrzeby ponownego zastrzegania oprogramowania ani przeprowadzania dodatkowych prac konfiguracyjnych, aby ich działanie było kontynuowane.

<span id="bkmk_UpdateClusters"></span>
Aktualizacja klastrów
---------------------

Jeśli usługi RMS zostały zainstalowane w konfiguracji klastra, należy tak planować aktualizację klastrów, aby zmniejszyć do minimum jej wpływ na instalację. Określając najlepszy sposób wdrożenia w organizacji usług RMS z dodatkiem SP2, należy wziąć pod uwagę następujące zalecenia:

-   Zaleca się instalowanie usług RMS z dodatkiem SP2 na jednej części klastra naraz, co pozwala zwiększyć przewidywalność procesu uaktualniania klastra i zmniejszyć prawdopodobieństwo, że pociągnie on za sobą pogorszenie jakości świadczenia tych usług.
-   W przypadku wielu klastrów RMS należy najpierw uaktualniać klastry głównej certyfikacji, a następnie zarejestrowane podrzędnie klastry licencjonowania.
-   Użytkownicy korzystający z przechodzenia grup między lasami mogą niezależnie uaktualniać klastry w lasach, nie wpływając na zdolność serwerów RMS do rozwinięcia przynależności do grupy między lasami.
-   Usługi RMS z dodatkiem SP2, RMS z dodatkiem SP1 i serwer RMS w wersji 1.0 mogą współistnieć i współpracować tylko wtedy, gdy znajdują się w różnych lasach usługi Active Directory. Nie zaleca się posiadania różnych wersji serwera RMS w tym samym klastrze.
-   Pakiet instalacyjny usług RMS z dodatkiem SP2 może także posłużyć do zainstalowania na serwerze nowego rozmieszczenia usług RMS z dodatkiem SP2. Usługi RMS z dodatkiem SP1 nie muszą być zainstalowane.

<span id="bkmk_UpdateClients"></span>
Aktualizacja klientów RMS
-------------------------

W witrynach Windows Update i Microsoft Download Center dostępny jest nowy klient usług RMS z dodatkiem SP2. Pakiet instalacyjny klienta usług RMS z dodatkiem SP2 może także posłużyć do zainstalowania na komputerze nowej wersji usług RMS z dodatkiem SP2. Klient RMS w wersji 1.0 nie musi być zainstalowany. Klient RMS z dodatkiem SP2 wyposażony został w funkcję zgodności wstecznej, dzięki której możliwe jest wykorzystanie go z aplikacjami obsługującymi RMS, które wymagają usług w wersji 1.0.

Aby uzyskać więcej informacji na temat instalowania i aktualizacji klienta RMS, zobacz artykuł Dystrybucja klienta programu RMS ([http://go.microsoft.com/fwlink/?LinkId=75070](http://go.microsoft.com/fwlink/?linkid=75070)).

<span id="bkmk_InterOp"></span>
Współdziałanie z RMS w wersji 1.0
---------------------------------

Usługi RMS z dodatkiem SP2 oferują liczne udoskonalenia i rozszerzenia funkcjonalności, dlatego należy zainstalować je podczas kolejnego cyklu uaktualniania. Pomimo pełnej współpracy serwerów i klientów RMS z oprogramowaniem RMS z dodatkiem SP2 z serwerami i klientami RMS, na których nie zainstalowano tego oprogramowania, należy zdawać sobie sprawę z następujących różnic w ich działaniu w środowisku mieszanym:

-   Tylko serwery z oprogramowaniem RMS z dodatkiem SP1 lub nowszym oferują możliwość rejestrowania w trybie offline.
-   Tylko klienci z oprogramowaniem RMS z dodatkiem SP1 lub nowszym oferują funkcję automatycznej aktywacji.
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
<th style="border:1px solid black;" >Funkcje obsługiwane przy klientach w wersji 1</th>
<th style="border:1px solid black;" >Funkcje obsługiwane przy klientach z dodatkiem SP2</th>
<th style="border:1px solid black;" >Funkcje obsługiwane w środowiskach z różnymi klientami</th>
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
Klienci z oprogramowaniem w wersji z dodatkiem SP2 mają funkcję automatycznej aktywacji.
W przypadku wersji 1 aktywacja klienta musi przebiegać za pośrednictwem Internetu.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">SP2</td>
<td style="border:1px solid black;">Wszystkie starsze funkcje.
Rejestrowanie serwera offline.
Brak klientów z funkcją automatycznej aktywacji.</td>
<td style="border:1px solid black;">Wszystkie funkcje SP1.
Rejestrowanie serwera offline.
Klienci z funkcją automatycznej aktywacji.
Skrytka serwera.
Obsługa programu Microsoft SQL Server™ 2005 nie wymaga żadnych przygotowań.</td>
<td style="border:1px solid black;">Wszystkie starsze funkcje i funkcje wersji z dodatkiem SP2.
Rejestrowanie serwera offline.
Klienci z oprogramowaniem w wersji z dodatkiem SP2 mają funkcję automatycznej aktywacji.
W przypadku wersji 1 aktywacja klienta musi przebiegać za pośrednictwem Internetu.</td>
</tr>
</tbody>
</table>
 

<span id="bkmk_RemovingRMS"></span>
Usuwanie usług RMS z dodatkiem SP2
----------------------------------

Aby po instalacji usług RMS z dodatkiem SP2 przywrócić poprzednią konfigurację serwera RMS, można usunąć usługi RMS z dodatkiem SP2 przy użyciu apletu **Dodaj lub usuń programy** w **Panelu sterowania**.
