---
TOCTitle: Instalacja z wiersza polecenia serwera programu RMS
Title: Instalacja z wiersza polecenia serwera programu RMS
ms:assetid: 'b55b1e2a-dd14-4168-a37f-9cdedbec660b'
ms:contentKeyID: 18123429
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747733(v=WS.10)'
---

Instalacja z wiersza polecenia serwera programu RMS
===================================================

Program RMS z dodatkiem Service Pack 2 (SP2) można instalować z wiersza polecenia, automatyzując instalację. Automatyzacja instalacji jest możliwa na dwa sposoby: wykonując instalację nienadzorowaną za pomocą pobranego klienta EXE lub instalując klienta programu RMS za pomocą wyodrębnionych plików MSI z pobranego pliku EXE. Aby wykonać instalację za pomocą pobranego pliku EXE, użyj następującej składni:

**WindowsRightsManagementServicesSP2-KB917275-Client-ENU.exe -override 1 /I MsDrmClient.msi REBOOT=ReallySuppress /q -override 2 /I RmClientBackCompat.msi REBOOT=ReallySuppress /q**

Aby zainstalować pliki Instalatora Windows® (.msi), należy najpierw wyodrębnić pliki msi z pliku wykonywalnego programu RMS z dodatkiem SP2. Poniższe polecenie można uruchomić z wiersza polecenia w celu wyodrębnienia plików msdrmclient.msi i RmClientBackCompat.msi:

**WindowsRightsManagementServiceSP2-KB917275-Server-ENU.exe /X:C:\\***Lokalizacja\_instalacji*

Po wyodrębnieniu plików .msi można zainstalować program RMS za pomocą poniższych poleceń:

**msiexec.exe /I MSDrmClient.msi /qn ALLUSERS=2 /m MSIDHOG /lei logfile.log DISPLYPAGE="NO" TARGETDIR=c:\\***Lokalizacja\_instalacji*

**msiexec.exe /I RMClientBackCompat.msi /qn ALLUSERS=2 /m MSIDHOG /lei logfile.log DISPLYPAGE="NO" TARGETDIR=c:\\***Lokalizacja\_instalacji*

Składnie poszczególnych poleceń opisano w poniższej tabeli.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Parametr</th>
<th>Definicja</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>/I MSDrmClient.msi</strong> lub <strong>/I RMClientBackCompat.msi</strong></td>
<td style="border:1px solid black;">Wymagany. Określa produkt do zainstalowania.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>/qn</strong></td>
<td style="border:1px solid black;">Opcjonalny. Określa instalację cichą, bez konieczności interakcji ze strony użytkownika.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>/lei</strong> <em>logfile.log</em></td>
<td style="border:1px solid black;">Opcjonalny. Określa plik, w którym mają być rejestrowane komunikaty o błędach i o stanie.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>DISPLAYPAGE=&quot;NO&quot;</strong></td>
<td style="border:1px solid black;">Opcjonalny. Określa, że po instalacji nie zostanie wyświetlona strona <strong>Administracja globalna</strong>.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>TARGETDIR=c:\</strong><em>Lokalizacja_instalacji</em></td>
<td style="border:1px solid black;">Opcjonalny. Określa katalog instalacyjny programu RMS z dodatkiem Service Pack 2. Jeśli użytkownik nie określi miejsca, zostanie użyte domyślne miejsce instalacji.</td>
</tr>
</tbody>
</table>
  
| ![](images/Cc747733.note(WS.10).gif)Uwaga                                                                                                                                             |  
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Niezależnie od wybranej metody instalacji należy prawidłowo zainstalować oba pliki .msi. Jeśli wystąpi błąd uniemożliwiający instalację pliku MSDrmClient.msi, nie należy instalować pliku RMClientBackCompat.msi. |
