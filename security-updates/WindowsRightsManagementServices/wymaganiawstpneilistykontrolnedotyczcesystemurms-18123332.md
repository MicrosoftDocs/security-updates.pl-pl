---
TOCTitle: Wymagania wstępne i listy kontrolne dotyczące systemu RMS
Title: Wymagania wstępne i listy kontrolne dotyczące systemu RMS
ms:assetid: '836d96ef-d0fd-4935-b595-e8dec19cbb2b'
ms:contentKeyID: 18123332
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747582(v=WS.10)'
---

Wymagania wstępne i listy kontrolne dotyczące systemu RMS
=========================================================

Przed przystąpieniem do instalacji programu RMS należy zapoznać się z technologicznymi wymaganiami wstępnymi dotyczącymi korzystania z tego programu. Każda z wymienionych technologii jest integralną częścią programu RMS i poznanie podstawowych informacji na ich temat jest niezbędne do pomyślnego rozmieszczenia programu RMS. Dzięki poniższym listom kontrolnym można utworzyć listy zadań i plany rozmieszczania programu RMS i administrowania nim:

-   [Wymagania technologiczne](#bkmk_9)
-   [Listy kontrolne — rozmieszczanie programu RMS](#bkmk_10)
-   [Listy kontrolne — administrowanie programem RMS](#bkmk_14)

<span id="BKMK_9"></span>
Wymagania technologiczne
------------------------

W tym zestawie dokumentacji podano informacje pomocne w zrozumieniu działania programu Windows RMS, sposobu planowania i wykonywania rozmieszczania w organizacji oraz metod codziennego administrowania systemem. Założono, że użytkownik posiada wiedzę w następujących dziedzinach:

-   Rozmieszczanie i administrowanie systemem operacyjnym Windows Server 2003
-   Rozmieszczanie i administrowanie środowiskiem Active Directory
-   Rozmieszczanie i administrowanie programem Internetowe usługi informacyjne 6.0 firmy Microsoft® 6.0 (IIS)
-   Administrowanie oprogramowaniem Microsoft® SQL Server™ 2000
-   Podstawowe pojęcia dotyczące infrastruktury kluczy publicznych (PKI)
-   Praca sieciowa serwerów i zabezpieczenia

Aby uzyskać więcej informacji, zobacz „Zasoby dodatkowe” w części [Obsługa serwerów programu RMS](http://go.microsoft.com/fwlink/?linkid=42495) w tym zestawie dokumentacji.

<span id="BKMK_10"></span>
Listy kontrolne — rozmieszczanie programu RMS
---------------------------------------------

W tej części znajdują się listy kontrolne dotyczące następujących zadań rozmieszczania:

-   [Rozmieszczanie instalacji z jednym serwerem](#bkmk_11)
-   [Rozmieszczanie klastrów głównej certyfikacji i licencji](#bkmk_12)
-   [Rozmieszczanie programu RMS w wielu lasach](#bkmk_13)

Aby uzyskać więcej informacji dotyczących rozmieszczania programu RMS, zobacz [Rozmieszczanie systemu RMS](http://go.microsoft.com/fwlink/?linkid=42494) w tym zestawie dokumentacji.

<span id="BKMK_11"></span>
Rozmieszczanie instalacji z jednym serwerem
-------------------------------------------

Na podstawie poniższej listy kontrolnej można rozmieścić jeden serwer programu RMS.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Krok</th>
<th>Informacje dodatkowe</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Zapoznawanie się z pojęciami i informacjami planistycznymi.</td>
<td style="border:1px solid black;">„Przygotowanie do rozmieszczenia programu RMS” w części <a href="http://go.microsoft.com/fwlink/?linkid=42494">Rozmieszczanie systemu RMS</a>.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Przeglądanie wymagań systemowych w celu sprawdzenia, czy dostępny jest cały wymagany sprzęt i oprogramowanie.</td>
<td style="border:1px solid black;">„Wymagania wstępne dotyczące infrastruktury systemu RMS” w części <a href="http://go.microsoft.com/fwlink/?linkid=37537.">Planowanie rozmieszczenia programu RMS</a>
„Planowanie infrastruktury serwera bazy danych” w części <a href="http://go.microsoft.com/fwlink/?linkid=37537.">Planowanie rozmieszczenia programu RMS</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Konfigurowanie infrastruktury, obejmujące zależnie od sytuacji warunki wstępne dotyczące sprzętu i oprogramowania, konta administracyjne i obsługę zasad grup lub SMS.</td>
<td style="border:1px solid black;">„Przygotowanie do rozmieszczenia programu RMS” w części <a href="http://go.microsoft.com/fwlink/?linkid=42494.">Rozmieszczanie systemu RMS</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Instalowanie i konfigurowanie programu RMS na serwerze</td>
<td style="border:1px solid black;">„Konfigurowanie usług certyfikacji i licencjonowania na pierwszym serwerze” w części <a href="http://go.microsoft.com/fwlink/?linkid=42494.">Rozmieszczanie systemu RMS</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Testowanie rozmieszczenia.</td>
<td style="border:1px solid black;">„Konfigurowanie środowiska testowego” w części <a href="http://go.microsoft.com/fwlink/?linkid=42494.">Rozmieszczanie systemu RMS</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Implementowanie programu RMS w środowisku produkcyjnym</td>
<td style="border:1px solid black;">„Definiowanie zakresu implementacji programu RMS” w części <a href="http://go.microsoft.com/fwlink/?linkid=42494.">Rozmieszczanie systemu RMS</a></td>
</tr>
</tbody>
</table>
  
<span id="BKMK_12"></span>
Rozmieszczanie klastrów głównej certyfikacji i licencji  
-------------------------------------------------------
  
Na podstawie poniższej listy kontrolnej można rozmieścić klastry głównej certyfikacji i licencji.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Krok</th>
<th>Informacje dodatkowe</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Zapoznawanie się z pojęciami i informacjami planistycznymi.</td>
<td style="border:1px solid black;">„Przygotowanie do rozmieszczenia programu RMS” w części <a href="http://go.microsoft.com/fwlink/?linkid=42494.">Rozmieszczanie systemu RMS</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Przeglądanie wymagań systemowych w celu sprawdzenia, czy dostępny jest cały wymagany sprzęt i oprogramowanie.</td>
<td style="border:1px solid black;">„Wymagania wstępne dotyczące infrastruktury systemu RMS” w części <a href="http://go.microsoft.com/fwlink/?linkid=37537.">Planowanie rozmieszczenia programu RMS</a>
„Planowanie infrastruktury serwera bazy danych” w części <a href="http://go.microsoft.com/fwlink/?linkid=37537.">Planowanie rozmieszczenia programu RMS</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Przeglądanie planu rozmieszczenia w celu zorientowania się w topologii i składnikach przeznaczonych do instalacji.</td>
<td style="border:1px solid black;">„Określanie topologii systemu RMS” w części <a href="http://go.microsoft.com/fwlink/?linkid=37537.">Planowanie rozmieszczenia programu RMS</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Konfigurowanie infrastruktury, obejmujące zależnie od sytuacji warunki wstępne dotyczące sprzętu i oprogramowania, konta administracyjne i obsługę zasad grup lub SMS.</td>
<td style="border:1px solid black;">„Przygotowanie do rozmieszczenia programu RMS” w części <a href="http://go.microsoft.com/fwlink/?linkid=42494.">Rozmieszczanie systemu RMS</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Instalowanie i konfigurowanie programu RMS na serwerach wchodzących w skład klastra głównej certyfikacji</td>
<td style="border:1px solid black;">„Konfigurowanie usług certyfikacji i licencjonowania na pierwszym serwerze” w części <a href="http://go.microsoft.com/fwlink/?linkid=42494.">Rozmieszczanie systemu RMS</a>
„Dodawanie serwerów do obsługi certyfikacji i licencjonowania ” w części <a href="http://go.microsoft.com/fwlink/?linkid=42494.">Rozmieszczanie systemu RMS</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Instalowanie i konfigurowanie programu RMS na serwerach wchodzących w skład klastrów licencji</td>
<td style="border:1px solid black;">„Konfigurowanie usług certyfikacji i licencjonowania na pierwszym serwerze” w części <a href="http://go.microsoft.com/fwlink/?linkid=42494.">Rozmieszczanie systemu RMS</a>
„Dodawanie serwerów do obsługi certyfikacji i licencjonowania ” w części <a href="http://go.microsoft.com/fwlink/?linkid=42494.">Rozmieszczanie systemu RMS</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Konfigurowanie równoważenia obciążenia.</td>
<td style="border:1px solid black;">„Rozbudowa infrastruktury podstawowej w celu obsługi klastrowania” w części <a href="http://go.microsoft.com/fwlink/?linkid=42494.">Rozmieszczanie systemu RMS</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Testowanie rozmieszczenia.</td>
<td style="border:1px solid black;">„Konfigurowanie środowiska testowego” w części <a href="http://go.microsoft.com/fwlink/?linkid=42494.">Rozmieszczanie systemu RMS</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Implementowanie programu RMS w środowisku produkcyjnym</td>
<td style="border:1px solid black;">„Definiowanie zakresu implementacji programu RMS” w części <a href="http://go.microsoft.com/fwlink/?linkid=42494.">Rozmieszczanie systemu RMS</a></td>
</tr>
</tbody>
</table>
  
<span id="BKMK_13"></span>
Rozmieszczanie programu RMS w wielu lasach  
------------------------------------------
  
Na podstawie poniższej listy kontrolnej można rozmieścić główny program RMS w wielu lasach.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Krok</th>
<th>Informacje dodatkowe</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Zapoznawanie się z pojęciami i informacjami planistycznymi.</td>
<td style="border:1px solid black;">„Przygotowanie do rozmieszczenia programu RMS” w części <a href="http://go.microsoft.com/fwlink/?linkid=42494.">Rozmieszczanie systemu RMS</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Konfigurowanie wymaganych uprawnień na podstawie własnego modelu zaufania.</td>
<td style="border:1px solid black;">„Rozmieszczanie programu RMS w wielu lasach” w części <a href="http://go.microsoft.com/fwlink/?linkid=42494.">Rozmieszczanie systemu RMS</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Ustawienie odpowiednich atrybutów usługi Active Directory dla lasów.</td>
<td style="border:1px solid black;">„Rozmieszczanie programu RMS w wielu lasach” w części <a href="http://go.microsoft.com/fwlink/?linkid=42494.">Rozmieszczanie systemu RMS</a></td>
</tr>
</tbody>
</table>
  
<span id="BKMK_14"></span>
Listy kontrolne — administrowanie programem RMS  
-----------------------------------------------
  
W tej części znajdują się listy kontrolne dotyczące następujących zadań administracyjnych:
  
-   [Implementowanie szablonu zasad praw dostępu](#bkmk_15)  
-   [Rozmieszczanie nowego klienta programu RMS](#bkmk_16)  
-   [Dodawanie zaufanej domeny użytkownika](#bkmk_17)  
-   [Dodawanie zaufanej domeny publikacji](#bkmk_18)
  
Aby uzyskać więcej informacji dotyczących zarządzania programem RMS, zobacz [Obsługa serwerów programu RMS](http://go.microsoft.com/fwlink/?linkid=42495) w tym zestawie dokumentacji.
  
<span id="BKMK_15"></span>
Implementowanie szablonu zasad praw dostępu  
-------------------------------------------
  
Na podstawie poniższej listy kontrolnej można zaimplementować szablon zasad praw dostępu.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Krok</th>
<th>Informacje dodatkowe</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Zapoznawanie się z pojęciami związanymi z tematem.</td>
<td style="border:1px solid black;">„Szablony zasad praw dostępu” w części <a href="http://go.microsoft.com/fwlink/?linkid=42496.">Informacje techniczne dotyczące programu RMS</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Określanie lokalizacji szablonu zasad praw dostępu.</td>
<td style="border:1px solid black;">„Określanie lokalizacji szablonów zasad praw dostępu” w części <a href="http://go.microsoft.com/fwlink/?linkid=42495.">Obsługa serwerów programu RMS</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Tworzenie szablonu zasad praw dostępu.</td>
<td style="border:1px solid black;">„Tworzenie i modyfikowanie szablonów zasad praw dostępu” w części <a href="http://go.microsoft.com/fwlink/?linkid=42495.">Obsługa serwerów programu RMS</a>
„Dodawanie szablonu zasad praw dostępu” w części <a href="http://go.microsoft.com/fwlink/?linkid=42495.">Obsługa serwerów programu RMS</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Rozpowszechnianie szablonu zasad praw dostępu.</td>
<td style="border:1px solid black;">„Rozpowszechnianie szablonu zasad praw dostępu” w części <a href="http://go.microsoft.com/fwlink/?linkid=42495.">Obsługa serwerów programu RMS</a></td>
</tr>
</tbody>
</table>
  
<span id="BKMK_16"></span>
Rozmieszczanie nowego klienta programu RMS  
------------------------------------------
  
Na podstawie poniższej listy kontrolnej można rozmieścić nową wersję klienta programu RMS.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Krok</th>
<th>Informacje dodatkowe</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Zapoznawanie się z pojęciami związanymi z tematem.</td>
<td style="border:1px solid black;">„Planowanie rozpowszechniania do klientów” w części <a href="http://go.microsoft.com/fwlink/?linkid=42494.">Rozmieszczanie systemu RMS</a>
„Wykluczanie wersji skrytki” w części <a href="http://go.microsoft.com/fwlink/?linkid=42495.">Obsługa serwerów programu RMS</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Aby wymusić aktualizację do najnowszej wersji skrytki u wszystkich klientów, należy wykluczyć przestarzałą wersję skrytki.</td>
<td style="border:1px solid black;">„Wykluczanie wersji skrytek” w części <a href="http://go.microsoft.com/fwlink/?linkid=42495.">Obsługa serwerów programu RMS</a></td>
</tr>
</tbody>
</table>
  
<span id="BKMK_17"></span>
Dodawanie zaufanej domeny użytkownika  
-------------------------------------
  
Na podstawie poniższej listy kontrolnej można dodać zaufaną domenę użytkowników.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Krok</th>
<th>Informacje dodatkowe</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Zapoznawanie się z pojęciami związanymi z tematem.</td>
<td style="border:1px solid black;">„Zaufane domeny użytkowników” w części <a href="http://go.microsoft.com/fwlink/?linkid=42496.">Informacje techniczne dotyczące programu RMS</a>
„Dodawanie i usuwanie zaufanych domen użytkowników” w części <a href="http://go.microsoft.com/fwlink/?linkid=42495.">Obsługa serwerów programu RMS</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Uzyskanie certyfikatu licencjodawcy serwera z domeny użytkownika, która ma zostać dodana. (Musi ją dostarczyć administrator instalacji, której ma dotyczyć zaufanie.) Następnie dodanie danej domeny użytkowników do własnej instalacji.</td>
<td style="border:1px solid black;">„Dodawanie zaufanej domeny użytkownika” w części <a href="http://go.microsoft.com/fwlink/?linkid=42495.">Obsługa serwerów programu RMS</a></td>
</tr>
</tbody>
</table>
  
<span id="BKMK_18"></span>
Dodawanie zaufanej domeny publikacji  
------------------------------------
  
Na podstawie poniższej listy kontrolnej można dodać zaufaną domenę publikacji.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Krok</th>
<th>Informacje dodatkowe</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Zapoznawanie się z pojęciami związanymi z tematem.</td>
<td style="border:1px solid black;">„Zaufane domeny publikacji” w części <a href="http://go.microsoft.com/fwlink/?linkid=42496.">Informacje techniczne dotyczące programu RMS</a>
„Dodawanie i usuwanie zaufanych domen publikacji” w części <a href="http://go.microsoft.com/fwlink/?linkid=42495.">Obsługa serwerów programu RMS</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Uzyskanie szyfrowanego certyfikatu licencjodawcy serwera i klucza prywatnego domeny publikacji, która ma zostać dodana, a następnie dodanie tej domeny publikacji do własnej instalacji.</td>
<td style="border:1px solid black;">„Dodawanie zaufanej domeny publikacji” w części <a href="http://go.microsoft.com/fwlink/?linkid=42495.">Obsługa serwerów programu RMS</a></td>
</tr>
</tbody>
</table>
