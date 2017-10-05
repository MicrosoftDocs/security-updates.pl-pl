---
TOCTitle: 'Krok 3. Konfigurowanie połączenia sieciowego w programie WSUS 3.0'
Title: 'Krok 3. Konfigurowanie połączenia sieciowego w programie WSUS 3.0'
ms:assetid: 'dbc9d9f7-cf52-4539-9f9e-3e823273218a'
ms:contentKeyID: 18136858
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc708602(v=WS.10)'
---

Krok 3. Konfigurowanie połączenia sieciowego w programie WSUS 3.0
=================================================================

Po zainstalowaniu programu WSUS 3.0 zostanie automatycznie uruchomiony kreator konfiguracji. Można także uruchomić go później za pośrednictwem strony **Opcje** konsoli programu WSUS 3.0.

Przed rozpoczęciem procesu konfiguracji należy uzyskać odpowiedzi na następujące pytania:

1. Czy zaporę serwera skonfigurowano tak, aby umożliwić klientom dostęp do serwera?

2. Czy ten komputer może nawiązać połączenie z serwerem nadrzędnym takim jak usługa Microsoft Update?

3. Czy znana jest nazwa serwera proxy i poświadczenia użytkownika dla tego serwera, jeśli są wymagane?

Domyślnie program WSUS jest skonfigurowany tak, aby aktualizacje były pobierane z witryny Microsoft Update. W przypadku korzystania w sieci z serwera proxy należy skonfigurować program WSUS w celu użycia tego serwera proxy. Jeśli między serwerem WSUS a Internetem znajduje się zapora firmowa, może być konieczne jej skonfigurowanie w celu umożliwienia pobierania aktualizacji przez program WSUS.

| ![](images/Cc708602.note(WS.10).gif)Uwaga                                                                                                                                    |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Aby można było pobierać aktualizacje z witryny Microsoft Update, konieczne jest połączenie z Internetem. Program WSUS umożliwia natomiast importowanie aktualizacji do sieci niepołączonych z Internetem. |

**Krok 3 obejmuje następujące procedury**:

-   Konfigurowanie zapory
-   Określanie sposobu pobierania aktualizacji przez ten serwer (z witryny Microsoft Update lub innego serwera WSUS)
-   Konfigurowanie ustawień serwera proxy w celu umożliwienia programowi WSUS pobierania aktualizacji

**Aby skonfigurować zaporę**
-   Jeśli między serwerem WSUS a Internetem znajduje się zapora firmowa, może być konieczne jej skonfigurowanie w celu umożliwienia pobierania aktualizacji przez program WSUS. Aby uzyskać aktualizacje z witryny Microsoft Update, serwer WSUS korzysta z portu 80 (protokół HTTP) oraz portu 443 (protokół HTTPS). Tych ustawień nie można zmienić.

-   Jeśli w danej organizacji porty 80 lub 443 nie mogą być otwarte dla wszystkich adresów, można ograniczyć dostęp tylko do następujących domen (dzięki temu program WSUS i funkcja Aktualizacje automatyczne będą mogły łączyć się z witryną Microsoft Update):

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

| ![](images/Cc708602.note(WS.10).gif)Uwaga                                                                                                                                                                                                                             |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Te instrukcje konfiguracji zapory dotyczą sytuacji, gdy między serwerem WSUS a Internetem znajduje się zapora firnowa. Ponieważ program WSUS inicjuje cały ruch w sieci (związany z realizowanymi przez siebie zadaniami), nie ma potrzeby konfigurowania zapory systemu Windows na serwerze WSUS. |

Mimo że połączenie między witryną Microsoft Update a programem WSUS wymaga otwartych portów 80 i 443, można skonfigurować kilka serwerów WSUS synchronizowanych za pośrednictwem portu niestandardowego.

W przypadku dwóch kolejnych procedur przyjęto założenie, że jest używany kreator konfiguracji. W dalszej części tego kroku zostanie przedstawiony sposób uruchamiania przystawki administracyjnej programu WSUS i konfigurowania serwera za pomocą strony **Opcje**.

**Aby określić sposób pobierania aktualizacji przez ten serwer**
1.  Po przystąpieniu do Programu poprawy jakości firmy Microsoft w kreatorze konfiguracji kliknij przycisk **Dalej**, aby wybrać serwer nadrzędny.

2.  W przypadku wybrania synchronizacji z witryną Microsoft Update zakończono konfigurowanie ustawień na tej stronie. Kliknij przycisk **Dalej** lub wybierz w lewym okienku pozycję **Określ serwer proxy**.

3.  Jeśli wybrano synchronizację z innym serwerem WSUS, należy określić nazwę serwera i port służący do komunikacji między tym serwerem a serwerem nadrzędnym.

4.  Aby używać protokołu SSL, zaznacz pole wyboru **Użyj protokołu SSL podczas synchronizowania informacji o aktualizacjach**. W takim przypadku serwery będą używały portu 443 do synchronizacji. Należy upewnić się, że ten serwer oraz serwer nadrzędny obsługują protokół SSL.

