---
TOCTitle: Ustawianie uprawnień do katalogu wirtualnego
Title: Ustawianie uprawnień do katalogu wirtualnego
ms:assetid: '45112111-9608-45b1-9a86-7b313d0a1579'
ms:contentKeyID: 18123262
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747549(v=WS.10)'
---

Ustawianie uprawnień do katalogu wirtualnego
============================================

Po włączeniu likwidowania, można korzystać z tej funkcji jako usługi. Usługa likwidowania jest jednak katalogiem wirtualnym Internetowych usług informacyjnych (IIS) ze skojarzonymi uprawnieniami dostępu. Aby użytkownicy mogli korzystać z tej usługi, należy ustawić uprawnienia do katalogu wirtualnego i odpowiedniego pliku, decommission.asmx.

Domyślnie dla katalogu wirtualnego jest włączone zintegrowane uwierzytelnianie systemu Windows, ale tylko konta systemowe i konta administratorów mają dostęp do odpowiedniego pliku. Po określeniu uprawnień dla listy DACL pliku decommission.asmx można udzielić dostępu odpowiedniej grupie zaufanych użytkowników, aby usunąć istniejące zabezpieczenie programu RMS, lub udzielić dostępu do usługi wszystkim osobom.

Aby użytkownicy mogli korzystać z usługi likwidowania, trzeba tak zmodyfikować ich aplikacje, aby było możliwe wysyłanie próśb o licencję użytkownika do nowego potoku likwidowania. W pakiecie Microsoft Office 2003 w tym celu dodaje się wpis w rejestrze na komputerze użytkownika. Jeśli użytkownik korzysta z pakietu Office 2003, w tym celu można wykonać następujące czynności:

1.  Otwórz edytor rejestru.
2.  Przejdź do lokalizacji `HKEY_CURRENT_USER\Software\Microsoft\Office\11,0\Common\DRM` i dodaj nowy klucz o nazwie `Decommissioning`.
3.  W kluczu Decommissioning dodaj następujący nowy wpis w polu **Wartość ciągu**, zastępując adres *Twój serwer licencji* nazwą serwera programu RMS:
    `http://`*Twój serwer licencji*`/_wmcs/licensing`
4.  Kliknij wpis prawym przyciskiem myszy i wybierz polecenie **Modyfikuj**, aby określić dane wartości, które trzeba wskazać usłudze likwidowania:
    `http://`*Twój serwer licencji*`/_wmcs/decommission`

> [!note]  
> Można zdefiniować kilka wartości tego klucza, jeśli wiele serwerów programu RMS w organizacji pracuje w trybie likwidowania. 
