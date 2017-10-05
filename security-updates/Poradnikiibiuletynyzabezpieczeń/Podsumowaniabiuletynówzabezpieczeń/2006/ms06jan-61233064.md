---
TOCTitle: 'MS06-JAN'
Title: Microsoft Security Bulletin Summary for styczeń 2006
ms:assetid: 'ms06-jan'
ms:contentKeyID: 61233064
ms:mtpsurl: 'https://technet.microsoft.com/pl-PL/library/ms06-jan(v=Security.10)'
---

Security Bulletin Summary

Microsoft Security Bulletin Summary for styczeń 2006
====================================================

Opublikowano: 5 stycznia 2006 | Zaktualizowano: 10 stycznia 2006

**Wersja:** 1.0

Wersja użytkownika końcowego tego biuletynu jest dostępna w następującej [witrynie sieci Web](http://www.microsoft.com/poland/security/).

**Chroń swój komputer:** Informacje dotyczące ochrony komputera firma Microsoft udostępnia w następujących lokalizacjach:

-   Użytkownicy końcowi mogą odwiedzić witrynę sieci Web [Chroń swój komputer](http://www.microsoft.com/poland/athome/security/protect/windowsxpsp2/default.mspx).
-   Specjaliści IT mogą odwiedzić witrynę sieci Web [Security Guidance Center](http://www.microsoft.com/poland/technet/security/) (centrum porad w zakresie bezpieczeństwa).

**Strategie zarządzania aktualizacjami:** W witrynie sieci Web [Zarządzanie poprawkami, aktualizacje bezpieczeństwa i pobieranie (j.ang.)](http://go.microsoft.com/fwlink/?linkid=21168) znajdują się dodatkowe informacje o metodach działania firmy Microsoft i zaleceniach dotyczących stosowania aktualizacji bezpieczeństwa.

**Witryna wspólnoty specjalistów branży IT w dziedzinie zabezpieczeń:** Dowiedz się, jak można poprawić bezpieczeństwo i zoptymalizować infrastrukturę informatyczną oraz weź udział w dyskusjach dotyczących zabezpieczeń wraz z innymi specjalistami branży IT, odwiedzając witrynę sieci Web [IT Pro Security Zone (Strefa zabezpieczeń dla specjalistów branży IT) (j.ang.)](http://go.microsoft.com/fwlink/?linkid=21164).

**Usługa powiadamiania o zabezpieczeniach firmy Microsoft:** Aby otrzymywać automatyczne powiadomienia pocztą e-mail o każdym wydaniu biuletynu zabezpieczeń firmy Microsoft, dokonaj subskrypcji usługi [Microsoft Security Notification Service (j.ang.)](http://go.microsoft.com/fwlink/?linkid=21163).

#### Streszczenie

Ten biuletyn obejmuje aktualizacje eliminujące nowo odkryte usterki. Poniżej przedstawiono te usterki z uwzględnieniem poziomu ważności:

Krytyczny (3)
-------------

<span></span>
| Identyfikator biuletynu               | Biuletyn zabezpieczeń firmy Microsoft MS06-001                                                                                                      |
|---------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**                   | [**Usterki silnika renderującego mogą pozwolić na zdalne wykonanie kodu (912919)**](http://technet.microsoft.com/security/bulletin/ms06-001)        |
| **Streszczenie**                      | Istniejąca usterka silnika renderującego może umożliwić zdalne wykonanie kodu.                                                                      |
| **Maksymalny wskaźnik ważności**      | [Krytyczny](http://technet.microsoft.com/security/bulletin/rating)                                                                                  |
| **Wpływ usterki**                     | Zdalne wykonanie kodu                                                                                                                               |
| **Programy, których dotyczy problem** | **System Windows**. Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki. |

| Identyfikator biuletynu               | Biuletyn zabezpieczeń firmy Microsoft MS06-002                                                                                                                         |
|---------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**                   | [**Usterka związana z osadzonymi czcionkami witryn sieci Web może umożliwić zdalne wykonanie kodu (908519)**](http://technet.microsoft.com/security/bulletin/ms06-002) |
| **Streszczenie**                      | Podczas wyświetlania osadzonych czcionek witryn sieci Web może dojść do zdalnego wykonania kodu.                                                                       |
| **Maksymalny wskaźnik ważności**      | [Krytyczny](http://technet.microsoft.com/security/bulletin/rating)                                                                                                     |
| **Wpływ usterki**                     | Zdalne wykonanie kodu                                                                                                                                                  |
| **Programy, których dotyczy problem** | **System Windows**. Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                    |

| Identyfikator biuletynu               | Biuletyn zabezpieczeń firmy Microsoft MS06-003                                                                                                                                                            |
|---------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**                   | [**Usterka dekodowania formatu TNEF w programach Microsoft Outlook i Microsoft Exchange potencjalnie umożliwia zdalne wykonanie kodu (902412)**](http://technet.microsoft.com/security/bulletin/ms06-003) |
| **Streszczenie**                      | W wiadomościach w formacie TNEF istnieje usterka, która umożliwia zdalne wykonanie kodu.                                                                                                                  |
| **Maksymalny wskaźnik ważności**      | [Krytyczny](http://technet.microsoft.com/security/bulletin/rating)                                                                                                                                        |
| **Wpływ usterki**                     | Zdalne wykonanie kodu                                                                                                                                                                                     |
| **Programy, których dotyczy problem** | **Exchange i Office.** Więcej informacji można znaleźć w częściach: Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki.                                                    |

Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki
---------------------------------------------------------------------------------

<span></span>
**W jaki sposób korzystać z tej tabeli?**

Tabela ta pozwala odczytać informacje o aktualizacjach zabezpieczeń, których zainstalowanie może być konieczne. Należy przejrzeć informacje dla każdego wymienionego programu lub składnika oprogramowania w celu sprawdzenia, czy są wymagane aktualizacje zabezpieczeń. Dla każdego programu lub składnika oprogramowania wymienionego na liście podany jest wpływ usterki oraz hiperłącze do dostępnej aktualizacji oprogramowania.

Podana w tabeli liczba w nawiasach kwadratowych \[x\] wskazuje, że dostępna jest uwaga bardziej szczegółowo opisująca problem. Uwagi takie znajdują się u dołu tabeli.

**Uwaga:** Jedna usterka może wymagać zainstalowania kilku aktualizacji zabezpieczeń. Aktualizacje, które należy zainstalować, gdy w systemie są zainstalowane określone programy lub składniki, można sprawdzić, przeglądając całą kolumnę w tabeli podsumowującej dla biuletynu o określonym identyfikatorze.

**Programy, których dotyczy problem, i lokalizacje, z których można pobrać poprawki**

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" ></th>
<th style="border:1px solid black;" >Szczegóły        </th>
<th style="border:1px solid black;" >Szczegóły        </th>
<th style="border:1px solid black;" >Szczegóły        </th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Identyfikator biuletynu</strong></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms06-001"><strong>MS06-001</strong></a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms06-002"><strong>MS06-002</strong></a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms06-003"><strong>MS06-003</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Maksymalny wskaźnik ważności</strong></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/rating"><strong>Krytyczny</strong></a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/rating"><strong>Krytyczny</strong></a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/rating"><strong>Krytyczny</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Programy systemu Windows, których dotyczy problem:</strong></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows Server 2003</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=1584aae0-51ce-47d6-9a03-db5b9077f1f2&amp;displaylang=pl">Krytyczny</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=5fc12654-486f-45bf-8d34-bdf0998869c5&amp;displaylang=pl">Krytyczny</a></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Server 2003 z dodatkiem Service Pack 1</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=1584aae0-51ce-47d6-9a03-db5b9077f1f2&amp;displaylang=pl">Krytyczny</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=5fc12654-486f-45bf-8d34-bdf0998869c5&amp;displaylang=pl">Krytyczny</a></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows Server 2003 x64 Edition</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=a8f4dcba-5d28-4d9d-a6a4-3b71108cfe2d">Krytyczny (j.ang.)</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=80b05c56-5bce-4262-8142-af0d8a7bc388">Krytyczny (j.ang.)</a></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Server 2003 dla systemów z procesorem Itanium</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=6e372d41-2c16-415e-8306-a5ca8845cc09">Krytyczny (j.ang.)</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=e39d2e29-8934-4aa1-844d-11efa57d9cc5">Krytyczny (j.ang.)</a></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows Server 2003 z dodatkiem SP1 dla systemów z procesorem Itanium</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=6e372d41-2c16-415e-8306-a5ca8845cc09">Krytyczny (j.ang.)</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=e39d2e29-8934-4aa1-844d-11efa57d9cc5">Krytyczny (j.ang.)</a></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Windows XP z dodatkiem Service Pack 1</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=0c1b4c96-57ae-499e-b89b-215b7bb4d8e9&amp;displaylang=pl">Krytyczny</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=6daea2af-3723-4cdf-b5bd-b21ac75b5243&amp;displaylang=pl">Krytyczny</a></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft Windows XP z dodatkiem Service Pack 2</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=0c1b4c96-57ae-499e-b89b-215b7bb4d8e9&amp;displaylang=pl">Krytyczny</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=6daea2af-3723-4cdf-b5bd-b21ac75b5243&amp;displaylang=pl">Krytyczny</a></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Windows XP Professional x64 Edition</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=1990b2cf-ae88-4849-aeab-3f833969e197">Krytyczny (j.ang.)</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=3a1166e6-5e9e-4e73-bcd4-28eca6ece877">Krytyczny (j.ang.)</a></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows 2000 Service Pack 4</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=dc6c2fe8-3c81-4661-994b-4146775bf590&amp;displaylang=pl">Krytyczny</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=aa9e27bd-cb9a-4ef1-92a3-00ffe7b2ac74&amp;displaylang=pl">Krytyczny</a></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Millennium Edition (Windows Me)</td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><strong>[1]</strong></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows 98 Second Edition (SE)</td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><strong>[1]</strong></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows 98</td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><strong>[1]</strong></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Oprogramowanie pakietu Office, którego dotyczy problem:</strong></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Office Outlook 2000</td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=64d0336d-f962-4ab1-a724-9f6ba2108cb9&amp;displaylang=pl">Krytyczny</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Office Outlook 2002</td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=9a85cebb-0d9a-465d-a4bc-af501562772d&amp;displaylang=pl">Krytyczny</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Office Outlook 2003</td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=1d156043-b041-4305-8442-3c4e3b832788&amp;displaylang=pl">Krytyczny</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Pakiety wielojęzyczne dla pakietu Office 2000 </td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=2c0fa7c7-91aa-49b4-9731-9e83e3e0823d&amp;displaylang=pl">Krytyczny</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Pakiety wielojęzycznego interfejsu użytkownika Office XP</td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=cca9399a-6da3-4163-8398-c58dc328182b&amp;displaylang=pl">Krytyczny</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Pakiety wielojęzycznego interfejsu użytkownika Office 2003</td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=d69554ad-196f-4789-91e5-b2a753eed854&amp;displaylang=pl">Krytyczny</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Podlegające oprogramowanie Exchange:</strong></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Exchange 5.0</td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=0a8df1c3-abf9-4a21-9b49-81fa362b251f">Krytyczny (j.ang.)</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Exchange 5.5</td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=ec6bd30e-12de-4ca1-9432-d2e73af62427">Krytyczny (j.ang.)</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Exchange 2000</td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=372ff07f-c3ca-4301-8559-9b90344edc02">Krytyczny (j.ang.)</a></td>
</tr>
</tbody>
</table>
  
**Uwagi**
  
**<sup>[1]</sup>** Krytyczne aktualizacje zabezpieczeń dla tych platform są dostępne w ramach niniejszego biuletynu zabezpieczeń i można je pobrać z witryny sieci Web Windows Update.
  
Wdrażanie  
---------
  
<span></span>
**Usługi Software Update Services:**
  
Usługi Microsoft Software Update Services (SUS) umożliwiają administratorom szybkie i niezawodne wdrażanie najnowszych aktualizacji krytycznych i aktualizacji zabezpieczeń na serwerach działających w systemach Windows 2000 oraz Windows Server 2003, a także na komputerach stacjonarnych z systemami Windows 2000 Professional lub Windows XP Professional.
  
Więcej informacji na temat sposobu wdrażania tej aktualizacji zabezpieczeń za pomocą usług Software Update Services można znaleźć w [witrynie sieci Web usług Software Update Services (j.ang.)](http://go.microsoft.com/fwlink/?linkid=21133).
  
**Windows Server Update Services:**
  
Korzystając z programu Windows Server Update Services (WSUS), administratorzy mogą szybko i niezawodnie wdrożyć najnowsze aktualizacje krytyczne i aktualizacje zabezpieczeń przeznaczonych dla systemu operacyjnego Windows 2000 i nowszych, pakietu Office XP i nowszych, programu Exchange Server 2003 oraz SQL Server 2000 w systemie operacyjnym Windows 2000 i nowszych.
  
Więcej informacji na temat sposobu wdrażania tej aktualizacji zabezpieczeń za pomocą programu Windows Server Update Services można znaleźć w [witrynie sieci Web programu Windows Server Update Services (j.ang.)](http://go.microsoft.com/fwlink/?linkid=50120).
  
**Systems Management Server:**
  
Program Systems Management Server (SMS) jest przeznaczonym dla przedsiębiorstw i w znacznym stopniu konfigurowalnym rozwiązaniem służącym do zarządzania aktualizacjami. Program SMS umożliwia administratorom znalezienie komputerów z systemem Windows, na których należy zainstalować aktualizację zabezpieczeń, a także przeprowadzić kontrolowane wdrożenie tych aktualizacji w całym przedsiębiorstwie, w minimalnym stopniu zakłócając przy tym pracę użytkowników końcowych. Więcej informacji na temat możliwości wykorzystania przez administratorów programu SMS 2003 do wdrażania aktualizacji zabezpieczeń można znaleźć w witrynie sieci Web [zarządzania poprawkami zabezpieczeń programu SMS 2003 (j.ang.)](http://go.microsoft.com/fwlink/?linkid=22939). Użytkownicy programu SMS 2.0 mogą także skorzystać z dodatku [Software Updates Service Feature Pack (j.ang.)](http://go.microsoft.com/fwlink/?linkid=33340) ułatwiającego wdrożenie aktualizacji zabezpieczeń. Więcej informacji na temat programu SMS można znaleźć w [witrynie sieci Web programu SMS (j.ang.)](http://go.microsoft.com/fwlink/?linkid=21158).
  
**Uwaga:** Program SMS zapewnia obsługę rozwiązań zawartych w biuletynach zabezpieczeń dzięki narzędziom Microsoft Baseline Security Analyzer oraz Microsoft Office Detection Tool. Narzędzia te mogą nie wykrywać wszystkich aktualizacji oprogramowania. W takich przypadkach administratorzy mogą wykorzystywać dostępne w programie SMS funkcje zarządzania zasobami do przyporządkowania poszczególnych aktualizacji określonym systemom. Więcej informacji na temat takiej procedury można znaleźć w poniższej [witrynie sieci Web (j.ang.)](http://go.microsoft.com/fwlink/?linkid=33341). Niektóre aktualizacje oprogramowania wymagają od użytkownika uprawnień administratora po ponownym uruchomieniu systemu. Do zainstalowania tych aktualizacji administratorzy mogą użyć narzędzia Elevated Rights Deployment Tool (dostępnego w dodatkach [SMS 2003 Administration Feature Pack (j.ang.)](http://go.microsoft.com/fwlink/?linkid=33387) oraz [SMS 2.0 Administration Feature Pack (j.ang.)](http://go.microsoft.com/fwlink/?linkid=21161)).
  
**Narzędzia QChain.exe i Update.exe:**
  
Firma Microsoft opublikowała narzędzie QChain.exe, które jest uruchamiane w wierszu polecenia i umożliwia administratorom systemu bezpieczne łączenie aktualizacji zabezpieczeń. *Instalacja łańcuchowa* polega na instalowaniu wielu aktualizacji jedna po drugiej, bez ponownego uruchamiania komputera po każdej z nich. Program Update.exe, wykorzystywany w aktualizacjach opisanych w niniejszym poradniku, posiada wbudowaną funkcję instalacji łańcuchowej. Klienci korzystający z systemu Windows 2000 z dodatkiem Service Pack 2 lub nowszym, z systemu Windows XP lub systemu Windows Server 2003, nie wymagają narzędzia Qchain.exe do łańcuchowej instalacji tych aktualizacji. Narzędzie Qchain.exe nadal obsługuje instalację łańcuchową tych aktualizacji systemu Windows, dzięki czemu administrator może utworzyć skrypt w celu spójnego wdrożenia aktualizacji na wszystkich platformach. Więcej informacji o programie Qchain znajduje się w [witrynie sieci Web (j.ang.)](http://go.microsoft.com/fwlink/?linkid=21156).
  
**Narzędzie Microsoft Baseline Security Analyzer:**
  
Narzędzie Microsoft Baseline Security Analyzer umożliwia administratorom skanowanie lokalnych i zdalnych systemów w poszukiwaniu brakujących aktualizacji zabezpieczeń oraz typowych błędów konfiguracji zabezpieczeń. [Więcej informacji na temat narzędzia MBSA można znaleźć w witrynie sieci Web](http://www.microsoft.com/poland/technet/security/tools/mbsa.mspx)Microsoft Baseline Security Analyzer.
  
**Porady dotyczące wykrywania i wdrażania:**
  
Firma Microsoft opublikowała porady dotyczące wykrywania i wdrażania, odnoszące się do aktualizacji zabezpieczeń udostępnionych w tym miesiącu. Porady te będą również pomocne dla informatyków, wyjaśniając jak mogą oni wdrażać aktualizacje za pomocą różnych narzędzi, takich jak Windows Update, Microsoft Update, Office Update, Microsoft Baseline Security Analyzer (MBSA), Office Detection Tool, Microsoft Systems Management Server (SMS), Extended Security Update Inventory Tool i Enterprise Update Scan Tool (EST). Więcej informacji na ten temat można znaleźć w [artykule 910723 bazy wiedzy Microsoft Knowledge Base](http://support.microsoft.com/kb/910723).
  
#### Inne informacje:
  
**Podziękowania**
  
Firma Microsoft [dziękuje (j.ang.)](http://go.microsoft.com/fwlink/?linkid=21127) wymienionym poniżej organizacjom i osobom za współpracę w dziedzinie ochrony klientów:
  
-   Dan Hubbard z firmy [WebSense (j.ang.)](http://websense.com/) za współpracę przy rozwiązaniu problemu opisanego w biuletynie [MS06-001](http://technet.microsoft.com/security/bulletin/ms06-001).  
-   Firmie eEye Digital Security za zgłoszenie usterki opisanej w biuletynie [MS06-002](http://technet.microsoft.com/security/bulletin/ms06-002).  
-   Johnowi Heasmanowi i Markowi Litchfieldowi z [NGS Software (j.ang.)](http://www.ngssoftware.com/index.htm) za zgłoszenie usterki opisanej w biuletynie [MS06-003](http://technet.microsoft.com/security/bulletin/ms06-003).
  
**Uzyskiwanie innych aktualizacji zabezpieczeń:**
  
Aktualizacje dotyczące innych problemów związanych z zabezpieczeniami można uzyskać w następujących lokalizacjach:
  
-   Aktualizacje zabezpieczeń są dostępne w [Centrum pobierania firmy Microsoft](http://www.microsoft.com/downloads/results.aspx?freetext=poprawka+zabezpiecze%c5%84&productid=&displaylang=pl). Najłatwiej je znaleźć, przeprowadzając wyszukiwanie wyrażenia „poprawka zabezpieczeń”.  
-   Aktualizacje dla poszczególnych platform są dostępne w [witrynie sieci Web Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747).
  
**Pomoc techniczna:**
  
-   Klienci mogą uzyskać pomoc techniczną w [Biurze Obsługi Klienta Microsoft](http://go.microsoft.com/fwlink/?linkid=21131) pod numerem 0 801 802 000 (Opłata według stawek Twojego operatora) lub (0-22) 594 19 99 w godzinach od 9:00 do 17:00, od poniedziałku do piątku. Połączenia z działem pomocy technicznej związane z aktualizacjami zabezpieczeń są bezpłatne.  
-   Klienci międzynarodowi mogą uzyskać pomoc w lokalnych przedstawicielstwach firmy Microsoft. Pomoc techniczna związana z aktualizacjami zabezpieczeń jest bezpłatna. Informacje o sposobie kontaktowania się z pomocą techniczną firmy Microsoft są dostępne w [międzynarodowej witrynie sieci Web pomocy technicznej (j.ang.)](http://go.microsoft.com/fwlink/?linkid=21155).
  
**Zasoby zabezpieczeń:**
  
-   Witryna sieci Web [Microsoft TechNet Security](http://www.microsoft.com/poland/technet/security/) zawiera dodatkowe informacje na temat zabezpieczeń w produktach firmy Microsoft.  
-   [Usługi Microsoft Software Update Services (j.ang.)](http://go.microsoft.com/fwlink/?linkid=21133)  
-   [Microsoft Windows Server Update Services (j.ang.)](http://go.microsoft.com/fwlink/?linkid=50120)  
-   [Narzędzie Microsoft Baseline Security Analyzer](http://www.microsoft.com/poland/technet/security/tools/mbsa.mspx) (MBSA)  
-   [Microsoft Update](http://update.microsoft.com/microsoftupdate)  
-   [Witryna Windows Update](http://go.microsoft.com/fwlink/?linkid=21130)  
-   Wykaz Windows Update. Więcej informacji na temat Wykazu Windows Update można znaleźć w [artykule 323166 bazy wiedzy Microsoft Knowledge Base](http://support.microsoft.com/kb/323166).  
-   [Witryna Office Update](http://go.microsoft.com/fwlink/?linkid=21135)
  
**Zrzeczenie odpowiedzialności:**
  
Informacje w bazie wiedzy Microsoft Knowledge Base są dostarczane „tak jak są” bez jakiejkolwiek gwarancji. Firma Microsoft odrzuca wszelkie gwarancje, wyraźne i dorozumiane, w tym gwarancje dotyczące wartości handlowej i przydatności do określonego celu. Firma Microsoft Corporation ani jej dostawcy w żadnym wypadku nie ponoszą odpowiedzialności za jakiekolwiek szkody, w tym bezpośrednie, pośrednie, przypadkowe, wynikowe, utratę zysków handlowych lub szkody specjalne, nawet jeżeli firmę Microsoft Corporation lub jej dostawców powiadomiono o możliwości zaistnienia takich szkód. W niektórych stanach wyłączenie lub ograniczenie odpowiedzialności za straty wynikowe lub przypadkowe, a więc i powyższe ograniczenia, nie mają zastosowania.
  
**Wersje:**
  
-   Wersja 1.0 (5 stycznia 2006): Opublikowano biuletyn.  
-   Wersja 2.0 (10 stycznia 2006 r.): Zaktualizowano o dodatkowe biuletyny zabezpieczeń firmy Microsoft
  
*Built at 2014-04-18T01:50:00Z-07:00*
