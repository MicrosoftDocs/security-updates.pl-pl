---
TOCTitle: Definiowanie wymagań zarządzania kluczami
Title: Definiowanie wymagań zarządzania kluczami
ms:assetid: 'f0e08fb8-bf5e-4278-a09f-daa57696e786'
ms:contentKeyID: 18123516
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747797(v=WS.10)'
---

Definiowanie wymagań zarządzania kluczami
=========================================

Program RMS używa kluczy kryptograficznych do zapewnienia ochrony zawartości oraz przestrzegania praw dostępu. Klucze kryptograficzne są podstawowymi elementami danych, które umożliwiają systemowi płynną i bezpieczną pracę. Administratorzy muszą dbać o prawidłowe zarządzanie tymi kluczami, aby zapobiegać utracie danych, awariom systemu oraz kradzieżom.

W konfiguracji domyślnej program RMS przechowuje parę kluczy serwera i powiązany z nią identyfikator GUID w tabeli znajdującej się w bazie danych konfiguracji. Para kluczy serwera jest szyfrowana hasłem wybieranym w procesie zastrzegania.

W celu dodatkowego zabezpieczenia pary kluczy serwera i powiązanego z nią identyfikatora GUID należy utworzyć kopię zapasową bazy danych konfiguracji na nośniku (na przykład dysku CD), a następnie umieścić nośnik w bezpiecznej lokalizacji (na przykład w zewnętrznym sejfie). Planowanie tworzenia kopii zapasowych zależy od tego, jak często dokonywane są zmiany administracyjne oraz od dopuszczalnego ryzyka utraty danych z powodu uszkodzenia nośnika lub innych niebezpieczeństw związanych z nośnikami. Należy zapewnić sobie możliwość poznania hasła klucza prywatnego, zastosowanego w bazie danych konfiguracji, dla której utworzono kopię zapasową. Bez odpowiedniego hasła przywrócenie kopii zapasowej na serwerze programu RMS będzie niemożliwe.

Jeśli używanym serwerem bazy danych jest program SQL Server, można użyć programu SQL Server Enterprise Manager do bezpośredniego skopiowania wartości zaszyfrowanych danych klucza prywatnego oraz identyfikatorów GUID na zabezpieczoną dyskietkę lub inny nośnik. Ponieważ klucz prywatny jest chroniony, instalacja programu RMS musi działać z użyciem tego samego konta usługi programu RMS co kopia zapasowa przywrócona z bezpiecznego nośnika do instalacji RMS.

W przypadku korzystania z programowego lub sprzętowego dostawcy usług kryptograficznych (CSP) do ochrony klucza prywatnego serwera należy ręcznie utworzyć kopię zapasową kontenera klucza oraz klucza. Użycie sprzętowego modułu zabezpieczeń zwiększa bezpieczeństwo kluczy prywatnych dzięki przechowywaniu kluczy w urządzeniu sprzętowym i nie udostępnianiu ich w oprogramowaniu. Dane do szyfrowania lub podpisywania są przekazywane do sprzętowego modułu zabezpieczeń, tam są szyfrowane lub podpisywane, a następnie zwracane.

Każdy dostawca usług kryptograficznych (zarówno sprzętowy, jak i programowy) ma określone procedury bezpiecznego tworzenia kopii zapasowych kluczy. Informacje na temat tych procedur można znaleźć w dokumentacji danego dostawcy CSP.
