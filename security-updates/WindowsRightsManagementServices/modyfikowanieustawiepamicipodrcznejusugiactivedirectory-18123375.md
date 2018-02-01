---
TOCTitle: Modyfikowanie ustawień pamięci podręcznej usługi Active Directory
Title: Modyfikowanie ustawień pamięci podręcznej usługi Active Directory
ms:assetid: '8789a7a5-2065-4fae-9104-e0a70f1f2fb6'
ms:contentKeyID: 18123375
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747586(v=WS.10)'
---

Modyfikowanie ustawień pamięci podręcznej usługi Active Directory
=================================================================

Ustawienia w rejestrze określają liczbę wpisów przechowywanych w pamięci podręcznej usługi Active Directory. Ustawienia te można zmodyfikować w celu skrócenia czasu odpowiedzi na żądania klientów. Aby uzyskać więcej informacji, zobacz „Optymalizowanie wydajności usług katalogowych” we wcześniejszej części tego tematu. Można także ustawić okres ważności informacji przechowywanych w pamięci podręcznej.

Na komputerach z 32-bitową wersją systemu Windows Server 2003 poniższy klucz zawiera pełną ścieżkę podklucza wpisów pamięci podręcznej.

**HKEY\_LOCAL\_MACHINE\\Software\\Microsoft\\DRMS\\1.0\\DirectoryServices**

Na komputerach z 64-bitową wersją systemu Windows Server 2003 poniższy klucz zawiera pełną ścieżkę podklucza wpisów pamięci podręcznej.

**HKEY\_LOCAL\_MACHINE\\SoftwareWOW6432Node\\Microsoft\\DRMS\\1.0\\DirectoryServices**

Poniższa tabela zawiera wpisy sterujące sposobem działania pamięci podręcznej w pamięci.

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Nazwa</th>
<th style="border:1px solid black;" >Typ</th>
<th style="border:1px solid black;" >Wartość domyślna</th>
<th style="border:1px solid black;" >Opis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">PrincipalCacheMax</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">1,000</td>
<td style="border:1px solid black;">Maksymalna liczba podmiotów oraz ich adresów e-mail i identyfikatorów SID, którą można przechowywać w pamięci podręcznej.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PrincipalCacheExpireMinutes</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">12</td>
<td style="border:1px solid black;">Okres ważności informacji dotyczących podmiotów przechowywanych w pamięci podręcznej.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">GroupIDCacheMax</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">1,000</td>
<td style="border:1px solid black;">Maksymalna liczba grup oraz ich adresów e-mail i identyfikatorów SID, które można przechowywać w pamięci podręcznej.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">GroupIDCacheExpireMinutes</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">12</td>
<td style="border:1px solid black;">Okres ważności informacji dotyczących członkostwa w grupach, które są przechowywane w pamięci podręcznej.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">GroupMembershipCacheMax</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">1,000</td>
<td style="border:1px solid black;">Maksymalna liczba kontaktów będących członkami grupy, które można przechowywać w pamięci podręcznej.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">GroupMembershipCacheExpireMinutes</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">12</td>
<td style="border:1px solid black;">Okres ważności informacji w pamięci podręcznej dotyczących kontaktów należących do danej grupy.</td>
</tr>
</tbody>
</table>
  
> [!Caution]  
> Nieprawidłowa edycja rejestru może spowodować poważne uszkodzenie systemu. Przed wprowadzaniem zmian w rejestrze należy wykonać kopię zapasową wszystkich wartościowych danych przechowywanych na komputerze. 
  
> [!note]  
> Wpisy rejestru **PrincipalCacheExpireMinutes**, **GroupIDCacheExpireMinutes**, **GroupMembershipCacheExpireMinutes** i **ContactMembersofGroupCacheExpireMinutes** również sterują wygaśnięciem pamięci podręcznej w lokalnej pamięci podręcznej usługi Active Directory zapisanej w bazie danych usług katalogowych na serwerze bazy danych. 
