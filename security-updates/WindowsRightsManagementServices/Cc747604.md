---
TOCTitle: Obsługa usług Active Directory w programie RMS
Title: Obsługa usług Active Directory w programie RMS
ms:assetid: '9589127d-19b3-44f1-b7a1-01992e78218a'
ms:contentKeyID: 18123351
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747604(v=WS.10)'
---

Obsługa usług Active Directory w programie RMS
==============================================

Program RMS używa usługi Active Directory w następujących celach:

-   **Uwierzytelnianie użytkowników.** Usługa Active Directory udostępnia usługi katalogowe używane do uwierzytelniania użytkowników programu RMS. Aby uzyskać więcej informacji dotyczących uwierzytelniania i programu RMS, zobacz „[Model zabezpieczeń w programie RMS](https://technet.microsoft.com/665db831-366d-4dca-9bb3-cc2912481fe1) w dalszej części tego tematu.
-   **Rozpoznawanie członkostwa w grupach oraz indywidualnych tożsamości kont użytkowników.** Usługa Active Directory dostarcza informacje o członkostwie w grupach, których program RMS używa w celu udzielania licencji użytkowania dla zawartości chronionej technologią RMS, w przypadku gdy licencja publikacji udziela prawa dostępu grupom, a nie pojedynczym kontom użytkowników. W celu zmniejszenia liczby kwerend LDAP wysyłanych do usługi Active Directory program RMS przechowuje uzyskane informacje w lokalnej pamięci podręcznej, a także w scentralizowanej bazie danych usług katalogowych. Aby uzyskać więcej informacji, zobacz „[Pamięć podręczna usługi Active Directory programu RMS](https://technet.microsoft.com/c721a2eb-2fe9-4346-b426-3cc169b97265)” i „[Baza danych usług katalogowych programu RMS](https://technet.microsoft.com/6f6b8586-5d17-4a40-94a3-4dc738195301)” we wcześniejszej części tego tematu.
-   **Przechowywanie lokalizacji odnajdowania usługi programu RMS.** Żądania usług (takie jak żądania licencji użytkowania, licencji publikacji lub podrejestracji serwera licencji) muszą być wysyłane na adres URL modułu wykonywalnego usługi sieci Web, która udziela żądania. Wszystkie żądania usługi zaczynają się kwerendą do usługi Active Directory dla adresu URL serwerowej usługi sieci Web (Server.asmx), co w rezultacie dostarcza odpowiedni adres URL dla żądania usługi. Aby uzyskać więcej informacji, zobacz „[Publikowanie i wykrywanie usług w programie RMS](https://technet.microsoft.com/336c0d55-fd7f-4aa9-b3e6-bfd6565b1086)” w dalszej części tego tematu.
