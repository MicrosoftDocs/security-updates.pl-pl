---
TOCTitle: Usługa likwidowania programu RMS
Title: Usługa likwidowania programu RMS
ms:assetid: '97677e3b-bc83-47ec-b6db-d326cd94566c'
ms:contentKeyID: 18123396
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747695(v=WS.10)'
---

Usługa likwidowania programu RMS
================================

Usługa likwidowania jest niestandardową usługą sieci Web, która jest instalowana przez Instalatora programu RMS. Działą na klastrze grłównym i klastrach licencji. Po włączeniu tej usługi wszystkie pozostałe usługi sieci Web programu RMS na serwerze są wyłączane.

Ta usługa deszyfruje klucz zawartości w licencji publikacji zawartości chronionej na podstawie praw i dostarcza ten klucz do klienta w odpowiedzi na żądanie licencji. Umożliwia to zapisanie zawartości bez ochrony technologią RMS. Usługa likwidowania rejestruje wszystkie żądania klienckie wykonane do tej usługi i wysyła je do usługi odbiornika rejestrowania w celu ich zapisania w bazie danych rejestrowania.

Usługę likwidowania można włączyć na stronie **Ustawienia zabezpieczeń** w administracyjnej witrynie sieci Web. Po włączeniu tej usługi nie można przywrócić serwera do standardowej konfiguracji programu RMS.

Po włączeniu usługi należy ustawić listę DACL pliku decommission.asmx, tak aby zezwalała użytkownikom z przedsiębiorstwa, którzy używali tego serwera, na licencjonowanie swojej zawartości, oraz dodać grupę RMS Service Group do listy DACL z uprawnieniami do odczytu i wykonywania, aby program RMS mógł zarządzać operacjami. Po wyłączeniu ochrony dla całej zawartości publikowanej przez ten serwer należy wykonać kopię zapasową informacji o kluczach prywatnych i usunąć program RMS z serwera.

W poniższej tabeli przedstawiono domyślną listę kontroli dostępu w ramach tej usługi:

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Użytkownik lub grupa</th>
<th style="border:1px solid black;" >Uprawnienie domyślne</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">SYSTEM</td>
<td style="border:1px solid black;">Pełna kontrola</td>
</tr>
</tbody>
</table>
