---
TOCTitle: Omówienie systemu RMS
Title: Omówienie systemu RMS
ms:assetid: 'cbd14635-e17e-42b8-9fd8-6fdce42ffe07'
ms:contentKeyID: 18123424
ms:mtpsurl: 'https://technet.microsoft.com/pl-pl/library/Cc747671(v=WS.10)'
---

Omówienie systemu RMS
=====================

Ten temat zawiera informacje o współpracy usług sieci Web programu RMS oraz technologii klienckich RMS w systemie RMS.

W poniższej tabeli przedstawiono typy serwerów, które działają w rozmieszczeniu programu RMS oraz opis ich funkcji. Aby uzyskać szczegółowe informacje na temat rozmieszczania, zobacz „Rozmieszczanie systemu RMS” w niniejszym zestawie dokumentacji.

 
<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Serwer lub klaster</th>
<th style="border:1px solid black;" >Funkcja</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Główna certyfikacja</td>
<td style="border:1px solid black;">Uruchamia następujące usługi programu RMS:
<ul>
<li><strong>Podrejestrowanie</strong>. Odpowiada za podrejestrowywanie serwerów licencji.<br />
<br />
</li>
<li><strong>Serwer proxy aktywacji</strong>. Działa jako serwer proxy sieci Internet dla żądań klientów dotyczących skrytek i certyfikatów komputerów RMS.<br />
<br />
</li>
<li><strong>Certyfikacja</strong>. Wystawia certyfikaty kont praw.<br />
<br />
</li>
<li><strong>Publikowanie</strong>. Wystawia licencje publikacji.<br />
<br />
</li>
<li><strong>Licencjonowanie</strong>. Wystawia licencje użytkowania.<br />
<br />
</li>
</ul>
Każde rozmieszczenie musi zawierać co najmniej jeden serwer lub klaster głównej certyfikacji. Każdy las usługi Active Directory może zawierać tylko jeden klaster głównej certyfikacji.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Licencjonowanie (opcjonalne)</td>
<td style="border:1px solid black;">Uruchamia następujące usługi programu RMS:
<ul>
<li><strong>Publikowanie</strong>. Wystawia licencje publikacji.<br />
<br />
</li>
<li><strong>Licencjonowanie</strong>. Wystawia licencje użytkowania.<br />
<br />
</li>
</ul>
Serwery licencji są często rozmieszczane w celu obsługi pojedynczych oddziałów lub w celu odciążenia klastra głównej certyfikacji w zakresie żądań licencjonowania. Serwery licencji są opcjonalne.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Serwer bazy danych, na przykład SQL Server</td>
<td style="border:1px solid black;"><ul>
<li>Uruchamia bazy danych konfiguracji, rejestrowania i usług katalogowych dla programu RMS.<br />
<br />
</li>
<li>Przechowuje certyfikaty kont praw w bazie danych konfiguracji klastra głównej certyfikacji.<br />
<br />
</li>
</ul></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Kontroler domeny i wykaz globalny</td>
<td style="border:1px solid black;"><ul>
<li>Zapewnia usługi uwierzytelniania użytkowników i usługi katalogowe.<br />
<br />
</li>
<li>Przechowuje lokalizację odnajdowania usług dla klastra głównej certyfikacji.<br />
<br />
</li>
</ul></td>
</tr>
</tbody>
</table>
 

Program RMS korzysta z usług rejestrowania i aktywacji obsługiwanych przez firmę Microsoft w celu zapewnienia wspólnego fundamentu zaufania systemu. Aby uzyskać więcej informacji, zobacz „[Hierarchia zaufania w programie RMS](https://technet.microsoft.com/2d44182f-a653-4383-aba1-dade53f7cf9a)” w dalszej części tego tematu.

Poniższy diagram przedstawia różne składniki systemu RMS oraz ich role w systemie. Strzałki przedstawiają żądania i odpowiedzi przekazywane między różnymi składnikami.

![](images/Cc747671.29138741-d45c-459b-8ead-b9bc3f708dd5(WS.10).gif)

Aby uzyskać więcej informacji dotyczących każdego ze składników, zobacz [Składniki oprogramowania RMS](https://technet.microsoft.com/e38a840e-f390-48fd-8354-50108a64f5ca).
