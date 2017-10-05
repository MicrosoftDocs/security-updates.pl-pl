---
TOCTitle: Zaufane domeny użytkowników
Title: Zaufane domeny użytkowników
ms:assetid: 'a09b883f-f455-4c46-a4fd-d37b689e1d24'
ms:contentKeyID: 18123363
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747618(v=WS.10)'
---

Zaufane domeny użytkowników
===========================

Domyślnie program RMS nie wystawia licencji użytkowania dla użytkowników, których certyfikaty kont praw zostały wystawione przez inną domenę użytkowników. Domena użytkowników jest instalacją programu RMS składającą się z klastra głównej certyfikacji, opcjonalnych serwerów lub klastrów licencji oraz skojarzonych z nimi baz danych.

Można skonfigurować program RMS, tak aby przetwarzał żądania tego typu, importując certyfikat licencjodawcy serwera z innej domeny użytkowników, a następnie dodając go do listy zaufanych domen użytkowników. W takim przypadku użytkownicy, których certyfikaty kont zostały wystawione przez zaufaną domenę użytkowników, mogą wysyłać żądania licencji użytkowania do tej instalacji. Licencje użytkowania będą przetwarzane tak jak żądania od użytkowników wewnętrznych.

| ![](images/Cc747618.note(WS.10).gif)Uwaga                                                                                          |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Klaster głównej certyfikacji jest automatycznie umieszczany na liście zaufanych domen użytkowników dla wszystkich serwerów programu RMS w tej samej instalacji. |

Można umożliwić użytkownikom z innych domen użytkowników współużytkowanie zawartości chronionej. Opisano to w poniższych przykładach:

-   Organizacja współpracuje z inną organizacją nad poufnymi dokumentami, które należy udostępniać i chronić. Zewnętrzna organizacja również posiada program RMS. Obie organizacje mogą dodać swoje instalacje programu RMS do swoich list zaufanych domen użytkowników, tak aby użytkownicy z obu organizacji mogli pracować razem nad chronioną zawartością i wymieniać zawartość przez Internet lub sieć ekstranet.
-   W każdym lesie usługi Active Directory może być tylko jedna instalacja programu RMS. Organizacja rozmieściła kilka lasów usługi Active Directory, a w każdym z nich znajduje się program RMS. Użytkownicy chcą udostępniać zawartość chronioną z innymi użytkownikami niezależnie od lasu, w którym się znajdują. Aby to umożliwić, można dodać instalacje programu RMS innych lasów do listy zaufanych domen użytkowników w każdym z lasów.
-   Użytkownicy w organizacji współpracują z użytkownikami z innej organizacji nad poufnymi dokumentami, które chcą chronić. Zewnętrzna organizacja nie posiada programu RMS. Użytkownicy w zewnętrznej organizacji mogą utworzyć konta usługi .NET Passport. Następnie można dodać konta .NET Passport do listy zaufanych domen użytkowników w instalacji programu RMS. Użytkownicy w obu firmach mogą teraz pracować nad zawartością chronioną i wymieniać zawartość przez Internet.

Aby uzyskać więcej informacji o zaufanych domenach użytkowników i instrukcjach krok po kroku, zobacz „Dodawanie i usuwanie zaufanych domen użytkowników” i „Ustanawianie zasad zaufania” w części „Obsługa serwerów programu RMS” w tym zestawie dokumentacji.
