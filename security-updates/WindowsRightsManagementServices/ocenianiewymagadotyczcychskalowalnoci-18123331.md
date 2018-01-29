---
TOCTitle: Ocenianie wymagań dotyczących skalowalności
Title: Ocenianie wymagań dotyczących skalowalności
ms:assetid: '89f0138c-946d-47d7-a286-041d4d9606a8'
ms:contentKeyID: 18123331
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747663(v=WS.10)'
---

Ocenianie wymagań dotyczących skalowalności
===========================================

Aby określić, czy rozmieścić jeden serwer czy wiele serwerów, należy określić liczbę użytkowników, którzy będą korzystać z funkcji rozmieszczania programu RMS, oraz liczbę plików, które mają być chronione.

W ten sposób można spełnić średnie wymagania dotyczące wykorzystania. Następnie należy zaplanować wymagania szczytowego wykorzystania, które będą około trzy razy większe niż wymagania średnie.

Należy także wziąć pod uwagę odporność na awarie i dostępność usługi w firmie.

W celu przeprowadzenia pomiaru wydajności program RMS był testowany na serwerze z procesorem Pentium 4 o szybkości 2,4 GHz i 1 GB pamięci RAM. W tej konfiguracji serwer programu RMS dostarcza około 50 licencji na sekundę.

Do wyznaczenia wymagań dotyczących użytkowania systemu programu RMS podczas planowania wydajności można użyć poniższych danych.


<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Transakcja</th>
<th style="border:1px solid black;" >Wystąpienie</th>
<th style="border:1px solid black;" >Wykorzystanie pasma między klientem a serwerem (KB)</th>
<th style="border:1px solid black;" >Wykorzystanie pasma między serwerem a klientem (KB)</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Żądanie licencji</td>
<td style="border:1px solid black;">Powtarzane dla każdego użytkownika i dla każdego fragmentu zawartości</td>
<td style="border:1px solid black;">64</td>
<td style="border:1px solid black;">18</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Certyfikaty kont praw</td>
<td style="border:1px solid black;">Tylko ruch inicjowania programu RMS</td>
<td style="border:1px solid black;">12</td>
<td style="border:1px solid black;">16</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Rejestrowanie klientów</td>
<td style="border:1px solid black;">Tylko ruch inicjowania programu RMS</td>
<td style="border:1px solid black;">17</td>
<td style="border:1px solid black;">16</td>
</tr>
</tbody>
</table>
  
Ponadto ruch związany z kwerendami do usługi Active Directory może mieć wpływ na przepustowość sieci. Jednak nie jest to typowy czynnik w przypadku rozmieszczania serwerów programu RMS w bliskim sąsiedztwie serwerów wykazów globalnych. Wyjątkiem będzie sytuacja, gdy awaria wszystkich serwerów wykazów globalnych w danej lokacji spowoduje awaryjne przeniesienie do innej lokalizacji podczas połączenia, która nie oferuje takiej samej wydajności.
  
W poniższej tabeli przedstawiono dane bazowe dotyczące wykorzystania pasma przez transakcje programu RMS, których można użyć w celu oceny wpływu ruchu kwerend usługi Active Directory na sieć w organizacji.
  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Transakcja</th>
<th style="border:1px solid black;" >Wykorzystanie pasma między programem RMS a wykazem globalnym (w bajtach)</th>
<th style="border:1px solid black;" >Wykorzystanie pasma między wykazem globalnym a programem RMS (w bajtach)</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Ustanowienie połączenia programu RMS (ldap_bind)</td>
<td style="border:1px solid black;">1600</td>
<td style="border:1px solid black;">200</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Ocena przynależności do grup programu RMS (ldap_search)</td>
<td style="border:1px solid black;">200</td>
<td style="border:1px solid black;">100</td>
</tr>
</tbody>
</table>
  
Korzystając z tabel referencyjnych, należy pamiętać, że w zawartości rozmieszczenia są używane numery. Na przykład jeśli użytkownik należy do 15 grup, w celu wyszukania żądania z programu RMS będzie wymagane 200 bajtów, a w celu uzyskania odpowiedzi z wykazu globalnego będzie wymagane 1500 bajtów (100 bajtów x 15).
  
Planowanie wydajności należy wykonywać na podstawie przewidywanego obciążenia żądaniami licencji zawartości, ponieważ stanowią one większość operacji wykonywanych przez program RMS. Szybkość operacji wejścia/wyjścia oraz przepustowość dysku nie są czynnikami krytycznymi dla programu RMS, ponieważ żądania licencji nie wymagają obsługi dużej ilości danych i mogą być wykonywane na podstawie danych umieszczonych w pamięci podręcznej.
  
