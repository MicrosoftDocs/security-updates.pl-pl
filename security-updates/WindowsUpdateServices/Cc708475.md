---
TOCTitle: 'Krok 7. Zatwierdzanie i rozmieszczanie aktualizacji w programie WSUS 3.0'
Title: 'Krok 7. Zatwierdzanie i rozmieszczanie aktualizacji w programie WSUS 3.0'
ms:assetid: '88fac442-a9d3-4e74-92f6-3822b7237af1'
ms:contentKeyID: 18136653
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc708475(v=WS.10)'
---

Krok 7. Zatwierdzanie i rozmieszczanie aktualizacji w programie WSUS 3.0
========================================================================

W tym kroku zatwierdza się aktualizację testowych komputerów klienckich z grupy testowej. Komputery z tej grupy nawiążą połączenie z serwerem WSUS w ciągu następnych 24 godzin. Po tym okresie można korzystać z funkcji raportowania WSUS w celu ustalenia, czy aktualizacje zostały rozmieszczone na komputerach. Jeśli test zakończy się pomyślnie, te same aktualizacje można zatwierdzić dla pozostałych komputerów w organizacji.

**Krok 7 obejmuje następujące procedury**:

-   Zatwierdzanie i rozmieszczanie aktualizacji.
-   Sprawdzanie stanu aktualizacji.

**Aby zatwierdzić i rozmieścić aktualizację**
1.  W konsoli administracyjnej programu WSUS kliknij ikonę **Aktualizacje**. Spowoduje to wyświetlenie podsumowania aktualizacji w widokach domyślnych (**Wszystkie aktualizacje**, **Aktualizacje krytyczne**, **Aktualizacje zabezpieczeń** i **Aktualizacje WSUS**). Użyj widoku **Wszystkie aktualizacje** dla tej procedury.

2.  Z listy aktualizacji wybierz te, które mają zostać zatwierdzone do instalacji. Informacje o wybranej aktualizacji są dostępne w najniższym okienku panelu Aktualizacje. Aby zaznaczyć kilka sąsiadujących ze sobą aktualizacji, podczas ich wybierania naciśnij i przytrzymaj klawisz **SHIFT**. Aby zaznaczyć kilka aktualizacji znajdujących się w różnych miejscach na liście, w czasie ich wybierania naciśnij i przytrzymaj klawisz **CTRL**.

3.  Kliknij prawym przyciskiem myszy odpowiednią pozycję, a następnie kliknij polecenie **Zatwierdź**. Pojawi się okno dialogowe **Zatwierdzanie aktualizacji**.

4.  Wybierz jedną z grup (na przykład **Test**), a następnie kliknij strzałkę z lewej strony. Zostanie wyświetlone menu kontekstowe z następującymi opcjami: **Zatwierdzone do instalacji**, **Zatwierdzone do usunięcia**, **Niezatwierdzone**, **Termin ostateczny**, **Taki sam jak nadrzędny** i **Zastosuj do podrzędnych**. Wybierz opcję **Zatwierdzone do instalacji**, a następnie kliknij przycisk **OK**.

5.  Zostanie wyświetlone nowe okno **Postęp zatwierdzania**, które przedstawia postęp różnych zadań wpływających na zatwierdzanie aktualizacji. Po zakończeniu potwierdzania kliknij przycisk **Zamknij**, aby zamknąć to okno.

> [!note]  
> Z zatwierdzaniem aktualizacji jest skojarzonych wiele opcji, na przykład ustawianie terminów ostatecznych i odinstalowywanie aktualizacji. 

Po 24 godzinach można skorzystać z funkcji raportowania WSUS w celu ustalenia, czy aktualizacje zostały rozmieszczone na komputerach.

**Aby sprawdzić stan aktualizacji**
1.  W konsoli administracyjnej programu WSUS kliknij ikonę **Raporty** w lewym okienku.

2.  Na stronie **Raporty** zostanie wyświetlonych wiele raportów standardowych. Kliknij raport **Podsumowanie stanu aktualizacji**. Zostanie wyświetlone okno **Raport o aktualizacjach**.

3.  Jeśli chcesz filtrować listę aktualizacji, wybierz kryteria filtrowania (na przykład **Uwzględnij aktualizacje w tych klasyfikacjach**), a następnie kliknij przycisk **Uruchom raport** na pasku narzędzi okna.

4.  Zostanie wyświetlone okienko **Raport o aktualizacjach**. Stan poszczególnych aktualizacji możesz sprawdzić, wybierając aktualizację w lewej części okienka. Ostatnia część okienka raportu przedstawia podsumowanie stanu aktualizacji.

5.  Raport można zapisać lub wydrukować, klikając odpowiednią ikonę na pasku narzędzi.

Jeśli aktualizacje zostaną pomyślnie rozmieszczone w grupie testowej, te same aktualizacje można zatwierdzić dla pozostałych komputerów w organizacji.
