---
TOCTitle: Alternatywy do likwidacji programu RMS
Title: Alternatywy do likwidacji programu RMS
ms:assetid: '4d32f35e-997d-4d10-ab66-efe217e853f7'
ms:contentKeyID: 18123257
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720268(v=WS.10)'
---

Alternatywy do likwidacji programu RMS
======================================

Jeśli nadal planujesz korzystać z programu RMS w organizacji, ale z pewnych przyczyn musisz zaprzestać używania określonych serwerów programu RMS, rozważ poniższe rozwiązania alternatywne wobec likwidacji.

**Konfigurowanie zaufanej domeny publikacji**

Wszystkie informacje chronione za pomocą technologii RMS są szyfrowane przy użyciu klucza prywatnego serwera programu RMS. Zaufana domena publikacji umożliwia importowanie klucza prywatnego jednego serwera programu RMS do innego serwera programu RMS. Dzięki temu serwer programu RMS może wystawiać licencje użytkowania na podstawie licencji publikacji utworzonych na innym serwerze programu RMS. Po wyeksportowaniu klucza można usunąć zastrzeżenie serwera, a sam serwer odinstalować.

**Konfigurowanie grupy administratorów**

Jeśli nie można otworzyć zawartości chronionej za pomocą programu RMS, ponieważ żaden użytkownik nie ma do niej uprawnień, można udzielić pełnej kontroli nad całą zawartością chronioną za pomocą programu RMS publikowaną przez dany serwer grupie administratorów. Członkom grupy administratorów udzielane są pełne prawa właścicielskie we wszystkich licencjach użytkowania wystawianych przez klaster lub serwer programu RMS, na których skonfigurowana jest ta grupa. Oznacza to, że członkowie tej grupy mogą odszyfrowywać dowolne pliki chronionej zawartości i usuwać z nich ochronę. Członek tej grupy może na przykład usunąć ochronę z plików opublikowanych przez pracownika, z którym rozwiązano umowę o pracę, dzięki czemu nowy właściciel jest w stanie publikować te pliki i zarządzać nimi.

W grupie administratorów nie są automatycznie umieszczani żadni członkowie, nawet administratorzy. Grupa ta musi istnieć w usłudze Active Directory jako grupa dystrybucyjna posiadająca atrybut adresu e-mail o tej samej wartości co nazwa grupy w formacie „*nazwa\_grupy*@*nazwa\_domeny*.com”. Nazwa grupy musi być dokładnie taka sama jak atrybut adresu e-mail. Uwzględniana jest w niej wielkość liter.
