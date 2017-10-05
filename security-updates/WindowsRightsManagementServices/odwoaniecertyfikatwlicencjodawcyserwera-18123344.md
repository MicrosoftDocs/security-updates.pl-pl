---
TOCTitle: Odwołanie certyfikatów licencjodawcy serwera
Title: Odwołanie certyfikatów licencjodawcy serwera
ms:assetid: '8020861d-d196-4431-8282-044675ef5616'
ms:contentKeyID: 18123344
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747578(v=WS.10)'
---

Odwołanie certyfikatów licencjodawcy serwera
============================================

W organizacji może zaistnieć potrzeba odwołania certyfikatu licencjodawcy serwera z powodu nieprzewidzianych okoliczności, które spowodują naruszenie zabezpieczeń serwera programu RMS. Klucz prywatny, którego nie przechowuje się w sprzętowym module zabezpieczeń, jest narażony na kradzież. Osoba dokonująca ataku, która przejmie kontrolę nad serwerem, może złamać certyfikat licencjodawcy serwera wraz z kluczem. Niezadowolony pracownik może także skopiować lub usunąć certyfikat albo klucz. Odwołanie to jeden ze sposobów na ograniczenie uszkodzeń i nadużyć ze strony użytkownika o złych zamiarach.

Domyślnie wszelkie licencje i certyfikaty może odwołać podmiot, który je wystawił. Ponieważ serwery programu RMS wystawiają licencje i certyfikaty skojarzone z chronioną zawartością w danej organizacji, zawsze można je odwołać, jeśli zajdzie taka potrzeba. Jeśli nastąpi naruszenie bezpieczeństwa serwera licencji, można odwołać odpowiadający mu certyfikat licencjodawcy serwera. Odwołanie certyfikatu licencjodawcy serwera powoduje unieważnienie wszystkich wystawionych przez niego certyfikatów i licencji. Instrukcje dotyczące odwołania licencji i certyfikatów znajdują się we wcześniejszej części tego tematu: „[Implementowanie odwołania](https://technet.microsoft.com/4735f060-7197-4ae2-830a-f91bcc4de30a)”.

Szczególnym przypadkiem jest klaster głównej certyfikacji. Certyfikat licencjodawcy serwera dla klastra głównej certyfikacji wystawia usługa rejestrowania firmy Microsoft i domyślnie tylko ona może odwołać ten certyfikat.

Firma Microsoft może odwołać certyfikat licencjodawcy serwera wystawiony dla serwera głównej certyfikacji tylko w przypadku, gdy użytkownik uzyska stosowny nakaz sądowy i dostarczy sądowi klucz publiczny danego serwera. Gdy sąd powiadomi firmę Microsoft o wydaniu nakazu odwołania, firma Microsoft określi dany certyfikat licencjodawcy serwera przy użyciu klucza publicznego na liście odwołania i udostępni tę listę publicznie. O sądowy nakaz odwołania można wnioskować, jeśli w odniesieniu do serwera, którego licencja ma być odwołana, zostanie spełniony jeden z poniższych warunków:

-   Użytkownik jest właścicielem serwera, a jego klucz publiczny został złamany.
-   Użytkownik jest właścicielem zawartości publikowanej na tym serwerze, a zawartość ta jest publikowana z naruszeniem praw autorskich.

Aby uzyskać i rozprowadzić listę odwołania od firmy Microsoft, która zawiera odwołany certyfikat licencjodawcy serwera dla serwera głównej certyfikacji, należy wykonać czynności opisane we wcześniejszej części tego tematu: „[Rozmieszczanie list odwołania](https://technet.microsoft.com/e331338b-66d4-45e4-8d3f-acccf2302ac4)”.

Podczas zastrzegania serwera głównej certyfikacji można określić klucz publiczny, z którym związane są uprawnienia do odwołania certyfikatu licencjodawcy serwera używanego przez klaster głównej certyfikacji. Ten klucz publiczny może należeć do organizacji lub do niezależnego podmiotu. Certyfikat licencjodawcy serwera można odwołać przy użyciu listy odwołania podpisanej odpowiednim kluczem prywatnym.

Aby odwołać certyfikat licencjodawcy serwera, z którego korzysta serwer głównej certyfikacji, można utworzyć listę odwołania określającą ten certyfikat licencjodawcy serwera, podpisać ją przy użyciu klucza prywatnego organizacji lub niezależnego podmiotu, a następnie rozprowadzić tę listę odwołania wśród wszystkich użytkowników. Aby uzyskać dalsze instrukcje, zobacz „Rozmieszczanie organizacyjnych list odwołania” we wcześniejszej części tego tematu: „[Rozmieszczanie list odwołania](https://technet.microsoft.com/e331338b-66d4-45e4-8d3f-acccf2302ac4)”.

Certyfikat licencjodawcy serwera można odwołać przy użyciu listy odwołania za pomocą następujących parametrów:

-   **Identyfikator GUID**. Certyfikat licencjodawcy serwera można odwołać na podstawie jego identyfikatora GUID. Aby uzyskać informacje dotyczące używania tego parametru na liście odwołania, zobacz „Odwołanie certyfikatów i licencji na podstawie identyfikatora GUID” we wcześniejszej części tego tematu: „[Tworzenie list odwołania](https://technet.microsoft.com/1ef75199-3344-4225-84de-a863a777696a)”.
-   **Wartość mieszania**. Certyfikat licencjodawcy serwera można odwołać na podstawie wartości mieszania SHA-1 znaków Unicode znajdujących się w treści certyfikatu. Aby uzyskać informacje dotyczące używania tego parametru na liście odwołania, zobacz „Odwołanie certyfikatów i licencji na podstawie wartości mieszania” we wcześniejszej części tego tematu: „[Tworzenie list odwołania](https://technet.microsoft.com/1ef75199-3344-4225-84de-a863a777696a)”.

Aby uzyskać certyfikat licencjodawcy serwera odpowiadający instalacji programu RMS, należy wykonać kwerendę w bazie danych konfiguracji tego programu. W poniższych krokach opisano, jak uzyskać te informacje z bazy danych konfiguracji w programie SQL Server oraz zapisać je w pliku, który można łatwo odczytać za pomocą przeglądarki:

1.  Otwórz program SQL Query Analyzer, a następnie połącz się z bazą danych konfiguracji serwera głównej certyfikacji.
2.  W menu **Query** (Kwerenda) kliknij polecenie **Results in Text** (Wyniki w postaci tekstu).
3.  W menu **Tools** (Narzędzia) kliknij polecenie **Options** (Opcje) w celu otwarcia okna dialogowego **Options** (Opcje). Kliknij kartę **Results** (Wyniki), a następnie w polu **Maximum characters per column** (Maksymalna liczba znaków w kolumnie) ustaw wartość **8192**.
        ```
1.  Skopiuj wyniki z okna **Results** (Wyniki), a następnie wklej je do edytora tekstu, na przykład do Notatnika. Zapisz wyniki w pliku z rozszerzeniem .xml.

Aby uzyskać więcej informacji dotyczących zastosowania tych informacji w liście odwołania, zobacz „[Tworzenie list odwołania](https://technet.microsoft.com/1ef75199-3344-4225-84de-a863a777696a)” we wcześniejszej części tego tematu.

Po zapisaniu informacji dotyczących certyfikatu licencjodawcy serwera w postaci pliku XML można z tego pliku wyodrębnić klucz publiczny, wykonując następujące kroki:

1.  Otwórz plik XML certyfikatu licencjodawcy serwera w edytorze plików XML lub plików tekstowych.
2.  W części &lt;ISSUEDPRINCIPALS&gt; skopiuj element &lt;PUBLICKEY&gt; element.
3.  Zapisz te informacje w pliku, który można przesłać do sądu lub umieścić na organizacyjnej liście odwołania.

Po odwołaniu certyfikatu licencjodawcy serwera wystawionego dla serwera głównej certyfikacji wszystkie certyfikaty i licencje wystawione przez instalację programu RMS staną się nieważne w odniesieniu do zawartości wymagającej listy odwołania, przez co zawartość ta stanie się niedostępna. Typ licencji posiadanej przez użytkownika nie ma wpływu na ten proces. Aby zachować zawartość opublikowaną przez serwer, którego licencja jest odwołana, przed zaimplementowaniem listy odwołania należy wykonać jedną z poniższych czynności:

-   Zapisać zawartość bez ochrony technologią RMS.
-   Opublikować zawartość ponownie bez wymagania listy odwołania.

W obu scenariuszach — odwołania przez firmę Microsoft oraz odwołania przez niezależny podmiot — lista odwołania zaczyna obowiązywać względem wszystkich żądań powiązania, ponieważ została podpisana przy użyciu klucza prywatnego podmiotu występującego w łańcuchu zaufania licencji użytkowania. Dlatego też niepowodzeniem zakończą się wszystkie żądania powiązania dotyczące licencji wystawionych przez daną instalację programu RMS przy użyciu odwołanego certyfikatu licencjodawcy serwera.

| ![](images/Cc747578.note(WS.10).gif)Uwaga                                            |
|-------------------------------------------------------------------------------------------------------------------|
| Firma Microsoft odwoła certyfikat licencjodawcy serwera tylko w sytuacji, gdy będzie to wymagane nakazem sądowym. |
