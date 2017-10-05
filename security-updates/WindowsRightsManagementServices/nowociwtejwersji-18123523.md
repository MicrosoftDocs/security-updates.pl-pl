---
TOCTitle: Nowości w tej wersji
Title: Nowości w tej wersji
ms:assetid: 'c68ec6fd-0ff5-467e-85a8-a53b9f089de3'
ms:contentKeyID: 18123523
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747748(v=WS.10)'
---

Nowości w tej wersji
====================

Program Usługi zarządzania prawami dostępu (RMS) z dodatkiem Service Pack 1 (SP1) obsługuje następujące funkcje:

-   **Rejestrowanie serwera programu RMS bez połączenia serwera z Internetem**. W poprzedniej wersji serwer programu RMS musiał mieć możliwość łączenia się z Internetem w celu rejestracji w usłudze rejestrowania firmy Microsoft i uzyskania głównego certyfikatu licencjodawcy serwera. W programie RMS SP1 główny certyfikat licencjodawcy serwera uzyskuje się wciąż za pomocą usługi rejestrowania firmy Microsoft, jednak można to zrobić za pomocą innego komputera z dostępem do Internetu, a następnie zaimportować ten certyfikat na serwer programu RMS po przeprowadzeniu procesu zastrzegania.
-   **Klienci mają funkcję automatycznej aktywacji**. W poprzedniej wersji certyfikaty oraz skrytki komputerów klienckich musiały być pobierane z usługi aktywacji firmy Microsoft. W programie RMS SP1 połączenie zwrotne z usługą aktywacji firmy Microsoft nie jest wymagane.
-   **Obsługa większej liczby typów klientów**. W tej wersji za pomocą serwera programu RMS można obsługiwać klientów na urządzeniach przenośnych i w usługach serwera. Jako administrator serwera programu RMS użytkownik może kontrolować, czy serwer ma udostępniać certyfikat tym klientom, gdy próbują oni korzystać z jego usług.
-   **Obsługa szablonów w wielu językach**. W poprzedniej wersji szablony opierały się na ustawieniu języka w programie Internet Explorer. W tej wersji na administracyjnej stronie sieci Web programu RMS można określić język tworzonego szablonu.
-   **Obsługa uwierzytelniania klientów za pomocą kart inteligentnych**. W tej wersji klient programu RMS może korzystać z poświadczeń przechowywanych w certyfikatach x.509 zapisanych na kartach inteligentnych, aby uwierzytelniać poświadczenia użytkowników na serwerze programu RMS w celu uzyskania certyfikatów kont praw dostępu (RAC) oraz licencji użytkowania.
