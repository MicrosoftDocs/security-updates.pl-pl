---
TOCTitle: Tworzenie konta usługi programu RMS
Title: Tworzenie konta usługi programu RMS
ms:assetid: '6eb38729-f0f0-431a-bc8c-17102cf175d8'
ms:contentKeyID: 18123310
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747546(v=WS.10)'
---

Tworzenie konta usługi programu RMS
===================================

Podczas instalacji program RMS tworzy grupę zabezpieczeń o nazwie **RMS Service Group** na komputerze lokalnym i udziela jej odpowiednie uprawnienia do wszystkich zasobów niezbędnych do działania programu RMS.

Podczas zastrzegania programu RMS na serwerze użytkownik określa konto użytkownika, które będzie używane jako konto usługi programu RMS. Określone konto staje się członkiem grupy RMS Service Group i tym samym otrzymuje uprawnienia skojarzone z tą grupą. Podczas normalnej pracy program RMS w większości przypadków działa na koncie usługi programu RMS.

| ![](images/Cc747546.note(WS.10).gif)Uwaga                          |
|-------------------------------------------------------------------------------------------------|
| Jako konta usługi programu RMS nie można użyć konta, za pomocą którego instalowano program RMS. |

Ze względów bezpieczeństwa zaleca się utworzenie specjalnego konta użytkownika, które będzie używane jak konto usługi programu RMS i nie będzie służyło do innych celów. Ponadto kontu temu nie należy udzielać żadnych dodatkowych uprawnień.

| ![](images/Cc747546.Important(WS.10).gif)Ważne                        |
|----------------------------------------------------------------------------------------------------|
| To specjalne konto użytkownika należy utworzyć przed zainstalowaniem i zastrzeżeniem programu RMS. |

Aby uzyskać więcej informacji dotyczących uprawnień udzielanych grupie RMS Service Group i kontom, w oparciu o które działa program RMS, zobacz „Model zabezpieczeń programu RMS” w części „Informacje techniczne dotyczące programu RMS” w tym zestawie dokumentacji.
