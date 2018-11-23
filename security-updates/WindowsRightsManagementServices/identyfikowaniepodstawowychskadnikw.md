---
TOCTitle: Identyfikowanie podstawowych składników
Title: Identyfikowanie podstawowych składników
ms:assetid: 'c9ec225b-0e51-42f5-aff6-0aecb62e3b27'
ms:contentKeyID: 18123453
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747751(v=WS.10)'
---

Identyfikowanie podstawowych składników
=======================================

W procesie ustalania prawidłowej topologii ważna jest znajomość podstawowych składników rozmieszczenia programu RMS i ich funkcji. Na poniższej liście wymieniono serwery, które powinny być częścią rozmieszczenia programu RMS:

-   Serwery głównej certyfikacji. Serwer głównej certyfikacji jest pierwszym składnikiem rozmieszczenia programu RMS, a wszystkie inne składniki są od niego zależne. Serwer głównej certyfikacji uruchamia wszystkie usługi programu RMS, w tym usługę certyfikacji kont, która zapewnia certyfikaty kont praw klientom programu RMS w organizacji. W każdym lesie usługi Active Directory może być tylko jeden serwer głównej certyfikacji. Można jednak do instalacji dodać wiele serwerów w celu utworzenia klastra głównej certyfikacji, który będzie służył do zapewnienia nadmiarowości i równoważenia obciążenia. Wszystkie serwery będące częściami klastra głównej certyfikacji używają tej samej bazy danych konfiguracji zdefiniowanej podczas zastrzegania pierwszego serwera certyfikacji w instalacji.
-   Serwery licencji. Serwer licencji jest opcjonalny i nie jest częścią klastra głównej certyfikacji; jednak jest on podrejestrowywany w serwerze głównej certyfikacji. Serwer licencji jest zależny od serwera głównej certyfikacji w przypadku certyfikacji i innych usług (nie może dostarczać usług certyfikacji kont), ale działają na nim usługi licencji, dostarczając licencje publikacji i licencje użytkowania. Aby skonfigurować nadmiarowość oraz równoważenie obciążenia, można dodać do instalacji wiele serwerów w celu utworzenia klastra licencji. Wszystkie serwery znajdujące się w klastrze licencji używają tej samej bazy danych konfiguracji, którą zdefiniowano podczas zastrzegania pierwszego serwera licencji w klastrze.
-   Serwery uruchamiające składniki infrastruktury. Dodatkowe serwery należące do rozmieszczenia mogą zapewniać niezbędną infrastrukturę, w tym składniki takie jak program SQL Server 2000 i usługa Active Directory. Lokalizacja rozmieszczenia tych składników i liczba wymaganych serwerów są zależne od wymagań użytkownika.

Topologia programu RMS zaprojektowana dla organizacji musi uwzględniać rozmieszczenie każdego z tych składników.
