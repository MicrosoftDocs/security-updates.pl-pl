---
TOCTitle: 'Krok 4. Konfigurowanie aktualizacji i synchronizacji'
Title: 'Krok 4. Konfigurowanie aktualizacji i synchronizacji'
ms:assetid: 'deeaa7e1-9b50-45cb-9537-d75f70de3405'
ms:contentKeyID: 21798698
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Dd939924(v=WS.10)'
---

Krok 4. Konfigurowanie aktualizacji i synchronizacji
====================================================

W tej sekcji opisano sposób konfigurowania zestawu aktualizacji do pobrania za pomocą programu Windows Server Update Services 3.0 z dodatkiem Service Pack 2 (WSUS 3.0 z dodatkiem SP2).

Procedury kroku 4
-----------------

Poniższe procedury można wykonać, używając Kreatora konfiguracji programu WSUS lub konsoli administracyjnej programu WSUS.

1.  Zapisywanie i pobieranie informacji o serwerze nadrzędnym i serwerze proxy.
2.  Wybieranie języka aktualizacji.
3.  Wybieranie produktów, dla których mają być pobierane aktualizacje.
4.  Wybieranie klasyfikacji aktualizacji.
5.  Określanie harmonogramu synchronizacji dla tego serwera.

Po skonfigurowaniu połączenia sieciowego można pobierać aktualizacje, przeprowadzając synchronizację z serwerem WSUS. Synchronizacja rozpoczyna się po nawiązaniu przez serwer WSUS połączenia z witryną Microsoft Update. Po nawiązaniu kontaktu program WSUS określa, czy od czasu ostatniej synchronizacji zostały udostępnione nowe aktualizacje. Podczas pierwszej synchronizacji serwera WSUS wszystkie aktualizacje są dostępne i gotowe do zatwierdzenia do instalacji. Synchronizacja wstępna może potrwać długo.

W tej sekcji przedstawiono procedury synchronizowania przy użyciu ustawień domyślnych. Program WSUS 3.0 z dodatkiem SP2 udostępnia też opcje do minimalizowania użycia przepustowości w trakcie synchronizowania.

Korzystanie z Kreatora konfiguracji programu Windows Server Update Services
---------------------------------------------------------------------------

W ramach procedur kroku 3 ukończono konfigurację serwera nadrzędnego i serwera proxy. Następny zestaw procedur zaczyna się na stronie **Połącz z serwerem nadrzędnym** kreatora konfiguracji.

**Aby zapisać i pobrać informacje o serwerze nadrzędnym i serwerze proxy**
1.  Na stronie Połącz z serwerem nadrzędnym kreatora konfiguracji kliknij przycisk **Rozpocznij połączenie**. Spowoduje to zapisanie i przekazanie ustawień oraz zebranie informacji o dostępnych aktualizacjach.

2.  Po nawiązaniu połączenia będzie dostępny przycisk **Zatrzymaj połączenie**. W przypadku problemów z połączeniem kliknij przycisk **Zatrzymaj połączenie**, rozwiąż problemy i nawiąż ponownie połączenie.

3.  Po pomyślnym zakończeniu pobierania kliknij przycisk **Dalej**.

**Aby wybrać języki aktualizacji**
1.  Na stronie Wybierz języki można określić, czy mają być pobierane aktualizacje dla wszystkich języków, czy dla określonego podzestawu języków. Wybranie podzestawu języków pozwala zaoszczędzić miejsce na dysku, ale ważne jest, aby wybrać wszystkie języki wymagane przez wszystkie komputery klienckie tego serwera WSUS.

    Jeśli chcesz pobrać aktualizacje tylko dla wybranych języków, wybierz opcję **Pobierz aktualizacje tylko w tych językach**, a następnie wybierz języki, dla których chcesz pobrać aktualizacje.

2.  Kliknij przycisk **Dalej**.

**Aby wybrać produkty do zaktualizowania**
1.  Na stronie Wybierz produkty można wybrać produkty, dla których mają zostać pobrane aktualizacje. Można wybrać kategorie produktów, np. system Windows, lub określone produkty, np. system Windows Server 2008. Wybranie kategorii produktów powoduje wybranie wszystkich produktów w danej kategorii.

2.  Kliknij przycisk **Dalej**.

**Aby wybrać klasyfikacje aktualizacji**
1.  Na stronie Wybierz klasyfikacje można wybrać klasyfikacje aktualizacji, które mają zostać pobrane. Można wybrać wszystkie klasyfikacje lub ich podzestaw.

2.  Kliknij przycisk **Dalej**.

**Aby skonfigurować harmonogram synchronizacji**
1.  Na stronie Ustaw harmonogram synchronizacji można określić, czy synchronizacja ma być wykonywana ręcznie, czy automatycznie.

    Jeśli zostanie wybrana opcja **Synchronizuj ręcznie**, proces synchronizacji trzeba będzie rozpoczynać z konsoli administracyjnej programu WSUS.

    Jeśli zostanie wybrana opcja **Synchronizuj automatycznie**, synchronizacja serwera WSUS będzie wykonywana w określonych odstępach czasu. W polu **Pierwsza synchronizacja** ustaw czas pierwszej synchronizacji, a następnie w polu **Liczba synchronizacji dziennie** określ liczbę synchronizacji wykonywanych przez serwer każdego dnia. Jeśli na przykład ustawiono cztery synchronizacje dziennie od godziny 3:00, synchronizacja będzie wykonywana o godzinie 3:00, 9:00, 15:00 i 21:00.

