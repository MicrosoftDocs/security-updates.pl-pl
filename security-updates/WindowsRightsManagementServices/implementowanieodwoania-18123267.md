---
TOCTitle: Implementowanie odwołania
Title: Implementowanie odwołania
ms:assetid: '4735f060-7197-4ae2-830a-f91bcc4de30a'
ms:contentKeyID: 18123267
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747554(v=WS.10)'
---

Implementowanie odwołania
=========================

Certyfikaty i licencje może odwołać dowolny podmiot znajdujący się w łańcuchu zaufania danego certyfikatu lub licencji. Serwer głównej certyfikacji może odwołać dowolny wystawiony przez siebie certyfikat lub licencję. Ponadto certyfikaty może odwołać niezależny podmiot wybrany przez administratora programu RMS.

Aby odwołać certyfikat lub licencję udzieloną przez serwer programu RMS, można utworzyć i rozprowadzić listę odwołania, a następnie umieścić tę listę jako wymaganie w szablonie zasad praw dostępu, tak jak to opisano w następujących krokach:  

1.  Utwórz listę odwołania określającą podmioty, których ma dotyczyć odwołanie. Jest to zwykły plik tekstowy w formacie XML, zgodny ze słownictwem języka XrML. Aby uzyskać więcej informacji, zobacz „[Tworzenie list odwołania](https://technet.microsoft.com/1ef75199-3344-4225-84de-a863a777696a)” w dalszej części tego tematu.
2.  Wygeneruj parę kluczy dla listy odwołania. Następnie podpisz plik kluczem prywatnym, korzystając z dostarczonego w tym celu narzędzia Podpisywanie listy odwołania. Aby uzyskać instrukcje, zobacz „Wstawianie podpisu do listy odwołania” w dalszej części tego tematu. Zautomatyzuj ten proces, tak aby występował regularnie, najlepiej codziennie.
3.  Umieść plik listy odwołania w lokalizacji, do której dostęp mają wszyscy potrzebujący go użytkownicy. Zalecane jest umieszczenie tego pliku w lokalizacji dostępnej zarówno z danej sieci, jak i z Internetu, najlepiej w witrynie sieci Web. Gwarantuje to, że użytkownicy będą mogli uzyskać dostęp do pliku zarówno z sieci firmowej, jak i spoza niej.
4.  Utwórz szablon zasad praw dostępu zawierający wymaganie dotyczące listy odwołania. Aby uzyskać więcej informacji, zobacz „[Tworzenie i modyfikowanie szablonów zasad praw dostępu](https://technet.microsoft.com/6014176f-ef71-4d29-b3e3-da129c18563d)” w dalszej części tego tematu.

Można także odwołać certyfikat licencjodawcy serwera, którym posługuje się serwer głównej certyfikacji. Ponieważ certyfikat ten został wystawiony przez usługę rejestrowania firmy Microsoft, właśnie firma Microsoft może odwołać certyfikat licencjodawcy serwera dla głównej certyfikacji. W tym celu firma Microsoft dodaje certyfikat licencjodawcy serwera do swojej listy odwołania i udostępnia tę listę publicznie.

Ponadto certyfikat licencjodawcy serwera może być odwołany przez niezależny urząd, jeśli administrator programu RMS włączył odpowiednią opcję podczas zastrzegania. Jeśli użyto tej opcji, klientom należy udostępnić listę odwołania, która zawiera certyfikat licencjodawcy serwera podpisany kluczem prywatnym niezależnego urzędu. Aby uzyskać więcej informacji, zobacz „[Odwołanie certyfikatów licencjodawcy serwera](https://technet.microsoft.com/8020861d-d196-4431-8282-044675ef5616)” w dalszej części tego tematu.

> [!Caution]  
> Podczas implementowania odwołania należy zachować ostrożność. Na podstawie określonego interwału odświeżania należy okresowo odnawiać listę odwołania, ponieważ w przeciwnym przypadku wygaśnie ona automatycznie, co uniemożliwi użytkownikom pobieranie zawartości wymagającej użycia tej listy. Aby zapewnić, że nie nastąpi przypadkowe uniemożliwienie użytkownikom pobierania zawartości, należy dokładnie oszacować interwał wymagany do odświeżania listy odwołania. Należy także zapewnić dostęp do listy odwołania zarówno z sieci, jak i spoza niej. Aby uzyskać więcej informacji, zobacz „[Definiowanie zasad odwołania](https://technet.microsoft.com/e2fffe9f-def7-439b-a8aa-43f8a065813d)” we wcześniejszej części tego tematu. 
