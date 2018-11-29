---
TOCTitle: 'Krok 1. Przegląd wymagań dotyczących instalacji programu WSUS 3.0'
Title: 'Krok 1. Przegląd wymagań dotyczących instalacji programu WSUS 3.0'
ms:assetid: '912b37d7-021e-4c95-b317-49dd15b4611c'
ms:contentKeyID: 18136667
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc708484(v=WS.10)'
---

Krok 1. Przegląd wymagań dotyczących instalacji programu WSUS 3.0
=================================================================

W niniejszym przewodniku opisano sposób instalowania programu WSUS 3.0. Aby uzyskać informacje o wymaganiach programowych oraz obsługiwanych platformach dla programu WSUS 3.0, zobacz stronę z informacjami o wersji ([http://go.microsoft.com/fwlink/?LinkId=71220](http://go.microsoft.com/fwlink/?linkid=71220)) systemów Windows Server 2003 z dodatkiem Service Pack 1 oraz Windows Server® 2008.

Wymagania programowe dotyczące instalowania programu WSUS 3.0 w systemie Windows Server 2003 z dodatkiem Service Pack 1
-----------------------------------------------------------------------------------------------------------------------

Aby zainstalować program WSUS 3.0 w systemie Windows Server 2003 z dodatkiem Service Pack 1, na komputerze musi być zainstalowane poniższe oprogramowanie. Jeśli dowolna z tych aktualizacji wymaga ponownego uruchomienia serwera po ukończeniu instalacji, należy wykonać tę czynność przed zainstalowaniem programu WSUS 3.0.

-   Internetowe usługi informacyjne firmy Microsoft (IIS) 6.0
-   Aktualizacja usługi inteligentnego transferu w tle (BITS) 2.0 i składnika WinHTTP 5.1 systemu Windows Server 2003. Aby pobrać tę aktualizację, przejdź do Centrum pobierania ([http://go.microsoft.com/fwlink/?LinkID=47251](http://go.microsoft.com/fwlink/?linkid=47251)).
-   Pakiet dystrybucyjny programu Microsoft .NET Framework 2.0 (x86). Aby pobrać to oprogramowanie, przejdź do Centrum pobierania ([http://go.microsoft.com/fwlink/?LinkID=68935](http://go.microsoft.com/fwlink/?linkid=68935)). W przypadku platform 64-bitowych także przejdź do Centrum pobierania ([http://go.microsoft.com/fwlink/?LinkID=70637](http://go.microsoft.com/fwlink/?linkid=70637)).
-   Pakiet dystrybucyjny programu Microsoft Report Viewer 2005. Aby pobrać to oprogramowanie, przejdź do Centrum pobierania ([http://go.microsoft.com/fwlink/?LinkID=70410](http://go.microsoft.com/fwlink/?linkid=70410)).
-   Program Microsoft Management Console 3.0 dla systemu Windows Server 2003 (KB907265). Aby pobrać to oprogramowanie, przejdź do Centrum pobierania ([http://go.microsoft.com/fwlink/?LinkID=70412](http://go.microsoft.com/fwlink/?linkid=70412)). W przypadku platform 64-bitowych także przejdź do Centrum pobierania ([http://go.microsoft.com/fwlink/?LinkID=70638](http://go.microsoft.com/fwlink/?linkid=70638)).

Wymagania programowe dotyczące instalowania programu WSUS 3.0 w systemie Windows Server 2008
--------------------------------------------------------------------------------------------

Aby zainstalować program WSUS 3.0 w systemie Windows Server 2008, na komputerze musi być zainstalowane poniższe oprogramowanie. Jeśli dowolna z tych aktualizacji wymaga ponownego uruchomienia serwera po ukończeniu instalacji, należy wykonać tę czynność przed zainstalowaniem programu WSUS 3.0.

-   Internetowe usługi informacyjne firmy Microsoft (IIS) 7.0 Należy sprawdzić, czy są włączone następujące składniki:
    -   Uwierzytelnianie systemu Windows
    -   ASP.NET
    -   Zgodność z narzędziami zarządzania usługami IIS w wersji 6
    -   Zgodność z metabazą usług IIS
-   Pakiet dystrybucyjny programu Microsoft Report Viewer 2005. Aby pobrać to oprogramowanie, przejdź do Centrum pobierania ([http://go.microsoft.com/fwlink/?LinkID=70410](http://go.microsoft.com/fwlink/?linkid=70410)).
-   Program SQL Server™ 2005 z dodatkiem Service Pack 1. Aby pobrać to oprogramowanie, przejdź do Centrum pobierania ([http://go.microsoft.com/fwlink/?LinkID=66143](http://go.microsoft.com/fwlink/?linkid=66143)).

Program .NET Framework 2.0 i aktualizacja usługi BITS 2.0 są dostępne w ramach systemu operacyjnego Windows Server 2008.

Wymagania i zalecenia dotyczące miejsca na dysku
------------------------------------------------

Aby można było zainstalować program WSUS 3.0, system plików na serwerze musi spełniać następujące wymagania:

-   Zarówno partycja systemowa, jak i partycja, na której jest instalowany program WSUS 3.0, muszą być sformatowane w systemie plików NTFS.
-   Dla partycji systemowej jest zalecany co najmniej 1 GB wolnego miejsca.
-   Dla woluminu, w którym będzie przechowywana zawartość programu WSUS, jest wymagane co najmniej 20 GB wolnego miejsca; zalecana optymalna wartość to 30 GB wolnego miejsca.
-   Dla woluminu, w którym Instalator programu WSUS zainstaluje składnik Windows® Internal Database, są zalecane co najmniej 2 GB wolnego miejsca.

Wymagania w przypadku instalacji tylko konsoli
----------------------------------------------

Program WSUS 3.0 umożliwia obecnie zainstalowanie konsoli administracyjnej programu WSUS w systemach zdalnych niezależnie od serwera WSUS. Wersję zawierającą tylko konsolę można zainstalować w następujących systemach operacyjnych:

-   Windows Server® 2008
-   Windows Vista®
-   Windows Server 2003 z dodatkiem Service Pack 1
-   Windows XP z dodatkiem Service Pack 2

Poniżej przedstawiono wymagania programowe dla wersji zawierającej tylko konsolę.

-   Pakiet dystrybucyjny programu Microsoft .NET Framework 2.0 (x86), dostępny w Centrum pobierania firmy Microsoft ([http://go.microsoft.com/fwlink/?LinkId=68935](http://go.microsoft.com/fwlink/?linkid=68935)). W przypadku platform 64-bitowych należy zainstalować pakiet dystrybucyjny programu Microsoft .NET Framework 2.0 (x64) ([http://go.microsoft.com/fwlink/?LinkId=70637](http://go.microsoft.com/fwlink/?linkid=70637)).
-   Program Microsoft Management Console 3.0 dla systemu Windows Server 2003 (KB907265), dostępny w Centrum pobierania firmy Microsoft ([http://go.microsoft.com/fwlink/?LinkId=70412](http://go.microsoft.com/fwlink/?linkid=70412)). W przypadku platform 64-bitowych należy zainstalować program Microsoft Management Console 3.0 dla systemu Windows Server 2003 x64 Edition (KB907265) ([http://go.microsoft.com/fwlink/?LinkId=70638](http://go.microsoft.com/fwlink/?linkid=70638)).
-   Pakiet dystrybucyjny programu Microsoft Report Viewer 2005, dostępny w Centrum pobierania firmy Microsoft ([http://go.microsoft.com/fwlink/?LinkId=70410](http://go.microsoft.com/fwlink/?linkid=70410)).

Wymagania składnika Aktualizacje automatyczne
---------------------------------------------

Aktualizacje automatyczne to składnik kliencki programu WSUS 3.0. Jedynym wymaganiem sprzętowym dla tej funkcji jest podłączenie do sieci. Składnika Aktualizacje automatyczne z programem WSUS 3.0 można używać na komputerach z dowolnym z następujących systemów operacyjnych:

-   Windows Vista.
-   Windows Server® 2008.
-   Microsoft Windows® Server 2003 (wszystkie wersje i dodatki Service Pack).
-   Microsoft Windows XP Professional (Service Pack 1 lub Service Pack 2).
-   Microsoft Windows 2000 Professional Service Pack 4, Windows 2000 Server Service Pack 4 lub Windows 2000 Advanced Server Service Pack 4.

Uprawnienia
-----------

Określeni użytkownicy we wskazanych katalogach muszą mieć następujące uprawnienia do dysków:

1.  Grupa wbudowana Użytkownicy lub konto Zarządzanie NT\\Usługa sieciowa (w systemie Windows Server 2003) powinno mieć uprawnienia do odczytu w folderze głównym na dysku zawierającym katalog zawartości programu WSUS. W przypadku braku tego uprawnienia pobieranie plików dla usługi BITS nie powiedzie się.
2.  Konto Zarządzanie NT\\Usługa sieciowa powinno mieć uprawnienie „Pełna kontrola” w katalogu zawartości programu WSUS (zwykle jest to katalog &lt;DyskSystemowy&gt;:WSUS\\WsusContent). To uprawnienie jest ustawiane przez instalatora serwera WSUS podczas tworzenia katalogu, jednak niektóre składniki oprogramowania zabezpieczeń mogą zresetować to uprawnienie. W przypadku braku tego uprawnienia pobieranie plików dla usługi BITS nie powiedzie się.
3.  Konto Zarządzanie NT\\Usługa sieciowa powinno mieć uprawnienie „Pełna kontrola” w następujących folderach, aby przystawka Administracja WSUS była wyświetlana poprawnie:
    -   %windir%\\Microsoft .NET\\Framework\\v2.0.50727\\Temporary ASP.NET Files
    -   %windir%\\Temp

Aby uzyskać więcej informacji o ustawianiu uprawnień, zobacz artykuł opisujący problem z narzędziem DCPROMO, polegający na tym, że nie zachowuje ono uprawnień dla niektórych folderów usług IIS ([http://go.microsoft.com/fwlink/?LinkID=76332](http://go.microsoft.com/fwlink/?linkid=76332)) (strona może zostać wyświetlona w języku angielskim).
