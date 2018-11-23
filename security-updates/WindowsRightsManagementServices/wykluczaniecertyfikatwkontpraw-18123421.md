---
TOCTitle: Wykluczanie certyfikatów kont praw
Title: Wykluczanie certyfikatów kont praw
ms:assetid: 'cba5e901-942c-4d06-9865-e6c4648c95e6'
ms:contentKeyID: 18123421
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747670(v=WS.10)'
---

Wykluczanie certyfikatów kont praw
==================================

Jeśli użytkownik jest zaufany, ale nastąpi naruszenie bezpieczeństwa jego poświadczeń RMS, można wykluczyć certyfikat konta praw tego użytkownika przez wykluczenie jego klucza publicznego. Spowoduje to, że program RMS będzie odrzucać nowe żądania licencji użytkowania, które dotyczą wykluczonego certyfikatu konta praw. Jeśli certyfikat konta praw zostanie wykluczony, to następnym razem, gdy użytkownik spróbuje uzyskać licencję użytkowania na nową zawartość, żądania będą odrzucane. W celu uzyskania licencji użytkowania użytkownik będzie musiał pobrać nowy certyfikat konta praw z nową parą kluczy.

Certyfikaty konta praw można wykluczać za pomocą strony **Zasady wykluczania** w administracyjnej witrynie sieci Web. Po wykluczeniu certyfikatu konta praw określonego użytkownika program RMS dodaje wykluczony klucz, nazwę konta tego użytkownika oraz datę i godzinę wykluczenia do tabeli DRMS\_GicExclusionList w bazie danych konfiguracji danego klastra głównej certyfikacji. Informacje te są także wyświetlane w administracyjnej witrynie sieci Web na stronie **Zasady wykluczania**. Ponadto program RMS usuwa z tabeli UD\_Users w bazie danych konfiguracji zarówno klucz publiczny, jak i prywatny skojarzony z wykluczonym certyfikatem konta.

Aby wykluczyć certyfikat konta praw znajdujący się w klastrze lub na serwerze głównej certyfikacji, należy określić konto domeny użytkownika na stronie **Zasady wykluczania** serwera głównej certyfikacji. Certyfikat konta praw należy wykluczyć w podrejestrowywanych serwerach w administracyjnej witrynie sieci Web każdego serwera. Aby wykluczyć użytkownika w podrejestrowywanym serwerze lub klastrze licencji, należy wprowadzić wartość klucza publicznego dla certyfikatu konta praw na stronie **Zasady wykluczania** w administracyjnej witrynie sieci Web danego serwera licencji. Wartość tę można uzyskać na stronie **Zasady wykluczania** w administracyjnej witrynie sieci Web klastra głównej certyfikacji.

Aby uprościć wykluczanie certyfikatów konta praw w rozmieszczeniu programu RMS obejmującym wiele klastrów, można wykonać replikę tabeli DRMS\_GicExclusionList z bazy danych konfiguracji klastra głównej certyfikacji w bazie danych konfiguracji każdego klastra licencji. W takim przypadku nie ma potrzeby ręcznego wprowadzania wartości klucza publicznego na każdym serwerze.