2.  Kliknij przycisk **Dalej**.

3.  Na stronie Zakończono można uruchomić konsolę administracyjną programu WSUS przez pozostawienie zaznaczonego pola wyboru **Uruchom przystawkę administracyjną programu Windows Server Update Services**. Pierwszą synchronizację można rozpocząć, pozostawiając zaznaczone pole wyboru **Rozpocznij wstępną synchronizację**.

4.  Kliknij przycisk **Zakończ**.

 
    <table style="border:1px solid black;">
    <colgroup>
    <col width="100%" />
    </colgroup>
    <thead>
    <tr class="header">
    <th><img src="images/Dd939924.Important(WS.10).gif" />Ważne</th>
    </tr>
    </thead>
    <tbody>
    <tr class="odd">
    <td style="border:1px solid black;">Podczas synchronizowania serwera nie można zapisać zmian dokonanych w konfiguracji. Aby dokonać zmian, należy poczekać na zakończenie synchronizacji.
    </td>
    </tr>
    </tbody>
    </table>
 

Korzystanie z konsoli administracyjnej programu WSUS
----------------------------------------------------

Poniżej przedstawiono procedury konfigurowania za pomocą konsoli administracyjnej programu WSUS.

**Aby wybrać produkty i klasyfikacje aktualizacji**
1.  W panelu **Opcje** kliknij pozycję **Produkty i klasyfikacje**. Zostanie wyświetlone okno dialogowe z kartami **Produkty** i **Klasyfikacje**.

2.  Na karcie **Produkty** wybierz kategorię produktów lub konkretne produkty, dla których aktualizacje mają być pobierane na serwer, albo wybierz pozycję **Wszystkie produkty**.

3.  Na karcie **Klasyfikacje** wybierz odpowiednią klasyfikację aktualizacji lub pozycję **Wszystkie klasyfikacje**.

4.  Kliknij przycisk **OK**, aby zapisać wybór.

**Aby wybrać pliki i języki aktualizacji**
1.  W panelu **Opcje** kliknij pozycję **Pliki i języki aktualizacji**. Zostanie wyświetlone okno dialogowe z kartami **Pliki aktualizacji** i **Języki aktualizacji**.

2.  Na karcie **Pliki aktualizacji** wybierz pozycję **Przechowuj pliki aktualizacji lokalnie na tym serwerze** lub określ, że wszystkie komputery klienckie mają przeprowadzać instalację z witryny Microsoft Update. Jeśli wybrano opcję przechowywania plików aktualizacji na tym serwerze, można również określić, czy mają być pobierane tylko zatwierdzone aktualizacje lub pliki instalacji ekspresowej.

3.  Jeśli pliki aktualizacji są przechowywane lokalnie, na karcie **Języki aktualizacji** wybierz opcję **Pobierz aktualizacje we wszystkich językach** (ustawienie domyślne) lub opcję **Pobierz aktualizacje tylko w wybranych językach**. Jeśli ten serwer WSUS ma serwery podrzędne, będą na nie pobierane tylko aktualizacje w językach określonych przez serwer nadrzędny.

4.  Kliknij przycisk **OK**, aby zapisać wybrane ustawienia.

**Aby zsynchronizować serwer WSUS**
1.  W panelu **Opcje** kliknij pozycję **Harmonogram synchronizacji**.

2.  Na karcie **Harmonogram synchronizacji** można określić, czy synchronizacja ma być wykonywana ręcznie, czy automatycznie.

    Jeśli zostanie wybrana opcja **Synchronizuj ręcznie**, proces synchronizacji trzeba będzie rozpoczynać z konsoli administracyjnej programu WSUS.

    Jeśli zostanie wybrana opcja **Synchronizuj automatycznie**, synchronizacja serwera WSUS będzie wykonywana w określonych odstępach czasu. W polu **Pierwsza synchronizacja** ustaw czas pierwszej synchronizacji, a następnie w polu **Liczba synchronizacji dziennie** określ liczbę synchronizacji wykonywanych przez serwer każdego dnia. Jeśli na przykład ustawiono cztery synchronizacje dziennie od godziny 3:00, synchronizacja będzie wykonywana o godzinie 3:00, 9:00, 15:00 i 21:00.

3.  Kliknij przycisk **OK**, aby zapisać wybrane ustawienia.

4.  W okienku nawigacji konsoli administracyjnej programu WSUS wybierz pozycję **Synchronizacje**.

5.  Kliknij prawym przyciskiem myszy lub przejdź do okienka **Akcje** po prawej stronie, a następnie kliknij pozycję **Synchronizuj teraz**.

    Jeśli po prawej stronie konsoli nie jest wyświetlane okienko **Akcje**, kliknij ikonę **Wyświetl** na pasku narzędzi konsoli, kliknij pozycję **Dostosuj** i upewnij się, że pole wyboru **Okienko akcji** jest zaznaczone.

6.  Po zakończeniu synchronizacji kliknij pozycję **Aktualizacje** w lewym panelu w celu wyświetlenia listy aktualizacji.

Następny krok
-------------

[Krok 5. Konfigurowanie aktualizacji klienta](https://technet.microsoft.com/5ae60ead-3e94-456c-a692-c0f193ea5d5a)

Materiały dodatkowe
-------------------

[Program Windows Server Update Services 3.0 z dodatkiem SP2 — przewodnik krok po kroku](https://technet.microsoft.com/4b504edc-93b3-45b0-a7e8-d0107f1a4442)
