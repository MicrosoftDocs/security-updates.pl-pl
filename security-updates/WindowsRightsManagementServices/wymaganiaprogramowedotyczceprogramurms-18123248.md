---
TOCTitle: Wymagania programowe dotyczące programu RMS
Title: Wymagania programowe dotyczące programu RMS
ms:assetid: '17faf2ad-2366-4a92-98a5-766e20a0f741'
ms:contentKeyID: 18123248
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720201(v=WS.10)'
---

Wymagania programowe dotyczące programu RMS
===========================================

W poniższej tabeli przedstawiono wymagania programowe dla instalacji serwerów RMS.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Wymagane</th>
<th style="border:1px solid black;" >oprogramowanie</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">System operacyjny</td>
<td style="border:1px solid black;">Dowolna edycja systemu Microsoft Windows Server® 2003, oprócz Web Edition.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">System plików</td>
<td style="border:1px solid black;">Zaleca się stosowanie systemu plików NTFS.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Składniki systemu operacyjnego</td>
<td style="border:1px solid black;"><ul>
<li>Zainstalowana usługa kolejkowania wiadomości (znana także pod nazwą MSMQ) z włączoną funkcją integracji z usługą katalogową Active Directory®.<br />
<br />
</li>
<li>Internetowe usługi informacyjne (IIS) z włączoną obsługą ASP.NET.<br />
<br />
</li>
<li>Platforma Microsoft .NET Framework 1.1<br />
<br />
</li>
</ul></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Usługa katalogowa Active Directory®</td>
<td style="border:1px solid black;">Program RMS musi być zainstalowany w domenie usługi Active Directory, w której na kontrolerach domeny zainstalowano system Windows Server 2000 z dodatkiem Service Pack w wersji 3 (SP3) lub nowszej. Wszyscy użytkownicy programu RMS i grupy go używające muszą mieć adresy e-mail skonfigurowane w usłudze Active Directory w celu korzystania z zawartości i jej publikowania.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Serwer bazy danych</td>
<td style="border:1px solid black;">Aby wykonywać operacje, program RMS wymaga bazy danych oraz procedur przechowywania. Można korzystać z programu Microsoft SQL Server 2000 z dodatkiem SP3a lub nowszym lub z programu Microsoft SQL Server 2005. W celach testowania bądź w przypadku wdrożenia na pojedynczym komputerze można używać programu Microsoft SQL Server Desktop Engine (MSDE 2000) z dodatkiem SP3 lub Microsoft SQL Server 2005 Express Edition.</td>
</tr>
</tbody>
</table>
  
Jeśli program RMS jest wdrażany w środowisku, w którym istnieje wiele lasów usługi Active Directory, należy użyć grup uniwersalnych usługi Active Directory, aby przynależność do grup została zreplikowana we wszystkich wykazach globalnych. W celu utworzenia grup uniwersalnych należy ustawić poziom funkcjonalny domeny co najmniej na poziomie macierzystym systemu Windows 2000, a poziom funkcjonalny lasu podwyższyć do poziomu systemu Windows Server 2003.
  
Zaleca się używanie programu MSDE 2000 lub Microsoft SQL Server 2005 Express Edition do obsługi baz danych programu RMS tylko w środowiskach testowych, ponieważ program MSDE 2000 lub Microsoft SQL Server 2005 Express Edition nie obsługuje żądanych interfejsów sieciowych. Ponadto zasady użytkowania programu MSDE 2000 lub Microsoft SQL Server 2005 Express Edition zabraniają używania narzędzi klienckich programu SQL Server do pracy z bazą danych programu MSDE 2000 lub Microsoft SQL Server 2005 Express Edition. To ograniczenie uniemożliwi przeglądanie informacji rejestrowania lub zmienianie danych przechowywanych w bazie danych konfiguracji.
  
Jeśli na serwerze nie jest zainstalowany program ASP.NET w wersji 1.1, proces instalacji różni się w zależności od tego, czy wykorzystywana jest 32-bitowa czy 64-bitowa wersja systemu Windows Server 2003.
  
Poniższe czynności umożliwią zainstalowanie i włączenie usługi ASP.NET w wersji 1.1 w przypadku korzystania z 32-bitowej wersji systemu Windows Server 2003:
  
