---
TOCTitle: 'Krok 7. Zatwierdzanie i rozmieszczanie aktualizacji'
Title: 'Krok 7. Zatwierdzanie i rozmieszczanie aktualizacji'
ms:assetid: '38db25a9-6702-4e43-b536-764e8814afc6'
ms:contentKeyID: 18136527
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720504(v=WS.10)'
---

Krok 7. Zatwierdzanie i rozmieszczanie aktualizacji
===================================================

W tym kroku zatwierdza się aktualizację testowych komputerów klienckich z grupy testowej. Komputery z tej grupy zostaną zarejestrowane na serwerze WSUS w ciągu następnych 24 godzin. Po tym okresie można korzystać z funkcji raportowania WSUS w celu ustalenia, czy aktualizacje zostały rozmieszczone na komputerach. Jeśli test zakończy się pomyślnie, tę samą aktualizację można zatwierdzić dla pozostałych komputerów w organizacji.

Krok 7 obejmuje następujące procedury:

-   Zatwierdzanie i rozmieszczanie aktualizacji
-   Sprawdzanie raportu Stan aktualizacji

**Aby zatwierdzić i rozmieścić aktualizację:**
1.  Na pasku narzędzi konsoli WSUS kliknij ikonę **Aktualizacje**. Domyślnie na liście aktualizacji są wyświetlane tylko aktualizacje krytyczne oraz aktualizacje zabezpieczeń, których wykrywanie na komputerach klienckich zostało zatwierdzone. Użyj domyślnego filtru dla tej procedury.

2.  Z listy aktualizacji wybierz te, które mają zostać zatwierdzone do instalacji. Informacje o wybranej aktualizacji są dostępne na karcie **Szczegóły**. Aby zaznaczyć kilka sąsiadujących ze sobą aktualizacji, podczas ich wybierania naciśnij i przytrzymaj klawisz SHIFT. Aby zaznaczyć kilka aktualizacji znajdujących się w różnych miejscach na liście, podczas ich wybierania naciśnij i przytrzymaj klawisz CTRL.

3.  W polu **Zadania aktualizacji** kliknij polecenie **Zmień zatwierdzenie**. Pojawi się okno dialogowe **Zatwierdzanie aktualizacji**.

4.  Na liście **Grupuj ustawienia zatwierdzeń dla wybranych aktualizacji** kliknij polecenie **Zainstaluj** (na liście w kolumnie **Zatwierdzenie** dla grupy testowej), a następnie kliknij przycisk **OK**.

| ![](images/Cc720504.note(WS.10).gif)Uwaga                                                                                                                                                                                                                |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Z zatwierdzaniem aktualizacji skojarzono wiele opcji, na przykład ustawianie terminów ostatecznych i odinstalowywanie aktualizacji. Zostały one omówione w oficjalnym dokumencie „Microsoft Windows Server Update Services Operations Guide” (dokument dostępny w języku angielskim). |

Po 24 godzinach można skorzystać z funkcji raportowania WSUS w celu ustalenia, czy aktualizacje zostały rozmieszczone na komputerach.

**Aby sprawdzić raport Stan aktualizacji:**
1.  Na pasku narzędzi konsoli WSUS kliknij ikonę **Raporty**.

2.  Na stronie **Raporty** kliknij pozycję **Stan aktualizacji**.

3.  Jeśli chcesz filtrować listę aktualizacji, w polu **Widok** wybierz kryteria do zastosowania, a następnie kliknij przycisk **Zastosuj**.

4.  Jeśli chcesz wyświetlić stan aktualizacji według grupy komputerów, a następnie według komputera, odpowiednio rozwiń widok aktualizacji.

5.  Jeśli chcesz wydrukować raport Stan aktualizacji, w polu **Zadania** kliknij polecenie **Drukuj raport**.

Jeśli aktualizacje zostaną pomyślnie rozmieszczone w grupie testowej, te same aktualizacje można zatwierdzić dla pozostałych komputerów w organizacji.
