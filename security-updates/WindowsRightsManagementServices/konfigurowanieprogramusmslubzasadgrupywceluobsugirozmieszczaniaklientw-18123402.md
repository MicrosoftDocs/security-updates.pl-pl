---
TOCTitle: Konfigurowanie programu SMS lub zasad grupy w celu obsługi rozmieszczania klientów
Title: Konfigurowanie programu SMS lub zasad grupy w celu obsługi rozmieszczania klientów
ms:assetid: '9e37c27b-8cc1-40c6-adb7-0937aa64c8db'
ms:contentKeyID: 18123402
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747703(v=WS.10)'
---

Konfigurowanie programu SMS lub zasad grupy w celu obsługi rozmieszczania klientów
==================================================================================

Jeśli rozmieszczany jest program RMS, na komputerach użytkowników musi być zainstalowana aplikacja obsługująca technologię RMS, ponieważ tylko wówczas użytkownicy mogą chronić i użytkować zawartość chronioną tą technologią.

Aplikacja obsługująca technologię RMS to aplikacja, z której działaniem zintegrowany jest składnik klienta programu RMS. W wersjach systemu wcześniejszych niż Windows Vista® klient programu RMS jest składnikiem systemu Windows pobieranym oddzielnie z Centrum pobierania firmy Microsoft. Jeśli jednak użytkownik nie chce pobierać klienta indywidualnie na każdy komputer kliencki w firmie, może użyć programu Systems Management Server (SMS) firmy Microsoft, przystawki Zasady grupy lub skryptów i w ten sposób zautomatyzować dostarczanie klientów programu RMS do komputerów klienckich.

| ![](images/Cc747703.Important(WS.10).gif)Ważne                                             |
|-------------------------------------------------------------------------------------------------------------------------|
| Klient programu RMS jest zintegrowany z systemem Windows Vista. Dzięki temu oddzielna instalacja nie jest już wymagana. |

Jeśli składnik klienta programu RMS ma być rozpowszechniany za pomocą programu SMS, należy wykonać następujące czynności:

-   Utwórz nowy plik definicji pakietu.
-   Wyodrębnij pliki Instalatora Windows z pliku WindowsRightsManagementServicesSP2-KB917275-Client-ENU.exe. W tym celu najpierw zapisz plik WindowsRightsManagementServicesSP2-KB917275-Client-ENU.exe. Nie instaluj go. W tym przykładzie załóżmy, że plik jest zapisywany w folderze c:\\nazwa\_folderu. Otwórz okno wiersza polecenia i wpisz następujące polecenie:
    `c:\folder_name\WindowsRightsManagementServicesSP2-KB917275-Client-ENU.exe /x/t:c:\folder_name`
    To polecenie powoduje wyodrębnienie plików MSDrmClient.msi i RMClientBackCompat.msi z pliku .exe i umieszczenie ich w folderze *c:\\nazwa\_folderu*.
-   Użyj plików Instalatora Windows dla definicji i źródła pakietu.
-   Zaanonsuj dostępność pakietu w sieci.

| ![](images/Cc747703.note(WS.10).gif)Uwaga                                                                                                                 |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Prawa administratora są wymagane do instalowania oprogramowania. Zasady zabezpieczeń w organizacji mogą wymagać, aby to administrator systemu instalował oprogramowanie klienckie RMS. |

Aby uzyskać więcej informacji dotyczących dystrybucji oprogramowania za pomocą programu SMS, zobacz Systems Management Server 2003 Concepts, Planning, and Deployment Guide (Podręcznik pojęć, planowania i wdrażania systemu Systems Management Server 2003) ([http://go.microsoft.com/fwlink/?LinkID=17401](http://go.microsoft.com/fwlink/?linkid=17401)).

Aby uzyskać więcej informacji dotyczących rozmieszczania oprogramowania klienckiego przy użyciu zasad grupy, zapoznaj się z tematami poświęconymi rozmieszczaniu oprogramowania na podstawie zasad grupy ([http://go.microsoft.com/fwlink/?LinkID=38997](http://go.microsoft.com/fwlink/?linkid=38997)).
