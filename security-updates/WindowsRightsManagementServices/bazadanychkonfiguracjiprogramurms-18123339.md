---
TOCTitle: Baza danych konfiguracji programu RMS
Title: Baza danych konfiguracji programu RMS
ms:assetid: '769adbdc-f32f-464b-85c4-e8b160036187'
ms:contentKeyID: 18123339
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747634(v=WS.10)'
---

Baza danych konfiguracji programu RMS
=====================================

Do przechowywania informacji dotyczących konfiguracji i zasad program RMS używa serwera bazy danych, takiego jak program Microsoft® SQL Server lub Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) wydanie A. Dla każdego serwera lub klastra programu RMS istnieje jedna baza danych konfiguracji. W tej bazie danych są przechowywane, udostępniane i pobierane dane konfiguracji, a także dane innego rodzaju.

Baza danych konfiguracji serwera lub klastra głównej certyfikacji zawiera listę tożsamości użytkowników systemu Windows oraz ich certyfikatów kont praw. Para kluczy certyfikatu jest szyfrowana do publicznego klucza serwera programu RMS przed jej zapisaniem w bazie danych. Baza danych konfiguracji serwerów licencji nie zawiera tych informacji.

Grupa RMS Service Group ma uprawnienia do wykonywania dla procedur przechowywanych w tej bazie danych.

**Ważne   **Zaleca się, aby korzystać z programu MSDE 2000 do obsługi baz danych RMS wyłącznie w środowiskach testowych, ponieważ program ten nie obsługuje żadnych interfejsów sieciowych. Oprócz tego w warunkach użytkowania programu MSDE 2000 określono, że nie można korzystać z narzędzi klienta programu SQL Server w celu obsługi bazy danych MSDE 2000. To ograniczenie uniemożliwi przeglądanie informacji rejestrowania lub zmienianie danych przechowywanych w bazie danych konfiguracji.
