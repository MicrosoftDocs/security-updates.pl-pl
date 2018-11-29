---
TOCTitle: 'Krok 7. Zatwierdzanie i wdrażanie aktualizacji programu WSUS'
Title: 'Krok 7. Zatwierdzanie i wdrażanie aktualizacji programu WSUS'
ms:assetid: 'c4e58e17-d5e3-4194-8f26-b459e0c03b86'
ms:contentKeyID: 21798669
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Dd939909(v=WS.10)'
---

Krok 7. Zatwierdzanie i wdrażanie aktualizacji programu WSUS
============================================================

W tym kroku zostanie zatwierdzona aktualizacja dla wszystkich komputerów w grupie testowej programu Windows Server Update Services 3.0 z dodatkiem Service Pack 2 (WSUS 3.0 z dodatkiem SP2). Komputery z tej grupy automatycznie skontaktują się z serwerem WSUS w ciągu następnych 24 godzin w celu pobrania tej aktualizacji. Można skorzystać z funkcji raportowania programu WSUS, aby ustalić, czy te aktualizacje zostały wdrożone na komputerach testowych. Jeśli testy zostaną zakończone pomyślnie, będzie można zatwierdzić aktualizacje dla odpowiednich grup komputerów w organizacji.

Procedury kroku 7
-----------------

-   Zatwierdzanie i rozmieszczanie aktualizacji.
-   Sprawdzanie stanu aktualizacji

**Aby zatwierdzić i rozmieścić aktualizację**
1.  W konsoli administracyjnej programu WSUS kliknij pozycję **Aktualizacje**. Zostanie wyświetlone podsumowanie stanu aktualizacji w obszarach **Wszystkie aktualizacje**, **Aktualizacje krytyczne**, **Aktualizacje zabezpieczeń** i **Aktualizacje WSUS**.

2.  W sekcji **Wszystkie aktualizacje** kliknij pozycję **Aktualizacje wymagane przez komputery**.

3.  Na liście aktualizacji zaznacz aktualizacje, które mają zostać zatwierdzone do instalacji w grupie komputerów testowych. Informacje o wybranej aktualizacji są dostępne w dolnym okienku panelu Aktualizacje. Aby zaznaczyć wiele sąsiadujących aktualizacji, podczas klikania aktualizacji przytrzymaj naciśnięty klawisz **SHIFT**. Aby zaznaczyć wiele aktualizacji znajdujących się w różnych miejscach na liście, podczas klikania aktualizacji przytrzymaj naciśnięty klawisz **CTRL**.

4.  Kliknij prawym przyciskiem myszy odpowiednią pozycję, a następnie kliknij polecenie **Zatwierdź**.

5.  W oknie dialogowym **Zatwierdzanie aktualizacji** wybierz grupę testową, a następnie kliknij strzałkę w dół.

6.  Wybierz opcję **Zatwierdzone do instalacji**, a następnie kliknij przycisk **OK**.

7.  Zostanie wyświetlone okno Postęp zatwierdzania, w którym będzie wyświetlany postęp zadań związanych z zatwierdzaniem aktualizacji. Po ukończeniu zatwierdzania kliknij przycisk **Zamknij**.

Po upływie 24 godzin można skorzystać z funkcji raportowania programu WSUS, aby ustalić, czy aktualizacje zostały wdrożone na komputerach testowych.

**Aby sprawdzić stan aktualizacji**
1.  W okienku nawigacji konsoli administracyjnej programu WSUS kliknij pozycję **Raporty**.

2.  Na stronie **Raporty** kliknij raport **Podsumowanie stanu aktualizacji**. Zostanie wyświetlone okno **Raport o aktualizacjach**.

3.  Aby przefiltrować listę aktualizacji, wybierz kryteria filtrowania (na przykład **Uwzględnij aktualizacje w tych klasyfikacjach**), a następnie kliknij przycisk **Uruchom raport** na pasku narzędzi okna.

4.  Zostanie wyświetlone okienko **Raport o aktualizacjach**. Stan poszczególnych aktualizacji możesz sprawdzić, wybierając aktualizację w lewej części okienka. Ostatnia część okienka raportu przedstawia podsumowanie stanu aktualizacji.

5.  Ten raport można zapisać lub wydrukować, klikając odpowiednią ikonę na pasku narzędzi.

6.  Po przetestowaniu aktualizacji można je zatwierdzić do instalacji w odpowiednich grupach komputerów w organizacji.

Materiały dodatkowe
-------------------

[Program Windows Server Update Services 3.0 z dodatkiem SP2 — przewodnik krok po kroku](https://technet.microsoft.com/4b504edc-93b3-45b0-a7e8-d0107f1a4442)

Aby uzyskać więcej informacji o korzystaniu z programu WSUS 3.0 z dodatkiem SP2, zobacz:

Przewodnik dotyczący wdrażania programu WSUS: [http://go.microsoft.com/fwlink/?LinkId=139832](http://go.microsoft.com/fwlink/?linkid=139832) (strona może zostać wyświetlona w języku angielskim).

Przewodnik obsługi programu WSUS: [http://go.microsoft.com/fwlink/?LinkId=139838](http://go.microsoft.com/fwlink/?linkid=139838) (strona może zostać wyświetlona w języku angielskim).
