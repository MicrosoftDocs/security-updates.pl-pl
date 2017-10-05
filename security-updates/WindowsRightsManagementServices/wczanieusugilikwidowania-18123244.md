---
TOCTitle: Włączanie usługi likwidowania
Title: Włączanie usługi likwidowania
ms:assetid: '45226e85-b50d-41cc-aca7-0f603f8509d5'
ms:contentKeyID: 18123244
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720261(v=WS.10)'
---

Włączanie usługi likwidowania
=============================

Likwidowanie systemu RMS wymaga klucza prywatnego do ochrony wszystkich publikowanych informacji. Klucz ten jest przechowywany w bazie danych konfiguracji, jest zaszyfrowany za pomocą interfejsu API ochrony danych (DPAPI, Data Protection API) i jest oparty na haśle wprowadzanym podczas zastrzegania. Jeśli klucz prywatny systemu RMS jest przechowywany w sprzętowym module zabezpieczeń (HSM), klucz prywatny jest przechowywany w module HSM, a nie w bazie danych konfiguracji.

| ![](images/Cc720261.Caution(WS.10).gif)Przestroga                                                                                                                          |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Przed zlikwidowaniem systemu RMS należy upewnić się, czy znane jest hasło klucza prywatnego. Jeśli to hasło nie jest znane, przed zlikwidowaniem serwera RMS należy zresetować hasło klucza prywatnego. |

Pierwszym krokiem mającym na celu usunięcie systemu RMS jest likwidacja serwerów w klastrze. Ponieważ likwidacja jest funkcją licencji, serwer znajdujący się w podrejestrowanym klastrze licencji programu RMS można zlikwidować bez wpływu na główny klaster programu RMS lub każdy inny podrejestrowany klaster licencji programu RMS. Dlatego należy oddzielnie likwidować główny klaster programu RMS i klastry licencji, ponieważ w każdym klastrze licencji jest przechowywany jego własny klucz prywatny, za pomocą którego tworzy się licencje publikacji.

Aby włączyć usługę likwidowania, wykonaj następujące czynności:

1.  Otwórz administracyjną witrynę sieci Web programu Windows RMS.
2.  Kliknij kolejno opcję **Administruj programem RMS**i **Ustawienia zabezpieczeń**.
3.  Zaznacz pole wyboru **Włącz likwidowanie instalacji programu RMS**.
4.  Po wyświetleniu okna dialogowego z prośbą o zatwierdzenie procesu likwidacji kliknij przycisk **OK**.

Po zlikwidowaniu serwera nie można przywrócić go do standardowej konfiguracji programu RMS. Jest to procedura nieodwracalna.

Po zlikwidowaniu programu RMS, przed próbą zainstalowania kolejnej jego instancji konieczne jest jego całkowite usunięcie za pomocą funkcji **Dodaj lub usuń programy**.
