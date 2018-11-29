---
TOCTitle: Określanie topologii systemu RMS
Title: Określanie topologii systemu RMS
ms:assetid: 'bf516f7d-b3a1-4e7f-971f-bfab1db41812'
ms:contentKeyID: 18123399
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747651(v=WS.10)'
---

Określanie topologii systemu RMS
================================

W podstawowej topologii RMS wszystkie usługi programu RMS są dostarczane przez serwer głównej certyfikacji programu RMS lub klaster w każdym lesie usługi Active Directory. Ta topologia RMS sprawdza się w dużych i małych organizacjach. W topologii rozproszonej RMS jeden lub kilka serwerów licencji (czasami nazywanych wydziałowymi serwerami licencji) może dostarczać niektóre lub wszystkie usługi licencji określonym użytkownikom lub grupom w organizacji. Chociaż serwer (lub klaster) głównej certyfikacji nadal umożliwia całej organizacji certyfikację kont oraz usługi serwera proxy aktywacji, topologia rozproszona RMS jest przeznaczona dla organizacji o bardzo specyficznych wymaganiach dotyczących licencji i chcących zachować kontrolę nad programem RMS w określonej części organizacji.

Chociaż istnieją tylko dwie podstawowe topologie programu RMS, składniki tych topologii mogą się bardzo różnić. Aby zdefiniować składniki odpowiednie dla danej organizacji i utworzyć prawidłową topologię rozmieszczenia programu RMS, należy:

-   ocenić cele i wymagania organizacyjne,
-   zdefiniować sposób użycia zarządzania prawami dostępu,
-   dokonać analizy projektowanych wzorców ruchu i obciążeń w celu zaimplementowania odpowiedniego poziomu usługi.

Definiowanie topologii i podejmowanie decyzji niezbędnych do zaimplementowania projektu jest procesem iteracyjnym, który będzie trwał przez cały proces planowania rozmieszczenia programu RMS.

Ten temat obejmuje następujące zagadnienia:

-   [Identyfikowanie podstawowych składników](https://technet.microsoft.com/c9ec225b-0e51-42f5-aff6-0aecb62e3b27)
-   [Ustalanie celów topologii](https://technet.microsoft.com/8275a04d-3e5b-40b0-be9d-2f31b7aeca6b)
-   [Definiowanie zakresu implementacji programu RMS](https://technet.microsoft.com/4b5fe1be-643e-47c4-bf9b-50d1e97108fb)
-   [Ocenianie wymagań dotyczących skalowalności](https://technet.microsoft.com/89f0138c-946d-47d7-a286-041d4d9606a8)
-   [Zapewnianie nadmiarowości i równoważenie obciążenia](https://technet.microsoft.com/162d547c-78a7-4848-b43e-58e481832af2)
-   [Ocenianie wymagań dotyczących migracji](https://technet.microsoft.com/cec07f45-dc52-4004-860b-5cc33e5fc209)
-   [Planowanie infrastruktury serwera bazy danych](https://technet.microsoft.com/b12354bd-3143-4d1f-b5aa-450c4550653c)
-   [Planowanie rozmieszczania w wielu lasach](https://technet.microsoft.com/2dfb40b7-95b1-4362-b32e-72867544b705)
-   [Planowanie dotyczące zewnętrznych użytkowników programu RMS](https://technet.microsoft.com/107e1338-4dcf-4ed5-a49d-e875cc883db1)
-   [Planowanie podstawowej topologii programu RMS](https://technet.microsoft.com/fec3201e-201f-4faf-910e-fa44132af83d)
-   [Planowanie rozproszonej topologii programu RMS](https://technet.microsoft.com/8773a1e0-6ac3-41f5-9866-5890cef08d04)
