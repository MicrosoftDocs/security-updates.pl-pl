---
TOCTitle: Problemy ze zgodnością FIPS dotyczące programu RMS
Title: Problemy ze zgodnością FIPS dotyczące programu RMS
ms:assetid: '720bdace-dcd8-431e-b0fa-01193782fe0b'
ms:contentKeyID: 18123314
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747551(v=WS.10)'
---

Problemy ze zgodnością FIPS dotyczące programu RMS
==================================================

Program Usługi zarządzania prawami dostępu (RMS) w wersji 1.0 z dodatkiem Service Pack 1 (SP1) powstał z myślą o skutecznej pracy w organizacjach wymagających stosowania funkcji kryptograficznych wykorzystujących algorytmy zgodne z normą FIPS.

Norma FIPS 140-1 (Federal Information Processing Standard 140-1) i następna, zastępująca ją, norma FIPS 140-2 zostały ustanowione przez rząd Stanów Zjednoczonych i stanowią punkt odniesienia dla wdrażania oprogramowania kryptograficznego. Zdefiniowano w nich najważniejsze wskazówki dotyczące wdrażania algorytmów kryptograficznych, obsługi kluczowych materiałów i buforów danych oraz pracy z systemem operacyjnym.

Program RMS można implementować w systemie zgodnym z normą FIPS i tworzyć w ten sposób narzędzie umożliwiające ochronę poufnych danych.

-   Dostawcy usług kryptograficznych zgodnych z normą FIPS ograniczają funkcjonalność do: **TLS\_RSA\_WITH\_3DES\_EDE\_CBC\_SHA**. To ograniczenie wymusza od dostawcy kanału zabezpieczeń negocjowanie tylko silniejszego protokołu TLS (Transport Layer Security) 1.0. Może być konieczne skonfigurowanie programu Internet Explorer, tak by obsługiwał protokół TLS. Jednak wiele serwerów sieci Web innych firm nie obsługuje tego protokołu. Aby uzyskać więcej informacji na temat tego problemu, zapoznaj się z artykułem nr 811834 z bazy wiedzy Knowledge Base w [witrynie firmy Microsoft w sieci Web](http://go.microsoft.com/fwlink/?linkid=43614.)

Klucz prywatny programu RMS można chronić za pomocą jednego z dwóch domyślnych dostawców usług kryptograficznych firmy Microsoft (CSP, Cryptographic Services Provider), jeśli ma być używana programowa ochrona klucza prywatnego. Dostawcy usług kryptograficznych spełniają odpowiednio wymagania normy FIPS 140-1 lub FIPS 140-2 rządu Stanów Zjednoczonych. Mimo że nie jest to wymagane, w wypadku klientów, dla których zabezpieczenia odgrywają kluczową rolę, zaleca się używanie sprzętowych modułów zabezpieczeń (np. nCipher lub IBM) do ochrony kluczy prywatnych serwera programu RMS wysokiego poziomu. Jeśli używane są sprzętowe moduły zabezpieczeń, dany dostawca usług kryptograficznych musi zostać wybrany do użytkowania odpowiedniego modułu. Może to wymagać ponownego uruchomienia systemu. Aby uzyskać więcej informacji na temat tego problemu, zapoznaj się z artykułem nr 830690 z bazy wiedzy Knowledge Base w [witrynie firmy Microsoft w sieci Web](http://go.microsoft.com/fwlink/?linkid=44138.)

W wypadku wdrażania systemu RMS należy postępować zgodnie z poniższymi wskazówkami.

-   Należy stosować się do zaleceń NSA dotyczących kryptografii w systemie Windows spełniającej wymagania normy FIPS.
-   Należy włączyć lokalne zasady zabezpieczeń dla kryptografii spełniającej wymagania normy FIPS.
-   W powyższym środowisku należy rozmieścić klientów i serwery RMS z dodatkiem SP1.
-   Należy włączyć protokół TLS (Transport Layer Security) w Internetowych usługach informacyjnych (IIS) na serwerze programu RMS.
-   Należy włączyć protokół TLS (Transport Layer Security) w programie Internet Explorer na potrzeby klientów.
-   Należy włączyć protokół TDS (Tabular Data Stream) dla SQL, który jest używany z dostawcą zabezpieczeń TLS/SSL systemu Windows między klientami SQL a serwerem SQL na serwerze bazy danych.
-   Należy tak skonfigurować SQL, aby wymagał protokołu TSL/SSL.
