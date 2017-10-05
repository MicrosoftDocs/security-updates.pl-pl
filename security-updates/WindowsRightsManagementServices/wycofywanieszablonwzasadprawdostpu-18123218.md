---
TOCTitle: Wycofywanie szablonów zasad praw dostępu
Title: Wycofywanie szablonów zasad praw dostępu
ms:assetid: '32bf98c7-edda-4507-a4b8-4c11bddd6e60'
ms:contentKeyID: 18123218
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720239(v=WS.10)'
---

Wycofywanie szablonów zasad praw dostępu
========================================

Aby wycofać szablon zasad praw dostępu, należy go usunąć. Ta procedura jest opisana w części „[Usuwanie szablonu zasad praw dostępu](https://technet.microsoft.com/9c9a1496-cf55-4c65-a4c6-9fe245edce00)” w dalszej części tego tematu. Ogólnie jednak nie powinno się usuwać szablonów zasad praw dostępu. Jeśli mimo wszystko zachodzi potrzeba wycofania szablonu zasad praw dostępu, należy także zadbać o usunięcie jego kopii z komputerów użytkowników. Czynność tę należy wykonać, ponieważ w momencie, gdy autor używa szablonu zasad praw dostępu do opublikowania zawartości, serwer programu RMS odbiera żądanie. Odpowiadając na to żądanie, program RMS korzysta z kopii szablonu zasad praw dostępu przechowywanej w bazie danych. Jeśli w bazie danych nie ma danego szablonu zasad praw dostępu, żądanie kończy się niepowodzeniem.

| ![](images/Cc720239.note(WS.10).gif)Uwaga                                                                                                                |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Aby odpowiednio zarządzać wycofywaniem szablonu zasad praw dostępu, można na przykład utworzyć skrypt, który spowoduje usunięcie tego szablonu ze wszystkich komputerów użytkowników. |
