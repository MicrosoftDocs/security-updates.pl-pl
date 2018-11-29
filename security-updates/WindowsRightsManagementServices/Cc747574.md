---
TOCTitle: Zabezpieczanie serwerów programu RMS
Title: Zabezpieczanie serwerów programu RMS
ms:assetid: '7e6c4d3a-6cfb-4e96-9dda-ead83f961a6e'
ms:contentKeyID: 18123325
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747574(v=WS.10)'
---

Zabezpieczanie serwerów programu RMS
====================================

Aby ułatwić sobie zarządzanie kontami użytkowników i ustawieniami zabezpieczeń na serwerach programu RMS, można skorzystać z poniższych zaleceń:

-   Katalogi wirtualne witryny sieci Web, która służy do administrowania programem RMS, zawierają swobodne listy kontroli dostępu (DACL), które ograniczają dostęp do lokalnych administratorów. W celu bardziej szczegółowej kontroli dostępu lokalny administrator może utworzyć dodatkową grupę zabezpieczeń przez dodanie lub usunięcie członków oraz przez ustawienie dodatkowych wpisów kontroli dostępu (ACE) na administracyjnych stronach sieci Web.
-   W celu uzyskania lepszych zabezpieczeń należy zmienić ustawienia list DACL dotyczące strony sieci Web Ustawienia zabezpieczeń (SecurityPolicy.aspx). Aby umożliwić zastrzeganie, domyślny wpis ACE udziela pełnej kontroli kontu, które dokonuje zastrzeżenia programu RMS. Po zastrzeganiu wpis ACE należy zmienić na pojedynczy podmiot lub na grupę zabezpieczeń podlegającą ograniczeniom.
-   Poza uprawnieniami i prawami do każdego serwera programu RMS należy zwrócić szczególną uwagę na wymagania związane z zabezpieczeniem bazy danych konfiguracji, które istotnie wpływa na zabezpieczenie całego rozmieszczenia. Aby uzyskać więcej informacji, zobacz „[Zabezpieczanie bazy danych konfiguracji](https://technet.microsoft.com/e023b96f-81d0-45fb-8cc5-becaf6d47ae1)” w dalszej części tego tematu.

Aby uzyskać więcej informacji na temat zabezpieczania programu Microsoft SQL Server™, odwiedź stronę sieci Web **SQL Server Security** (Zabezpieczenia programu SQL Server) dostępnej w [witrynie sieci Web firmy Microsoft](http://www.microsoft.com/) (http://www.microsoft.com/).

Aby uzyskać więcej informacji na temat zabezpieczania komputerów, na których uruchomiony jest system operacyjny z rodziny Microsoft Windows Server 2003, pobierz „Windows Server 2003 Security Guide” (Podręcznik zabezpieczeń systemu Windows Server 2003) z Centrum pobierania firmy Microsoft, które znajduje się w [witrynie sieci Web firmy Microsoft](http://www.microsoft.com/) (http://www.microsoft.com/).