5.  Jeśli ten serwer jest serwerem repliki, zaznacz pole wyboru **To jest replika serwera nadrzędnego**.

6.  W ten sposób zakończono konfigurowanie serwera nadrzędnego. Kliknij przycisk **Dalej** lub wybierz w lewym panelu pozycję **Określ serwer proxy**.

**Aby skonfigurować ustawienia serwera proxy**
1.  Na stronie kreatora konfiguracji **Określ serwer proxy** zaznacz pole wyboru **Użyj serwera proxy podczas synchronizowania**, a następnie wpisz w odpowiednich polach nazwę i numer portu serwera proxy (domyślnie jest to port 80).

2.  Jeśli w trakcie nawiązywania połączenia z serwerem proxy mają być używane określone poświadczenia użytkownika, zaznacz pole wyboru **Użyj poświadczeń użytkownika, aby połączyć się z serwerem proxy**, a następnie w odpowiednich polach wpisz nazwę użytkownika, domenę oraz hasło użytkownika. Aby dla połączenia użytkownika z serwerem proxy włączyć opcję uwierzytelniania podstawowego, zaznacz pole wyboru **Zezwalaj na uwierzytelnianie podstawowe (hasło wysyłane zwykłym tekstem)**.

3.  W ten sposób zakończono konfigurowanie serwera proxy. Kliknij przycisk **Dalej**, aby przejść do następnej strony, na której można rozpocząć konfigurowanie procesu synchronizacji.

W przypadku dwóch poniższych procedur przyjęto założenie, że do konfigurowania jest używana przystawka administracyjna programu WSUS. Te dwie procedury przedstawiają sposób uruchamiania przystawki administracyjnej programu WSUS i konfigurowania serwera za pomocą strony **Opcje**.

**Aby uruchomić konsolę administracyjną programu WSUS**
-   Aby uruchomić konsolę administracyjną programu WSUS, kliknij przycisk **Start**, wskaż kolejno polecenia **Wszystkie programy** i **Narzędzia administracyjne**, a następnie kliknij pozycję **Microsoft Windows Server Update Services 3.0**.

| ![](images/Cc708602.note(WS.10).gif)Uwaga                                                                                                                                                                                                                                                                   |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Ze wszystkich funkcji konsoli WSUS mogą korzystać wyłącznie użytkownicy należący do grupy zabezpieczeń Administratorzy WSUS lub lokalnej grupy zabezpieczeń Administratorzy (na serwerze z zainstalowanym programem WSUS). Jednakże członkowie grupy zabezpieczeń Raporty WSUS mają dostęp tylko do odczytu do konsoli administracyjnej. |

**Aby określić źródło aktualizacji i serwer proxy**
1.  W konsoli programu WSUS kliknij w lewym panelu pozycję **Opcje** poniżej nazwy serwera, a następnie kliknij w środkowym panelu pozycję **Źródło aktualizacji i ustawienia serwera proxy**.

2.  Zostanie wyświetlone okno dialogowe z kartami **Źródło aktualizacji** i **Serwer proxy**.

3.  Na karcie **Źródło aktualizacji** wybierz lokalizację, z której serwer będzie pobierać aktualizacje. W przypadku wybrania synchronizacji z witryną Microsoft Update (ustawienie domyślne) zakończono konfigurowanie ustawień na tej stronie.

4.  Jeśli wybrano synchronizację z innym serwerem WSUS, należy określić port służący do komunikacji między serwerami (domyślnie jest to port 80). W przypadku wybrania innego portu należy upewnić się, że oba serwery mogą korzystać z tego portu.

5.  Można także określić, czy podczas synchronizowania z nadrzędnym serwerem WSUS ma być używany protokół SSL. W takim przypadku serwery będą używały portu 443 do synchronizacji z serwerem nadrzędnym.

6.  Jeśli ten serwer jest repliką innego serwera WSUS, zaznacz pole wyboru **To jest replika serwera nadrzędnego**. W tym przypadku wszystkie aktualizacje muszą być zatwierdzane tylko na nadrzędnym serwerze WSUS.

7.  Na karcie **Serwer proxy** zaznacz pole wyboru **Użyj serwera proxy podczas synchronizowania**, a następnie w odpowiednich polach wpisz nazwę serwera proxy oraz numer portu (domyślnie jest to port 80).

8.  Jeśli w trakcie nawiązywania połączenia z serwerem proxy mają być używane określone poświadczenia użytkownika, zaznacz pole wyboru **Użyj poświadczeń użytkownika, aby połączyć się z serwerem proxy**, a następnie w odpowiednich polach wpisz nazwę użytkownika, domenę oraz hasło użytkownika. Aby dla połączenia użytkownika z serwerem proxy włączyć opcję uwierzytelniania podstawowego, zaznacz pole wyboru **Zezwalaj na uwierzytelnianie podstawowe (hasło wysyłane zwykłym tekstem)**.

9.  Kliknij przycisk **OK**, aby zapisać wybrane ustawienia.
