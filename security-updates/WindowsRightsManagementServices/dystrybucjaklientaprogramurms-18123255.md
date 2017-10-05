---
TOCTitle: Dystrybucja klienta programu RMS
Title: Dystrybucja klienta programu RMS
ms:assetid: '4b8dd930-4105-4e73-918c-12d2b05d5fb5'
ms:contentKeyID: 18123255
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720266(v=WS.10)'
---

Dystrybucja klienta programu RMS
================================

Klient programu RMS jest częścią systemu operacyjnego Windows Vista®, co oznacza, że nie jest on już instalowany oddzielnie. Systemy operacyjne w wersjach wcześniejszych niż Windows Vista wymagają zainstalowania oprogramowania klienckiego programu RMS, a następnie jego aktywacji.

W ramach procesu aktywacji tworzona jest skrytka oraz certyfikat komputera dla aktualnie zalogowanego użytkownika. Aktywacja jest procesem lokalnym i nie wymaga połączenia sieciowego. Po pomyślnym wykonaniu aktywacji pierwsze żądanie użycia licencji przez włączenie programu RMS za pośrednictwem odpowiedniej aplikacji spowoduje pobranie certyfikatu użytkownika. Klienta programu RMS można zainstalować na każdym komputerze klienckim w organizacji, korzystając z przystawki Zasady grupy, usługi Windows Update lub skryptu administracyjnego.

| ![](images/Cc720266.note(WS.10).gif)Uwaga                                                                                                                                                                                                                                                 |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Niezależnie od zastosowanej metody dystrybucji klient programu RMS komunikuje się z serwerem programu RMS za pomocą portu; domyślnie jest to port 80 lub 443. Należy upewnić się, że komputer kliencki obsługuje żądania wychodzące do klastra głównego i klastrów licencji programu RMS za pośrednictwem tych portów. |

**Korzystanie z zasad grupy**

Jeśli organizacja dokonuje dystrybucji oprogramowania za pomocą przystawki Zasady grupy, za pomocą tej metody można dokonywać dystrybucji klienta programu RMS na podstawie szerszych uprawnień. Jeśli dystrybucja klienta programu RMS odbywa się w ten właśnie sposób, użytkownik nie musi mieć uprawnień administratora i może zainstalować klienta RMS za pomocą apletu **Dodaj lub usuń programy** w **Panelu sterowania** lub poprzez otwarcie zawartości chronionej prawami za pomocą aplikacji obsługującej technologię RMS.

**Korzystanie z usługi Windows Update**

Usługa Windows Update jest najprostszym sposobem instalacji klienta programu RMS na komputerze. Jej zaletą jest korzystanie z mechanizmu dobrze znanego użytkownikom, jednak wymaga ona, aby użytkownik dokonujący instalacji klienta programu RMS miał prawa administratora lokalnego na komputerze.

**Korzystanie z instalacji skryptowej**

W celu uzyskania najwyższego poziomu kontroli nad procesem instalacji klienta, można pobrać oprogramowanie i sprawdzić jego integralność na każdym z etapów instalacji poprzez uruchomienie skryptu. Ten skrypt może zostać napisany i dodany do obiektu zasad grupy jako skrypt uruchamiania. Dzięki temu użytkownik nie musi być administratorem lokalnym, a klient programu RMS jest automatycznie instalowany po ponownym uruchomieniu.

        ```
Podstawowe informacje dotyczące dystrybucji klienta programu RMS za pomocą przystawki Zasady grupy znajdują się w części [Konfigurowanie programu SMS lub zasad grupy w celu obsługi rozmieszczania klientów](https://technet.microsoft.com/9e37c27b-8cc1-40c6-adb7-0937aa64c8db) w dalszej części tego tematu.

Wskazówki dotyczące procedury rozmieszczania klienta programu RMS znajdują się w części [Jak wdrażać klienta programu RMS](https://technet.microsoft.com/c84f1724-cf71-4385-9003-ff68bc23c927) w dalszej części tego tematu.
