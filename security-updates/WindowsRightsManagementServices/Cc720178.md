---
TOCTitle: Wymagane konta i uprawnienia dotyczące programu RMS
Title: Wymagane konta i uprawnienia dotyczące programu RMS
ms:assetid: '07a51daa-6823-41e6-b453-92f1a0592361'
ms:contentKeyID: 18123167
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720178(v=WS.10)'
---

Wymagane konta i uprawnienia dotyczące programu RMS
===================================================

W poniższej tabeli przedstawiono prawa dostępu i uprawnienia użytkownika wymagane do rozmieszczenia programu RMS i zarządzania nim.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Działanie</th>
<th style="border:1px solid black;" >Konto i uprawnienia użytkownika</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Instalowanie programu RMS</td>
<td style="border:1px solid black;">Należy zalogować się przy użyciu konta domeny należącego do lokalnej grupy Administratorzy.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Zastrzeganie programu RMS</td>
<td style="border:1px solid black;">Należy zalogować się przy użyciu konta domeny należącego do lokalnej grupy Administratorzy. Ponadto używane konto musi mieć nazwę logowania SQL z rolą administratora systemu przydzieloną w bazie danych serwera programu SQL Server, co umożliwi skonfigurowanie bazy danych z poziomu programu RMS.

Podczas zastrzegania należy określić konto usługi programu RMS, które musi już być utworzone. To konto powinno być standardowym kontem użytkownika domeny bez dodatkowych uprawnień. To konto będzie należeć do grupy RMS Service Group i będzie na nim działać program RMS wykonujący rutynowe operacje.

W przypadku rozmieszczania na jednym serwerze, gdzie baza danych znajduje się na tym samym komputerze co serwer głównej certyfikacji, można określić konto System lokalny. Ze względów bezpieczeństwa zaleca się jednak, aby zawsze określać konto usługi programu RMS, a nie konto System lokalny. Gdy baza danych znajduje się na osobnym serwerze, należy określić konto usługi programu RMS.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Administrowanie programem RMS</td>
<td style="border:1px solid black;">Należy zalogować się przy użyciu konta domeny należącego do lokalnej grupy Administratorzy. Można dostosować ustawienia zabezpieczeń w celu zarządzania dostępem do administracyjnych stron sieci Web.</td>
</tr>
</tbody>
</table>
  
> [!note]  
> Nie jest wymagane, aby konto używane do logowania się na serwerze programu RMS należało do dodatkowej grupy domeny, np. Administratorzy domeny. Jednak aby wykonać niektóre zadania administracyjne, takie jak rejestrowanie punktu połączenia usługi i modyfikowanie zasad zabezpieczeń, należy posiadać konto z dodatkowymi uprawnieniami. 
