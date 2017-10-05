---
TOCTitle: 'MS04-JUN'
Title: Microsoft Security Bulletin Summary for czerwiec 2004
ms:assetid: 'ms04-jun'
ms:contentKeyID: 61233046
ms:mtpsurl: 'https://technet.microsoft.com/pl-PL/library/ms04-jun(v=Security.10)'
---

Security Bulletin Summary

Microsoft Security Bulletin Summary for czerwiec 2004
=====================================================

Opublikowano: 8 czerwca 2004

**Wersja:** 1.0

**Opublikowano:** 8 czerwca 2004 r.
**Numer wersji:** 1.0

Wersja użytkownika końcowego tego biuletynu jest dostępna w następującej [witrynie sieci Web (j.ang.)](http://go.microsoft.com/fwlink/?linkid=28529).

**Chroń swój komputer:** Informacje dotyczące ochrony komputera firma Microsoft udostępnia w następujących lokalizacjach:

-   Użytkownicy końcowi mogą odwiedzić witrynę sieci Web [Chroń swój komputer](http://go.microsoft.com/fwlink/?linkid=21169).
-   Specjaliści branży IT mogą odwiedzić witrynę sieci Web [centrum pomocy dotyczącej zabezpieczeń](http://go.microsoft.com/fwlink/?linkid=21171).

**Strategie zarządzania aktualizacjami:** W witrynie sieci Web dotyczącej [zarządzania poprawkami, aktualizacji zabezpieczeń i pobierania](http://go.microsoft.com/fwlink/?linkid=21168) można znaleźć dodatkowe informacje o zalecanych przez firmę Microsoft najlepszych sposobach stosowania poprawek zabezpieczeń.

**Witryna wspólnoty specjalistów branży IT w dziedzinie zabezpieczeń:** Dowiedz się, jak można poprawić bezpieczeństwo i zoptymalizować infrastrukturę informatyczną oraz weź udział wraz z innymi specjalistami branży IT w dyskusjach dotyczących zabezpieczeń, odwiedzając witrynę sieci Web [IT Pro Security Zone](http://go.microsoft.com/fwlink/?linkid=21164).

**Usługa powiadamiania o zabezpieczeniach firmy Microsoft:** Aby otrzymywać automatyczne powiadomienia pocztą e-mail o każdym wydaniu biuletynu zabezpieczeń firmy Microsoft, zasubskrybuj [usługę powiadamiania o zabezpieczeniach firmy Microsoft](http://go.microsoft.com/fwlink/?linkid=21163).

#### Streszczenie

Ten biuletyn obejmuje aktualizacje eliminujące nowo odkryte usterki. Poniżej przedstawiono te usterki z uwzględnieniem poziomu ważności:

Średni (2)
----------

<span></span>

| Identyfikator biuletynu          | Biuletyn zabezpieczeń firmy Microsoft MS04-016                                                                                                                              |
|----------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**              | [**Usterka programu DirectPlay umożliwia odmowę usługi (839643)**](http://technet.microsoft.com/security/bulletin/ms04-016)                                                 |
| **Podsumowanie**                 | Usterka typu odmowa usługi istnieje w interfejsie API IDirectPlay4 programu Microsoft DirectPlay ze względu na brak niezawodnej procedury sprawdzania poprawności pakietów. |
| **Maksymalny wskaźnik ważności** | [Średni](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                      |
| **Wpływ usterki**                | Odmowa usługi                                                                                                                                                               |
| **Podlegające oprogramowanie**   | **System Windows**. Więcej informacji zawiera sekcja Podlegające oprogramowanie i lokalizacje, z których można pobrać poprawki.                                             |

| Identyfikator biuletynu          | Biuletyn zabezpieczeń firmy Microsoft MS04-017                                                                                                                                                                                     |
|----------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tytuł biuletynu**              | [**Usterka składnika Web Form Viewer programu Crystal Reports może pozwolić na ujawnienie informacji i odmowę usługi (842689)**](http://technet.microsoft.com/security/bulletin/ms04-017)                                          |
| **Podsumowanie**                 | W programach Crystal Reports i Crystal Enterprise firmy Business Objects istnieje usterka dostępu do katalogu, która umożliwia w systemie podlegającym usterce ataki prowadzące do ujawnienia informacji lub odmowy usługi.        |
| **Maksymalny wskaźnik ważności** | [Średni](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                             |
| **Wpływ usterki**                | Ujawnienie informacji i odmowa usługi                                                                                                                                                                                              |
| **Podlegające oprogramowanie**   | **Visual Studio .NET 2003, Outlook 2003 z dodatkiem Business Contact Manager, Microsoft Business Solutions CRM 1.2.**. Więcej informacji zawiera sekcja Podlegające oprogramowanie i lokalizacje, z których można pobrać poprawki. |

Podlegające oprogramowanie i lokalizacje, z których można pobrać poprawki
-------------------------------------------------------------------------

<span></span>

**W jaki sposób należy korzystać z tej tabeli?**

Z tabeli tej należy odczytać informacje o poprawkach zabezpieczeń, których zainstalowanie może być potrzebne. Należy przejrzeć informacje dla każdego wymienionego programu lub składnika oprogramowania w celu sprawdzenia, czy wymagane są aktualizacje zabezpieczeń. Dla każdego podanego na liście programu lub składnika oprogramowania podany jest wpływ usterki oraz hiperłącze do dostępnej aktualizacji oprogramowania.

Występujące w tabeli liczby w nawiasach \[x\] wskazują, że istnieje uwaga szczegółowo wyjaśniająca dany problem. Uwagi znajdują się u dołu tabeli.

**Uwaga** Dla jednej usterki może być potrzebne zainstalowanie kilku aktualizacji zabezpieczeń. Należy przyjrzeć całą kolumnę dla każdego wymienionego identyfikatora biuletynu w celu sprawdzenia, które aktualizacje trzeba zainstalować ze względu na programy lub składniki zainstalowane w danym systemie.

Na przykład w biuletynie zabezpieczeń **MS04-017** omówiono kilka aktualizacji zabezpieczeń, które mogą być wymagane zależnie od tego, jakie podlegające oprogramowanie i składniki są zainstalowane w systemie.

**Podlegające oprogramowanie i lokalizacje, z których można pobrać poprawki**

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" ></th>
<th style="border:1px solid black;" >Szczegóły        </th>
<th style="border:1px solid black;" >Szczegóły        </th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Identyfikator biuletynu</strong></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms04-016"><strong>MS04-016</strong></a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms04-017"><strong>MS04-017</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Maksymalny wskaźnik ważności</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Średni</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Krytyczny</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Podlegające oprogramowanie systemu Windows:</strong></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows Server™ 2003</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=7f1713fc-f95c-43e5-b825-3cf72c1a0a3e&amp;displaylang=en">Średni</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=00b24cdc-4e4e-4ae1-9b36-7ce23e397f0f&amp;displaylang=en">Krytyczny</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Server 2003 w wydaniu 64-bitowym</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=7f1713fc-f95c-43e5-b825-3cf72c1a0a3e&amp;displaylang=en">Średni</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=49d6e1c6-aeb0-4ce7-8d25-58a7db99c1de&amp;displaylang=en">Krytyczny</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows XP</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=7f1713fc-f95c-43e5-b825-3cf72c1a0a3e&amp;displaylang=en">Średni</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=3666222f-ca61-4726-bb8a-764cd824dcf0&amp;displaylang=en">Krytyczny</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows XP z dodatkiem Service Pack 1</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=7f1713fc-f95c-43e5-b825-3cf72c1a0a3e&amp;displaylang=en">Średni</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=3666222f-ca61-4726-bb8a-764cd824dcf0&amp;displaylang=en">Krytyczny</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">System operacyjny Windows XP w wydaniu 64-bitowym, wersja 2003</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=7f1713fc-f95c-43e5-b825-3cf72c1a0a3e&amp;displaylang=en">Średni</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=49d6e1c6-aeb0-4ce7-8d25-58a7db99c1de&amp;displaylang=en">Krytyczny</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">System operacyjny Windows XP w wydaniu 64-bitowym z dodatkiem Service Pack 1</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=7f1713fc-f95c-43e5-b825-3cf72c1a0a3e&amp;displaylang=en">Średni</a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=ab25bfdd-77a0-4615-aa80-efbd63855900&amp;displaylang=en">Krytyczny</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows 2000 z dodatkiem Service Pack 2</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=7f1713fc-f95c-43e5-b825-3cf72c1a0a3e&amp;displaylang=en">Średni</a></td>
<td style="border:1px solid black;"><strong>[1]</strong></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows 2000 z dodatkiem Service Pack 3</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=7f1713fc-f95c-43e5-b825-3cf72c1a0a3e&amp;displaylang=en">Średni</a></td>
<td style="border:1px solid black;"><strong>[1]</strong></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows 2000 z dodatkiem Service Pack 4</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=7f1713fc-f95c-43e5-b825-3cf72c1a0a3e&amp;displaylang=en">Średni</a></td>
<td style="border:1px solid black;"><strong>[1]</strong></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows NT® Workstation 4.0 z dodatkiem Service Pack 6a</td>
<td style="border:1px solid black;"><strong>[1]</strong></td>
<td style="border:1px solid black;"><strong>[1]</strong></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows NT Server 4.0 z dodatkiem Service Pack 6a</td>
<td style="border:1px solid black;"><strong>[1]</strong></td>
<td style="border:1px solid black;"><strong>[1]</strong></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows NT Server 4.0 Terminal Server Edition z dodatkiem Service Pack 6</td>
<td style="border:1px solid black;"><strong>[1]</strong></td>
<td style="border:1px solid black;"><strong>[1]</strong></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows Millennium Edition (Me)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=7f1713fc-f95c-43e5-b825-3cf72c1a0a3e&amp;displaylang=en">Średni</a></td>
<td style="border:1px solid black;"><strong>[1]</strong></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows 98 Second Edition (SE)</td>
<td style="border:1px solid black;"><strong>[1]</strong></td>
<td style="border:1px solid black;"><strong>[1]</strong></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows 98</td>
<td style="border:1px solid black;"><strong>[1]</strong></td>
<td style="border:1px solid black;"><strong>[1]</strong></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Podlegające składniki systemu operacyjnego Windows:</strong></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft .NET Framework wersja 1.0</td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=7f1713fc-f95c-43e5-b825-3cf72c1a0a3e&amp;displaylang=en">Krytyczny</a> <strong>[2]</strong></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft .NET Framework wersja 1.1</td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=7f1713fc-f95c-43e5-b825-3cf72c1a0a3e&amp;displaylang=en">Krytyczny</a> <strong>[2]</strong></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Internet Explorer 6 z dodatkiem Service Pack 1</td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=7f1713fc-f95c-43e5-b825-3cf72c1a0a3e&amp;displaylang=en">Krytyczny</a><strong>[2]</strong></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Direct X (wersja 7.0 i nowsze)</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=27992">Średni</a></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Podlegające oprogramowanie pakietu Office:</strong></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Office System 2003 (wszystkie wersje i produkty<br />
zawarte w pakiecie Office System 2003)</td>
<td style="border:1px solid black;"><strong> </strong></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=106bcf99-1ba9-4035-94c5-2a7fa90e5971&amp;displaylang=en">Krytyczny</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Office XP z dodatkiem Service Pack 3 (wszystkie wersje i produkty<br />
zawarte w pakiecie Office XP)</td>
<td style="border:1px solid black;"><strong> </strong></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=7d128614-6d34-49df-8d63-6c17e9a2d312&amp;displaylang=en">Krytyczny</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Visio 2003 (wszystkie wersje)</td>
<td style="border:1px solid black;"><strong> </strong></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=c07d40a5-6f87-4d50-9640-34ffd2f189e1&amp;displaylang=en">Ważny</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Visio 2002 z dodatkiem Service Pack 2 (wszystkie wersje)</td>
<td style="border:1px solid black;"><strong> </strong></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=16c2dffd-7b73-43c4-ab0d-2b5efc80eb63&amp;displaylang=en">Ważny</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Project 2003 (wszystkie wersje)</td>
<td style="border:1px solid black;"><strong> </strong></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=9e37b6b0-a028-47ea-8fa1-3705877a2908&amp;displaylang=en">Ważny</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Project 2002 z dodatkiem Service Pack 1 (wszystkie wersje)</td>
<td style="border:1px solid black;"><strong> </strong></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=b3ebccea-b0e4-41c7-a6f4-413864d2ccf3&amp;displaylang=en">Ważny</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Outlook 2003 z dodatkiem Business Contact Manager</td>
<td style="border:1px solid black;"><strong> </strong></td>
<td style="border:1px solid black;"><strong> </strong></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong> </strong>
<strong>Podlegające narzędzia programistyczne i platformy .NET:</strong></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Visual Studio .NET 2003 (wszystkie wersje i produkty<br />
zawarte w pakiecie Visual Studio .NET 2003)</td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=a13b7a21-463c-4286-ad68-e692417e80e2&amp;displaylang=en">Ważny</a> <strong>[3]</strong></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Visual Studio .NET 2002 (wszystkie wersje i produkty<br />
zawarte w pakiecie Visual Studio .NET 2002)</td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=44004d19-b22f-4af2-a701-1fcb0467fbf9&amp;displaylang=en">Ważny</a> <strong>[3]</strong></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">.NET Framework SDK wersja 1.0</td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=69703d1d-2ce3-42da-abf8-353d2121dab0&amp;displaylang=en">Ważny</a> <strong>[3]</strong></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Plik redystrybuowany w ramach pakietu Platform SDK: GDI+</td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?displaylang=en&amp;familyid=bfc0b436-9015-43e2-81a3-54938b6f4614">Ważny</a> <strong>[3]</strong></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Inne podlegające oprogramowanie firmy Microsoft:</strong></td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Picture It!® 2002 (wszystkie wersje)</td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=235ebc80-564b-4b52-a344-502e25aad7fe&amp;displaylang=en">Ważny</a> <strong>[2]</strong></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Greetings 2002</td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=235ebc80-564b-4b52-a344-502e25aad7fe&amp;displaylang=en">Ważny</a> <strong>[2]</strong></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Picture It! wersja 7.0 (wszystkie wersje)</td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=235ebc80-564b-4b52-a344-502e25aad7fe&amp;displaylang=en">Ważny</a> <strong>[2]</strong></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Digital Image Pro wersja 7.0</td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=235ebc80-564b-4b52-a344-502e25aad7fe&amp;displaylang=en">Ważny</a>  <strong>[2]</strong></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Picture It! wersja 9 (wszystkie wersje, łącznie z programem Picture It! Library</td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=235ebc80-564b-4b52-a344-502e25aad7fe&amp;displaylang=en">Ważny</a> <strong>[2]</strong></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Digital Image Pro wersja 9</td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=235ebc80-564b-4b52-a344-502e25aad7fe&amp;displaylang=en">Ważny</a> <strong>[2]</strong></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Digital Image Suite wersja 9</td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=235ebc80-564b-4b52-a344-502e25aad7fe&amp;displaylang=en">Ważny</a> <strong>[2]</strong></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Producer for Microsoft Office PowerPoint (wszystkie wersje)</td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=235ebc80-564b-4b52-a344-502e25aad7fe&amp;displaylang=en">Ważny</a> <strong>[2]</strong></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Business Solutions CRM 1.2</td>
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"></td>
</tr>
</tbody>
</table>
  
**Uwagi**
  
**<sup>[1]</sup>** Ten system operacyjny przy ustawieniach domyślnych nie jest narażony na skutki tej usterki. Może jednak zostać narażony po zainstalowaniu innych programów lub składników oprogramowania. Więcej szczegółów zawiera odpowiedni biuletyn zabezpieczeń.
  
**<sup>[2]</sup>** Ta aktualizacja nie jest wymagana w przypadku korzystania z systemu Windows XP lub Windows Server 2003. Więcej szczegółów zawiera odpowiedni [biuletyn zabezpieczeń](http://www.microsoft.com/poland/technet/).
  
**<sup>[3]</sup>** Ta aktualizacja nie jest wymagana w przypadku systemu Windows XP lub Windows Server 2003, z wyjątkiem sytuacji, gdy użytkownik tworzy aplikacje, w których redystrybuowany jest plik Gdiplus.dll przy użyciu produktów .NET Framework SDK wersja 1.0, Visual Studio .NET 2002, Visual Studio .NET 2003 lub plik redystrybuowany w ramach pakietu Platform SDK: GDI+. Więcej szczegółów zawiera odpowiedni [biuletyn zabezpieczeń](http://www.microsoft.com/poland/technet/).
  
Wdrażanie  
---------
  
<span></span>
**Usługi Software Update Services:**
  
Usługi Microsoft Software Update Services (SUS) umożliwiają administratorom szybkie i niezawodne wdrażanie najnowszych aktualizacji krytycznych i aktualizacji zabezpieczeń na serwerach działających w systemach Windows 2000 oraz Windows Server 2003, a także na komputerach stacjonarnych z systemami Windows 2000 Professional lub Windows XP Professional.
  
Więcej informacji dotyczących sposobu wdrażania tej aktualizacji zabezpieczeń za pomocą usług Software Update Services zawiera witryna sieci Web usług [Software Update Services](http://go.microsoft.com/fwlink/?linkid=21133).
  
**Program Systems Management Server:**
  
Program Systems Management Server (SMS) jest przeznaczonym dla przedsiębiorstw i w znacznym stopniu konfigurowalnym rozwiązaniem służącym do zarządzania aktualizacjami. Program SMS umożliwia administratorom znalezienie komputerów z systemem Windows, w których wymagane jest zainstalowanie aktualizacji zabezpieczeń, a także przeprowadzenie kontrolowanego wdrożenia tych aktualizacji w całym przedsiębiorstwie, przy minimalnym zakłóceniu pracy użytkowników końcowych. Więcej informacji o tym, jak administratorzy mogą wykorzystać program SMS 2003 do wdrażania aktualizacji zabezpieczeń zawiera [witryna sieci Web zarządzania poprawkami zabezpieczeń przy użyciu programu SMS 2003](http://www.microsoft.com/smserver/evaluation/capabilities/patch.asp). Użytkownicy programu SMS 2.0 mogą także skorzystać z dodatku [Software Updates Service Feature Pack](http://www.microsoft.com/smserver/downloads/20/featurepacks/suspack/) ułatwiającego wdrażanie aktualizacji zabezpieczeń. Więcej informacji na temat programu SMS można znaleźć w [witrynie sieci Web programu SMS](http://go.microsoft.com/fwlink/?linkid=21158).
  
**Uwaga** Dzięki narzędziom Microsoft Baseline Security Analyzer oraz Microsoft Office Detection Tool program SMS zapewnia obsługę wykrywania i wdrażania aktualizacji zabezpieczeń zawartych w biuletynach. Jednak niektóre aktualizacje oprogramowania mogą nie zostać wykryte przez te narzędzia. W takich przypadkach administratorzy mogą korzystać z funkcji zarządzania zasobami programu SMS w celu przyporządkowywania poszczególnych aktualizacji do określonych komputerów. Aby uzyskać więcej informacji o tej procedurze, odwiedź następującą [witrynę sieci Web](http://www.microsoft.com/technet/prodtechnol/sms/sms2003/patchupdate.mspx). Niektóre aktualizacje zabezpieczeń wymagają uprawnień administratora i ponownego uruchomienia systemu. Do zainstalowania tych aktualizacji administratorzy mogą użyć narzędzia Elevated Rights Deployment Tool (dostępnego w dodatkach [**SMS 2003 Administration Feature Pack**](http://www.microsoft.com/smserver/downloads/2003/adminpack.asp) oraz [SMS 2.0 Administration Feature Pack](http://www.microsoft.com/smserver/downloads/20/featurepacks/adminpack/)).
  
**Narzędzia QChain.exe i Update.exe:**
  
Firma Microsoft wydała narzędzie QChain.exe, które jest uruchamiane w wierszu polecenia i umożliwia administratorom systemu bezpieczne łączenie aktualizacji zabezpieczeń. *W przypadku łączenia* można instalować wiele aktualizacji bez ponownego uruchamiania komputera między kolejnymi instalacjami. Narzędzie Update.exe, używane w aktualizacjach opisanych w tym biuletynie, ma wbudowaną funkcję łączenia. Klienci używający systemu Windows 2000 z dodatkiem Service Pack 2 lub nowszym, Windows XP albo Windows Server 2003 nie potrzebują narzędzia Qchain.exe do łączenia tych aktualizacji. Narzędzie Qchain.exe obsługuje jednak łączenie tych aktualizacji systemu Windows, dlatego administrator może utworzyć jeden spójny skrypt wdrażania dla wszystkich platform. Więcej informacji na temat narzędzia Qchain zawiera następująca [witryna sieci Web](http://go.microsoft.com/fwlink/?linkid=21156).
  
**Narzędzie Microsoft Baseline Security Analyzer:**
  
Narzędzie Microsoft Baseline Security Analyzer (MBSA) umożliwia administratorom skanowanie lokalnych i zdalnych systemów w poszukiwaniu brakujących aktualizacji zabezpieczeń oraz typowych błędów konfiguracji zabezpieczeń. Więcej informacji na temat narzędzia MBSA można znaleźć w [witrynie sieci Web narzędzia Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134).
  
#### Inne informacje:
  
**Podziękowania**
  
Firma Microsoft [dziękuje](http://go.microsoft.com/fwlink/?linkid=21127) wymienionym poniżej organizacjom i osobom za współpracę w dziedzinie ochrony klientów:
  
-   Panu Johnowi Lampe z firmy [Tenable Network Security](http://www.tenablesecurity.com) za zgłoszenie problemu opisanego w biuletynie zabezpieczeń [MS04-016](http://technet.microsoft.com/security/bulletin/ms04-016).  
-   [Firmie eEye Digital Security](http://www.eeye.com/html/) za zgłoszenie problemu opisanego w biuletynie zabezpieczeń [MS04-017](http://technet.microsoft.com/security/bulletin/ms04-017).
  
**Uzyskiwanie innych aktualizacji zabezpieczeń:**
  
Aktualizacje dotyczące innych problemów związanych z zabezpieczeniami można uzyskać w następujących lokalizacjach:
  
-   Aktualizacje zabezpieczeń są dostępne w [Centrum pobierania firmy Microsoft](http://go.microsoft.com/fwlink/?linkid=21129). Najłatwiej je znaleźć, przeprowadzając wyszukiwanie wyrażenia „poprawka zabezpieczeń”.  
-   Aktualizacje dla poszczególnych platform są dostępne w witrynie sieci Web [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130).
  
**Pomoc techniczna:**
  
-   Klienci mogą uzyskać pomoc techniczną w [Biurze Obsługi Klienta Microsoft](http://go.microsoft.com/fwlink/?linkid=21131) pod numerem 0 801 802 000 (Opłata według stawek Twojego operatora) lub (0-22) 594 19 99 w godzinach od 9:00 do 17:00, od poniedziałku do piątku. Połączenia z działem pomocy technicznej dotyczące aktualizacji zabezpieczeń są bezpłatne.  
-   Klienci międzynarodowi mogą otrzymać pomoc w lokalnych przedstawicielstwach firmy Microsoft. Połączenia z działem pomocy technicznej związane z aktualizacjami zabezpieczeń są bezpłatne. Więcej informacji o sposobie kontaktowania się z firmą Microsoft w sprawach dotyczących pomocy technicznej zawiera [międzynarodowa witryna sieci Web pomocy technicznej](http://go.microsoft.com/fwlink/?linkid=21155).
  
**Zasoby zabezpieczeń:**
  
-   Witryna sieci Web [Microsoft TechNet Security](http://go.microsoft.com/fwlink/?linkid=21132) zawiera dodatkowe informacje na temat zabezpieczeń w produktach firmy Microsoft.  
-   [Usługi Microsoft Software Update Services](http://go.microsoft.com/fwlink/?linkid=21133)  
-   [Narzędzie Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134) (MBSA)  
-   [Witryna Windows Update](http://go.microsoft.com/fwlink/?linkid=21130)  
-   Wykaz Windows Update: Aby uzyskać więcej informacji o wykazie Windows Update, zobacz artykuł [323166](http://support.microsoft.com/default.aspx?scid=kb;en-us;323166) w bazie wiedzy Microsoft Knowledge Base.  
-   [Witryna Office Update](http://go.microsoft.com/fwlink/?linkid=21135)
  
**Zrzeczenie odpowiedzialności:**
  
Informacje w bazie wiedzy Microsoft Knowledge Base są dostarczane „tak jak są” bez jakiejkolwiek gwarancji. Firma Microsoft odrzuca wszelkie gwarancje, wyraźne i dorozumiane, w tym gwarancje dotyczące wartości handlowej i przydatności do określonego celu. Firma Microsoft Corporation ani jej dostawcy w żadnym wypadku nie ponoszą odpowiedzialności za jakiekolwiek szkody, w tym bezpośrednie, pośrednie, przypadkowe, wynikowe, utratę zysków handlowych lub szkody specjalne, nawet jeżeli firmę Microsoft Corporation lub jej dostawców powiadomiono o możliwości zaistnienia takich szkód. W niektórych stanach wyłączenie lub ograniczenie odpowiedzialności za straty wynikowe lub przypadkowe, a więc i powyższe ograniczenia, nie mają zastosowania.
  
**Wersje:**
  
-   Wersja 1.0 (8 czerwca 2004 r.): Opublikowano biuletyn
  
*Built at 2014-04-18T01:50:00Z-07:00*
