---
TOCTitle: Zabezpieczanie baz danych używanych przez program RMS
Title: Zabezpieczanie baz danych używanych przez program RMS
ms:assetid: '65802f9a-81bc-4398-968a-00c9b1dca2fa'
ms:contentKeyID: 18123302
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720285(v=WS.10)'
---

Zabezpieczanie baz danych używanych przez program RMS
=====================================================

Program RMS tworzy i wykorzystuje trzy bazy danych, z którymi wiążą się różne wymagania w dziedzinie zabezpieczeń:

-   **Usługi katalogowe**. Ta baza danych służy jako pamięć podręczna, w której umieszczane są wyniki kwerend dotyczących członkostwa w grupach usługi Active Directory. Ponieważ zawiera ona tylko informacje usługi Active Directory, nie wymaga dodatkowych zabezpieczeń poza tymi, które konfigurowane są automatycznie podczas zastrzegania programu RMS.
-   **Rejestrowanie**. Informacje w tej bazie danych są cenniejsze niż te, które znajdują się w bazie danych usług katalogowych, ponieważ ich ujawnienie mogłoby negatywnie wpłynąć na prywatność użytkownika. Firma Microsoft dołożyła szczególnych starań w celu zagwarantowania, że nie będą rejestrowane żadne informacje umożliwiające personalną identyfikację (PII) oraz że wszelkie informacje rejestrowane w tej bazie danych będą chronione przy użyciu odpowiednich środków bezpieczeństwa. Nie są wymagane żadne dodatkowe modyfikacje zabezpieczeń tej bazy danych, chyba że jest ona przenoszona na inny komputer z programem SQL Server. Jeśli baza danych przenoszona jest na inny serwer, należy zapewnić zastosowanie w nowym środowisku tych samych mechanizmów ochrony.
-   **Konfiguracja**. Ta baza danych, obok kluczy prywatnych serwera, stanowi najważniejszy i najcenniejszy zasób w rozmieszczeniu programu RMS. Zawiera ona cenne i kluczowe informacje, które wymagają ścisłej ochrony. Poza informacjami o konfiguracji znajdują się w niej wszystkie certyfikaty i klucze, szyfrowany klucz prywatny serwera (chyba że użyto zalecanego szyfrowania sprzętowego) oraz wartość (hash) hasła klucza prywatnego.

Kiedy program RMS tworzy bazę danych konfiguracji, ustawia uprawnienia, które ograniczają dostęp i pomagają w zapewnieniu jej bezpieczeństwa.

Zwiększanie zabezpieczeń baz danych
-----------------------------------

Wykonując czynności dodatkowe wymienione poniżej, można zwiększyć ogólne zabezpieczenia baz w środowisku sieci i serwerów:

-   Serwer bazy danych należy uruchomić na komputerze z systemem Windows Server 2003. Ten system operacyjny jest domyślnie lepiej zabezpieczony niż system Microsoft Windows 2000 Server. Komputer z systemem Windows 2000 Server można co prawda zablokować, jest to jednak proces czasochłonny i można podczas niego popełnić błędy, które pozwolą użytkownikom o złych zamiarach na uzyskanie dostępu do bazy danych.
-   Należy ograniczyć dostęp fizyczny do serwera bazy danych.
-   Należy upewnić się, że uprawnienia bazy danych oraz list DACL występujące w plikach bazy danych ograniczają dostęp do autoryzowanego personelu. Domyślne uprawnienia i listy DACL skonfigurowane przez program RMS są bezpieczne. Przy zmianie jakichkolwiek ustawień domyślnych należy zachować ostrożność.
-   Nie należy na serwerze baz danych uruchamiać niepotrzebnych usług, takich jak Internetowe usługi informacyjne (IIS) firmy Microsoft, Usługa kolejkowania wiadomości czy Usługi terminalowe.
-   Nie należy na serwerze baz danych uruchamiać żadnych baz danych poza bazami programu RMS.

Należy zabezpieczyć bazy danych serwera programu SQL Server, konfigurując protokół SSL (Secure Sockets Layer) lub IPsec (Internet Protocol Security) w celu zapewnienia szyfrowanych kanałów. Szyfrowanie komunikacji baz danych zapobiega przechwyceniu lub zmodyfikowaniu rejestrowanych danych przez użytkowników o złych zamiarach.

Więcej informacji na temat konfigurowania protokołu SSL dla serwera programu SQL Server można znaleźć w witrynie sieci Web MSDN ([http://go.microsoft.com/fwlink/?LinkID=17060](http://go.microsoft.com/fwlink/?linkid=17060)).

Więcej informacji na temat konfigurowania protokołu IPsec dla serwera programu SQL Server 2000 można znaleźć w witrynie sieci Web MSDN ([http://go.microsoft.com/fwlink/?LinkID=17061](http://go.microsoft.com/fwlink/?linkid=17061)).

Więcej informacji na temat zabezpieczeń rodziny systemów operacyjnych Microsoft Windows Server 2003 można uzyskać w dokumencie „Windows Server 2003 Security Guide” (Przewodnik po zabezpieczeniach systemu Windows Server 2003) dostępnym w Centrum pobierania firmy Microsoft ([http://go.microsoft.com/fwlink/?LinkId=36719](http://go.microsoft.com/fwlink/?linkid=36719)).
