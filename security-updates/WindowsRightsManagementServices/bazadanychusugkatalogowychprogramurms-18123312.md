---
TOCTitle: Baza danych usług katalogowych programu RMS
Title: Baza danych usług katalogowych programu RMS
ms:assetid: '6f6b8586-5d17-4a40-94a3-4dc738195301'
ms:contentKeyID: 18123312
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747617(v=WS.10)'
---

Baza danych usług katalogowych programu RMS
===========================================

Serwer bazy danych obsługuje bazę danych usług katalogowych, która zawiera informacje o użytkownikach, identyfikatorach (takich jak adresy e-mail), identyfikatorach zabezpieczeń (SID), członkostwie w grupach oraz identyfikatorach alternatywnych. Te informacje są pobierane z kwerend LDAP wysyłanych do wykazu globalnego usługi Active Directory przez usługę licencjonowania programu RMS. Aby uzyskać więcej informacji o tym procesie i jego funkcji, zobacz „[Pamięć podręczna usługi Active Directory programu RMS](https://technet.microsoft.com/c721a2eb-2fe9-4346-b426-3cc169b97265)” w dalszej części tego tematu.

Grupa usługi RMS ma uprawienia do wykonywania procedur przechowywanych w bazie danych usług katalogowych.

W poniższej tabeli przedstawiono atrybuty usługi Active Directory przechowywane w tabelach bazy danych usług katalogowych.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Tabela</th>
<th>Atrybut</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">GroupAliases</td>
<td style="border:1px solid black;"><ul>
<li>GroupName: alias dla grupy<br />
<br />
</li>
<li>GroupID: unikatowy identyfikator dla tej grupy<br />
<br />
</li>
</ul></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">GroupIdentifiers</td>
<td style="border:1px solid black;"><ul>
<li>GroupDN: nazwa wyróżniająca usługi Active Directory dla tej grupy<br />
<br />
</li>
<li>GroupID: unikatowy identyfikator dla tej grupy<br />
<br />
</li>
<li>Expiration: data i godzina wygaśnięcia informacji przechowywanych w tej grupie<br />
<br />
</li>
</ul></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">GroupMembership</td>
<td style="border:1px solid black;"><ul>
<li>GroupID: unikatowy identyfikator dla tej grupy<br />
<br />
</li>
<li>ParentID: unikatowy identyfikator dla grupy, do której należy ta grupa<br />
<br />
</li>
</ul></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PrincipalAliases</td>
<td style="border:1px solid black;"><ul>
<li>PrincipalName: alias nazwy obiektu głównego<br />
<br />
</li>
<li>PrincipalID: unikatowy identyfikator dla tego obiektu głównego<br />
<br />
</li>
</ul></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PrincipalIdentifiers</td>
<td style="border:1px solid black;"><ul>
<li>PrincipalID: unikatowy identyfikator dla tego obiektu głównego<br />
<br />
</li>
<li>Expiration: data i godzina wygaśnięcia informacji przechowywanych w tym obiekcie głównym<br />
<br />
</li>
</ul></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PrincipalMembership</td>
<td style="border:1px solid black;">Każdy wiersz tej tabeli zawiera unikatowy identyfikator obiektu głównego i unikatowy identyfikator grupy, która należy do tego obiektu.
<ul>
<li>PrincipalID: unikatowy identyfikator dla tego obiektu głównego<br />
<br />
</li>
<li>ParentID: unikatowy identyfikator dla grupy, do której należy ten obiekt główny<br />
<br />
</li>
</ul></td>
</tr>
</tbody>
</table>
