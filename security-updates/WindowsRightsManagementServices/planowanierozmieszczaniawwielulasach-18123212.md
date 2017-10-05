---
TOCTitle: Planowanie rozmieszczania w wielu lasach
Title: Planowanie rozmieszczania w wielu lasach
ms:assetid: '2dfb40b7-95b1-4362-b32e-72867544b705'
ms:contentKeyID: 18123212
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720233(v=WS.10)'
---

Planowanie rozmieszczania w wielu lasach
========================================

Jeśli program RMS jest rozmieszczany w środowisku z wieloma lasami, należy określić, jaki typ obsługi może być wymagany w przypadku użytkowników lub grup spoza lasu, w którym zostanie rozmieszczony program RMS. Problemem jest zazwyczaj brak obiektów odpowiadających obiektom użytkowników lub grup z innych lasów w lesie, w którym znajduje się program RMS. Jeśli planowane jest użycie programu RMS do ograniczania uprawnień do użytkowników lub grup znajdujących się w innych lasach, należy odpowiednio skonfigurować las, aby było możliwe rozszerzanie grupy między lasami.

Obsługę rozszerzania grupy między lasami w programie RMS można zaimplementować na dwa sposoby:

-   rozmieszczając program RMS w lesie, w którym zdefiniowane są grupy, gdzie program będzie używany do rozszerzania przynależności do tych grup;
-   synchronizując definicje grup między lasami w celu umożliwienia lokalnej instalacji programu RMS wyznaczenia całkowitej przynależności do grupy dla dowolnego użytkownika. Jeśli użytkownik żądający licencji użytkowania ma konto systemu Windows w odrębnym lesie, w lesie lokalnym musi istnieć obiekt kontaktowy odzwierciedlający przynależność użytkownika do grupy. W celu implementacji synchronizacji o zupełnej dokładności obiektów grup między lasami można używać metakatalogów, np. Microsoft® Identity Integration Server (MIIS) 2003 lub Identity Integration Feature Pack (IIFP).

Jeśli program RMS ma być używany tylko dla jednego lasu, można zoptymalizować proces wystawiania licencji użytkowania, modyfikując zasadę klastra **MaxCrossForestCalls** w bazie danych konfiguracji programu RMS. Zasada ta określa maksymalną liczbę przekroczeń granic lasu przez członkostwo w grupie. Domyślną wartością jest 10. Aby zmienić tę wartość na 0, należy wprowadzić następujące polecenie w języku SQL:

`update DRMS_ClusterPolicies set PolicyData=0 where PolicyName='MaxCrossForestCalls'`
