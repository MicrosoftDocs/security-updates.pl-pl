---
TOCTitle: Odinstalowywanie i usuwanie zastrzeżenia programu RMS
Title: Odinstalowywanie i usuwanie zastrzeżenia programu RMS
ms:assetid: 'cae1ed5b-f716-41f0-8e14-7cbfef405331'
ms:contentKeyID: 18123454
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747753(v=WS.10)'
---

Odinstalowywanie i usuwanie zastrzeżenia programu RMS
=====================================================

Może się zdarzyć, że z jakiegoś powodu konieczne będzie usunięcie programu RMS z serwera. W przypadku serwera głównej certyfikacji pierwszym krokiem jest usunięcie zastrzeżenia programu RMS na tym serwerze. Czynność tę można wykonać na stronie **Administracja globalna** serwera, którego zastrzeżenie ma być usunięte, klikając łącze **Usuń program RMS z tej witryny sieci Web**. W przypadku serwera licencji nie trzeba usuwać zastrzeżenia przed odinstalowaniem programu RMS.

> [!note]  
> Usunięcie zastrzeżenia ostatniego serwera głównej certyfikacji w lesie usługi Active Directory spowoduje usunięcie z usługi Active Directory obiektu punktu połączenia usługi. Jeśli zastrzeżenie tego serwera nie zostanie usunięte przed odinstalowaniem programu RMS, nie będzie można w danym lesie zastrzec nowego serwera głównej certyfikacji do momentu ręcznego usunięcia obiektu punktu połączenia usługi z usługi Active Directory. 

Następnie należy odinstalować program RMS.

Usunięcie zastrzeżenia i odinstalowanie programu RMS z serwera autonomicznego lub z ostatniego serwera w klastrze powoduje usunięcie bazy danych usług katalogowych. Nie są usuwane bazy danych konfiguracji i rejestrowania, jeśli jednak na serwerze nastąpi uaktualnienie lub ponowna instalacja programu RMS, istniejąca baza danych rejestrowania zostanie zastąpiona nową bazą.

Usunięcie zastrzeżenia i odinstalowanie programu RMS z serwera wchodzącego w skład klastra nie powoduje usunięcia baz danych konfiguracji, rejestrowania i usług katalogowych. Następuje jednak aktualizacja tabeli DRMS\_ClusterServer w bazie danych konfiguracji, dzięki czemu odzwierciedla ona fakt usunięcia serwera z klastra.

Aby uzyskać więcej informacji dotyczących wycofywania serwerów i związanych z nim zagadnień, zobacz „[Wycofywanie serwerów](https://technet.microsoft.com/52005e2e-9563-4ba0-906c-3cc76f9c378f)” we wcześniejszej części tego tematu.