Podczas wyznaczania przepustowości serwera najważniejszą zmienną jest wykorzystanie procesora, dlatego bardzo ważne jest wybranie odpowiednich procesorów. Wymagania dotyczące pamięci na serwerach programu RMS zwiększają się wraz ze wzrostem obciążenia serwera i mogą przekroczyć maksymalną przepustowość serwera. W takiej sytuacji program Internetowe usługi informacyjne (IIS) kolejkuje w pamięci przychodzące żądania do momentu, gdy serwer będzie mógł je przetworzyć. Na podstawie limitu kolejki skonfigurowanego w programie IIS przychodzące żądania nie będą kolejkowane, ale będą odrzucane, gdy długość kolejki osiągnie określoną maksymalną wartość.
  
Wymagania dotyczące pamięci w programie RMS (zestaw roboczy) dla wzorca obciążenia nie powinny przekraczać ograniczeń rozmiaru pamięci fizycznej. Całkowity rozmiar pamięci jest najbardziej zależny od buforowania rozszerzania grupy. Zalecane jest, aby każdy serwer programu RMS miał co najmniej 1 GB pamięci RAM.
  
Każdy serwer programu RMS może obsłużyć określoną liczbę żądań klientów w określonym czasie (około 30–50 licencji na sekundę). Z tego powodu dodanie kolejnych serwerów powoduje liniowe skalowanie całkowitych możliwości wydawania licencji w klastrze, a ponadto zwiększa niezawodność. W rezultacie skalowanie dotyczy nie tylko poszczególnych serwerów, ale także liczby rozmieszczanych serwerów. Dzięki poniższym konfiguracjom przykładowym można zrozumieć, jak można wykorzystać te założenia do obliczenia wymaganych wartości związanych ze skalowalnością rozmieszczenia programu RMS.
  
-   Konfiguracja z małym wykorzystaniem  
    Niektóre organizacje mają stosunkowo niewielkie wymagania dotyczące wykorzystania programu RMS. Na przykład w przypadku organizacji z około 5000 użytkowników, z których 10 procent regularnie używa programu RMS w celu ochrony zawartości poczty e-mail, można oszacować, że przeciętny użytkownik chce chronić 3 wiadomości e-mail w ciągu godziny. Na podstawie tych wymagań można określić, że serwery programu RMS będą dostarczać 1500 licencji na godzinę, a więc 0,42 licencji na sekundę. Jest to średnie wymaganie dotyczące wykorzystania; mnożąc tę liczbę przez 3, otrzymuje się kalkulację szczytowego wykorzystania, które wynosi 1,25 licencji na sekundę.  
    Na podstawie tej kalkulacji można uznać, że wykorzystanie jest stosunkowo niewielkie. Dlatego też dla takiej organizacji powinien wystarczyć jeden serwer programu RMS.  
-   Konfiguracja ze średnim wykorzystaniem  
    W wielu organizacjach występują stosunkowo duże grupy użytkowników o umiarkowanych wymaganiach dotyczących wykorzystania. Na przykład w przypadku organizacji z około 40 000 użytkowników, z których 50 procent regularnie używa programu RMS w celu ochrony zawartości, można oszacować, że przeciętny użytkownik chce chronić 7 wiadomości e-mail i 1 dokument lub inny plik w ciągu godziny. Na podstawie tych wymagań można określić, że serwery programu RMS będą dostarczać 160 000 licencji na godzinę, a więc 44,4 licencji na sekundę. Jest to średnie wymaganie dotyczące wykorzystania; mnożąc tę liczbę przez 3, otrzymuje się kalkulację szczytowego wykorzystania, które wynosi 133.3 licencji na sekundę.  
    Na podstawie tej kalkulacji można uznać, że wykorzystanie będzie umiarkowanie duże i w celu zaspokojenia bieżących potrzeb użytkowników należy używać trzech serwerów programu RMS, natomiast zastosowanie 6 serwerów programu RMS zaspokoi bieżące potrzeby użytkowników oraz umożliwi zwiększenie wykorzystania.  
-   Konfiguracja z dużym wykorzystaniem  
    W dużych organizacjach często występują bardzo duże grupy użytkowników mających duże wymagania dotyczące wykorzystania. Na przykład w przypadku organizacji z około 150 000 użytkowników, z których 70 procent regularnie używa programu RMS w celu ochrony zawartości, można oszacować, że przeciętny użytkownik chce chronić 15 wiadomości e-mail i 3 dokumenty lub inne pliki w ciągu godziny. Na podstawie tych wymagań można określić, że serwery programu RMS będą dostarczać 1 890 000 licencji na godzinę, a więc 525 licencji na sekundę. Jest to średnie wymaganie dotyczące wykorzystania; mnożąc tę liczbę przez 3, otrzymuje się kalkulację szczytowego wykorzystania, które wynosi 1575 licencji na sekundę.  
    Na podstawie tej kalkulacji można uznać, że wykorzystanie będzie bardzo duże i w celu zaspokojenia bieżących potrzeb użytkowników należy używać 32 serwerów programu RMS, podczas gdy 51 serwerów programu RMS będzie zaspokajać bieżące potrzeby użytkowników, a także umożliwi zwiększenie wykorzystania.
  
Gdy z kalkulacji wynika, że w ciągu sekundy ma być dostarczanych 30-50 licencji, zazwyczaj potrzebny jest kolejny serwer programu RMS.
