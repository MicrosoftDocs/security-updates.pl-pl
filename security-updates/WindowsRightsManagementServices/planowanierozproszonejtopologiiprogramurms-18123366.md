---
TOCTitle: Planowanie rozproszonej topologii programu RMS
Title: Planowanie rozproszonej topologii programu RMS
ms:assetid: '8773a1e0-6ac3-41f5-9866-5890cef08d04'
ms:contentKeyID: 18123366
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747657(v=WS.10)'
---

Planowanie rozproszonej topologii programu RMS
==============================================

W niektórych okolicznościach może zaistnieć konieczność rozmieszczenia jednego lub kilku serwerów licencji, które nie należą do klastra głównej certyfikacji. Zazwyczaj tę czynność wykonuje się w celu obsługi działów wymagających bezpośredniej kontroli wydawania licencji użytkowania i publikacji, takich jak dział prawny z wymaganiami dotyczącymi zabezpieczeń, które muszą być kontrolowane na poziomie działu. Klaster głównej certyfikacji oferuje usługę certyfikacji kont dla serwerów licencji. Połączenie klastra głównej certyfikacji i instalacji jednego lub kilku serwerów licencji nazywane jest topologią rozproszoną.

Należy zauważyć, że serwery licencji, podobnie jak serwer głównej certyfikacji, można również rozmieścić w klastrze. Ponadto klaster licencji, podobnie jak klaster głównej certyfikacji, używa własnej usługi równoważenia obciążenia. Każdy serwer licencji lub klaster licencji używa osobnego wystąpienia programu SQL Server w celu dostarczenia baz danych konfiguracji i rejestrowania dla określonego serwera lub klastra.

Chociaż instalację programu RMS można skonfigurować tak, aby uruchamiane były tylko usługi certyfikacji z instalacji głównej, to możliwie jest także uruchamianie całej usługi licencji z jednego lub kilku serwerów albo klastrów licencji. Nie jest to jednak typowa konfiguracja. Zazwyczaj w celu spełnienia wymagań dotyczących wydajności i nadmiarowości zamiast rozmieszczania odrębnych serwerów licencji można zwiększyć liczbę fizycznych serwerów znajdujących się w klastrze głównej certyfikacji (o ile nie jest wymagana wydziałowa obsługa licencji). Poniższy diagram przedstawia takie rozmieszczenie.

![](images/Cc747657.01fa5a85-5711-41aa-932a-124049d34186(WS.10).gif)

Utworzenie topologii rozproszonej może zwiększyć koszty administracyjne w organizacji, ponieważ jest ona z zasady bardziej złożona. Jeśli w organizacji znajduje się wiele klastrów licencji i wiele lasów, może zaistnieć konieczność zastąpienia wartości rejestru na komputerach klienckich RMS w celu zapewnienia, że będą kierowały żądania licencji do właściwego serwera programu RMS. Dodatkowo mogą wystąpić problemy z zaufaniem między domenami. Wymaga to dalszej konfiguracji domen w celu umożliwienia korzystania z zawartości chronionej technologią RMS.

Punkty połączenia usługi w topologii rozproszonej
-------------------------------------------------

Po zastrzeżeniu serwera programu RMS adres URL klastra zostanie dodany do lasu usługi Active Directory w punkcie połączenia usługi (SCP). Swoje punkty SCP mają klaster głównej certyfikacji i każdy klaster licencji, który zastrzeżono w lesie. Przed zastrzeżeniem klastra licencji należy zarejestrować punkt SCP klastra głównej certyfikacji. Podczas zastrzegania klastra licencji w procesie podrejestrowywania ten adres URL używany jest w celu znalezienia klastra głównej certyfikacji w sieci oraz uzyskania certyfikatu licencjodawcy serwera.

Jeśli rozmieszczany jest klaster głównej certyfikacji, a nie pojedynczy serwer głównej certyfikacji, każdy serwer w klastrze musi zapewniać możliwość używania wirtualnego adresu poza współużytkowanym adresem URL.

Istnieje wiele implementacji adresowania wirtualnego, np. karuzela DNS, usługa równoważenia obciążenia sieci, rozwiązania sprzętowe i inne. Adresowanie wirtualne umożliwia równoważenie obciążenia między serwerami i powoduje usunięcie zależności licencji i publikowania z dowolnego serwera.

W programie RMS współużytkowany adres URL używany jest jako adres URL pobierania licencji oraz dla publikowanej wartości używanej przez komputery użytkowników końcowych podczas wyszukiwania klastra programu RMS w usłudze Active Directory lub w rejestrze. Komputery użytkowników końcowych nie wymagają bezpośredniego dostępu do poszczególnych serwerów znajdujących się w klastrze.
