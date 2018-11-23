---
TOCTitle: Wykluczanie aplikacji
Title: Wykluczanie aplikacji
ms:assetid: 'b68ae4b2-b9ba-44ae-90cb-c88df600ec86'
ms:contentKeyID: 18123394
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747644(v=WS.10)'
---

Wykluczanie aplikacji
=====================

Można określić wersję aplikacji obsługującej technologię RMS, która sprawdzana jest we wszystkich żądaniach licencji. Wykluczanie aplikacji powoduje, że w każdej licencji użytkowania umieszczany jest warunek, zgodnie z którym licencja ta może być powiązana z odpowiednią zawartością chronioną technologią RMS tylko wtedy, gdy aplikacja zgłaszająca żądanie licencji nie znajduje się na liście wykluczania.

Funkcja ta może przydać się na przykład w sytuacji, gdy w przedsiębiorstwie rozmieszczana jest aktualizacja zabezpieczeń aplikacji. Administratorzy systemów mogą przy użyciu zwykłego mechanizmu doprowadzić do zainstalowania tej aktualizacji zabezpieczeń na komputerach klienckich. Następnie mogą ustawić zasady wykluczania aplikacji, które definiuje się przy użyciu informacji o wersji aplikacji używanych w administracyjnej witrynie sieci Web. Takie zasady wykluczania nie pozwalają programowi RMS na wystawianie licencji klientom, na których uruchomione są poprzednie wersje danego oprogramowania.

Aplikacje obsługujące technologię RMS wykluczane są na podstawie nazwy pliku i numeru wersji. Dzięki tej metodzie można mieć pewność, że użytkownicy zainstalują nowszą, bezpieczniejszą wersję aplikacji, kiedy tylko stanie się ona dostępna. Przypuśćmy na przykład, że w organizacji zostaje rozmieszczona wersja 1.0.4.2315 aplikacji obsługującej technologię RMS. Następnie twórca aplikacji wykrywa w niej problem związany z zabezpieczeniami i wydaje eliminującą go wersję 1.0.4.4200. Poza wdrożeniem nowej wersji aplikacji można ustanowić zasady wykluczania, które spowodują, że korzystanie z chronionej zawartości przy użyciu poprzedniej wersji aplikacji będzie niemożliwe.

Tak jak w przypadku pozostałych typów wykluczania, również wykluczanie aplikacji należy skonfigurować w każdym klastrze, w którym ma działać ta funkcja.

Kiedy na serwerze zostaną zastosowane te zasady wykluczania, klienci nie będą mogli za pomocą wykluczonej aplikacji żądać i wiązać nowych licencji użytkowania z zawartością chronioną technologią RMS. Klienci będą jednak mogli w dalszym ciągu korzystać z wcześniej licencjonowanych plików za pomocą wykluczonej aplikacji.

> [!note]  
> Program RMS wymaga określenia wersji aplikacji w formacie 4-cyfrowym z separatorem w postaci kropki (\#.\#.\#.\# ). Jednak oznaczenia wersji niektórych aplikacji składają się z 2 lub 3 cyfr rozdzielonych kropkami. W takim przypadku należy odpowiednio dopisać .0, aby format numeru wersji był zgodny z formatem wymaganym przez program RMS. 
