---
TOCTitle: Obsługa serwerów baz danych w programie RMS
Title: Obsługa serwerów baz danych w programie RMS
ms:assetid: 'c9844783-e6c4-49b4-8e7f-0f0377143b44'
ms:contentKeyID: 18123416
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747664(v=WS.10)'
---

Obsługa serwerów baz danych w programie RMS
===========================================

Do obsługi baz danych usług katalogowych, rejestrowania i konfiguracji program RMS używa takich serwerów baz danych, jak program SQL Server lub Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) wydanie A. Programu MSDE 2000 można użyć tylko w rozmieszczeniu z jednym serwerem. W celu uzyskania ochrony przed awariami można zaimplementować klaster serwera bazy danych.

W celu realizacji wymagań dotyczących rejestrowania można również uruchamiać bazy danych konfiguracji i rejestrowania w osobnych wystąpieniach serwera bazy danych lub rozmieścić oddzielne wystąpienie lub klaster serwera bazy danych dla serwera lub klastra głównej certyfikacji oraz klastrów licencji. Aby uzyskać więcej informacji dotyczących tych opcji, zobacz temat „Rozmieszczanie systemu RMS” w niniejszej dokumentacji.

Domyślnie grupa RMS Service group ma uprawnienia do wykonywania procedur przechowywanych dla tych baz danych. Konto użytkownika używane do logowania podczas zastrzegania ma uprawnienia właściciela dla tych baz danych.

> [!note]  
> Zaleca się używanie programu Microsoft SQL Server Desktop Engine do obsługi baz danych programu RMS tylko w środowiskach testowych, ponieważ ten program nie zawiera narzędzi niezbędnych do pełnej obsługi baz danych obejmujących całe przedsiębiorstwo. Poza tym program MSDE musi być zainstalowany na tym samym serwerze co program RMS oraz nie można dodawać dodatkowych serwerów do klastra programu RMS, gdyż program MSDE nie obsługuje zdalnej pracy w sieci. Zasady użytkowania programu Microsoft SQL Server Desktop Engine zabraniają używania narzędzi klienckich programu SQL Server do pracy z bazami danych programu Microsoft SQL Server Desktop Engine. Ograniczenie to uniemożliwia tworzenie kopii zapasowych i przywracanie baz danych konfiguracji programu RMS, przeglądanie informacji rejestrowania oraz bezpośrednie modyfikowanie danych przechowywanych w bazie danych konfiguracji. 
