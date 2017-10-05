---
TOCTitle: Obsługa Internetowych usług informacyjnych w programie RMS
Title: Obsługa Internetowych usług informacyjnych w programie RMS
ms:assetid: 'bd4dc69f-1e4e-4e95-9ae2-c925d8a14d4c'
ms:contentKeyID: 18123469
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747649(v=WS.10)'
---

Obsługa Internetowych usług informacyjnych w programie RMS
==========================================================

Podstawowe usługi programu RMS są dostarczane przez zbiór usług sieci Web ASP .NET. Te usługi sieci Web działają w programie Internetowe usługi informacyjne (IIS) firmy Microsoft®. Podczas procesu zastrzegania serwera program RMS konfiguruje katalogi wirtualne w usługach IIS. Pliki aplikacji dla usług sieci Web są instalowane w katalogach wirtualnych.

Podczas zastrzegania serwera można z listy witryn sieci Web na serwerze wybrać witrynę sieci Web, w której zostaną skonfigurowane katalogi wirtualne. Przed zastrzeżeniem serwera użytkownik może utworzyć specjalną witrynę sieci Web dla programu RMS. W takim przypadku można skonfigurować ograniczenia dotyczące uwierzytelniania oraz dostępu, które będą specyficzne dla rozmieszczenia programu RMS.

Domyślnie pliki usług sieci Web i katalogi wirtualne są chronione przez listy arbitralnej kontroli dostępu (DACL) w celu zapobiegania przed nieautoryzowanym dostępem do ich funkcji. Wpisy kontroli dostępu (ACE) dla tych elementów są następujące:

-   Grupa administratorów ma pełną kontrolę
-   Konto System lokalny ma pełną kontrolę
-   Grupa usługi RMS  ma uprawnienia do odczytu i wykonywania
-   Grupy Goście i Użytkownicy mają uprawienia do odczytu i wykonywania, wyświetlania zawartości folderu oraz odczytu.
-   Dostęp anonimowy nie jest dozwolony

W poniższej tabeli przedstawiono listę katalogów wirtualnych, które są tworzone w usługach IIS, oraz usług instalowanych w katalogach wirtualnych.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Katalog wirtualny</th>
<th style="border:1px solid black;" >Usługa</th>
<th style="border:1px solid black;" >Plik usługi sieci Web</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">_wmcs</td>
<td style="border:1px solid black;">To jest administracyjny katalog wirtualny klastra programu RMS</td>
<td style="border:1px solid black;">Nie dotyczy</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Certification</td>
<td style="border:1px solid black;">Ten katalog wirtualny zawiera usługi obsługujące certyfikację programu RMS</td>
<td style="border:1px solid black;">Nie dotyczy</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Serwer proxy aktywacji</td>
<td style="border:1px solid black;">Activation.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Certyfikacja kont</td>
<td style="border:1px solid black;">Certification.asmx</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Certyfikacja wstępna</td>
<td style="border:1px solid black;">Precertification.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Lokalizator usług</td>
<td style="border:1px solid black;">ServiceLocator.asmx</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Serwer</td>
<td style="border:1px solid black;">Server.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Certyfikacja serwera</td>
<td style="border:1px solid black;">ServerCertification.asmx</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Certyfikacja urządzenia przenośnego</td>
<td style="border:1px solid black;">MobileDeviceCertfication.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Rejestrowanie</td>
<td style="border:1px solid black;">SubEnrollService.asmx</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Licencjonowanie</td>
<td style="border:1px solid black;">Ten katalog wirtualny zawiera usługi obsługujące licencjonowanie programu RMS</td>
<td style="border:1px solid black;">Nie dotyczy</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Licencjonowanie</td>
<td style="border:1px solid black;">License.asmx</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Publikowanie</td>
<td style="border:1px solid black;">Publish.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Serwer</td>
<td style="border:1px solid black;">Server.asmx</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Lokalizator usług</td>
<td style="border:1px solid black;">ServiceLocator.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Admin</td>
<td style="border:1px solid black;">Ten katalog wirtualny zawiera usługi obsługujące administrację programu RMS</td>
<td style="border:1px solid black;">Nie dotyczy</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Administracja</td>
<td style="border:1px solid black;">AdminSvc.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DrmRemote</td>
<td style="border:1px solid black;">Interfejs .NET Remoting</td>
<td style="border:1px solid black;">Nie dotyczy</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DirectoryServices</td>
<td style="border:1px solid black;">To jest podkatalog katalogu DrmRemote</td>
<td style="border:1px solid black;">Nie dotyczy</td>
</tr>
</tbody>
</table>
  
| ![](images/Cc747649.note(WS.10).gif)Uwaga                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |  
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Usługa administracji ma większe ograniczenia niż pozostałe usługi sieci Web, ponieważ udostępniane przez nią interfejsy umożliwiają konfigurowanie programu RMS. Z tego powodu członkowie grup użytkowników nie mogą uzyskiwać dostępu do usługi administracji. Ponadto filtrowanie protokołu IP jest ustawione, tak aby udzielać dostępu tylko komputerowi lokalnemu. Katalog wirtualny Usługi katalogowe nie udziela dostępu użytkownikom z grupy Goście. Usługa lokalizatora usług udziela również pełnej kontroli kontu Usługa sieciowa. W celu zastrzeżenia serwera licencji należy zmienić domyślne ustawienia ACE, tak aby umożliwiały dostęp administratorowi programu RMS. |
