---
TOCTitle: 'Krok 6. Tworzenie grupy komputerów na potrzeby aktualizacji'
Title: 'Krok 6. Tworzenie grupy komputerów na potrzeby aktualizacji'
ms:assetid: 'fe219654-eae8-45ca-a44b-c1e05c3c3e93'
ms:contentKeyID: 18136913
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc708629(v=WS.10)'
---

Krok 6. Tworzenie grupy komputerów na potrzeby aktualizacji
===========================================================

Grupy komputerów są ważnym składnikiem operacji rozmieszczania WSUS (także operacji rozmieszczania podstawowego). Dzięki tym grupom można kierować aktualizacje do określonych komputerów. Istnieją dwie domyślne grupy komputerów: Wszystkie komputery oraz Komputery nieprzypisane. Domyślnie każdy komputer kliencki wstępnie kontaktujący się z serwerem WSUS jest dodawany do obydwu grup.

Można także tworzyć niestandardowe grupy komputerów. Korzyścią wynikającą z utworzenia grup komputerów jest możliwość przetestowania aktualizacji przed ich dalszym rozmieszczeniem. Jeśli testowanie zakończy się pomyślnie, można zastosować aktualizacje względem wszystkich grup komputerów. Można utworzyć dowolną liczbę grup niestandardowych.

**Aby skonfigurować grupy komputerów**
1.  Określ sposób przypisywania komputerów do grup. Dostępne są dwie opcje: kierowanie po stronie serwera oraz kierowanie po stronie klienta. Kierowanie po stronie serwera polega na ręcznym dodawaniu komputerów do grup przy użyciu programu WSUS. Kierowanie po stronie klienta polega na automatycznym dodawaniu klientów przy użyciu zasad grupy lub kluczy rejestru.

2.  Utwórz grupę komputerów w programie WSUS.

3.  Przenieś komputery do grup, korzystając z metody wybranej w kroku 1.

Ta sekcja zawiera informacje na temat ręcznego przenoszenia komputerów do grup na konsoli WSUS (z zastosowaniem opcji kierowania po stronie serwera). W celu przypisania kilku komputerów klienckich do grup można użyć opcji kierowania po stronie klienta, która służy do automatycznego przenoszenia komputerów do grup.

Na podstawie informacji przedstawionych w kroku 6 można skonfigurować grupę testową zawierającą co najmniej jeden komputer.

**Krok 6 obejmuje następujące procedury:**

-   Tworzenie grupy
-   Dodawanie komputera do grupy

**Aby utworzyć grupę**
1.  W konsoli administracyjnej programu WSUS rozwiń węzeł **Komputery** i wybierz pozycję **Wszystkie komputery**.

2.  Kliknij prawym przyciskiem myszy pozycję **Wszystkie komputery** lub przejdź do okienka **Akcje** i kliknij pozycję **Dodaj grupę komputerów**.

3.  Zostanie wyświetlone okno dialogowe **Dodaj grupę komputerów**. Określ nazwę nowej grupy.

Następna procedura służy do przypisywania komputera klienckiego do grupy testowej. Takim komputerem jest dowolny komputer o charakterystyce sprzętowej i programowej odpowiadającej większości komputerów w sieci (nie może to być komputer z przypisaną rolą krytyczną). W ten sposób można sprawdzić, jak zatwierdzone aktualizacje przebiegną w przypadku komputerów porównywalnych z komputerem testowym.

**Aby dodać komputer do grupy**
1.  W konsoli administracyjnej programu WSUS kliknij pozycję **Komputery**.

2.  Kliknij grupę komputerów, do której ma zostać przeniesiony komputer.

3.  Z listy komputerów wybierz komputer do przeniesienia.

4.  Kliknij prawym przyciskiem myszy pozycję **Zmień członkostwo**.

5.  Zostanie wyświetlone okno dialogowe **Ustawianie członkostwa grup komputerów** z listą grup.

6.  Wybierz grupę, do której komputer ma zostać przeniesiony, a następnie kliknij przycisk **OK**.
