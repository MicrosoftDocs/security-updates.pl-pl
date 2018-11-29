---
TOCTitle: Włączanie obsługi programu RMS dla usług serwera
Title: Włączanie obsługi programu RMS dla usług serwera
ms:assetid: '6288323c-0638-41b6-bef8-67a7c9433424'
ms:contentKeyID: 18123291
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747593(v=WS.10)'
---

Włączanie obsługi programu RMS dla usług serwera
================================================

Program RMS może udostępniać certyfikaty konta praw i licencji użytkowania także aplikacjom serwera programu RMS Podczas konfigurowania usług serwera należy zwrócić uwagę na kilka zagadnień:

-   Listy DACL w potokach programu RMS korzystają domyślnie z ustawień o największym poziomie zabezpieczeń. W przypadku korzystania z usług serwera RMS należy zmodyfikować listę DACL.
-   Jeśli klient RMS jest zainstalowany na serwerze z systemem Windows Server 2003 i jest włączona Konfiguracja zwiększonych zabezpieczeń programu Internet Explorer, należy dodać adres URL klastra programu RMS do strefy Zaufane witryny programu Internet Explorer.
-   Wiele usług serwera korzysta z zaawansowanych funkcji usług katalogowych Active Directory, które są dostępne jedynie wtedy, gdy na wszystkich kontrolerach domeny usługi Active Directory jest zainstalowany system Windows Server 2003. W przypadku korzystania z jakichkolwiek usług serwera (na przykład Microsoft Office SharePoint Server 2007 lub Microsoft Exchange Server 2007) zalecane jest, aby na wszystkich kontrolerach domeny był zainstalowany system Windows Server 2003 oraz aby poziomy funkcjonalne domeny i lasu usługi Active Directory znajdowały się na poziomie systemu Windows Sever 2003.

Domyślna lista DACL w potoku certyfikacji serwera
-------------------------------------------------

Aplikacje, takie jak Microsoft Office SharePoint Server 2007 lub Microsoft Exchange Server 2007, obsługują technologię RMS i wymagają licencji w imieniu użytkowników. W ramach domyślnej instalacji programu RMS lista DACL potoku certyfikacji serwera RMS jest ograniczona, co oznacza, że aplikacje nie mogą uzyskiwać certyfikatów i licencji dla ich użytkowników. Jeśli jednak użytkownik posiada aplikację programu RMS dla tych komputerów, może włączyć te komputery, aby stanowiły one część systemu RMS. W tym celu musi skonfigurować listy arbitralnej kontroli dostępu (DACL) w potoku certyfikacji serwera programu RMS.

Aplikacje serwera obsługujące technologię RMS łączą się z usługą certyfikacji programu RMS, korzystając z pliku ServerCertification.asmx.

Po utworzeniu tych plików przez program RMS listy DACL plików zostaną ustawione w taki sposób, aby umożliwić dostęp tylko procesom systemowym.. Zaleca się, aby utworzyć grupę zabezpieczeń usługi Active Directory dla usług serwera, a następnie wypełnić tę grupę obiektami komputerów żądających licencji w imieniu ich użytkowników.

Po utworzeniu tych grup można zmodyfikować listę DACL dla pliku ServerCertification.asmx, aby nadać grupie uprawnienie Odczyt & Wykonywanie dla tej usługi. Należy także dodać grupę RMS Service Group do listy DACL z uprawnieniem Odczyt & Wykonywanie.

> [!note]  
> Jeśli w klastrze znajduje się więcej niż jeden serwer RMS, należy zmienić listy DACL w pliku ServerCertification.asmx file na wszystkich serwerach w klastrze. 

W przypadku programu Microsoft Exchange Server 2007 do grupy usług serwera należy dodać obiekt komputera usługi Active Directory na każdym serwerze czołowym Exchange. W przeciwnym razie serwer czołowy Exchange nie będzie obsługiwać żądań licencji w imieniu użytkowników, którzy odebrali wiadomość e-mail.

W przypadku programu Office SharePoint Server 2007 do grupy usług serwera należy dodać obiekt komputera usługi Active Directory na serwerze z programem Office SharePoint Server 2007. Jeśli konfiguracja serwera Office SharePoint Server 2007 przewiduje używanie domyślnego serwera w usłudze Active Directory, należy dodać grupę RMS Service Group oraz grupę utworzoną dla usług serwera do pliku ServiceLocater.asmx file zezwolić na uprawnienie Odczyt & Wykonywanie.

> [!Important]  
> Po zmianie listy DACL w pliku ServerCertification.asmx i ServiceLocater.asmx jest wymagane ponowne uruchomienie Internetowych usług informacyjnych (IIS). W tym celu uruchom polecenie **iisreset** z wiersza polecenia. 
