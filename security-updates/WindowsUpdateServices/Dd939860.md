---
TOCTitle: 'Krok 6. Konfigurowanie grup komputerów'
Title: 'Krok 6. Konfigurowanie grup komputerów'
ms:assetid: '70518732-2179-4e41-9609-7f9999867f41'
ms:contentKeyID: 21798604
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Dd939860(v=WS.10)'
---

Krok 6. Konfigurowanie grup komputerów
======================================

Grupy komputerów są istotnym elementem wdrożeń programu Windows Server Update Services 3.0 z dodatkiem Service Pack 2 (WSUS 3.0 z dodatkiem SP2). Grupy komputerów umożliwiają testowanie aktualizacji i kierowanie ich do określonych komputerów. Istnieją dwie domyślne grupy komputerów: Wszystkie komputery oraz Komputery nieprzypisane. Domyślnie każdy komputer kliencki kontaktujący się wstępnie z serwerem WSUS jest dodawany do obu grup.

Można utworzyć dowolną liczbę grup komputerów potrzebnych do zarządzania aktualizacjami w organizacji. Najlepszym rozwiązaniem jest utworzenie co najmniej jednej grupy komputerów umożliwiającej testowanie aktualizacji przed wdrożeniem ich na komputerach w organizacji.

Procedury kroku 6
-----------------

1.  Tworzenie testowej grupy komputerów
2.  Przenoszenie co najmniej jednego komputera do grupy testowej

**Aby utworzyć grupę testową**
1.  W konsoli administracyjnej programu WSUS rozwiń węzeł **Komputery** i wybierz pozycję **Wszystkie komputery**.

2.  Kliknij prawym przyciskiem myszy pozycję **Wszystkie komputery**, a następnie kliknij polecenie **Dodaj grupę komputerów**.

3.  W oknie dialogowym **Dodawanie grupy komputerów** w polu **Nazwa** wpisz nazwę nowej grupy testowej, a następnie kliknij przycisk **Dodaj**.

Następna procedura służy do przypisania komputera klienckiego do grupy testowej. Komputer testowy to dowolny komputer o charakterystyce sprzętowej i programowej odpowiadającej większości komputerów klienckich w sieci, lecz nie może to być komputer o istotnym znaczeniu. Jeśli testy zostaną zakończone pomyślnie, będzie można zatwierdzić aktualizacje na potrzeby komputerów w wybranej grupie.

**Aby przypisać komputer do grupy testowej**
1.  W konsoli administracyjnej programu WSUS kliknij pozycję **Komputery**.

2.  Kliknij nazwę grupy komputera, który chcesz przypisać do grupy testowej.

3.  Na liście komputerów zaznacz komputery, które chcesz przypisać do grupy testowej.

4.  Kliknij prawym przyciskiem myszy pozycję **Zmień członkostwo**.

5.  W oknie dialogowym **Ustawianie członkostwa grup komputerów** wybierz utworzoną wcześniej grupę testową, a następnie kliknij przycisk **OK**.

Powtórz dwie powyższe procedury, czyli utwórz grupę i przypisz do niej komputery, aby utworzyć tyle dodatkowych grup komputerów, ile jest potrzebnych do zarządzania aktualizacjami w lokacji.

Następny krok
-------------

[Krok 7. Zatwierdzanie i wdrażanie aktualizacji programu WSUS](https://technet.microsoft.com/c4e58e17-d5e3-4194-8f26-b459e0c03b86)

Materiały dodatkowe
-------------------

[Program Windows Server Update Services 3.0 z dodatkiem SP2 — przewodnik krok po kroku](https://technet.microsoft.com/4b504edc-93b3-45b0-a7e8-d0107f1a4442)
