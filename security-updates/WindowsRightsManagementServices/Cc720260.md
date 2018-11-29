---
TOCTitle: Rejestrowanie punktu połączenia usługi
Title: Rejestrowanie punktu połączenia usługi
ms:assetid: '446d83ec-3224-45e2-9697-625e7db338f3'
ms:contentKeyID: 18123243
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720260(v=WS.10)'
---

Rejestrowanie punktu połączenia usługi
======================================

Punkt połączenia usługi (SCP) w programie RMS określa adres URL połączenia danej usługi na potrzeby istniejących w organizacji klientów obsługujących technologię RMS. Bez prawidłowego punktu SCP klienci nie są w stanie odnaleźć programu RMS w celu żądania licencji użytkowania, licencji publikacji lub certyfikatów konta praw.

Adres URL punktu SCP dla klastra głównej certyfikacji można zarejestrować na stronie **Punkt połączenia usługi** w administracyjnej witrynie sieci Web. Jeśli z jakiegoś powodu wystąpi potrzeba zresetowania adresu URL punktu SCP, adres ten można także wyrejestrować na stronie **Punkt połączenia usługi**. Aby zarejestrować lub wyrejestrować adres URL punktu SCP, użytkownik musi być zalogowany przy użyciu prawidłowego konta użytkownika domeny, którego uprawnienia wystarczają do utworzenia obiektu kontenera w kontenerze Usługi.

W kontenerze usług w usłudze Active Directory zostanie utworzony nowy obiekt kontenera o nazwie „RightsManagementServices”. W tym kontenerze zostanie utworzony obiekt SCP o nazwie „MSRMRootCluster”. Atrybut keywords w tym obiekcie SCP ma dwie wartości:

-   MSRMRootCluster
-   1.0

Są to atrybuty, za pomocą których klienci i inne serwery odnajdują adres URL głównego klastra w usłudze Active Directory. Parametr serviceBindingInformation w obiekcie SCP będzie zawierać adres URL głównego klastra w postaci http://*nazwa\_klastra*/\_wmcs/Certification.
