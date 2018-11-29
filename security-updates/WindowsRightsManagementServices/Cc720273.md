---
TOCTitle: Zmienianie hasła konta usługi programu RMS
Title: Zmienianie hasła konta usługi programu RMS
ms:assetid: '435c9cef-b622-48b3-9d4d-4bf5cac7d52d'
ms:contentKeyID: 18123250
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720273(v=WS.10)'
---

Zmienianie hasła konta usługi programu RMS
==========================================

Zależnie od zasad haseł, które określono dla serwerów programu RMS, hasło konta usługi programu RMS jest ustawiane, tak aby po pewnym czasie wygasało. Jeśli hasło wygaśnie, program RMS przestanie działać. Dlatego też hasło należy zmienić zanim wygaśnie.

**Stosowanie jednego konta usługi programu RMS**

Jeśli stosowane jest jedno konto usługi programu RMS, hasło na każdym serwerze programu RMS można zmienić w następujący sposób:

1.  Jeśli serwer wchodzi w skład klastra, wycofaj serwer z obiegu.
2.  Zaloguj się do serwera przy użyciu poświadczeń konta usługi programu RMS.
3.  Zmień hasło konta usługi programu RMS.
    Na pozostałych serwerach korzystających z tego samego konta usługi programu RMS wystąpi przestój usługi, ponieważ po zmianie hasła poświadczenia przechowywane na tych serwerach będą nieprawidłowe.
4.  Wyloguj się z serwera.
5.  Zaloguj się do serwera ponownie przy użyciu poświadczeń administratora programu RMS.
6.  Aby ponownie skonfigurować tożsamość użytkownika na serwerze, na stronie **Administracja globalna** kliknij łącze **Zmień konto usługi programu RMS**, a następnie na stronie **Zmień konto usługi programu RMS** określ domenę, nazwę użytkownika i hasło.
7.  Ponownie uruchom usługi IIS.
8.  Jeśli jest to wymagane, ponownie wprowadź serwer do obiegu.
9.  Powtórz kroki od 6 do 8 dla każdego serwera wchodzącego w skład klastra.

Jest to najprostsza metoda zmiany hasła konta usługi RMS. Może jednak spowodować pewne przestoje w działaniu programu RMS, ponieważ zmiana hasła konta usługi RMS na serwerze powoduje aktualizację usługi Active Directory przy użyciu nowego hasła. Internetowe usługi informacyjne (IIS) firmy Microsoft co pewien czas uruchamiają ponownie pule aplikacji, a te pule aplikacji, które działają w oparciu o stare poświadczenia, można uruchomić dopiero po zmianie konta usługi programu RMS i ponownym uruchomieniu usług IIS na danym serwerze. Do momentu ponownego uruchomienia pul aplikacji program RMS nie działa.

**Stosowanie dwóch kont usługi programu RMS**

Korzystając z tej metody, należy najpierw utworzyć dwa konta usługi programu RMS o różnych zasadach lub datach wygaśnięcia. W normalnych warunkach program RMS działa na pierwszym koncie. Kiedy zajdzie potrzeba zmiany hasła pierwszego konta, należy na każdym serwerze programu RMS wykonać następujące kroki:

1.  Jeśli serwer wchodzi w skład klastra, wycofaj serwer z obiegu.
2.  Określ drugie konto usługi programu RMS jako konto, na którym ma działać program RMS. Aby uzyskać instrukcje dotyczące zmieniania konta, zobacz „[Zmienianie konta usługi programu RMS](https://technet.microsoft.com/f257d66d-b823-41e4-bcb7-7c90eb295238)” w dalszej części tego tematu.
3.  Ponownie uruchom usługi IIS.
4.  Jeśli jest to wymagane, ponownie wprowadź serwer do obiegu.

Gdy wszystkie serwery programu RMS korzystają z drugiego konta usługi programu RMS, można zmienić hasło pierwszego konta usługi programu RMS i nie ma to wpływu na działanie tego programu. W ten sposób można przełączać się między dwoma kontami i unikać przestojów w działaniu programu RMS.
