---
TOCTitle: 'Krok 3. Konfigurowanie połączeń sieciowych'
Title: 'Krok 3. Konfigurowanie połączeń sieciowych'
ms:assetid: '42a144c5-f08e-4a6e-b360-47ddea77bd24'
ms:contentKeyID: 21798590
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Dd939815(v=WS.10)'
---

Krok 3. Konfigurowanie połączeń sieciowych
==========================================

Po zakończeniu instalacji programu Windows Server Update Services 3.0 z dodatkiem Service Pack 2 (WSUS 3.0 z dodatkiem SP2) zostanie automatycznie uruchomiony kreator konfiguracji. Można także uruchomić tego kreatora później na stronie **Opcje** konsoli administracyjnej programu WSUS.

Przed rozpoczęciem procesu konfiguracji należy uzyskać odpowiedzi na następujące pytania:

1. Czy zaporę serwera skonfigurowano tak, aby umożliwić klientom dostęp do serwera?

2. Czy ten komputer może nawiązać połączenie z serwerem nadrzędnym takim jak usługa Microsoft Update?

3. Czy jest znana nazwa serwera proxy i są dostępne poświadczenia użytkownika dla tego serwera, jeśli są wymagane?

Domyślnie program WSUS 3.0 z dodatkiem SP2 jest skonfigurowany tak, aby uzyskiwać aktualizacje z witryny Microsoft Update. Jeśli w sieci znajduje się serwer proxy, można skonfigurować program WSUS 3.0 z dodatkiem SP2 do używania tego serwera proxy. Jeśli między programem WSUS a Internetem znajduje się zapora firmowa, może być konieczne skonfigurowanie jej w celu umożliwienia pobierania aktualizacji przez program WSUS.

 
<table style="border:1px solid black;">
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th><img src="images/Dd939815.note(WS.10).gif" />Uwaga</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Aby można było pobierać aktualizacje z witryny Microsoft Update, niezbędne jest połączenie z Internetem, jednak program WSUS umożliwia importowanie aktualizacji do sieci niepołączonych z Internetem.
</td>
</tr>
</tbody>
</table>
 

Krok 3 obejmuje następujące procedury:

-   Konfigurowanie zapory
-   Określanie sposobu pobierania aktualizacji przez ten serwer (z witryny Microsoft Update lub innego serwera WSUS)
-   Konfigurowanie ustawień serwera proxy w celu umożliwienia programowi WSUS pobierania aktualizacji

**Aby skonfigurować zaporę**
-   Jeśli między programem WSUS a Internetem znajduje się zapora firmowa, może być konieczne skonfigurowanie jej w celu umożliwienia pobierania aktualizacji przez program WSUS. Aby uzyskać aktualizacje z witryny Microsoft Update, serwer WSUS korzysta z portu 80 (protokół HTTP) oraz portu 443 (protokół HTTPS). Tych ustawień nie można zmienić.

-   Jeśli w danej organizacji port 80 lub 443 nie może być otwarty dla wszystkich adresów, można ograniczyć dostęp tylko do następujących domen (dzięki temu program WSUS i funkcja Aktualizacje automatyczne będą mogły komunikować się z witryną Microsoft Update):

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

 
<table style="border:1px solid black;">
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th><img src="images/Dd939815.note(WS.10).gif" />Uwaga</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Te instrukcje konfiguracji zapory dotyczą sytuacji, gdy między serwerem WSUS a Internetem znajduje się zapora firnowa. Ponieważ program WSUS inicjuje cały ruch w sieci, z którego korzysta, nie ma potrzeby konfigurowania Zapory systemu Windows na serwerze WSUS.
</td>
</tr>
</tbody>
</table>
 

Mimo że połączenie między witryną Microsoft Update a programem WSUS wymaga otwartych portów 80 i 443, można skonfigurować kilka serwerów WSUS synchronizowanych za pośrednictwem portu niestandardowego.

W przypadku dwóch kolejnych procedur przyjęto założenie, że jest używany kreator konfiguracji. W dalszej części tego kroku zostanie przedstawiony sposób uruchamiania przystawki administracyjnej programu WSUS i konfigurowania serwera na stronie Opcje.

**Aby określić sposób pobierania aktualizacji przez ten serwer**
1.  Po przystąpieniu do Programu poprawy jakości rozszerzenia Microsoft Update w kreatorze konfiguracji kliknij przycisk **Dalej**, aby wybrać serwer nadrzędny.

2.  W przypadku wybrania synchronizacji z witryną Microsoft Update praca ze stroną Opcje jest zakończona. Kliknij przycisk **Dalej** lub w okienku nawigacji wybierz pozycję **Określ serwer proxy**.

3.  Jeśli wybrano synchronizację z innym serwerem WSUS, należy określić nazwę serwera i port służący do komunikacji między tym serwerem a serwerem nadrzędnym.

4.  Aby używać protokołu SSL, zaznacz pole wyboru **Użyj protokołu SSL podczas synchronizowania informacji o aktualizacjach**. W takim przypadku serwery będą używały portu 443 do synchronizacji. (Upewnij się, że zarówno ten serwer, jak i serwer nadrzędny obsługują protokół SSL).

5.  Jeśli ten serwer jest serwerem repliki, zaznacz pole wyboru **To jest replika serwera nadrzędnego**.

