---
TOCTitle: 'Krok 3. Konfigurowanie połączenia sieciowego'
Title: 'Krok 3. Konfigurowanie połączenia sieciowego'
ms:assetid: 'cd77566d-7780-4ce4-aa56-41183c65c4a7'
ms:contentKeyID: 18136874
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc708559(v=WS.10)'
---

Krok 3. Konfigurowanie połączenia sieciowego
============================================

Po zainstalowaniu programu WSUS można już korzystać z konsoli WSUS, która pozwala skonfigurować ten program i rozpocząć pracę. Domyślnie program WSUS jest skonfigurowany tak, aby aktualizacje były pobierane z witryny Microsoft Update. W przypadku korzystania w sieci z serwera proxy, należy go skonfigurować za pomocą konsoli WSUS. Jeśli między serwerem WSUS a Internetem znajduje się firmowa zapora, może być konieczne jej skonfigurowanie w celu umożliwienia pobierania aktualizacji przez program WSUS.

> [!note]  
> Aby można było pobierać aktualizacje z witryny Microsoft Update, konieczne jest połączenie z Internetem. Program WSUS umożliwia natomiast importowanie aktualizacji do sieci niepołączonych z Internetem. Więcej informacji na ten temat można znaleźć w oficjalnym dokumencie „Deploying Microsoft Windows Server Update Services” (dokument dostępny w języku angielskim). 

Krok 3 obejmuje następujące procedury:

-   Konfigurowanie zapory w celu umożliwienia programowi WSUS pobierania aktualizacji
-   Otwieranie konsoli WSUS
-   Konfigurowanie ustawień serwera proxy w celu umożliwienia programowi WSUS pobierania aktualizacji

**Aby skonfigurować zaporę:**
-   Jeśli między serwerem WSUS a Internetem znajduje się firmowa zapora, może być konieczne jej skonfigurowanie w celu umożliwienia pobierania aktualizacji przez program WSUS. Aby uzyskać aktualizacje z witryny Microsoft Update, serwer WSUS korzysta z portu 80 (protokół HTTP) oraz portu 443 (protokół HTTPS). Tych ustawień nie można zmienić.

-   Jeśli w danej organizacji te porty i protokoły nie mogą być otwarte dla wszystkich adresów, można ograniczyć dostęp tylko do następujących domen (dzięki temu program WSUS i funkcja Aktualizacje automatyczne będą mogły łączyć się z witryną Microsoft Update):

    -   http://windowsupdate.microsoft.com
    -   http://\*.windowsupdate.microsoft.com
    -   https://\*.windowsupdate.microsoft.com
    -   http://\*.update.microsoft.com
    -   https://\*.update.microsoft.com
    -   http://\*.windowsupdate.com
    -   http://download.windowsupdate.com
    -   http://download.microsoft.com
    -   http://\*.download.windowsupdate.com
    -   http://wustat.windows.com
    -   http://ntservicepack.microsoft.com

> [!note]  
> Powyższe kroki konfiguracji zapory dotyczą sytuacji, gdy między serwerem WSUS a Internetem znajduje się firnowa zapora. Ponieważ program WSUS inicjuje cały ruch w sieci (związany z realizowanymi przez siebie zadaniami), nie ma potrzeby konfigurowania zapory systemu Windows na serwerze WSUS. Mimo że połączenie między witryną Microsoft Update a programem WSUS wymaga otwartych portów 80 i 443, można skonfigurować kilka serwerów WSUS synchronizowanych za pośrednictwem portu niestandardowego. Więcej informacji na temat synchronizowania serwerów WSUS za pośrednictwem portu niestandardowego można znaleźć w oficjalnym dokumencie „Deploying Microsoft Windows Server Update Services” (dokument dostępny w języku angielskim). 

**Aby otworzyć konsolę WSUS:**
-   Na serwerze WSUS kliknij przycisk **Start**, wskaż polecenie **Wszystkie programy**, wskaż polecenie **Narzędzia administracyjne**, a następnie kliknij pozycję **Microsoft Windows Server Update Services**.

> [!note]  
> Z konsoli WSUS mogą korzystać wyłącznie użytkownicy należący do grupy zabezpieczeń Administratorzy WSUS lub lokalnej grupy zabezpieczeń Administratorzy (na serwerze z zainstalowanym programem WSUS). Jeśli do listy witryn nie zostanie dodany adres **http://&lt;***nazwa witryny WSUS w sieci Web***&gt;** (w strefie Lokalny intranet w przeglądarce Microsoft Internet Explorer zainstalowanej w systemie Windows Server 2003), przy każdorazowym otwarciu konsoli WSUS może być konieczne podanie poświadczeń. Jeśli po zainstalowaniu programu WSUS zostanie zmieniony przydział portu w programie IIS, będzie konieczne ręczne zaktualizowanie skrótu w menu **Start**. Konsolę WSUS można otworzyć w przeglądarce Internet Explorer na dowolnym serwerze lub komputerze w sieci po wprowadzeniu następującego adresu URL: **http://***nazwa\_serwera\_WSUS***/WSUSAdmin** 

**Aby określić serwer proxy:**
1.  Na pasku narzędzi konsoli WSUS kliknij ikonę **Opcje**, a następnie kliknij pozycję **Opcje synchronizacji**.

2.  W obszarze **Serwer proxy** zaznacz pole wyboru **Użyj serwera proxy podczas synchronizowania**, a następnie w odpowiednich polach wpisz nazwę serwera proxy oraz numer portu (domyślnie jest to port 80).

3.  Jeśli w trakcie nawiązywania połączenia z serwerem proxy mają być używane określone poświadczenia użytkownika, zaznacz pole wyboru **Użyj poświadczeń użytkownika, aby połączyć się z serwerem proxy**, a następnie w odpowiednich polach wpisz nazwę użytkownika, domenę oraz hasło użytkownika. Aby dla połączenia użytkownika z serwerem proxy włączyć opcję uwierzytelniania podstawowego, zaznacz pole wyboru **Zezwalaj na uwierzytelnianie podstawowe (hasło wysyłane zwykłym tekstem)**.

4.  W obszarze **Zadania** kliknij pozycję **Zapisz ustawienia**, a następnie kliknij przycisk **OK** w oknie dialogowym z potwierdzeniem.
