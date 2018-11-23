---
TOCTitle: Ocenianie wymagań dotyczących migracji
Title: Ocenianie wymagań dotyczących migracji
ms:assetid: 'cec07f45-dc52-4004-860b-5cc33e5fc209'
ms:contentKeyID: 18123466
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747759(v=WS.10)'
---

Ocenianie wymagań dotyczących migracji
======================================

W organizacjach, w których rozmieszczany jest program RMS należy ustalić plan migracji minimalizujący czas wyłączenia serwera. Pozwala to na zachowanie obsługi serwera i scenariuszy uaktualniania bez wstrzymywania dostępu do zawartości chronionej technologią RMS. Ponieważ w programie RMS mogą być używane poprzednie bazy danych konfiguracji i rejestrowania, migracja programu RMS na inny serwer powinna mieć minimalny wpływ na organizację, jeśli zostaną użyte odpowiednie procedury. W scenariuszu migracji przyjęto założenie, że mają być używane istniejące bazy danych; w przeciwnym przypadku należy wykonać nową instalację programu RMS.

Jeśli w zastępowanym serwerze programu RMS używany jest sprzętowy moduł zabezpieczeń (HSM), taki jak nCipher, należy przesłać konfigurację tego modułu do nowego serwera przed zainstalowaniem i zastrzeżeniem programu RMS na serwerze. Aby uzyskać instrukcje, zobacz dokumentację dostarczoną ze sprzętowym modułem zabezpieczeń.

Przed rozpoczęciem migracji:

-   Upewnij się, że bazy danych są dostępne.
-   Zdecyduj, które komputery będą używane w nowej instalacji.

Aby przeprowadzić migrację instalacji programu RMS, należy wykonać następujące kroki:

1.  Przed rozpoczęciem migracji wykonaj kopie zapasowe wszystkich składników, w tym baz danych, kluczy prywatnych i stanu systemu.
2.  Upewnij się, że bazy danych z poprzedniej instalacji programu RMS znajdują się na serwerze bazy danych, który będzie używany w nowym rozmieszczeniu.
3.  Zainstaluj i zastrzeż program RMS na odpowiednich serwerach i określ lokalizację baz danych.

W typowym scenariuszu migracji serwera programu RMS pilotażowe rozmieszczenie programu jest przenoszone do środowiska produkcyjnego. Aby uzyskać więcej informacji o tym scenariuszu, zobacz „Przekształcanie pilotażowego rozmieszczenia programu w środowisko produkcyjne” w części „Rozmieszczanie programu RMS” w tym zestawie dokumentacji.
