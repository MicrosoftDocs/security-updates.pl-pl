---
TOCTitle: 'Krok 4. Konfigurowanie aktualizacji i synchronizacji'
Title: 'Krok 4. Konfigurowanie aktualizacji i synchronizacji'
ms:assetid: '734cc2ed-98be-4772-a42c-8fd38b39d864'
ms:contentKeyID: 18136644
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc708447(v=WS.10)'
---

Krok 4. Konfigurowanie aktualizacji i synchronizacji
====================================================

Przed pobraniem aktualizacji należy określić, które aktualizacje mają zostać pobrane. Ta sekcja przedstawia sposób konfigurowania zestawu aktualizacji do pobrania.

W procedurach zawartych w tym kroku opisano:

-   Zapisywanie i pobieranie informacji o serwerze nadrzędnym i serwerze proxy.
-   Wybieranie odpowiedniego języka aktualizacji.
-   Wybieranie produktów, dla których mają być pobierane aktualizacje.
-   Wybieranie odpowiednich klasyfikacji aktualizacji.
-   Określanie harmonogramu synchronizacji dla tego serwera.

Pięć następnych procedur przedstawia sposób konfigurowania aktualizacji przy użyciu kreatora konfiguracji. Kolejne procedury przedstawiają sposoby wykonania takiej konfiguracji w konsoli administracyjnej programu WSUS poprzez wybranie określonych opcji.

**Zapisywanie i pobieranie informacji o serwerze nadrzędnym i serwerze proxy**
1.  Konfiguracja serwera nadrzędnego i serwera proxy powinna już być wykonana za pomocą kreatora konfiguracji, a na ekranie powinna być wyświetlana strona **Połącz z serwerem nadrzędnym**.

2.  Kliknij przycisk **Rozpocznij połączenie**, co spowoduje zapisanie i przesłanie ustawień oraz pobranie informacji o dostępnych aktualizacjach.

3.  Po nawiązaniu połączenia będzie dostępny przycisk **Zatrzymaj połączenie**. W przypadku problemów z połączeniem kliknij przycisk **Zatrzymaj połączenie**, rozwiąż problemy i nawiąż ponownie połączenie.

4.  Po pomyślnym ukończeniu pobierania kliknij przycisk **Dalej**, aby przejść do strony **Wybierz języki** lub wybierz inną stronę w lewym panelu.

**Wybieranie języków aktualizacji**
1.  Strona **Wybierz języki** umożliwia pobranie aktualizacji dla wszystkich języków lub określonego podzestawu języków. Wybranie podzestawu języków umożliwi oszczędzenie miejsca na dysku, ale ważne jest, aby wybrać wszystkie języki wymagane przez wszystkie komputery klienckie tego serwera WSUS.

2.  Jeśli chcesz pobrać aktualizacje tylko dla kilku języków, wybierz opcję **Pobierz aktualizacje tylko w tych językach**, a następnie wybierz języki, dla których mają zostać pobrane aktualizacje. Kliknij przycisk **Dalej**, aby przejść do strony **Wybierz produkty** lub wybierz inną stronę w lewym panelu.

**Wybieranie produktów do zaktualizowania**
1.  Strona **Wybierz produkty** umożliwia określenie produktów, dla których mają zostać pobrane aktualizacje.

2.  Można zaznaczyć kategorie produktów takich jak system Windows lub określonych produktów takich jak system Windows Server 2003. Zaznaczenie kategorii produktów powoduje zaznaczenie również wszystkich jego produktów podrzędnych. Kliknij przycisk **Dalej**, aby przejść do strony **Wybierz klasyfikacje** lub wybierz inną stronę w lewym panelu.

**Wybieranie klasyfikacji aktualizacji**
1.  Strona **Wybierz klasyfikacje** umożliwia wybranie klasyfikacji aktualizacji, które mają zostać pobrane. Można zaznaczyć wszystkie klasyfikacje lub ich podzestaw.

2.  Kliknij przycisk **Dalej**, aby przejść do strony **Konfiguruj harmonogram synchronizacji** lub wybierz inną stronę w lewym panelu.

**Konfigurowanie harmonogramu synchronizacji**
1.  Zostanie wyświetlona strona **Ustaw harmonogram synchronizacji**, która pozwala określić, czy synchronizacja ma być wykonywana ręcznie czy automatycznie.

2.  Aby wybrać ręczną synchronizację dla danego serwera, należy ręcznie zainicjować proces synchronizacji z poziomu konsoli administracyjnej programu WSUS.

3.  Jeśli wybrano synchronizację automatyczną, serwer WSUS będzie wykonywać synchronizację z określonym interwałem. Ustaw czas pierwszej synchronizacji, a następnie określ liczbę synchronizacji wykonywanych przez serwer każdego dnia. Na przykład, jeśli ustawiono cztery synchronizacje na dzień, począwszy od godziny 3:00, synchronizacja będzie wykonywana o godzinie 3:00, 9:00, 15:00 i 21:00.

