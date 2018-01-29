---
TOCTitle: 'Krok 1. Przegląd wymagań dotyczących instalacji programu WSUS'
Title: 'Krok 1. Przegląd wymagań dotyczących instalacji programu WSUS'
ms:assetid: '57d7f8ec-1523-4485-9967-604be9ba2aac'
ms:contentKeyID: 18136876
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720547(v=WS.10)'
---

Krok 1. Przegląd wymagań dotyczących instalacji programu WSUS
=============================================================

Ten przewodnik zawiera instrukcje dotyczące instalowania programu Microsoft Windows Server Update Services (WSUS) w systemach operacyjnych Microsoft Windows Server 2003 (poza wersją Web Edition oraz wszystkimi wersjami 64-bitowymi). Użytkownicy serwera z systemem Microsoft Windows 2000 Server mogą znaleźć dodatkowe informacje w oficjalnym dokumencie „Deploying Microsoft Windows Server Update Services” (dokument dostępny w języku angielskim).

Poniżej przedstawiono podstawowe wymagania dotyczące instalacji z zastosowaniem opcji domyślnych. Informacje na temat wymagań sprzętowych i programowych w przypadku innych instalacji można znaleźć w oficjalnym dokumencie „Deploying Microsoft Windows Server Update Services” (dokument dostępny w języku angielskim).

Zalecenia sprzętowe w przypadku serwera z maksymalnie 500 klientami są następujące:

-   Procesor o częstotliwości taktowania 1 GHz
-   1 GB pamięci RAM

Wymagania dotyczące oprogramowania
----------------------------------

Aby zainstalowanie programu WSUS z zastosowaniem opcji domyślnych było możliwe, na komputerze musi zostać zainstalowane poniższe oprogramowanie. Więcej informacji na temat wymagań programowych w przypadku programu WSUS można znaleźć w oficjalnym dokumencie „Deploying Microsoft Windows Server Update Services” (dokument dostępny w języku angielskim). Jeśli którakolwiek aktualizacja wymaga ponownego uruchomienia serwera po zakończeniu instalacji, należy to zrobić przez rozpoczęciem instalowania programu WSUS.

-   Internetowe usługi informacyjne (IIS) 6.0. Instrukcje dotyczące sposobu instalowania tego programu można znaleźć w oficjalnym dokumencie „Deploying Microsoft Windows Server Update Services” (dokument dostępny w języku angielskim) lub w Centrum pomocy i obsługi technicznej dla systemu Windows Server 2003.
-   Dodatek Service Pack 1 dla architektury Microsoft .NET Framework 1.1 przeznaczony dla systemu Windows Server 2003. Aby uzyskać to oprogramowanie, przejdź do [Centrum pobierania](http://go.microsoft.com/fwlink/?linkid=47358) (http://go.microsoft.com/fwlink/?LinkId=35326).
    Innym rozwiązaniem jest przejście do witryny sieci Web pod adresem http://www.windowsupdate.com i przeskanowanie komputera pod kątem krytycznych aktualizacji oraz dodatków Service Pack, a następnie zainstalowanie dodatku Service Pack 1 dla architektury Microsoft .NET Framework 1.1 przeznaczonego dla systemu Windows Server 2003.
-   Usługa inteligentnego transferu w tle (BITS) 2.0 Aktualnie program BITS 2.0 dla Windows Server 2003 nie jest dostępny w Centrum pobierania. Aby uzyskać to oprogramowanie, przejdź na stronę programu Windows Server Update Services Open Evaluation w [witrynie firmy Microsoft w sieci Web](http://go.microsoft.com/fwlink/?linkid=47357) (http://go.microsoft.com/fwlink/?LinkId=47357).

> [!note]  
> Chociaż w celu zainstalowania programu WSUS wymagane jest oprogramowanie bazy danych, nie zostało ono wymienione w tym miejscu, ponieważ w ramach domyślnej instalacji programu WSUS w systemie Windows Server 2003 jest instalowane oprogramowanie bazy danych Windows SQL Server™ 2000 Desktop Engine (WMSDE). 

Wymagania i zalecenia dotyczące miejsca na dysku
------------------------------------------------

Aby zainstalować program WSUS, system plików serwera musi spełniać następujące wymagania:

-   Partycja systemowa oraz partycja z zainstalowanym programem WSUS muszą być sformatowane w systemie plików NTFS.
-   Na partycji systemowej musi być dostępne co najmniej 1 GB wolnego miejsca.
-   W przypadku woluminu służącego do przechowywania danych programu WSUS musi być dostępne co najmniej 6 GB wolnego miejsca (zalecane 30 GB).
-   W przypadku woluminu, na którym Instalator programu WSUS instaluje oprogramowanie Windows SQL Server 2000 Desktop Engine (WMSDE), musi być dostępne co najmniej 2 GB wolnego miejsca.

Wymagania dotyczące funkcji Aktualizacje automatyczne
-----------------------------------------------------

Funkcja Aktualizacje automatyczne jest składnikiem klienckim programu WSUS. Jedynym wymaganiem sprzętowym dla tej funkcji jest podłączenie do sieci. Z funkcji Aktualizacje automatyczne (w ramach programu WSUS) można korzystać na komputerach z następującymi systemami operacyjnymi:

-   Microsoft Windows 2000 Professional z dodatkiem Service Pack 3 (SP3) lub Service Pack 4 (SP4), Windows 2000 Server z dodatkiem SP3 lub SP4, Windows 2000 Advanced Server z dodatkiem SP3 lub SP4;
-   Microsoft Windows XP Professional z lub bez dodatku Service Pack 1 lub Service Pack 2;
-   Microsoft Windows Server 2003, Standard Edition; Windows Server 2003, Enterprise Edition; Windows Server 2003, Datacenter Edition; Windows Server 2003, Web Edition.
