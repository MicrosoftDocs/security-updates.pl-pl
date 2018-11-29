---
TOCTitle: Monitorowanie za pomocą pakietu Microsoft Operations Manager
Title: Monitorowanie za pomocą pakietu Microsoft Operations Manager
ms:assetid: 'ce372598-7421-4f1f-b8eb-f62da26e85d1'
ms:contentKeyID: 18123460
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747758(v=WS.10)'
---

Monitorowanie za pomocą pakietu Microsoft Operations Manager
============================================================

Program RMS zawiera pakiet pakiet zarządzania, którego można używać wraz z pakietem Microsoft® Operations Manager (MOM). Pakiet MOM wspomaga zarządzanie działaniem serwerów pracujących w organizacji dzięki następującym funkcjom:

-   Monitorowanie zdarzeń umieszczanych przez program RMS w dzienniku zdarzeń aplikacji.
-   Wyróżnianie zdarzeń mogących wskazywać na potencjalne awarie usług lub problemy z konfiguracją, dzięki czemu można szybko podjąć czynności naprawcze lub zapobiegawcze.
-   Powiadamianie o ostrzeżeniach i błędach, na przykład o wygaśnięciu certyfikatu licencjodawcy serwera lub awarii usługi sieci Web.

Pakiet RMS Management Pack (RMS\_MOMPack.akm) jest instalowany wraz z programem RMS w folderze %programfiles%\\Windows Rights Management Services\\Tools.

Ten pakiet zarządzania zawiera następujące zestawy zasad, których ułatwiają administratorom systemu RMS zarządzanie rozmieszczaniem serwera programu RMS.

**Zasady pakietu zarządzania RMS MOM**

1.  PMC Measure - Activation Proxy total failure
2.  PMC Measure - Activation Proxy Total time
3.  PMC Measure - Activation Total Processing Time
4.  PMC Measure - Activation Total Reqs
5.  PMC Measure - ActivationProxy total reqs
6.  PMC Measure - AD cache (DB cache) hits
7.  PMC Measure - AD cache (DB cache) misses
8.  PMC Measure - Average License Processing time
9.  Event - Configuration Info corruption
10. PMC Measure - Dead GC connections
11. PMC Measure - Enroll failures
12. Event - General Error
13. Event - Init Failure
14. Event - Licensor Cert has expired
15. Event - Licensor Cert Request Failure
16. Zdarzenie — błąd usługi logowania
17. PMC Measure - Max GC connections available
18. Event - Missing License Acq Point generation plugin
19. PMC Measure - MSMQ Queue length on all RM servers
20. Event - No GCs available
21. Event - Plugin Init Failure
22. Event - PrivateKey protection password changed
23. Event - RM Server Shut Down
24. Event - RM Server ShutDown Failure
25. Event - Server Startup Failure
26. PMC Measure - SubEnroll failures
27. Event - SuperUser privileged override power was invoked
28. PMC Threshold - Too Many GetLicensorCert failures
29. Event - Upcoming Licensor Cert Expiry - 1 Month
30. Event - Upcoming Licensor Cert expiry - 1 Week

Więcej informacji na temat rozmieszczania pakietów zarządzania MOM w organizacji można uzyskać w [witrynie sieci Web firmy Microsoft](http://www.microsoft.com/) (http://www.microsoft.com/).
