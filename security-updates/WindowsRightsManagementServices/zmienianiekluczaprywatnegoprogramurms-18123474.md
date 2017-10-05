---
TOCTitle: Zmienianie klucza prywatnego programu RMS
Title: Zmienianie klucza prywatnego programu RMS
ms:assetid: 'da32137e-394a-42b2-9552-ba20f4547c23'
ms:contentKeyID: 18123474
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747765(v=WS.10)'
---

Zmienianie klucza prywatnego programu RMS
=========================================

Podczas zastrzegania program RMS tworzy klucz prywatny programu RMS przeznaczony dla serwera. Klucz prywatny programu RMS jest zaszyfrowany i przechowywany w bazie danych konfiguracji. Zaleca się, aby przechowywać klucz prywatny w bezpiecznej lokalizacji i wykonać jego kopię zapasową. Oprócz tego należy rozważyć zastosowanie sprzętowego modułu zabezpieczeń w celu ochrony klucza prywatnego programu RMS, ponieważ klucz ten jest używany w schemacie szyfrowania stosowanym w przypadku całej zawartości chronionej przez serwer programu RMS. Jeżeli w jakiś sposób klucz prywatny programu RMS zostanie złamany, konieczne będzie usunięcie zastrzeżenia programu RMS na serwerze, a następnie ponowne zastrzeżenie programu RMS w celu uzyskania nowego klucza prywatnego programu RMS.

Jeżeli serwer był używany do ochrony zawartości, wszyscy właściciele zawartości powinni zostać poinformowani o tym fakcie, a zawartość należy ponownie opublikować, korzystając z serwera programu RMS z nowym kluczem prywatnym. Wszystkie kopie zawartości chronione za pomocą klucza prywatnego, który został złamany, powinny zostać zniszczone, ponieważ nie są one już właściwie chronione.

| ![](images/Cc747765.Important(WS.10).gif)Ważne                                                                                                                                                                                                                                     |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Niezależnie od tego, czy serwer został zarejestrowany w usłudze rejestrowania firmy Microsoft, konieczne jest powtórzenie procesu rejestracji serwera w celu uzyskania nowego klucza prywatnego. W przypadku ponownej rejestracji serwera programu RMS zostanie użyty wcześniejszy klucz prywatny programu RMS. |
