---
TOCTitle: Zarządzanie rozmiarem dziennika
Title: Zarządzanie rozmiarem dziennika
ms:assetid: '431b32b3-02f0-4666-b52c-183eb65154fd'
ms:contentKeyID: 18123246
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720271(v=WS.10)'
---

Zarządzanie rozmiarem dziennika
===============================

Usługa rejestrowania wysyła duże ilości danych do bazy danych serwera programu SQL Server. Należy regularnie sprawdzać, czy baza danych rejestrowania dysponuje wystarczającą ilością miejsca na dysku na potrzeby danych. Jeśli okaże się, że ilość danych jest nadmierna i że istniejące potrzeby w zakresie raportowania nie wymagają części tych informacji, należy rozważyć możliwość ustawienia filtrów programu SQL Server, dzięki którym w plikach dziennika przechowywane byłyby tylko faktycznie potrzebne dane. Aby uzyskać instrukcje dotyczące filtrowania informacji rejestrowania, zobacz Pomoc programu SQL Server Enterprise Manager.

Jeśli okaże się, że baza danych rejestrowania jest zbyt duża w stosunku do dostępnego miejsca na dysku, można przenieść ją na inny serwer, tak jak to opisano w części „[Zmienianie lokalizacji bazy danych rejestrowania](https://technet.microsoft.com/34ea8045-dc94-422e-9601-29927cfc1534)” w dalszej części tego tematu.

| ![](images/Cc720271.Important(WS.10).gif)Ważne                                                                                                                                                                                                                                                                                                                          |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Należy także korzystać z Monitora systemu, aby regularnie monitorować rozmiar wychodzącej kolejki wiadomości rejestrowania. Jeśli rozmiar kolejki znacznie się zwiększy, należy sprawdzić, czy usługa odbiornika rejestrowania działa prawidłowo. Aby uzyskać więcej informacji dotyczących korzystania z Monitora systemu, zobacz Centrum pomocy i obsługi technicznej systemu Windows Server 2003. |
