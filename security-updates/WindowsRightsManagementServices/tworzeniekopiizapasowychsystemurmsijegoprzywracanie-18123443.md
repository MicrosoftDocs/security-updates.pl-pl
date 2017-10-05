---
TOCTitle: Tworzenie kopii zapasowych systemu RMS i jego przywracanie
Title: Tworzenie kopii zapasowych systemu RMS i jego przywracanie
ms:assetid: 'c11f3ac1-e512-402b-bf13-9ff21f5fe745'
ms:contentKeyID: 18123443
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747745(v=WS.10)'
---

Tworzenie kopii zapasowych systemu RMS i jego przywracanie
==========================================================

Planując przywracanie systemu, należy wziąć pod uwagę awarię serwera bazy danych oraz awarię serwera programu RMS. Jeśli wystąpi awaria serwera bazy danych, serwer lub klaster programu RMS można przywrócić z kopii zapasowej bazy danych konfiguracji. W tym celu nie trzeba uzyskiwać nowego certyfikatu licencjodawcy serwera ani klucza prywatnego serwera programu RMS, ponieważ są one przechowywane w bazie danych konfiguracji.

Planowanie tworzenia kopii zapasowej systemu RMS
------------------------------------------------

Poza kluczem serwera w bazie danych konfiguracji przechowywane są także dane użytkowników, w tym informacje o kluczach publicznych. Aby zapewnić ochronę cennych danych dotyczących kluczy, należy utworzyć kopię zapasową bazy danych konfiguracji na nośniku, a następnie schować ten nośnik w bezpiecznym miejscu. Baza danych konfiguracji odpowiadająca klastrowi głównej certyfikacji podlega częstym zmianom, dlatego zaleca się częste tworzenie kopii zapasowych. Im częściej do organizacji dodawani są nowi użytkownicy, tym częściej należy wykonywać kopie zapasowe. Podczas tworzenia kopii zapasowej serwera głównej certyfikacji należy także uwzględnić tabelę **sysmessages** z głównej bazy danych. Jeśli w tej tabeli nie znajdą się komunikaty programu RMS, serwer głównej certyfikacji nie będzie działać i będzie wyświetlany komunikat o błędzie. Jeśli tabela ta nie zostanie uwzględniona podczas tworzenia kopii zapasowej, można ją ponownie utworzyć, powtarzając proces zastrzegania za pomocą istniejącej bazy danych.

Baza danych rejestracji systemu RMS zawiera dzienniki, w których znajdują się przydatne dane statystyczne i informacje pomocne w rozwiązywaniu problemów. Nie ma ona jednak zazwyczaj krytycznego znaczenia dla systemu RMS. Baza danych usług katalogowych jest lokalnym buforem bazy danych usługi Active Directory. Dlatego jest automatycznie odtwarzana podczas przywracania systemu RMS. Aby określić plan tworzenia kopii zapasowej baz danych RMS, należy skonsultować się z administratorem serwera programu SQL Server.

Jeśli do ochrony kluczy prywatnych programu RMS używany jest sprzętowy moduł zabezpieczeń, należy także utworzyć kopię zapasową konfiguracji tego modułu. Aby uzyskać więcej informacji na temat tworzenia kopii zapasowej i przywracania konfiguracji sprzętowego modułu zabezpieczeń, zobacz dokumentację tego modułu.

| ![](images/Cc747745.note(WS.10).gif)Uwaga                                                                                                                                                                                                                                                                                                         |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Jeśli do szyfrowania kluczy prywatnych programu RMS użyto programowego dostawcy usług kryptograficznych (CSP) innego niż domyślny programowy dostawca CSP, przed użyciem tego dostawcy CSP z programem RMS należy upewnić się, że istnieją odpowiednie dla niego organizacyjne praktyki zarządzania kluczami (na przykład procedury tworzenia kopii zapasowej i przywracania). |

Planowanie przywracania systemu RMS
-----------------------------------

Przywracając serwer bazy danych z kopii zapasowej, należy upewnić się, że aktualnie używana wersja systemu RMS jest taka sama jak wersja używana podczas tworzenia kopii zapasowej. Należy powiadomić użytkowników systemu RMS o tym, że jeśli rozpoczęli użytkowanie systemu RMS po utworzeniu kopii zapasowej, będą musieli uzyskać nowy certyfikat konta praw. Dzięki temu nie traci się zawartości chronionej.

Aby przywrócić jeden serwer systemu RMS z klastra, należy odbudować serwer, ponownie zainstalować system RMS, a następnie dołączyć serwer do klastra, korzystając z istniejącej bazy danych. Nie ma to wpływu na użytkowników systemu RMS, ponieważ serwery klastrowane działają jako jeden serwer.
