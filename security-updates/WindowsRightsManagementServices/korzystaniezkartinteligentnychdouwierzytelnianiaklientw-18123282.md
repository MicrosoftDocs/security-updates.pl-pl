---
TOCTitle: Korzystanie z kart inteligentnych do uwierzytelniania klientów
Title: Korzystanie z kart inteligentnych do uwierzytelniania klientów
ms:assetid: '5caacd67-fb16-46f1-b1ad-4aef0a632bf0'
ms:contentKeyID: 18123282
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747579(v=WS.10)'
---

Korzystanie z kart inteligentnych do uwierzytelniania klientów
==============================================================

W przypadku gdy w organizacji są używane karty inteligentne, które służą zapewnieniu dodatkowego zabezpieczenia i kontroli nad poświadczeniami użytkowników, można z nich korzystać podczas uzyskiwania certyfikatów konta praw dostępu i używać licencji z serwera programu RMS. Aby skonfigurować serwer programu RMS w taki sposób, aby wymagane było uwierzytelnianie klienta, należy włączyć protokół SSL (Secure Sockets Layer) dla witryny sieci Web, na której został zastrzeżony program RMS, i skonfigurować metodę uwierzytelniania w programie Internetowe usługi informacyjne (IIS). W tym celu można wykonać następujące kroki:

1.  Otwórz **Menedżera internetowych usług informacyjnych**.
2.  Rozwiń element serwera, kliknij prawym przyciskiem myszy folder witryny sieci Web, a następnie kliknij przycisk **Właściwości**.
3.  Kliknij kartę **Zabezpieczenia katalogów**, a następnie w obszarze **Bezpieczna komunikacja** zaznacz pole wyboru **Włącz mapowanie usługi katalogowej systemu Windows**.
4.  Rozwiń folder witryny sieci Web, otwórz katalog wirtualny **\_wmcs**, następnie rozwiń katalog wirtualny (**Licencjonowanie** lub **Certyfikacja**), dla którego chcesz skonfigurować uwierzytelnianie.
    -   Aby skonfigurować uwierzytelnianie dla sytuacji, gdy użytkownik żąda licencji użytkowania, kliknij prawym przyciskiem myszy plik license.asmx, a następnie kliknij przycisk **Właściwości**.
    -   Aby skonfigurować uwierzytelnianie dla sytuacji, gdy użytkownik żąda certyfikatu użytkownika, kliknij prawym przyciskiem myszy plik certification.asmx, a następnie kliknij przycisk **Właściwości**.
5.  Kliknij kartę **Zabezpieczenia plików**, a następnie w obszarze **Bezpieczna komunikacja** kliknij przycisk **Edytuj**, aby otworzyć okno dialogowe **Bezpieczna komunikacja**.
6.  Wybierz opcję **Wymagaj bezpiecznego kanału (SSL)**, a następnie kliknij jedną z dwóch następujących opcji:
    -   **Wymagaj certyfikatów klienta**, jeżeli chcesz, aby z usługą mogli łączyć się tylko klienci z certyfikatami po stronie klienta, np. przechowywanymi na kartach inteligentnych.
    -   **Akceptuj certyfikaty klienta**, jeżeli chcesz, aby klienci mogli podawać poświadczenia uwierzytelniania, korzystając z certyfikatu karty inteligentnej lub nazwy użytkownika i hasła.
7.  Wybierz opcję **Włącz mapowanie certyfikatów klienta**, a następnie kliknij przycisk **OK**.
8.  Jeżeli chcesz korzystać z uwierzytelniania zarówno w przypadku certyfikacji, jak i licencjonowania, powtórz tę procedurę, wybierając tym razem inny katalog wirtualny.

Po skonfigurowaniu tych ustawień, użytkownik próbujący otworzyć zawartość chronioną technologią RMS i opublikowaną przez ten serwer zostanie poproszony o podanie swoich poświadczeń uwierzytelniania, zanim serwer udostępni mu certyfikat konta praw dostępu lub licencję użytkowania.
