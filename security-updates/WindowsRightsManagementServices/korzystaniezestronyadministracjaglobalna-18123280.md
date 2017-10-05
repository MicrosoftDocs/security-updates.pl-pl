---
TOCTitle: Korzystanie ze strony Administracja globalna
Title: Korzystanie ze strony Administracja globalna
ms:assetid: '57bbf402-2351-4dee-823c-27f4dd32447c'
ms:contentKeyID: 18123280
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747575(v=WS.10)'
---

Korzystanie ze strony Administracja globalna
============================================

Na stronie **Administracja globalna** w witrynie administracyjnej sieci Web można zastrzec oraz usunąć zastrzeżenie serwera programu RMS, a także zmienić konto usługi programu RMS.

Aby uzyskać dostęp do tej strony sieci Web z serwera, którego ma dotyczyć administrowanie, wykonaj następujące kroki:

1.  Zaloguj się jako administrator lokalny.
2.  Kliknij przycisk **Start**, wskaż polecenie **Wszystkie programy**, wskaż polecenie **Windows RMS**, a następnie kliknij polecenie **Administracja programem Windows RMS**.

Dostępu do strony **Administracja globalna** nie można uzyskać z przeglądarki na komputerze zdalnym.

Jeśli nie zastrzeżono jeszcze serwera, z którego uzyskiwany jest dostęp do strony **Administracja globalna**, dla każdej witryny sieci Web uruchomionej na serwerze wyświetlane są następujące opcje:

-   **Zastrzeż program RMS w tej witrynie sieci Web**. Łącze to należy kliknąć, jeśli jest to pierwszy serwer, który ma być zastrzeżony w danym klastrze. Spowoduje to uruchomienie procesu zastrzegania, w trakcie którego instalowane są zasoby programu RMS, na przykład katalogi wirtualne. Ponadto na serwerze bazy danych instalowane są bazy danych. Aby uzyskać więcej informacji, zobacz „[Zastrzeganie pierwszego serwera głównej certyfikacji](https://technet.microsoft.com/debc42f3-74ff-4c99-b7a4-4921fccdabc2)” w dalszej części tego tematu.
-   **Dodaj ten serwer do klastra**. To łącze należy kliknąć, jeśli serwer ma zostać zastrzeżony i dodany do istniejącego klastra. Serwer można dołączyć do klastra głównej certyfikacji lub klastra licencji. Instalowane są zasoby programu RMS, na przykład katalogi wirtualne. Nie są jednak tworzone bazy danych, ponieważ serwer ten będzie korzystać z baz danych klastra. Aby uzyskać więcej informacji, zobacz „[Dodawanie serwera do klastra](https://technet.microsoft.com/db635238-5528-4bec-9cc6-8244e2b3d733)” w dalszej części tego tematu.

Jeśli dostęp do strony **Administracja globalna** uzyskiwany jest z serwera, który już został zastrzeżony, wyświetlane są następujące opcje:

-   **Administruj programem RMS w tej witrynie sieci Web.** To łącze należy kliknąć, aby wyświetlić stronę Administrowanie klastrem. Aby uzyskać więcej informacji, zobacz „[Korzystanie ze strony głównej administracji](https://technet.microsoft.com/6c155977-bd0e-47d6-ac65-1746cddb505e)” w dalszej części tego tematu.
-   **Zmień konto usługi programu RMS.** To łącze należy kliknąć, aby określić inne konto usługi programu RMS, na którym ma działać program RMS. Aby uzyskać więcej informacji, zobacz „[Zmienianie konta usługi programu RMS](https://technet.microsoft.com/f257d66d-b823-41e4-bcb7-7c90eb295238)” w dalszej części tego tematu.
-   **Usuń program RMS z tej witryny sieci Web.**To łącze należy kliknąć, aby usunąć zastrzeżenie programu RMS. Usunięcie zastrzeżenia programu RMS powoduje, że z danego serwera usuwane są aplikacje i katalogi wirtualne programu RMS, ale sam program RMS nie jest odinstalowywany. Aby uzyskać więcej informacji, zobacz „[Odinstalowywanie programu RMS](https://technet.microsoft.com/885e3b4f-ea32-466f-9f7f-d8440b0f7c28)” w dalszej części tego tematu.

| ![](images/Cc747575.note(WS.10).gif)Uwaga                                                                                                                                                                                                                                                                                                                      |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| W administracyjnej witrynie sieci Web programu RMS używane są okna wyskakujące służące do konfigurowania niektórych funkcji. W przypadku korzystania z programu do blokowania okien wyskakujących w przeglądarce sieci Web należy skonfigurować ustawienia przeglądarki w taki sposób, aby zezwolić na wyświetlanie okien wyskakujących w administracyjnej witrynie sieci Web programu RMS. |