1.  Otwórz aplet **Dodaj lub usuń programy** w **Panelu sterowania**, a następnie kliknij polecenie **Dodaj/usuń składniki systemu Windows**.  
2.  Kliknij pozycję **Serwer aplikacji**, a następnie przycisk **Szczegóły**.  
3.  W Kreatorze składników systemu Windows zaznacz pozycję **ASP.NET**.  
4.  Jeśli program ASP.NET 1.1 jest zainstalowany, lecz jest zablokowany jako rozszerzenie usługi sieci Web IIS:  
    -   Otwórz Menedżera internetowych usług informacyjnych.  
    -   Kliknij pozycję **Rozszerzenie usługi sieci Web IIS**, zaznacz pozycję ASP.NET v1.1.4322, a następnie kliknij przycisk **Zezwalaj**.
  
Poniższe czynności umożliwią zainstalowanie i włączenie usługi ASP.NET w wersji 1.1 w przypadku korzystania z 64-bitowej wersji systemu Windows Server 2003:
  
1.  Zainstaluj pakiet .NET Framework 1.1, a wraz z nim zostanie zainstalowany program ASP.NET 1.1. Pakiet Microsoft .NET Framework w wersji 1.1 do dystrybucji można pobrać z Centrum pobierania firmy Microsoft ([http://go.microsoft.com/fwlink/?LinkID=69985](http://go.microsoft.com/fwlink/?linkid=69985)).  
2.  Otwórz Menedżera internetowych usług informacyjnych.  
3.  Kliknij pozycję Rozszerzenie usługi sieci Web IIS, zaznacz pozycję ASP.NET v1.1.4322, a następnie kliknij przycisk Zezwalaj.
  
W przypadku korzystania z programu RMS w 64-bitowej wersji systemu Windows Server 2003 należy wykonać poniższe czynności, aby usługi IIS mogły współpracować z programem RMS:
  
1.  Kliknij przycisk **Start**, a następnie polecenie **Uruchom**.  
2.  W polu **Otwórz** wpisz następujące polecenie, po czym naciśnij klawisz ENTER:
  
**„cscript %SystemDrive%\\inetpub\\AdminScripts\\adsutil.vbs set w3svc/AppPools/Enable32bitAppOnWin64 1"**
  
Program RMS nie jest przeznaczony dla platformy .NET Framework w wersji 2.0. Podczas gdy instalacja wspólna jest obsługiwana, należy upewnić się, że platforma ASP.NET została skonfigurowana w taki sposób, aby korzystała z usługi ASP.NET v1.1.4322. Poprawność instalacji wspólnej można sprawdzić na dwa sposoby:
  
-   Przed zainstalowaniem serwera RMS zainstaluj platformę .NET Framework w wersji 2.0.  
-   Przywróć wersję 1.1.4322 usługi ASP.NET na domyślnej witrynie sieci Web w Internetowych usługach informacyjnych, uruchamiając poniższe polecenie:
  
**"%SystemRoot%\\Microsoft.NET\\Framework\\v1.1.4322\\aspnet\_regiis -s w3svc/1/root"**
  
Aby uzyskać więcej informacji na temat usługi Active Directory, usługi kolejkowania wiadomości i Internetowych usług informacyjnych (IIS), odwiedź Centrum pomocy i obsługi technicznej systemu Windows Server 2003.
  
> [!Caution]  
> Można zastrzec serwer programu RMS w domyślnej witrynie sieci Web lub w dowolnej witrynie uprzednio zdefiniowanej w Internetowych usługach informacyjnych (IIS) na tym serwerze. Ze względów bezpieczeństwa nie należy uruchamiać na tym serwerze dodatkowych witryn ani usług. Wykonanie tych czynności może spowodować, że wiele aplikacji i usług będzie działać na jednym koncie jako program RMS (szczególnie na koncie LocalSystem), co może spowodować, że klucze prywatne będą narażone na działania niebezpiecznych operacji. Serwera programu RMS nie należy zastrzegać w tej samej witrynie sieci Web, w której zastrzeżono program Microsoft Office SharePoint Server 2007. Programu RMS nie można używać razem z uwierzytelnianiem Kerberos. Zastrzeżenie serwera programu RMS w witrynie sieci Web spowoduje wyłączenie uwierzytelniania Kerberos na tym serwerze. Jeśli program RMS nie został skonfigurowany w taki sposób, aby korzystał z usługi ASP.NET v1.1.4322, w bazie danych rejestrowania nie są rejestrowane żadne informacje, co prowadzi do utraty danych. 
  
Zobacz też:  
-----------
  
####  
  
[Planowanie infrastruktury serwera bazy danych](https://technet.microsoft.com/b12354bd-3143-4d1f-b5aa-450c4550653c)
