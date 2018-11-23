---
TOCTitle: Klucze użytkownika
Title: Klucze użytkownika
ms:assetid: '12dad6e2-64e7-4bab-bde7-b72f90f5cb05'
ms:contentKeyID: 18123181
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720202(v=WS.10)'
---

Klucze użytkownika
==================

Użytkownik programu RMS ma parę 1024-bitowych kluczy RSA. Para kluczy użytkownika jest przechowywana w bazie danych konfiguracji programu RMS, tak więc każdy użytkownik ma zawsze tę samą parę kluczy w obrębie całego systemu RMS.

Certyfikat konta praw zawiera klucz publiczny użytkownika. Ten klucz służy do szyfrowania klucza zawartości w licencji użytkowania, tak aby dzięki tej licencji tylko określony użytkownik mógł korzystać z zawartości chronionej technologią RMS.

Ten sam certyfikat konta praw zawiera również klucz prywatny użytkownika szyfrowany kluczem publicznym komputera klienckiego. Dzięki temu certyfikat konta praw może być używany tylko na komputerze, dla którego został wystawiony, a każdy certyfikat konta praw dla danego użytkownika zawiera tę samą parę kluczy. Klucz prywatny użytkownika jest wymagany do korzystania z dowolnej zawartości chronionej za pomocą technologii RMS.
