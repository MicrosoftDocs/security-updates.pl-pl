---
TOCTitle: Jak działa odwołanie w programie RMS
Title: Jak działa odwołanie w programie RMS
ms:assetid: '469e3938-a59b-4c92-9779-ead64e724d00'
ms:contentKeyID: 18123247
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720263(v=WS.10)'
---

Jak działa odwołanie w programie RMS
====================================

Odwołanie uniemożliwia dowiązywanie – czyli proces pozwalający użytkownikowi na wykorzystanie zawartości – gdy odwołana jednostka jest uwzględniona w żądaniu dowiązania. Odwołanie jest implementowane w postaci list odwołania rozpowszechnianych do komputerów klienckich. Te listy są podpisanymi plikami XrML określającymi zawartość, aplikacje, użytkowników lub inne podmioty, które zostały odwołane przez podmiot wystawiający listę.

Za każdym razem, gdy użytkownik próbuje skorzystać z zawartości chronionej, skojarzona aplikacja obsługująca technologię RMS wysyła żądanie dotyczące odpowiedniego prawa dostępu – w ramach żądania dowiązania – do klienta programu RMS. Jeśli na przykład użytkownik próbuje otworzyć plik, aplikacja żąda prawa przeglądania, które umożliwia otwarcie pliku. Jeśli użytkownik próbuje edytować plik, aplikacja żąda prawa edycji.

Podczas przetwarzania żądania dowiązania klient programu RMS wykonuje następujące czynności:

1.  Sprawdza, czy licencja użytkowania wymaga list odwołania.
2.  Jeśli licencja użytkowania wymaga odwołania, składnik klienta sprawdza, czy określona lista odwołania jest obecna, zarejestrowana i aktualna, zgodnie z interwałem czasu odświeżania określonym w licencji użytkowania.
3.  Sprawdza, czy podmiot, który podpisał listę odwołania, jest określony w licencji użytkowania jako podmiot uprawniony do odwołania licencji.
4.  Jeśli te testy zakończą się pomyślnie, składnik klienta określi, czy podmioty znajdujące się w oryginalnym żądaniu dowiązania nie zostały odwołane. Jeśli tak jest, składnik odmawia żądaniu dowiązania.

Listy odwołania mogą być rozpowszechniane do komputerów klienckich przez administratora lub mogą być pobierane przez komputer za pomocą aplikacji obsługującej technologię RMS, gdy są wymagane przez licencję użytkowania. Jeśli lista odwołania została użyta do dowiązania zawartości, to została zarejestrowana i może być używana dla żądań dowiązania dotyczących innych licencji użytkowania, tak długo jak aplikacja pozostanie uruchomiona. Po zamknięciu aplikacji lista odwołania jest wyrejestrowywana.

Poniższy diagram przedstawia proces dowiązywania oraz rolę odwołania w tym procesie.

![](images/Cc720263.81aa2d70-d261-49ad-b446-96a2eddba1a5(WS.10).gif)

Odwołanie jest opcjonalne. Administrator programu RMS może wymagać odwołania, określając je w jednym lub kilku szablonach zasad praw dostępu organizacji. Jeśli odwołanie jest wymagane, licencja nie może zostać dowiązana, jeśli wymagana lista odwołania nie jest dostępna, nie jest zarejestrowana na komputerze użytkownika lub jest starsza niż interwał czasu odświeżania określony w licencji użytkowania.

Należy jednak pamiętać, że nawet jeśli dana licencja użytkowania nie wymaga odwołania, funkcja ta może zostać użyta w odniesieniu do tej licencji. Odwołanie zachodzi zawsze, gdy dowolny podmiot wystawiający dowolny certyfikat w łańcuchu zaufania biorącym udział w żądaniu dowiązania wystawił listę odwołania zarejestrowaną na komputerze klienckim. W takim przypadku lista odwołania jest używana do przetworzenia żądań dowiązania, nawet jeśli licencje użytkowania nie wymagają odwołania. Dzieje się tak do momentu zamknięcia aplikacji obsługującej technologię RMS, kiedy lista odwołania jest wyrejestrowywana.

Na przykład jeśli użytkownik próbuje użyć zawartości, której licencja użytkowania, wystawiona przez jednostkę A, wymaga listy odwołania wystawionej przez jednostkę A, aplikacja obsługująca technologię RMS uzyska listę odwołania poprzez adres URL określony w licencji użytkowania, a następnie ją zarejestruje. Podczas przetwarzania żądania dowiązania klient programu RMS sprawdza listę odwołania w poszukiwaniu możliwych odwołań.

Pozostawiając otwartą aplikację obsługującą technologię RMS, użytkownik próbuje użyć innego fragmentu zawartości, którego licencja użytkowania została również wystawiona przez jednostkę A. Chociaż ta licencja użytkowania nie zawiera warunku odwołania, lista odwołania od jednostki A jest aktualnie zarejestrowana na komputerze użytkownika. W tej sytuacji składnik klienta sprawdzi listę odwołania przed przetworzeniem żądania dowiązania.

Następnie użytkownik próbuje użyć fragmentu zawartości, którego licencja użytkowania została wystawiona przez jednostkę C. Licencja użytkowania nie zawiera warunku odwołania. Ponieważ jedyną listą odwołania zarejestrowaną na komputerze klienckim jest lista odwołania wystawiona przez jednostkę A, a jednostka A nie jest w łańcuchu zaufania dla tej licencji użytkowania, dla procesu dowiązania nie będzie wykonywane odwołanie.

W końcu użytkownik zamyka aplikację obsługującą technologię RMS, a następnie ponownie otwiera drugi fragment zawartości, który nie zawierał warunku odwołania. Ponieważ lista odwołania wystawiona przez jednostkę A została wyrejestrowana podczas zamykania aplikacji, klient programu RMS nie sprawdzi listy przed przetworzeniem żądania dowiązania.
