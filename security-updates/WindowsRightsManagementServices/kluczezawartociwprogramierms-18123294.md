---
TOCTitle: Klucze zawartości w programie RMS
Title: Klucze zawartości w programie RMS
ms:assetid: '63c814bf-2809-477e-a2db-d90370442075'
ms:contentKeyID: 18123294
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720284(v=WS.10)'
---

Klucze zawartości w programie RMS
=================================

Gdy autor publikuje zawartość chronioną technologią RMS, aplikacja obsługująca tę technologię tworzy symetryczny klucz zawartości i używa go do zaszyfrowania zawartości. Klucz zawartości tworzony jest za pomocą technologii Advanced Encryption Standard (AES).

Klucz ten jest dołączany do licencji publikacji i jest szyfrowany kluczem publicznym serwera programu RMS wystawiającego licencję.

Po otrzymaniu żądania licencji użytkowania serwer deszyfruje klucz zawartości za pomocą klucza prywatnego serwera, a następnie ponownie szyfruje klucz zawartości kluczem publicznym użytkownika (otrzymanego jako część żądania). Klucz zawartości jest następnie dodawany do licencji użytkowania.
