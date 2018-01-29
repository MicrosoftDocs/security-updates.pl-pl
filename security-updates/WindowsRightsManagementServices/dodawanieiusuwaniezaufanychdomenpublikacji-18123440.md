---
TOCTitle: Dodawanie i usuwanie zaufanych domen publikacji
Title: Dodawanie i usuwanie zaufanych domen publikacji
ms:assetid: 'd87b502d-5497-4ccd-badf-f6807d587cee'
ms:contentKeyID: 18123440
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747687(v=WS.10)'
---

Dodawanie i usuwanie zaufanych domen publikacji
===============================================

Domyślnie serwer programu RMS może wystawiać licencje użytkowania tylko na podstawie licencji publikacji wystawionych przez siebie lub inny serwer z własnego klastra. Jeżeli zawartość została opublikowana z wykorzystaniem innego serwera głównej certyfikacji w organizacji, na przykład w lokalnym oddziale organizacji w innym lesie, lub w innej osobnej organizacji, serwer programu RMS może przyznać użytkownikom licencje użytkowania do tej zawartości, jeżeli na serwerze programu RMS zostanie skonfigurowana zaufana domena publikacji. Dodanie zaufanej domeny publikacji umożliwia skonfigurowanie zaufanej relacji między serwerem programu RMS i innym serwerem głównej certyfikacji przez zaimportowane certyfikatu licencjodawcy serwera dotyczącego innego serwera. Dla serwera programu RMS można skonfigurować nieograniczoną liczbę zaufanych domen publikacji.

Dodaną zaufaną domenę publikacji można w dowolnym momencie usunąć przez usunięcie jej certyfikatu z listy certyfikatów zaufanych domen publikacji.

Aby dodać zaufaną domenę publikacji, należy zaimportować certyfikat licencjodawcy serwera, klucz prywatny (jeśli klucz ten jest przechowywany w programowym, a nie sprzętowym module zabezpieczeń) oraz wszystkie szablony zasad praw dostępu odpowiadające serwerowi lub klastrowi programu RMS, który ma być dodany. Najpierw administrator musi wyeksportować te elementy z serwera lub klastra, który ma być objęty zaufaniem, do pliku chronionego hasłem, a następnie określić hasło wymagane do jego odszyfrowania. Administrator musi umieścić ten plik w udostępnionym folderze i przekazać użytkownikowi hasło. Następnie można zaimportować ten plik, określając jego lokalizację i hasło. Aby zapisać plik, konto, na którym uruchomiona jest pula aplikacji **Admin**, musi mieć uprawnienia do udostępnionego folderu.

Aby uzyskać instrukcje krok po kroku dotyczące ustanawiania zaufanej domeny publikacji, zobacz „[Dodawanie zaufanej domeny publikacji](https://technet.microsoft.com/731416d8-ddf4-4d4a-9f1a-bbd1ea48fe3c)” we dalszej części tego tematu.

Jeśli klucz prywatny jest przechowywany w sprzętowym module zabezpieczeń, klucz ten należy przenieść do sprzętowego modułu zabezpieczeń na zaufanym serwerze, postępując zgodnie z instrukcjami zamieszczonymi w dokumentacji sprzętowego modułu zabezpieczeń. Zależnie od typu sprzętowego modułu zabezpieczeń na każdym z serwerów oraz od konfiguracji urządzeń tego modułu, przeniesienie klucza prywatnego z jednego sprzętowego modułu zabezpieczeń do innego może nie być możliwe. Należy zapoznać się z dokumentacją sprzętowego modułu zabezpieczeń w celu określenia, czy można przenieść klucz prywatny bez spowodowania utraty danych znajdujących się w docelowym sprzętowym module zabezpieczeń. Jeśli pomyślne przeniesienie klucza prywatnego nie jest możliwe, nie jest również możliwe ustanowienie zaufanej domeny publikacji między dwoma serwerami.

> [!note]  
> Jeśli klucz prywatny programu RMS jest chroniony przy użyciu sprzętowego modułu zabezpieczeń, a import certyfikatu licencjodawcy serwera odbywa się z instalacji programu RMS, w której stosowana jest programowa ochrona klucza prywatnego, przed zaimportowaniem certyfikatu należy określić hasło klucza prywatnego na stronie Ustawienia zabezpieczeń serwera każdego serwera programu RMS w klastrze. 
