---
TOCTitle: Konfigurowanie środowiska testowego
Title: Konfigurowanie środowiska testowego
ms:assetid: 'cdd96b05-49e2-4b6f-bfae-40b5c028ec66'
ms:contentKeyID: 18123426
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747673(v=WS.10)'
---

Konfigurowanie środowiska testowego
===================================

Program RMS integruje się z istniejącą infrastrukturą i serwerami bazy danych usługi Active Directory, np. tymi, na których jest zainstalowany program Microsoft SQL Server™ 2000. Ze względu na krytyczne znaczenie tych składników pomocniczych należy dokładnie przetestować program RMS w odizolowanym środowisku testowym przed rozmieszczeniem go w organizacji. Wymaga to skonfigurowania osobnych instalacji usługi Active Directory i serwera bazy danych w środowisku testowym.

Należy rozpocząć od najbardziej podstawowej konfiguracji serwera programu RMS w lesie z serwerem bazy danych i klientem. Po zapoznaniu się z programem RMS konfiguracja może rozrosnąć się tak, że będzie prawie tak duża jak topologia, która ma być wdrożona w środowisku produkcyjnym organizacji. Jest to związane z dodawaniem wielu lasów i dostępu zewnętrznego w miarę potrzeb. Chociaż środowisko testowe może nie zawierać wszystkich konfiguracji nadmiarowości i konfiguracji dla wielu lokacji zawartych w planach rozmieszczania w organizacji, to powinno zawierać co najmniej jeden działający serwer z każdego rodzaju składników, które zostaną rozmieszczone.

Poniższa lista zawiera informacje o minimalnych wymaganiach dotyczących konfiguracji nowego środowiska testowego, w którym można testować konfigurację podstawową dla programu RMS:

-   Kontroler domeny z systemem Windows 2000 Server z dodatkiem Service Pack 3 (SP3) lub nowszym oraz zainstalowany program SQL Server 2000 z dodatkiem SP3a. Program SQL Server obsługuje bazy danych rejestrowania, konfiguracji i usług katalogowych programu RMS. Program RMS może pracować z programem Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) w wersji A lub programem SQL Server, jeśli baza danych będzie przechowywana na tym samym serwerze, co program RMS. Jeśli do obsługi baz danych będzie używany serwer zdalny, wymagany jest program SQL Server. Program MSDE 2000 można pobrać z witryny firmy Microsoft w sieci Web.

| ![](images/Cc747673.note(WS.10).gif)Uwaga                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| System Windows 2000 Server z dodatkiem Service Pack 3 (SP3) to minimum odnośnie kontrolera domeny, ale zalecany jest system Windows Server 2003. Jest to związane z optymalizacją wydajności wynikającą z rozszerzenia grup usługi Active Directory. Zaleca się, aby korzystać z programu MSDE 2000 w celu obsługi baz danych RMS wyłącznie w środowiskach testowych, ponieważ program ten nie obsługuje żadnych interfejsów sieciowych. Ponadto warunki użytkowania programu MSDE 2000 stanowią, że nie można używać narzędzi klienta SQL do obsługi programu MSDE 2000. Dlatego nie można wyświetlać informacji dotyczących rejestrowania ani zmieniać danych przechowywanych w bazie danych konfiguracji. |

-   Serwer głównej certyfikacji z systemem Windows Server 2003, na którym zainstalowano i zastrzeżono program RMS. Jeśli to konieczne, można dodać więcej serwerów, aby utworzyć klaster głównej certyfikacji wraz z postępem testowania.
-   Komputer kliencki z systemem Windows XP Professional, klientem programu RMS i aplikacją obsługującą program RMS.
-   Konta e-mail użytkowników, których atrybuty adresów e-mail znajdują się w usłudze Active Directory.

Aby uzyskać informacje dotyczące instalacji i konfiguracji podstawowej infrastruktury programu RMS oraz spełnienia wymagań związanych z infrastrukturą w środowisku produkcyjnym, zobacz „[Konfigurowanie infrastruktury podstawowej](https://technet.microsoft.com/3a0a3a47-e755-4455-bb22-0e05053723e4)” w dalszej części tego tematu.
