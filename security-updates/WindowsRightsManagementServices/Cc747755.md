---
TOCTitle: Planowanie podstawowej topologii programu RMS
Title: Planowanie podstawowej topologii programu RMS
ms:assetid: 'fec3201e-201f-4faf-910e-fa44132af83d'
ms:contentKeyID: 18123508
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747755(v=WS.10)'
---

Planowanie podstawowej topologii programu RMS
=============================================

Topologia podstawowa programu RMS składa się z jednego lub kilku fizycznych serwerów działających jako klaster głównej certyfikacji. Ten klaster służy do certyfikowania, licencjonowania i publikowania w organizacji. W przypadku wszystkich rozmieszczeń, oprócz najmniejszych, kilka fizycznych serwerów konfiguruje się zazwyczaj jako klaster dostępny pod jednym adresem URL. Proces tworzenia tego klastra polega na zastrzeżeniu pierwszego serwera w celu utworzenia serwera głównej certyfikacji, a następnie dodawaniu serwerów do klastra, aż do chwili uzyskania liczby serwerów głównej certyfikacji niezbędnych do obsługi przewidywanej aktywności. Poniższy rysunek przedstawia tę topologię.

![](images/Cc747755.a3332719-4d25-4694-a89a-7c31fd97ca3b(WS.10).gif)

Serwery połączone w klaster współużytkują bazy danych konfiguracji i rejestrowania będące bazami danych serwera programu SQL Server. Program SQL Server może znajdować się na serwerze głównej certyfikacji lub na osobnym serwerze.

Równoważenie obciążenia konfiguruje się na wszystkich serwerach w klastrze głównej certyfikacji. Wszystkie żądania certyfikatów i licencji są przekazywane do klastra głównej certyfikacji przez wspólny adres URL określony podczas konfigurowania pierwszego serwera w tym klastrze.

Jeśli planowane jest obsługiwanie małej liczby klientów, można skonfigurować program RMS na jednym serwerze z lokalną bazą danych. Ten serwer będzie odpowiedzialny za całą certyfikację i wszystkie licencje w organizacji. Ta konfiguracja obejmuje pojedynczy punkt awarii, dlatego też zalecane jest regularne wykonywanie kopii zapasowych.
