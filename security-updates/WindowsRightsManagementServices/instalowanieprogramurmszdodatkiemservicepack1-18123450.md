---
TOCTitle: Instalowanie programu RMS z dodatkiem Service Pack 1
Title: Instalowanie programu RMS z dodatkiem Service Pack 1
ms:assetid: 'dab20175-a690-43f8-b943-768d289daa0d'
ms:contentKeyID: 18123450
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747689(v=WS.10)'
---

Instalowanie programu RMS z dodatkiem Service Pack 1
====================================================

Aby wykonać tę procedurę, należy zalogować się lokalnie w administracyjnej witrynie sieci Web przy użyciu konta należącego do grupy Administratorzy na komputerze, do którego użytkownik uzyskuje dostęp. Członkowie grupy Administratorzy domeny również mogą wykonać tę procedurę. Ze względu na najważniejsze wskazówki dotyczące bezpieczeństwa należy rozważyć użycie trybu **Uruchom jako** w celu wykonania tej procedury.

Komputer, na którym instalowany jest program RMS, musi być serwerem członkowskim w domenie lub musi być kontrolerem domeny. Programu RMS nie można rozmieścić na autonomicznym serwerze w grupie roboczej.

| ![](images/Cc747689.Important(WS.10).gif)Ważne                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Przed ukończeniem instalacji i zastrzegania pierwszego serwera głównej certyfikacji nie należy zastrzegać programu RMS na żadnym innym serwerze. Aby uzyskać instrukcje, zobacz „[Zastrzeganie pierwszego serwera głównej certyfikacji](https://technet.microsoft.com/debc42f3-74ff-4c99-b7a4-4921fccdabc2)”, „[Zastrzeganie serwera licencji](https://technet.microsoft.com/4d67b898-0ba9-4eef-ab7d-ee0ca55a688e)” lub „[Dodawanie serwera do klastra](https://technet.microsoft.com/db635238-5528-4bec-9cc6-8244e2b3d733)” w dalszej części tego tematu. |

| ![](images/Cc747689.Important(WS.10).gif)Ważne                                                                                                                                                                                          |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Program RMS z dodatkiem SP1 można zainstalować na serwerze z poprzednią wersją programu RMS. Jednak po zlikwidowaniu programu RMS, przed próbą zainstalowania programu RMS z dodatkiem SP1 należy program całkowicie usunąć za pomocą opcji Dodaj lub usuń programy. |

Instalowanie programu RMS z dodatkiem Service Pack 1
----------------------------------------------------

#### Instalowanie programu RMS z dodatkiem Service Pack 1

1.  Na serwerze, na którym chcesz zainstalować program RMS z dodatkiem SP1, zaloguj się, korzystając z konta domeny będącym członkiem lokalnej grupy Administratorzy.

2.  Gdy zostanie wyświetlone okno dialogowe **Zapraszamy!**, przejrzyj listę oprogramowania, które ma zostać zainstalowane, a następnie kliknij przycisk **Dalej**.

3.  W oknie dialogowym **Umowa licencyjna** przeczytaj umowę, zaznacz opcję **Zgadzam się**, a następnie kliknij przycisk **Dalej**.

4.  W polu **Folder** zaakceptuj folder domyślny lub określ nowy, a następnie kliknij przycisk **Dalej**.

5.  W oknie dialogowym **Potwierdzanie instalacji** kliknij przycisk **Zainstaluj**, aby rozpocząć instalację.

6.  Po wyświetleniu okna dialogowego **Instalacja ukończona** kliknij przycisk **Zamknij**.

    | ![](images/Cc747689.note(WS.10).gif)Uwaga                                                                                                            |
    |-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Jeśli zostanie wyświetlony komunikat o błędzie „Trwa ponowne uruchamianie aplikacji”, należy w programie Microsoft Internet Explorer odświeżyć stronę **Administracja globalna**. |

Program RMS można również zainstalować z poziomu wiersza polecenia. Aby uzyskać instrukcje, zobacz „[Instalacja z wiersza polecenia serwera programu RMS](https://technet.microsoft.com/b55b1e2a-dd14-4168-a37f-9cdedbec660b)” w dalszej części tego tematu.
