---
TOCTitle: Licencje użytkowania i użytkownicy zewnętrzni
Title: Licencje użytkowania i użytkownicy zewnętrzni
ms:assetid: '02db9bda-180e-438f-863d-26252083a471'
ms:contentKeyID: 18123165
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720176(v=WS.10)'
---

Licencje użytkowania i użytkownicy zewnętrzni
=============================================

Program RMS umożliwia autorom udostępnianie zawartości chronionej autoryzowanym użytkownikom zewnętrznym przez sieć Internet. Program RMS oferuje jednakową ochronę dla zawartości publikowanej dla użytkowników wewnętrznych i zewnętrznych, ponieważ prawa dostępu dołączone do zawartości muszą być licencjonowane przez serwer programu RMS. Dzięki temu organizacje mogą pracować nad poufnymi dokumentami, takimi jak kontrakty, z użyciem sieci Internet.

Użytkownik zewnętrzny zwykle uzyskuje dostęp do serwera programu RMS przez sieć Internet. (Jeśli użytkownik zewnętrzny może uzyskać dostęp bezpośrednio do sieci wewnętrznej, na przykład za pomocą połączenia wirtualnej sieci prywatnej, jest funkcjonalnie równorzędny z użytkownikami wewnętrznymi). Niezależnie od tego czy użytkownik należy do organizacji publikującej, czy nie, proces uzyskiwania licencji użytkowania jest taki sam, jak opisany w „[Uzyskiwanie licencji użytkowania](https://technet.microsoft.com/0b6cde34-418a-4dee-9d27-b65b93b535ac)” we wcześniejszej części tego tematu. Użytkownik nie musi być wewnątrz sieci autora ani nie musi posiadać w niej konta użytkownika, aby żądać licencji użytkowania.

Wymagania są następujące:

-   Użytkownik musi posiadać ważny certyfikat konta praw.
-   Użytkownik musi mieć dostęp do serwera licencji programu RMS, który wystawił licencję publikacji. Serwer może znajdować się w sieci intranet lub ekstranet.
-   Instalacja programu RMS, która wystawiła certyfikat konta użytkownika, musi znajdować się na liście zaufanych domen użytkowników instalacji programu RMS, która wystawia licencję użytkowania.

Następujące typy użytkowników zewnętrznych mogą uzyskiwać licencje użytkowania:

-   Użytkownicy, których konta są częścią innego lasu usługi Active Directory mającego własną instalację programu RMS. Instalacja programu RMS w innym lesie musi być zdefiniowana jako zaufana domena użytkownika dla tej instalacji.
-   Użytkownicy w innej organizacji mającej instalację programu RMS, którą dodano do listy zaufanych domen użytkowników dla tej instalacji.
-   Użytkownicy posiadający certyfikaty kont praw oparte na usłudze .NET Passport, w przypadku gdy usługa certyfikacji RMS firmy Microsoft znajduje się na liście zaufanych domen użytkowników dla tej instalacji.

Osobną organizację lub inną instalację programu RMS w organizacji można dodać do listy zaufanych domen użytkowników. Po dodaniu domeny można zdefiniować zaufane domeny poczty e-mail w tej domenie, a także określić, czy należy ufać identyfikatorom zabezpieczeń (SID) w tej domenie.

Inne organizacje lub instalacje programu RMS w organizacji mogą dodawać daną instalację programu RMS do własnych list zaufanych domen użytkowników, tak aby ich serwery programu RMS mogły przetwarzać żądania licencji użytkowania od użytkowników z tej instalacji.

Aby uzyskać więcej informacji dotyczących tworzenia zaufanych domen użytkowników między instalacją programu RMS i innymi organizacjami, zobacz „[Zaufane domeny użytkowników](https://technet.microsoft.com/a09b883f-f455-4c46-a4fd-d37b689e1d24)” w dalszej części tego tematu oraz „Dodawanie i usuwanie zaufanych domen publikacji” w części „Obsługa serwerów programu RMS” w tym zestawie dokumentacji.
