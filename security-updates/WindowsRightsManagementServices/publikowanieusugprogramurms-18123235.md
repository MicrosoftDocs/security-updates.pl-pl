---
TOCTitle: Publikowanie usług programu RMS
Title: Publikowanie usług programu RMS
ms:assetid: '3cca9325-6bd3-49ad-aa3f-e0693205d3f4'
ms:contentKeyID: 18123235
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720247(v=WS.10)'
---

Publikowanie usług programu RMS
===============================

Adresy URL usług programu RMS są publikowane w usłudze Active Directory podczas zastrzegania serwera. Podczas zastrzegania Instalator programu RMS wysyła kwerendę do usługi Active Directory, aby określić, czy w tym lesie zostały zainstalowane inne serwery programu RMS. Jeśli nie są zainstalowane żadne inne serwery programu RMS, Instalator programu RMS konfiguruje serwer jako serwer głównej certyfikacji. Przed użyciem serwera programu RMS należy zarejestrować punkt połączenia usługi (SCP) w usłudze Active Directory, aby umożliwić klientom odnajdowanie adresu URL serwera głównej certyfikacji. Klienci żądający połączenia z usługami działającymi na serwerze głównej certyfikacji rozpoczynają tę czynność od wysłania kwerendy do usługi Active Directory w celu uzyskania adresu URL tego serwera. Aby uzyskać więcej informacji, zobacz "Rejestrowanie punktu połączenia usługi" w temacie "Obsługa serwerów programu RMS" niniejszej dokumentacji.

> [!note]  
> Jeśli topologia zawiera wiele serwerów w klastrze głównej certyfikacji, adres URL wskazuje serwer równoważenia obciążenia dla klastra określony przez administratora podczas zastrzegania. 
