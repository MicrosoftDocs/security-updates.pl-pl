---
TOCTitle: Grupy zabezpieczeń w programie RMS
Title: Grupy zabezpieczeń w programie RMS
ms:assetid: '25749a83-8c12-48ec-96ad-296d31fd55d4'
ms:contentKeyID: 18123208
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720215(v=WS.10)'
---

Grupy zabezpieczeń w programie RMS
==================================

Instalator programu RMS tworzy dwie grupy: RMS Service Group oraz Administratorzy.

Grupa RMS Service Group jest lokalną grupą zabezpieczeń, której udzielane są odpowiednie uprawnienia do uzyskiwania dostępu do wszystkich zasobów wymaganych do działania programu RMS. Podczas instalacji administrator określa konto użytkownika, które będzie używane jako konto usługi programu RMS. To konto użytkownika jest automatycznie dodawane do grupy RMS Service Group i przez to otrzymuje jej uprawnienia. Program RMS wykonuje większość normalnych operacji jako to konto użytkownika.

Inną ważną grupą programu RMS jest grupa Administratorzy. Ta grupa ma pełną kontrolę nad całą zawartością, co oznacza, że członek tej grupy może deszyfrować wszystkie pliki zawartości chronionej technologią RMS i usuwać ochronę dla całej zawartości. Grupa Administratorzy domyślnie nie ma członków i nie uwzględnia automatycznie administratorów programu RMS. Zarządzanie członkostwem w tej grupie jest kluczowe dla zabezpieczeń zawartości chronionej technologią RMS. Aby uzyskać więcej informacji, zobacz „Używanie grupy administratorów” w części „Obsługa serwerów programu RMS” w tym zestawie dokumentacji.
