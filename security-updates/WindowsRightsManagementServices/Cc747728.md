---
TOCTitle: Usługi sieci Web programu RMS
Title: Usługi sieci Web programu RMS
ms:assetid: 'ed8dbb2e-0590-4502-afc4-54f66b96d515'
ms:contentKeyID: 18123496
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747728(v=WS.10)'
---

Usługi sieci Web programu RMS
=============================

Program RMS dostarcza składnik serwera systemu RMS. Jego główne funkcje zostały zaimplementowane jako zestaw usług sieci Web Microsoft® ASP.NET, które działają w programie Microsoft® Internet Information Services (IIS). Usługi sieci Web programu RMS udostępniane są poprzez interfejs SOAP lub komunikację zdalną .NET.

Usługi sieci Web zapewniają:

-   Rejestrację podrzędną serwerów
-   Certyfikowanie kont zaufanych jednostek
-   Licencjonowanie informacji chronionych prawami dostępu
-   Funkcje administracyjne programu RMS

Poniższa tabela zawiera opis usług sieci Web programu RMS.


<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Usługa</th>
<th style="border:1px solid black;" >Opis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Rejestracja podrzędna</td>
<td style="border:1px solid black;">Zapewnia certyfikaty licencjodawcy serwera podrzędnego serwerom w klastrach przeznaczonych tylko do licencjonowania. Certyfikaty te umożliwiają klastrom przeznaczonym tylko do licencjonowania wystawianie licencji publikacji i użytkowania.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Certyfikowanie konta</td>
<td style="border:1px solid black;">Zapewnia certyfikaty kont praw dla użytkowników. Certyfikaty te muszą posiadać użytkownicy, którzy chcą uzyskać licencje publikacji i użytkowania, aby tworzyć i wykorzystywać zawartość chronioną prawami dostępu.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Serwer proxy aktywacji</td>
<td style="border:1px solid black;">Usługa ta została zachowana w celu zapewnienia zgodności z wersją 1 klienta RMS. Przekazuje ona żądania aktywacji komputera do usługi aktywacji firmy Microsoft i zwraca skrytki oraz certyfikaty komputera RMS do klientów RMS w wersji 1. Usługa ta nie jest używana przez klientów RMS z dodatkiem Service Pack 1 (SP1) lub nowszym.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Publikowanie</td>
<td style="border:1px solid black;">Wystawia licencje publikacji umożliwiające tworzenie i rozpowszechnianie zawartości chronionej prawami dostępu. Wystawia także certyfikaty licencjodawcy klienta, które pozwalają użytkownikom na publikację zawartości chronionej prawami dostępu bez połączenia z siecią wewnętrzną obsługującą RMS.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Licencjonowanie</td>
<td style="border:1px solid black;">Wystawia licencje użytkowania, które umożliwiają użytkownikom korzystanie z zawartości chronionej prawami dostępu.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Administracja</td>
<td style="border:1px solid black;">Umożliwia administratorowi zarządzanie programem RMS.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DrmRemote</td>
<td style="border:1px solid black;">Umożliwia wzajemną komunikację między usługami sieci Web oraz z innymi składnikami systemu RMS poprzez udostępnienie komunikacji zdalnej .NET.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Likwidowanie</td>
<td style="border:1px solid black;">Zmienia zawartość chronioną prawami dostępu w niechronioną i zwraca ją do klienta. Usługa ta instalowana jest przez Instalatora programu RMS, ale do momentu włączenia jej przez administratora nie ma odpowiadającego jej wirtualnego katalogu głównego w programie IIS. Włączenie tej usługi powoduje wyłączenie wszystkich pozostałych usług.</td>
</tr>
</tbody>
</table>
  
Poza usługami sieci Web program RMS instaluje także usługę odbiornika rejestrowania. Każda usługa sieci Web przesyła zarejestrowane dane do kolejki komunikatów rejestrowania. Usługa odbiornika rejestrowania przesyła następnie zarejestrowane dane z kolejki komunikatów do bazy danych rejestrowania.
  
Aplikacje usług sieci Web znajdują się w katalogach wirtualnych usług IIS. Te katalogi wirtualne zainstalowane są na każdym serwerze RMS w obrębie witryny sieci Web, która została wybrana podczas zastrzegania.
  
Ustawienia uwierzytelniania i dostępu konfigurowane są oddzielnie dla każdego katalogu wirtualnego. Ponadto ustawienia dostępu konfigurowane są oddzielnie dla każdej usługi sieci Web . Aby uzyskać informacje o ustawieniach zabezpieczeń dla katalogów wirtualnych i plików usług sieci Web, zobacz [Obsługa Internetowych usług informacyjnych w programie RMS](https://technet.microsoft.com/bd4dc69f-1e4e-4e95-9ae2-c925d8a14d4c) w dalszej części tego tematu.
  
Aby uzyskać więcej informacji o każdej z usług sieci Web, zobacz [Składniki oprogramowania RMS](https://technet.microsoft.com/e38a840e-f390-48fd-8354-50108a64f5ca) w dalszej części tego tematu.
