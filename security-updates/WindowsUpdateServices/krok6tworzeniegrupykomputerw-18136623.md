---
TOCTitle: 'Krok 6. Tworzenie grupy komputerów'
Title: 'Krok 6. Tworzenie grupy komputerów'
ms:assetid: '6039e5dc-d2ce-4d4b-b737-17ebcadbd4a7'
ms:contentKeyID: 18136623
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720536(v=WS.10)'
---

Krok 6. Tworzenie grupy komputerów
==================================

Grupy komputerów są ważnym składnikiem operacji rozmieszczania WSUS (także operacji rozmieszczania podstawowego). Dzięki tym grupom można kierować aktualizacje do określonych komputerów. Istnieją dwie domyślne grupy komputerów: Wszystkie komputery oraz Komputery nieprzypisane. Domyślnie każdy komputer kliencki wstępnie kontaktujący się z serwerem WSUS jest dodawany do obydwu grup.

Można również tworzyć niestandardowe grupy komputerów. Korzyścią wynikającą z utworzenia grup komputerów jest możliwość przetestowania aktualizacji przed ich dalszym rozmieszczeniem. Jeśli testowanie zakończy się pomyślnie, można zastosować aktualizacje względem wszystkich grup komputerów. Można utworzyć dowolną liczbę grup niestandardowych.

Proces konfigurowania grup komputerów składa się z trzech kroków. Najpierw należy określić sposób przypisywania komputerów do grup. Dostępne są dwie opcje: *kierowanie po stronie serwera* oraz *kierowanie po stronie klienta*. Kierowanie po stronie serwera polega na ręcznym dodawaniu komputerów do grup przy użyciu programu WSUS. Kierowanie po stronie klienta polega na automatycznym dodawaniu klientów przy użyciu zasad grupy lub kluczy rejestru. Następnie tworzy się grupę komputerów w programie WSUS. Na koniec należy przenieść komputery do grup, korzystając z metody wybranej w pierwszym kroku.

Ten dokument zawiera informacje na temat ręcznego przenoszenia komputerów do grup na konsoli WSUS (z zastosowaniem opcji kierowania po stronie serwera). W celu przypisania kilku komputerów klienckich do grup można użyć opcji kierowania po stronie klienta, która służy do automatycznego przenoszenia komputerów do grup.

Na podstawie informacji przedstawionych w kroku 6 można skonfigurować grupę testową zawierającą co najmniej jeden komputer.

W tym kroku zostały opisane następujące procedury:

-   Wybór opcji kierowania po stronie serwera
-   Tworzenie grupy
-   Przenoszenie komputerów do grupy

**Aby określić metodę przypisywania komputerów do grup:**
1.  Na pasku narzędzi konsoli WSUS kliknij ikonę **Opcje**, a następnie kliknij pozycję **Opcje komputerów**.

2.  W polu **Opcje komputerów** kliknij opcję **Użyj zadania Przenoszenie komputerów w programie Windows Server Update Services**.

3.  W obszarze **Zadania** kliknij pozycję **Zapisz ustawienia**, a następnie kliknij przycisk **OK** w wyświetlonym oknie dialogowym potwierdzenia.

**Aby utworzyć grupę:**
1.  Na pasku narzędzi konsoli WSUS kliknij ikonę **Komputery**.

2.  W obszarze **Zadania** kliknij pozycję **Utwórz grupę komputerów**.

3.  W polu **Nazwa grupy** wpisz wartość **Test**, a następnie kliknij przycisk **OK**.

Następna procedura służy do przypisywania komputera klienckiego do przetestowania do grupy testowej. Takim komputerem jest dowolny komputer o charakterystyce sprzętowej i programowej odpowiadającej większości komputerów w sieci (nie może to być komputer z przypisaną rolą krytyczną). W ten sposób można sprawdzić, jak zatwierdzone aktualizacje przebiegną w przypadku komputerów porównywalnych z komputerem testowym.

**Aby ręcznie dodać komputer do grupy testowej:**
1.  Na pasku narzędzi konsoli WSUS kliknij ikonę **Komputery**.

2.  W polu **Grupy** kliknij grupę, do której należy komputer do przeniesienia.

3.  Z listy komputerów wybierz komputer do przeniesienia.

4.  W obszarze **Zadania** kliknij pozycję **Przenieś wybrany komputer**.

5.  Z listy **Grupa komputerów** wybierz grupę, do której komputer ma zostać przeniesiony, a następnie kliknij przycisk **OK**.
