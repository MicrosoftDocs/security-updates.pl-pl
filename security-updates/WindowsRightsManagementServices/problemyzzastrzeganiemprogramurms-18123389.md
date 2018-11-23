---
TOCTitle: Problemy z zastrzeganiem programu RMS
Title: Problemy z zastrzeganiem programu RMS
ms:assetid: 'b0e6ef48-ab38-4426-be5b-811cf64c45c0'
ms:contentKeyID: 18123389
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747638(v=WS.10)'
---

Problemy z zastrzeganiem programu RMS
=====================================

W ramach operacji zastrzegania programu RMS następuje skonfigurowanie i ustanowienie plików zasobów oraz połączeń między różnymi składnikami, od których zależy praca programu RMS. W razie wystąpienia błędu w czasie, gdy program RMS próbuje skonfigurować zasób, operacja zastrzegania kończy się niepowodzeniem i wyświetlany jest komunikat o błędzie. W niniejszej sekcji omówiono najczęściej spotykane przyczyny tych błędów i wskazówki pomocne w eliminowaniu przeszkód w pomyślnym zakończeniu zastrzegania w programie RMS.

Nie można zastrzec serwera głównej certyfikacji
-----------------------------------------------

Zastrzeganie serwera głównej certyfikacji może okazać się niemożliwe, ponieważ nie są wyświetlane prawidłowe strony do zastrzegania. Może tak się zdarzyć, gdy kliknięto polecenie Zastrzeż program RMS w tej witrynie sieci Web w celu zastrzeżenia pierwszego serwera głównej certyfikacji na stronie Administracja globalna. Jednak zamiast stron zastrzegania dla serwera głównej certyfikacji wyświetlane są strony służące do zastrzegania serwera licencji.

Ten problem występuje wtedy, gdy nie usunięto zastrzeżenia ostatniego serwera głównej certyfikacji w tym lesie usługi Active Directory przed odinstalowaniem z niego programu RMS, a następnie próbowano zastrzec serwer głównej certyfikacji. Po usunięciu zastrzeżenia jedynego serwera głównej certyfikacji w lesie usługi Active Directory punkt połączenia usługi jest usuwany z usługi Active Directory. Jeśli dla ostatniego serwera głównej certyfikacji w lesie nie zostanie usunięte zastrzeżenie przed odinstalowaniem programu RMS, nie będzie możliwe ponowne zastrzeżenie serwera głównej certyfikacji w tym lesie, zanim punkt połączenia usługi nie zostanie ręcznie usunięty z usługi Active Directory.

Jeśli podczas próby zastrzeżenia pierwszego serwera głównej certyfikacji w lesie Active Directory wyświetlane są strony zastrzegania dla serwera licencji, należy usunąć punkt połączenia usługi z usługi Active Directory w następujący sposób:

**Aby usunąć punkt połączenia usługi dla programu RMS**
1.  W razie potrzeby zainstaluj narzędzia pomocnicze serwera Windows:

    W systemie Windows Server 2003, w folderze \\Support\\Tools na dysku instalacyjnym CD uruchom plik Suptools.msi.

    W systemie Windows 2000 Server, w folderze \\Support Tools na dysku instalacyjnym CD uruchom program Setup.exe.

2.  Zaloguj się na kontrolerze domeny, do której należy serwer głównej certyfikacji, korzystając z konta należącego do grupy Administratorzy domeny.

3.  W wierszu polecenia wpisz poniższe polecenie, a następnie naciśnij klawisz ENTER:

    **ldp**

4.  Kliknij pozycję **Połączenie**, a następnie polecenie **Połącz**.

5.  Naciśnij klawisz ENTER. Nie wpisuj żadnych informacji.

6.  Kliknij pozycję **Połączenie**, a następnie polecenie **Dowiąż**.

7.  Naciśnij klawisz ENTER. Nie wpisuj żadnych informacji.

8.  Kliknij pozycję **Widok**, a następnie kliknij opcję **Drzewo**.

9.  Naciśnij klawisz ENTER. Nie wpisuj żadnych informacji.

    W lewym okienku będzie wyświetlany tekst **dc=TwojaDomena,dc=com**.

10. Rozwiń element **dc=TwojaDomena,dc=com**.

11. Rozwiń element **Konfiguracja**.

12. Rozwiń element **Usługi**.

13. Usuń pozycję **RightsManagementServices**.

— lub —

1.  Pobierz i zainstaluj pakiet narzędzi administracyjnych programu RMS. Pakiet można pobrać na [witrynie sieci Web firmy Microsoft](http://go.microsoft.com/fwlink/?linkid=33841.)
2.  Otwórz wiersz poleceń, wybierając z menu **Start** polecenie **Uruchom**. W oknie dialogowym **Uruchom** wpisz polecenie **cmd** i kliknij przycisk **OK**.
3.  W wierszu poleceń wpisz następujące polecenie:
    **ADSCPRegister.exeunregisterscp** &lt;*URLtoUnRegister*&gt;
4.  W miejscu parametru &lt;*URLtoUnRegister*&gt; wpisz adres URL punktu połączenia usługi RMS, na przykład https://my\_domain/\_wmcs/Certification.

Po zakończeniu tych kroków można zastrzec serwer głównej certyfikacji.

Nie można wygenerować kontekstu SSPI
------------------------------------

Podczas zastrzegania może zostać wyświetlony komunikat „Nie można wygenerować kontekstu SSPI”, jeśli wystąpił problem z uwierzytelnianiem konta usługi programu RMS podczas rejestrowania serwera głównej certyfikacji w usłudze rejestracji firmy Microsoft.

W przypadku wystąpienia tego komunikatu o błędzie należy sprawdzić, czy konto usługi programu RMS jest prawidłowym kontem domeny. Jeśli konto jest kontem grupowym, należy sprawdzić, czy członkostwo w grupie jest aktualne, czy można uzyskiwać informacje o wszystkich kontach użytkowników w grupie domeny oraz czy konta mają uprawnienia do baz danych programu SQL Server.
