---
TOCTitle: Modyfikowanie ustawień rejestru dotyczących puli połączeń
Title: Modyfikowanie ustawień rejestru dotyczących puli połączeń
ms:assetid: 'c61d91db-a1ad-4ca5-a492-015da629afbc'
ms:contentKeyID: 18123409
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747660(v=WS.10)'
---

Modyfikowanie ustawień rejestru dotyczących puli połączeń
=========================================================

Aby podnieść wydajność systemu, można za pomocą wpisów kluczy rejestru określić właściwości puli połączeń protokołu LDAP (Lightweight Directory Access Protocol) w usłudze Active Directory, których używa program RMS.

Na komputerach z 32-bitową wersją systemu Windows Server 2003 poniższy klucz rejestru zawiera pełną ścieżkę podklucza wpisów rejestru dotyczących puli połączeń.

**HKEY\_LOCAL\_MACHINE\\Software\\Microsoft\\DRMS\\1.0**

Na komputerach z 64-bitową wersją systemu Windows Server 2003 poniższy klucz rejestru zawiera pełną ścieżkę podklucza wpisów rejestru dotyczących puli połączeń.

**HKEY\_LOCAL\_MACHINE\\SoftwareWOW6432Node\\Microsoft\\DRMS\\1.0**

Poniższa tabela zawiera wpisy, które można dodać w celu zastąpienia domyślnych ustawień puli połączeń usługi Active Directory. Wyświetlone wartości to wartości domyślne. Aby uzyskać więcej informacji dotyczących konstruowania listy kwerend i używania tych ustawień w programie RMS, zobacz „Optymalizowanie ustawień puli połączeń usługi Active Directory” we wcześniejszej części tego tematu.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th>Nazwa</th>
<th>Typ</th>
<th>Wartość domyślna</th>
<th>Opis</th>
<th>Uwagi</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">GC</td>
<td style="border:1px solid black;">String</td>
<td style="border:1px solid black;">nazwa-1, ..., nazwa-n</td>
<td style="border:1px solid black;">Rozdzielona przecinkami lista wykazów globalnych (z nazwami DNS). Ten klucz określa ograniczenie dotyczące używania w programie RMS tylko określonych wykazów globalnych.</td>
<td style="border:1px solid black;">Jeśli w programie RMS nie mają być tworzone listy kwerend, należy za pomocą tego ustawienia określić używane wykazy globalne.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">MinGC</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">1</td>
<td style="border:1px solid black;">Minimalna liczba wykazów globalnych, które muszą być dostępne przed uruchomieniem programu RMS.</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">MaxGC</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">15</td>
<td style="border:1px solid black;">Maksymalna liczba wykazów globalnych, którą algorytm wykrywania topologii doda do listy kwerend.</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ThreshHoldAlive</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">1</td>
<td style="border:1px solid black;">Minimalna liczba połączeń, które powinny odpowiadać, aby usługa DiscoveryServices rozpoczęła wyszukiwanie wykazów globalnych w celu ich dodania do listy kwerend, dzięki czemu program RMS będzie mógł przyjmować żądania.</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">RetryDown</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">5</td>
<td style="border:1px solid black;">Liczba określająca liczbę prób ponownego użycia niedziałającego połączenia przed uznaniem go za nieodpowiadające.</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">TimeRetryDown</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">300</td>
<td style="border:1px solid black;">Liczba określająca, ile sekund należy odczekać przed ponowną próbą użycia niedziałającego połączenia.</td>
<td style="border:1px solid black;">Zmiana tego domyślnego ustawienia nie jest wymagana, chyba że w szczególnych okolicznościach.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">TimeRetrySlow</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">30</td>
<td style="border:1px solid black;">Liczba określająca, ile sekund należy odczekać przed ponowną próbą użycia wolnego połączenia.</td>
<td style="border:1px solid black;">Zmiana tego domyślnego ustawienia nie jest wymagana, chyba że w szczególnych okolicznościach.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">WtRoundRobin</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">1</td>
<td style="border:1px solid black;">Waga działania okrężnego podczas równoważenia obciążenia.</td>
<td style="border:1px solid black;">Względna waga działania okrężnego w równoważeniu obciążenia. Najniższą wartością jest 1.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">WtThreadCount</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">100</td>
<td style="border:1px solid black;">Waga liczby wątków na połączenie podczas równoważenia obciążenia.</td>
<td style="border:1px solid black;">Względna waga małej liczby wątków.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">WtSlow</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">1,000</td>
<td style="border:1px solid black;">Waga wolnego działania połączenia podczas równoważenia obciążenia.</td>
<td style="border:1px solid black;">Względna waga połączenia, które nie jest wolne.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">TimeOutForGC</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">5</td>
<td style="border:1px solid black;">Liczba sekund, po odczekaniu której upływa limit czasu dotyczący żądania dodania wykazu globalnego do listy kwerend.</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">LdapTimeOut</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">5</td>
<td style="border:1px solid black;">Liczba sekund, po odczekaniu której upływa limit czasu interfejsów API LDAP</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">TopDownExpansionLDAPTimeOut</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">40</td>
<td style="border:1px solid black;">Liczba sekund, po odczekaniu której upływa limit czasu rozszerzania kwerend LDAP z wysokiego poziomu do niskiego.</td>
<td style="border:1px solid black;"></td>
</tr>
</tbody>
</table>
  
| ![](images/Cc747660.Caution(WS.10).gif)Przestroga                                                                                                                                |  
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Nieprawidłowa edycja rejestru może spowodować poważne uszkodzenie systemu. Przed wprowadzaniem zmian w rejestrze należy wykonać kopię zapasową wszystkich wartościowych danych przechowywanych na komputerze. |
