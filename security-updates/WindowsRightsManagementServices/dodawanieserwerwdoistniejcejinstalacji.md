---
TOCTitle: Dodawanie serwerów do istniejącej instalacji
Title: Dodawanie serwerów do istniejącej instalacji
ms:assetid: '7f3598ff-cd19-4daa-aa65-877f7f95a8ec'
ms:contentKeyID: 18123359
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747648(v=WS.10)'
---

Dodawanie serwerów do istniejącej instalacji
============================================

Do instalacji programu RMS można w razie potrzeby dodawać serwery w celu obsłużenia zwiększonego zapotrzebowania lub zastąpienia serwerów, które należy wycofać. Każda instalacja programu RMS musi zawierać co najmniej jeden serwer głównej certyfikacji, a opcjonalnie również dodatkowe serwery głównej certyfikacji w klastrze. Każda instalacja programu RMS może ponadto zawierać autonomiczne lub wchodzące w skład klastra serwery licencji.

Serwery do instalacji programu RMS można dodawać przy użyciu dowolnej z poniższych metod:

-   Dodając jeden lub więcej serwerów programu RMS do klastra głównej certyfikacji.
-   Dodając nowy autonomiczny serwer licencji.
-   Dodając jeden lub więcej serwerów programu RMS do klastra licencji.

**Dodawanie serwerów głównej certyfikacji**

W większości zastosowań dodanie jednego lub większej liczby serwerów programu RMS do klastra głównej certyfikacji jest najlepszym sposobem zwiększenia dostępności i nadmiarowości rozmieszczenia. Klaster głównej certyfikacji to jeden lub kilka serwerów głównej certyfikacji. W odróżnieniu od serwerów licencji, które udostępniają wyłącznie usługi licencjonowania i publikacji, serwery głównej certyfikacji udostępniają wszystkie usługi programu RMS.

Podczas instalacji i zastrzegania można wybrać opcję dodania serwera do klastra. W takim przypadku nowy serwer programu RMS jest automatycznie konfigurowany jako członek klastra. Aby uzyskać instrukcje krok po kroku dotyczące instalowania i zastrzegania serwera programu RMS w celu dodania go do klastra głównej certyfikacji, zobacz „[Instalowanie programu RMS z dodatkiem Service Pack 1](https://technet.microsoft.com/dab20175-a690-43f8-b943-768d289daa0d)” i „[Dodawanie serwera do klastra](https://technet.microsoft.com/db635238-5528-4bec-9cc6-8244e2b3d733)” w dalszej części tego tematu.

Poza opisanym tu krokiem zastrzegania, jeśli klaster tworzony jest po raz pierwszy, należy także odpowiednio skonfigurować funkcje klastrów i równoważenia obciążenia w sprzęcie lub oprogramowaniu. Jeśli klaster został już zaimplementowany, należy skonfigurować oprogramowanie lub sprzęt równoważący obciążenie do współpracy z nowym członkiem klastra.

**Dodawanie serwerów licencji**

W odróżnieniu od serwera głównej certyfikacji, który udostępnia wszystkie usługi programu RMS, serwer licencji udostępnia tylko usługi licencjonowania i publikacji.

Serwery licencji mają charakter opcjonalny i są najczęściej rozmieszczane do obsługi konkretnych wymagań związanych z licencjonowaniem, takich jak:

-   Obsługa szczególnych wymagań danego działu w zakresie zarządzania prawami dostępu. Na przykład pewna grupa w obrębie organizacji może wymagać innych zabezpieczeń zarządzania prawami dostępu niż cała organizacja i dlatego może domagać się pełnej kontroli nad implementacją licencjonowania, która jej dotyczy. Ponieważ w lesie może istnieć tylko jeden serwer głównej certyfikacji, skonfigurowanie oddzielnego serwera głównej certyfikacji nie będzie prawdopodobnie odpowiednim rozwiązaniem. W takim przypadku można skonfigurować serwer licencji lub klaster licencji dedykowany dla potrzeb tej grupy. Następnie można skonfigurować oddzielne zasady praw dla tego serwera lub klastra licencji.
-   Obsługa zarządzania prawami dostępu na potrzeby zewnętrznych partnerów firmy w sieci ekstranet, w której wymagane jest ścisłe rozdzielenie i śledzenie zasobów potrzebnych poszczególnym partnerom. Aby uzyskać więcej informacji, zobacz „[Konfigurowanie adresu URL w sieci ekstranet](https://technet.microsoft.com/88fec9ff-c96c-4d20-8856-0485e7507572)” w dalszej części tego tematu.
-   Odciążenie serwera głównej certyfikacji przez zdjęcie z niego zadań licencjonowania. Dzięki temu może wzrosnąć wydajność w organizacjach, w których istnieje tylko jeden serwer głównej certyfikacji (a nie klaster głównej certyfikacji).

W większości zastosowań zaleca się dodawanie serwerów programu RMS do klastra głównej certyfikacji, co pozwala skonfigurować nadmiarowość i równoważenie obciążenia we wszystkich serwerach występujących w rozmieszczeniu. Co prawda za pomocą serwerów licencji można także zapewnić odciążenie przy przetwarzaniu żądań licencji i publikacji, nie można jednak równoważyć obciążenia tych serwerów za pomocą klastra głównej certyfikacji. Jeśli nie istnieje konkretna potrzeba rozmieszczania oddzielnych serwerów licencji, lepiej jest równoważyć obciążenie wszystkich serwerów programu RMS przez umieszczenie ich w klastrze głównej certyfikacji.

Aby uzyskać instrukcje krok po kroku dotyczące instalowania i zastrzegania serwera licencji programu RMS, zobacz „[Instalowanie programu RMS z dodatkiem Service Pack 1](https://technet.microsoft.com/dab20175-a690-43f8-b943-768d289daa0d)” i „[Zastrzeganie serwera licencji](https://technet.microsoft.com/4d67b898-0ba9-4eef-ab7d-ee0ca55a688e)” w dalszej części tego tematu.