Po wykonaniu wszystkich powyższych kroków konfiguracji wybierz stronę **Zakończono** w kreatorze konfiguracji. Konsolę administracyjną programu WSUS można uruchomić poprzez pozostawienie zaznaczonego pola wyboru **Uruchom przystawkę administracyjną programu Windows Server Update Services**. Pierwszą synchronizację można rozpocząć, pozostawiając zaznaczone pole wyboru **Rozpocznij wstępną synchronizację**.

> [!note]  
> Podczas synchronizowania serwera nie można zapisać zmian dokonanych w konfiguracji. Aby dokonać zmian, należy poczekać na zakończenie synchronizacji. 

![](images/Cc708447.3f774fd1-af87-47d8-8f50-a5d585687d70(WS.10).gif)

Przedstawione poniżej procedury przedstawiają sposób wykonania powyższych kroków konfiguracji na stronie **Opcje** konsoli administracyjnej programu WSUS:

-   Wybieranie produktów i klasyfikacji
-   Pliki i języki aktualizacji

**Wybieranie produktów i klasyfikacji**
1.  Uruchom konsolę administracyjną programu WSUS: Kliknij przycisk **Start**, wskaż kolejno polecenia **Wszystkie programy** i **Narzędzia administracyjne**, a następnie kliknij pozycję **Microsoft Windows Server Update Services**.

2.  Wybierz pozycję **Opcje** poniżej serwera WSUS w lewym okienku.

3.  W środkowym okienku wybierz opcję **Produkty i klasyfikacje**.

4.  Zostanie wyświetlone okno dialogowe z dwiema kartami: **Produkty** i **Klasyfikacje**.

5.  Na karcie **Produkty** wybierz kategorię produktów lub określony produkt, dla którego serwer ma pobierać aktualizacje. W przeciwnym razie wybierz pozycję **Wszystkie produkty**.

6.  Na karcie **Klasyfikacje** wybierz odpowiednią klasyfikację aktualizacji lub pozycję **Wszystkie klasyfikacje**.

7.  Kliknij przycisk **OK**, aby zapisać wybór.

**Pliki i języki aktualizacji**
1.  Na stronie **Opcje** wybierz opcję **Pliki i języki aktualizacji**.

2.  Zostanie wyświetlone okno dialogowe z dwiema kartami: **Pliki aktualizacji** i **Języki aktualizacji**.

3.  Na karcie **Pliki aktualizacji** można wybrać, czy pliki aktualizacji będą zapisywane lokalnie, czy też wszystkie komputery klienckie będą pobierać je z witryny Microsoft Update. Jeśli wybrano opcję przechowywania plików aktualizacji na określonym serwerze, można ustawić pobieranie tylko zatwierdzonych aktualizacji lub plików instalacji ekspresowej.

4.  Na karcie **Języki aktualizacji** można wybrać pobieranie aktualizacji dla wszystkich języków (ustawienie domyślne) lub tylko dla określonych języków. Jeśli określony serwer WSUS ma serwery podrzędne, będą one pobierać aktualizacje tylko w językach określonych przez serwer nadrzędny.

5.  Kliknij przycisk **OK**, aby zapisać wybrane ustawienia.

Po skonfigurowaniu połączenia sieciowego można pobierać aktualizacje, przeprowadzając synchronizację z serwerem WSUS.

Operacja synchronizacji dotyczy serwera WSUS połączonego z witryną Microsoft Update. Po nawiązaniu połączenia program WSUS ustala, czy od czasu ostatniej synchronizacji zostały udostępnione nowe aktualizacje. W przypadku pierwszej synchronizacji serwera WSUS wszystkie aktualizacje są dostępne i gotowe do zatwierdzenia do instalacji. Początkowa synchronizacja może potrwać dość długo.

> [!note]  
> W tym dokumencie została opisana synchronizacja przy użyciu ustawień domyślnych, ale w programie WSUS można skorzystać z opcji pozwalających na zminimalizowanie wykorzystania przepustowości w procesie synchronizacji. 

**Aby przeprowadzić synchronizację serwera WSUS**
1.  W konsoli administracyjnej programu WSUS kliknij pozycję **Synchronizacje**.

2.  Kliknij prawym przyciskiem myszy lub przejdź do okienka **Akcje** po prawej stronie, a następnie kliknij pozycję **Synchronizuj teraz**.

> [!note]  
> Jeśli po prawej stronie konsoli nie jest wyświetlane okienko **Akcje**, kliknij ikonę **Wyświetl** na pasku narzędzi konsoli, kliknij pozycję **Dostosuj** i upewnij się, że pole wyboru **Okienko akcji** jest zaznaczone. 

Po zakończeniu synchronizacji kliknij pozycję **Aktualizacje** w lewym panelu w celu wyświetlenia listy aktualizacji.
