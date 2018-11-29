---
TOCTitle: Zapewnianie nadmiarowości i równoważenie obciążenia
Title: Zapewnianie nadmiarowości i równoważenie obciążenia
ms:assetid: '162d547c-78a7-4848-b43e-58e481832af2'
ms:contentKeyID: 18123186
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720199(v=WS.10)'
---

Zapewnianie nadmiarowości i równoważenie obciążenia
===================================================

Aby zapewnić użytkownikom możliwość pobierania licencji i publikowania zawartości zawsze, gdy będzie to konieczne, zdecydowanie zalecane jest rozmieszczenie nadmiarowych serwerów programu RMS za pomocą klastrów. Jako minimum należy rozmieścić klaster głównej certyfikacji składający się co najmniej z dwóch serwerów. Jeśli zostanie również rozmieszczony odrębny serwer licencji w celu obsługi określonych potrzeb dotyczących licencji dla poszczególnych grup w organizacji, należy również rozmieścić serwer licencji jako klaster składający się z co najmniej dwóch serwerów.

Wiele fizycznych serwerów w klastrze głównej certyfikacji lub w dowolnym klastrze licencji tworzy „farmę sieci Web” dostępną pod współużytkowanym adresem URL lub adresem wirtualnym. Jeśli w organizacji używana jest farma serwerów, można zintegrować program RMS z dowolną używaną techniką adresowania wirtualnego, taką jak karuzela DNS, usługa równoważenia obciążenia sieci lub dedykowane rozwiązania sprzętowe.

Poza przypadkiem równoważenia obciążenia adresowanie wirtualne jest korzystne, gdy jest używane z programem RMS, ponieważ eliminuje ono zależność od serwera fizycznego w przypadku usług certyfikacji lub licencjonowania. Komputery użytkowników końcowych nie wymagają bezpośredniego dostępu do poszczególnych serwerów znajdujących się w klastrze.
