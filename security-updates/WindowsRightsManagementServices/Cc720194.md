---
TOCTitle: Uzyskiwanie licencji użytkowania
Title: Uzyskiwanie licencji użytkowania
ms:assetid: '0b6cde34-418a-4dee-9d27-b65b93b535ac'
ms:contentKeyID: 18123171
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720194(v=WS.10)'
---

Uzyskiwanie licencji użytkowania
================================

W celu użycia zawartości chronionej technologią RMS użytkownik musi uzyskać licencję użytkowania od usługi licencjonowania programu RMS. Poniższy rysunek przedstawia proces żądania i otrzymywania licencji użytkowania.

![](images/Cc720194.37b8d28c-9749-4e81-bc6a-22692fefb8b6(WS.10).gif)

Proces uzyskiwania licencji użytkowania składa się z następujących kroków:

1.  Użytkownik otrzymuje typowym kanałem rozpowszechniania plik chroniony, a następnie otwiera go za pomocą aplikacji obsługującej technologię RMS. Jeśli użytkownik nie posiada certyfikatu konta praw na bieżącym komputerze lub urządzeniu, musi go uzyskać.
2.  Aplikacja obsługująca technologię RMS wysyła żądanie licencji użytkowania do serwera, który wystawił licencję publikacji dla zawartości chronionej. Żądanie obejmuje certyfikat konta praw użytkownika (zawierający klucz publiczny użytkownika) oraz licencję publikacji (zawierającą symetryczny klucz zawartości).  
    Licencja publikacji wystawiona przez certyfikat licencjodawcy klienta zawiera adres URL serwera, który wystawił certyfikat. W tym przykładzie żądanie licencji użytkowania jest przesyłane do serwera, który wystawił certyfikat licencjodawcy klienta, a nie do komputera, który wystawił licencję publikacji.
3.  Serwer licencjonowania sprawdza, czy użytkownik jest autoryzowany oraz czy został wymieniony w licencji publikacji, a następnie tworzy licencję użytkowania. Serwer sprawdza certyfikat konta użytkownika, a następnie określa, jakich uprawnień udzielono użytkownikowi – wprost lub jako członkowi grupy, której udzielono uprawnień.  
    Serwer deszyfruje symetryczny klucz zawartości kluczem prywatnym serwera, ponownie szyfruje go kluczem publicznym odbiorcy i dodaje do licencji użytkowania. Dzięki temu tylko właściwy użytkownik może deszyfrować klucz zawartości oraz zawartość chronioną.
    Serwer dodaje odpowiednie warunki do licencji użytkowania, takie jak wykluczenia dotyczące aplikacji lub wersji systemu Windows. Te warunki są wymuszane przez klienta, gdy licencja użytkowania jest dowiązywana do zawartości chronionej technologią RMS.
4.  Po zakończeniu sprawdzania serwer licencji zwraca licencję użytkowania do komputera klienckiego użytkownika.
