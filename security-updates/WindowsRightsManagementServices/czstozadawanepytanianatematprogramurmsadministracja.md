---
TOCTitle: 'Często zadawane pytania na temat programu RMS: Administracja'
Title: 'Często zadawane pytania na temat programu RMS: Administracja'
ms:assetid: '43f77336-5e62-4405-9efb-55417a402d62'
ms:contentKeyID: 18123254
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747547(v=WS.10)'
---

Często zadawane pytania na temat programu RMS: Administracja
============================================================

Pytania dotyczące administrowania programem RMS
-----------------------------------------------

-   [Jaka jest najlepsza metoda odwoływania uprawnień do dokumentów użytkownikowi, który odchodzi z organizacji?](#bkmk_1)
-   [Czy certyfikat licencji XrML, przekazywany organizacji ufającej przy ustanawianiu zaufania między dwiema organizacjami pod względem wymiany zawartości RMS, wymaga jakichś specjalnych zabiegów?](#bkmk_2)
-   [Jak program RMS obsługuje ruchome profile użytkowników?](#bkmk_3)
-   [W jakich sytuacjach może być potrzebne likwidowanie programu RMS w organizacji?](#bkmk_4)
-   [Jak ogólnie wygląda proces likwidowania?](#bkmk_5)
-   [Czy można w taki sposób zlikwidować serwer RMS, aby tylko niektórzy użytkownicy mogli odzyskiwać dokumenty?](#bkmk_6)
-   [Co oznacza komunikat Serwer nie może uzyskać dostępu do katalogu aplikacji?](#bkmk_7)
-   [Czy można używać śledzenia w przypadku serwera RMS?](#bkmk_8)
-   [Co to jest odchylenie zegara i jak sobie z nim poradzić?](#bkmk_9)

<span id="BKMK_1"></span>
#### Jaka jest najlepsza metoda odwoływania uprawnień do dokumentów użytkownikowi, który odchodzi z organizacji?

Najlepiej licencjonować dokumenty dla grup użytkowników zdefiniowanych w katalogu Active Directory, a nie dla indywidualnych kont użytkowników. Taka praktyka jest zalecana, ponieważ, gdy użytkownik odchodzi z organizacji, można go usunąć z grupy Active Directory, a użytkownik tym samym straci dostęp do dokumentów przeznaczonych dla tej grupy. Użytkownik taki może jednak w dalszym ciągu odczytywać dokumenty opatrzone aktualnymi licencjami użytkowania, chyba że uprawnienia dla dokumentów skonfigurowano w taki sposób, aby użytkownik musiał uzyskać licencję użytkowania przy każdym otwarciu dokumentu. Jeśli takie uprawnienie nie zostało zdefiniowane, jedynym sposobem na to, by uniemożliwić użytkownikowi otwieranie dokumentów mających aktualne licencje użytkowania jest wykasowanie zawartości magazynu licencji na komputerze użytkownika.

<span id="BKMK_2"></span>
#### Czy certyfikat licencji XrML, przekazywany organizacji ufającej przy ustanawianiu zaufania między dwiema organizacjami pod względem wymiany zawartości RMS, wymaga jakichś specjalnych zabiegów?

Definiowanie zaufanej domeny użytkownika lub zaufanej domeny publikowania oznacza, że organizacja partnerska zostaje zaufanym użytkownikiem systemu zarządzania prawami danej organizacji. Wiąże się to z założeniem, że obdarzona zaufaniem organizacja nie ujawni danych partnera. Zgodnie z zalecaną praktyką, organizacja partnerska powinna przysłać swój certyfikat licencjodawcy serwera RMS uwierzytelnionym kanałem, takim jak wiadomość e-mail S/MIME, aby do minimum ograniczyć ryzyko zmodyfikowania certyfikatu przed jego importem na serwer RMS.

<span id="BKMK_3"></span>
#### Jak program RMS obsługuje ruchome profile użytkowników?

Certyfikaty kont praw służące do identyfikowania użytkowników są związane z komputerem. W przypadku profili ruchomych pierwsze użycie programu RMS na danym komputerze spowoduje utworzenie nowego certyfikatu konta praw dla użytkownika na tym komputerze.

<span id="BKMK_4"></span>
#### W jakich sytuacjach może być potrzebne likwidowanie programu RMS w organizacji?

Likwidowanie programu RMS powoduje usunięcie serwera RMS z infrastruktury i daje użytkownikom możliwość zapisywania zawartości chronionej prawami dostępu bez ochrony. Na taki krok organizacja może się zdecydować z trzech powodów:

-   Uproszczenie architektury, na przykład konsolidowanie serwerów w klaster.
-   Przekształcanie środowiska pilotażowego do środowiska produkcyjnego.
-   Łączenie serwerów RMS, na przykład po fuzji przedsiębiorstw.

<span id="BKMK_5"></span>
#### Jak ogólnie wygląda proces likwidowania?

Proces likwidowania rozpoczyna się w klastrze głównym RMS przez uruchomienie usługi likwidowania. Gdy usługa likwidowania jest włączona, wszystkie inne usługi (na przykład licencjonowanie i certyfikowanie) zostają wyłączone. W następnym kroku aplikacja obsługująca technologię RMS musi być kierowana do usługi likwidowania przy każdym wywołaniu funkcji RMS. Przykładem aplikacji obsługujących technologię RMS jest pakiet Microsoft Office 2003. W pakiecie Office 2003 klient RMS jest kierowany do usług RMS za pośrednictwem kluczy rejestru. Jeden z kluczy rejestru identyfikuje usługę likwidowania. Po skonfigurowaniu tego klucza tak, aby kierował klientów do usługi likwidowania, klaster RMS będzie udzielał licencji użytkowania przyznających użytkownikowi pełne prawa (odczyt, zapis, kopiowanie, drukowanie, edycja itp.) względem zawartości bez względu na to, czy użytkownik dysponował pierwotnie tymi uprawnieniami. Użytkownikom należy wówczas polecić usunięcie wszelkich ustawień ochrony praw z dokumentów, które mają zostać zachowane po całkowitej likwidacji klastra RMS. Następnie można całkowicie wyłączyć klaster RMS z użytku.

Zaleca się wykonanie kopii zapasowej bazy danych konfiguracji klastra RMS na wypadek, gdyby po wycofaniu klastra z użytku zaistniała konieczność odzyskania jakiegoś dokumentu chronionego prawami dostępu. Po usunięciu serwera tylko autor dokumentu będzie mógł otworzyć dokument bez klucza prywatnego klastra głównego RMS.

<span id="BKMK_6"></span>
#### Czy można w taki sposób zlikwidować serwer RMS, aby tylko niektórzy użytkownicy mogli odzyskiwać dokumenty?

Zastosowanie listy kontroli dostępu do usługi likwidowania (decommission.asmx) pozwala kontrolować dostęp do usługi likwidowania tak, aby tylko wybrani użytkownicy mogli uzyskiwać klucze deszyfrujące dla zawartości chronionej prawami dostępu.

<span id="BKMK_7"></span>
#### Co oznacza komunikat Serwer nie może uzyskać dostępu do katalogu aplikacji?

Ten komunikat jest czasem wyświetlany przy pierwszej próbie otwarcia administracyjnej witryny sieci Web programu RMS bezpośrednio po jego instalacji. Wyświetlenie tego błędu oznacza, że konfigurowanie i administrowanie programem RMS nie będzie możliwe.

Błąd ten występuje najczęściej, gdy Internetowe usługi informacyjne działają w trybie izolacji IIS 5.0. Następująca procedura pozwala wyłączyć to ustawienie na serwerze i ponownie uruchomić serwer IIS w celu wyeliminowania tego problemu.

**Aby wyłączyć tryb izolacji IIS 5.0**
1.  Zaloguj się na serwer RMS jako członek lokalnej grupy Administratorzy .

2.  Kliknij przycisk **Start**, wskaż polecenie **Narzędzia administracyjne**, a następnie kliknij polecenie **Menedżer internetowych usług informacyjnych (IIS)**.

3.  W **Menedżerze usług IIS** rozwiń węzeł komputera lokalnego, kliknij prawym przyciskiem myszy folder **Witryny sieci Web**, a następnie kliknij polecenie **Właściwości**.

4.  Kliknij kartę **Usługa**, wyczyść pole wyboru **Uruchom usługę WWW w trybie izolacji z programem IIS 5.0**, a następnie kliknij przycisk **OK**.

5.  Uwzględnienie tej zmiany wymaga ponownego uruchomienia usługi IIS. Gdy pojawi się pytanie o ponowne uruchomienie usługi IIS, kliknij przycisk **Tak**.

<span id="BKMK_8"></span>
#### Czy można używać śledzenia w przypadku serwera RMS?

Ponieważ program Usługi zarządzania prawami dostępu powstał przy użyciu platformy Microsoft® .NET Framework, można wykorzystać funkcję śledzenia do obserwacji zdarzeń systemowych i rozwiązywania problemów.

Śledzenie można uruchomić po zmodyfikowaniu pliku Web.config lub Machine.config. Po uruchomieniu śledzenia w pliku Machine.config śledzenie jest uruchamiane dla każdego składnika programowego na komputerze, podczas gdy po włączeniu śledzenia w pliku Web.config obejmuje ono wyłącznie zdarzenia dotyczące usług sieci Web.

**Aby włączyć śledzenie**
1.  Otwórz plik Machine.config lub Web.config, a następnie dodaj poniższe wiersze w sekcji &lt;system.diagnostics&gt; tego pliku:
	
	```
	<system.diagnostics>
	<switches>
	<add name="Microsoft Windows Rights Management Services-Global" value="4" />
	<add name="Microsoft Windows Rights Management Services-TimeStamps" value="1" /> 
	<add name="Microsoft Windows Rights Management Services-Indents" value="0" /> 
	</switches>
	<trace autoflush="false" indentsize="4"/>
	</system.diagnostics>
    ```

2.  Uruchom ponownie usługi IIS, wykonując polecenie IISRESET w wierszu polecenia.

3.  Po zebraniu potrzebnych danych usuń z pliku .config wiersze, które dodano w kroku 1.

4.  Uruchom ponownie usługi IIS, wykonując polecenie IISRESET w wierszu polecenia.

> [!Important]  
> W przypadku korzystania ze śledzenia na serwerze programu RMS mogą wystąpić problemy z wydajnością, takie jak dłuższe oczekiwanie na uzyskanie licencji lub na wystawienie certyfikatu konta praw. Śledzenia należy używać tylko w szczególnych przypadkach do diagnozowania i rozwiązywania istniejących problemów. 

<span id="BKMK_9"></span>
#### Co to jest odchylenie zegara i jak sobie z nim poradzić?

Odchylenie zegara występuje wtedy, gdy czas na zegarze jednego komputera jest różny od czasu na zegarze innego komputera. Taka sytuacja zdarza się dosyć często, tak jak często zegarki różnych osób w tym samym pokoju wskazują nieco inną godzinę. Odchylenie zegara może powodować problemy, gdy określono czas ważności w licencji.

Czas ważności licencji jest ustawiany zgodnie z zegarem użytkownika publikującego zawartość. Odchylenie zegara od tych czasów może powodować problemy w dwóch miejscach cyklu publikowania i korzystania z zawartości:

-   Gdy aplikacja próbuje uzyskać licencję użytkowania, korzystając z licencji publikacji, której okres ważności już dobiegł końca albo jeszcze się nie rozpoczął według zegara serwera programu RMS. W takim przypadku żądanie nie powiedzie się. Taka sytuacja może dotyczyć użytkownika końcowego żądającego licencji użytkowania lub aplikacji, która próbuje uzyskać wstępną licencję dokumentu (uzyskać licencję użytkowania w imieniu użytkownika).
-   Jeśli czas ważności licencji wygasł (lub się jeszcze nie zaczął), próba użycia licencji nie powiedzie się. W innym przypadku tylko prawa, które wygasły (lub jeszcze nie są ważne) nie będą dostępne.

Na przykład, jeśli zegar komputera publikującego spóźnia się o 15 minut w stosunku do zegara na komputerze korzystającym z zawartości, a licencja publikacji zawiera ograniczenie czasu ważności do 15 minut, użytkownik uzyskałby z serwera licencję nieważną, ponieważ już w momencie jej wydania prawa do wyświetlania zawartości nadawane przez licencję użytkowania byłyby przedawnione.

Nie ma doskonałego rozwiązania problemów związanych z odchyleniem zegara. Dobrym rozwiązaniem jest ustawienie początku czasu ważności prawa na godzinę wcześniejszą niż aktualna godzina dla użytkowników z zegarami wskazującymi wcześniejszą godzinę, i w miarę możliwości wydłużenie czasu ważności licencji dla użytkowników z zegarami wskazującymi późniejszą godzinę. O problemie odchylenia zegara należy pamiętać zwłaszcza w przypadku licencji o bardzo krótkich okresach ważności.
