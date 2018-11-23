---
TOCTitle: Rejestrowanie punktu połączenia usługi
Title: Rejestrowanie punktu połączenia usługi
ms:assetid: '630cc3c3-9ed9-4423-8874-cbaceb43b353'
ms:contentKeyID: 18123288
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc720283(v=WS.10)'
---

Rejestrowanie punktu połączenia usługi
======================================

Rejestrowanie punktu połączenia usługi
--------------------------------------

W przypadku rejestrowania punktu połączenia usługi z serwera programu RMS znajdującego się w domenie podrzędnej może zostać wyświetlony komunikat o błędzie informujący o tym, że rejestracja SCP została zakończona niepowodzeniem. W wielu wypadkach proces rejestracji został przeprowadzony pomyślnie, jednak rejestracja ma miejsce w domenie najwyższego poziomu i jej replikacja na domeny podrzędne, w których serwer programu RMS sprawdza obecność obiektu SCP, zajmuje trochę czasu. Komunikat o błędzie przestaje być wyświetlany zaraz po replikacji obiektu SCP do wszystkich serwerów wykazu globalnego w lesie. Jeżeli komunikat ten zostanie wyświetlony, przed rozpoczęciem czynności dotyczących rozwiązywania problemów należy odczekać pewien czas, aby sprawdzić, czy problem ten został rozwiązany.

#### Rejestrowanie punktu połączenia usługi

1.  Zaloguj się na serwerze, na którym ma zostać zarejestrowany punkt połączenia usługi, za pomocą konta domeny mającego uprawnienia do tworzenia obiektu kontenera w kontenerze Usługi kontenera Konfiguracja lasu usługi Active Directory. Predefiniowana grupa zabezpieczeń — **Enterprise Admins** — jest przykładem konta mającego wymagane uprawnienia.

2.  Otwórz stronę **Administracja globalna**, a następnie kliknij łącze **Administruj programem RMS w tej witrynie sieci Web**.

3.  Na stronie głównej **Administracja** kliknij łącze **Punkt połączenia usługi programu RMS**.

4.  Na stronie **Punkt połączenia usługi programu RMS** kliknij przycisk **Zarejestruj URL**.
