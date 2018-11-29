---
TOCTitle: Korzystanie z zawartości chronionej technologią RMS
Title: Korzystanie z zawartości chronionej technologią RMS
ms:assetid: '3cf6d64b-1187-433c-bbb2-c68069bc3c30'
ms:contentKeyID: 18123233
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720251(v=WS.10)'
---

Korzystanie z zawartości chronionej technologią RMS
===================================================

Gdy użytkownicy korzystają z chronionej zawartości, występują dwa procesy niezauważalne dla użytkownika. Po pierwsze, aplikacja obsługująca technologię RMS żąda licencji użytkowania, gdy użytkownik otwiera dokument. Po drugie, aplikacja obsługująca technologię RMS bada licencję użytkowania, aby określić, czy wymaga ona listy odwoływania, i sprawdza, czy żaden certyfikat w jej łańcuchu zaufania lub w łańcuchu zaufania certyfikatu konta praw nie został odwołany. Po zakończeniu obu procesów aplikacja obsługująca technologię RMS przetwarza zawartość chronioną technologią RMS, jeśli wszystkie prawa i odwołania jej na to zezwalają.

Jeśli wymagana jest lista odwołania, aplikacja szuka lokalnej kopii listy odwołania, która nie straciła ważności. W razie potrzeby pobiera aktualną kopię listy odwołania. Następnie aplikacja stosuje warunki odwołania, które mają zastosowanie w bieżącym kontekście.

Jeśli żaden warunek odwołania nie blokuje dostępu do zawartości, aplikacja przetwarza zawartość i użytkownik może skorzystać z praw dostępu, których mu udzielono.

Można skonfigurować program RMS, tak aby przetwarzał żądania licencji użytkowania od autoryzowanych użytkowników zewnętrznych. Umożliwia to użytkownikom udostępnianie chronionej zawartości przez Internet.

Ta część zawiera następujące tematy:

-   [Uzyskiwanie licencji użytkowania](https://technet.microsoft.com/0b6cde34-418a-4dee-9d27-b65b93b535ac)
-   [Licencje użytkowania i użytkownicy zewnętrzni](https://technet.microsoft.com/02db9bda-180e-438f-863d-26252083a471)