6.  W tym momencie konfigurowanie serwera nadrzędnego jest zakończone. Kliknij przycisk **Dalej** lub w lewym okienku nawigacji wybierz pozycję **Określ serwer proxy**.

**Aby skonfigurować ustawienia serwera proxy**
1.  Na stronie kreatora konfiguracji **Określ serwer proxy** zaznacz pole wyboru **Użyj serwera proxy podczas synchronizowania**, a następnie wpisz w odpowiednich polach nazwę i numer portu serwera proxy (domyślnie jest to port 80).

2.  Jeśli w trakcie nawiązywania połączenia z serwerem proxy mają być używane określone poświadczenia użytkownika, zaznacz pole wyboru **Użyj poświadczeń użytkownika, aby połączyć się z serwerem proxy**, a następnie w odpowiednich polach wpisz nazwę użytkownika, domenę oraz hasło użytkownika. Aby dla połączenia użytkownika z serwerem proxy włączyć opcję uwierzytelniania podstawowego, zaznacz pole wyboru **Zezwalaj na uwierzytelnianie podstawowe (hasło wysyłane zwykłym tekstem)**.

3.  W tym momencie konfigurowanie serwera proxy jest zakończone. Kliknij przycisk **Dalej**, aby przejść do następnej strony, na której można rozpocząć konfigurowanie procesu synchronizacji.

W przypadku dwóch poniższych procedur przyjęto założenie, że do konfigurowania jest używana przystawka administracyjna programu WSUS. Te dwie procedury przedstawiają sposób uruchamiania przystawki administracyjnej programu WSUS i konfigurowania serwera na stronie **Opcje**.

**Aby uruchomić konsolę administracyjną programu WSUS**
-   Aby uruchomić konsolę administracyjną programu WSUS, kliknij przycisk **Start**, wskaż polecenie **Wszystkie programy**, wskaż polecenie **Narzędzia administracyjne**, a następnie kliknij pozycję **Microsoft Windows Server Update Services 3.0**.

 
<table style="border:1px solid black;">
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th><img src="images/Dd939815.note(WS.10).gif" />Uwaga</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Aby można było korzystać ze wszystkich funkcji konsoli, należy zalogować się na serwerze z zainstalowanym programem WSUS jako członek grupy zabezpieczeń Administratorzy WSUS lub lokalnej grupy zabezpieczeń Administratorzy. Członkowie grupy zabezpieczeń Raporty WSUS mają dostęp do konsoli w trybie tylko do odczytu.
</td>
</tr>
</tbody>
</table>
 

**Aby określić źródło aktualizacji i serwer proxy**
1.  W konsoli programu WSUS w lewym okienku kliknij pozycję **Opcje** w obszarze nazwy serwera, a następnie w środkowym okienku kliknij pozycję **Źródło aktualizacji i ustawienia serwer proxy**.

    Zostanie wyświetlone okno dialogowe z kartami **Źródło aktualizacji** i **Serwer proxy**.

2.  Na karcie **Źródło aktualizacji** wybierz lokalizację, z której serwer będzie pobierać aktualizacje. W przypadku wybrania synchronizacji z witryną Microsoft Update (ustawienie domyślne) zakończono konfigurowanie ustawień na tej stronie.

3.  W przypadku wybrania synchronizacji z innym serwerem WSUS należy określić port służący do komunikacji między tymi serwerami (domyślnie jest to port 80). Wybierając inny port, należy upewnić się, że oba serwery mogą korzystać z tego portu.

4.  Można także określić, czy podczas synchronizowania z nadrzędnym serwerem WSUS ma być używany protokół SSL. W takim przypadku serwery będą używały portu 443 do synchronizacji z serwerem nadrzędnym.

5.  Jeśli ten serwer jest repliką innego serwera WSUS, zaznacz pole wyboru **To jest replika serwera nadrzędnego**. W tym przypadku wszystkie aktualizacje muszą być zatwierdzane tylko na nadrzędnym serwerze WSUS.

6.  Na karcie **Serwer proxy** zaznacz pole wyboru **Użyj serwera proxy podczas synchronizowania**, a następnie w odpowiednich polach wpisz nazwę serwera proxy oraz numer portu (domyślnie jest to port 80).

7.  Jeśli w trakcie nawiązywania połączenia z serwerem proxy mają być używane określone poświadczenia użytkownika, zaznacz pole wyboru **Użyj poświadczeń użytkownika, aby połączyć się z serwerem proxy**, a następnie w odpowiednich polach wpisz nazwę użytkownika, domenę oraz hasło użytkownika. Aby dla połączenia użytkownika z serwerem proxy włączyć opcję uwierzytelniania podstawowego, zaznacz pole wyboru **Zezwalaj na uwierzytelnianie podstawowe (hasło wysyłane zwykłym tekstem)**.

8.  Kliknij przycisk **OK**, aby zapisać wybrane ustawienia.

Następny krok
-------------

[Krok 4. Konfigurowanie aktualizacji i synchronizacji](https://technet.microsoft.com/deeaa7e1-9b50-45cb-9537-d75f70de3405)

Materiały dodatkowe
-------------------

[Program Windows Server Update Services 3.0 z dodatkiem SP2 — przewodnik krok po kroku](https://technet.microsoft.com/4b504edc-93b3-45b0-a7e8-d0107f1a4442)
