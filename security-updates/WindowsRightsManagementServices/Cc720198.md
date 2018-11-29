---
TOCTitle: Używanie grupy administratorów
Title: Używanie grupy administratorów
ms:assetid: '0febcb3e-7124-4e51-971a-1013b928d33b'
ms:contentKeyID: 18123178
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720198(v=WS.10)'
---

Używanie grupy administratorów
==============================

Podczas zastrzegania program RMS tworzy specjalną grupę administratorów, której przysługuje pełna kontrola nad całą zawartością chronioną prawami. Członkom grupy administratorów udzielane są pełne prawa właścicielskie we wszystkich licencjach użytkowania wystawianych przez klaster lub serwer programu RMS, na których skonfigurowana jest ta grupa. Oznacza to, że członkowie tej grupy mogą odszyfrowywać dowolne pliki chronionej zawartości i usuwać z nich ochronę. Członek tej grupy może na przykład usunąć ochronę z plików opublikowanych przez pracownika, z którym rozwiązano umowę o pracę, dzięki czemu nowy właściciel jest w stanie publikować te pliki i zarządzać nimi.

W grupie administratorów domyślnie nie znajdują się żadni członkowie, nawet administratorzy. Za pomocą administracyjnej witryny sieci Web można określić grupę zabezpieczeń usługi Active Directory, która ma służyć jako grupa administratorów programu RMS. Można użyć istniejącej grupy usługi Active Directory lub utworzyć w tym celu nową grupę. Grupa musi istnieć w tym samym lesie usługi Active Directory, co instalacja programu RMS. Wszystkim kontom użytkowników należącym do grupy określonej jako grupa administratorów programu RMS są automatycznie przyznawane uprawnienia grupy administratorów.

Aby uzyskać informacje dotyczące sposobu określania grupy administratorów w programie RMS, zobacz „[Konfigurowanie grupy administratorów](https://technet.microsoft.com/f2ef847e-2824-471f-9079-5c343094aba8)”.

> [!note]  
> Jako grupę administratorów programu RMS można wyznaczyć tylko grupę istniejącą już w tym samym lesie usługi Active Directory, co informacja programu RMS. Właściwości tej grupy muszą obejmować adres e-mail, w tym w pełni kwalifikowaną nazwę domeny (FQDN) identyczną z nazwą konta. Adres e-mail powinien mieć format *nazwa\_grupy*@*nazwa\_domeny*. 
