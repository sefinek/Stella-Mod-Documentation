[//]: # (Title: Polityka prywatności - Stella Mod Documentation)
[//]: # (Description: Poznaj zasady ochrony danych w Genshin Stella Mod. Dowiedz się, jak oprogramowanie chroni Twoją prywatność. Nigdy nie gromadzi żadnych danych osobowych. Zawsze zapewnia bezpieczeństwo.)
[//]: # (Tags: Polityka prywatności, Ochrona danych, Genshin Stella Mod, Prywatność użytkownika, Bezpieczeństwo danych, API v8, Honeypot, Logi aplikacji, RODO, Stella Mod Documentation, Bezpieczne oprogramowanie)
[//]: # (Canonical: /genshin-stella-mod/docs?page=privacy-policy)
[//]: # (Contributors: Sefinek)

# Polityka prywatności i bezpieczeństwo danych <!-- {#privacy-overview} -->
Oprogramowanie zostało zaprojektowane z pełnym poszanowaniem prywatności Użytkowników. Twoja prywatność jest naszym priorytetem.

## Jakie dane zbieramy? <!-- {#what-data-we-collect} -->

### Dane techniczne (zbierane automatycznie)
Oprogramowanie automatycznie zbiera i wysyła do serwera Autora następujące dane techniczne:
1. **Identyfikator urządzenia (Device ID)** – unikalny hash generowany na podstawie numerów seryjnych podzespołów komputera (procesor, płyta główna, dysk systemowy itp.). Służy do weryfikacji licencji, anonimowych statystyk oraz zapobiegania nadużyciom.
2. **Podstawowe informacje** – adres IP, wersja systemu operacyjnego, region systemowy, numer build Windows.
3. **Dane anty-fraudowe** – wyniki detekcji maszyn wirtualnych oraz debuggerów (w celu ochrony przed nadużyciami). Analiza ta odbywa się lokalnie na komputerze Użytkownika.

Każde dane są **szyfrowane za pomocą kryptografii** przed wysłaniem ich na serwer.

### Dane dla subskrybentów Stella Mod Plus
W przypadku posiadania aktywnej subskrypcji Stella Mod Plus, zbierane są dodatkowo adresy email oraz nazwy użytkowników.
Token subskrypcji jest powiązany z adresem email użytym podczas zakupu (przetwarzanym przez Stripe).

### Logowanie adresów IP i żądań API <!-- {#ip-logging} -->
Serwery Genshin Stella Mod automatycznie zapisują podstawowe informacje o zapytaniach do backendu, w tym:
- **adres IP klienta API**,
- **dokładny timestamp zapytania**,
- **endpoint API**,
- **informacje o kliencie HTTP (wyłącznie sam User-Agent)**: `Mozilla/5.0 (compatible; StellaLauncher/X.Y.Z.W; +https://stella.sefinek.net)`,
- **status odpowiedzi serwera**.

#### Cel przetwarzania:
Dane te są zapisywane wyłącznie w celach:
- zapewnienia bezpieczeństwa i stabilności infrastruktury,
- ochrony przed nadużyciami i atakami (np. DDoS, brute-force, flood),
- diagnozowania błędów technicznych,
- analizy wydajności systemu oraz prowadzenia anonimowych statystyk technicznych.

#### Podstawa prawna przetwarzania:
Podstawą prawną przetwarzania adresu IP jest **art. 6 ust. 1 lit. f RODO**. Uzasadniony interes Administratora w zapewnieniu bezpieczeństwa i prawidłowego działania usługi.

#### Okres przechowywania:
Dane z logów są **przechowywane tymczasowo**, zwykle nie dłużej niż **2 lata**, chyba że wymagają dłuższego przechowania w związku z incydentem bezpieczeństwa lub dochodzeniem naruszenia.

#### Zakres i dostęp:
Dostęp do logów mają wyłącznie **właściciel systemu**. Dane nie są przekazywane osobom trzecim, z wyjątkiem sytuacji wymaganych przepisami prawa (np. na żądanie organów ścigania).
Wszystkie dane są przechowywane na prywatnym serwerze w Polsce, bez użycia zewnętrznych usług chmurowych lub innych serwerów VPS/dedykowanych. Żaden inny podmiot zewnętrzny nie ma dostępu do tych danych.

### Czy zbieramy dane osobowe?
- **Wersja darmowa**: Oprogramowanie **nie zbiera danych osobowych** w standardowym użyciu. Device ID sam w sobie nie pozwala na identyfikację konkretnej osoby.  
  Jednak **adres IP** może być uznany za daną osobową w rozumieniu RODO, dlatego jest on przetwarzany wyłącznie w celach technicznych opisanych powyżej.
- **Stella Mod Plus**: Adres e-mail użyty podczas zakupu, w połączeniu z Device ID, adresem IP oraz tokenem subskrypcji, stanowi dane osobowe w zakresie niezbędnym do weryfikacji licencji, zarządzania subskrypcją oraz świadczenia usługi.  
  Adres e-mail jest przetwarzany wyłącznie w celu przypisania licencji do konta użytkownika i obsługi płatności (np. weryfikacja statusu subskrypcji w Stripe). Należy pamiętać, że nazwa użytkownika i adres e-mail zostaną przekazane do firmy Stripe podczas procesu płatności.

Oprogramowanie **nie monitoruje aktywności Użytkownika** podczas grania w Genshin Impact i **nie zapisuje historii działań**.  
Oprogramowanie **nie wykorzystuje plików cookie ani narzędzi analitycznych**.


## Logi Oprogramowania <!-- {#application-logs} -->
Oprogramowanie może co pewien czas zapytać, czy Użytkownik chce przesłać Logi Oprogramowania na serwer Autora.
Decyzja ta należy **wyłącznie do Użytkownika** i **nie wpływa na działanie Oprogramowania**.

### Co jest wysyłane podczas przesyłania logów?
Jeśli Użytkownik wyrazi zgodę na przesłanie logów, na serwer zostanie wysłane zaszyfrowane oraz zabezpieczone archiwum ZIP zawierające:
1. pliki logów Oprogramowania,
2. Device ID,
3. konfigurację FPS Unlocker,
4. plik ReShade.ini,
5. raport diagnostyczny dxdiag.
6. specyfikacja sprzętu (CPU, RAM, GPU, dyski, BIOS, bateria),
7. informacje sieciowe, w tym adresy IP prywatne, jak i publiczne oraz inne szczegóły połączenia sieciowego.

### Dodatkowe informacje
- Logi Oprogramowania** mają wyłącznie cel diagnostyczny. Ich przesłanie może pomóc w wykrywaniu błędów lub problemów technicznych, jednak decyzja o ich analizie należy w pełni do Autora.
- Autor nie ma obowiązku przeglądania ani analizowania logów. Może je przejrzeć według własnego uznania lub kaprysu, jeśli uzna to za przydatne w danym momencie. Większość przesłanych logów nigdy nie jest analizowana ani sprawdzana.
- Logi nie są wykorzystywane do żadnych innych celów. W szczególności nie służą do profilowania, marketingu ani analizy zachowań Użytkowników.
- Użytkownik może w każdej chwili poprosić o wgląd w przesłane logi lub zażądać ich trwałego usunięcia z serwera. Po otrzymaniu takiego żądania logi zostaną całkowicie i nieodwracalnie usunięte.


## Bezpieczne przechowywanie danych <!-- {#secure-storage} -->
Wszystkie dane identyfikacyjne (np. ID urządzenia) przechowywane są w **bazie danych na prywatnym serwerze fizycznie zlokalizowanym w Polsce**.
Serwer działa w **środowisku domowym**, bez użycia infrastruktury chmurowej ani zewnętrznych centrów danych.
Takie rozwiązanie zapewnia pełną kontrolę nad przetwarzaniem informacji i eliminuje ryzyko przekazywania danych podmiotom trzecim.
**[sefinek.net](https://sefinek.net)** pozostaje **jedynym właścicielem i administratorem danych**.
ŻADNE dane nie są udostępniane żadnym osobom ani instytucjom zewnętrznym.


## Bezpieczeństwo API i zapobieganie nadużyciom <!-- {#api-security} -->
Aktualna wersja API (v8) zawiera liczne mechanizmy zabezpieczające przed nadużyciami, nieautoryzowanym dostępem oraz atakami automatycznymi.

### Mechanizm Honeypot: obrona przed zagrożeniami <!-- {#honeypot-mechanism} -->
**Honeypot** to specjalny mechanizm służący do wykrywania i neutralizacji prób włamań.
Symuluje on podatne środowisko w celu wykrycia podejrzanych działań, rejestruje próby ataku oraz analizuje ich charakter.

### Procedura odwołania od błędnej klasyfikacji <!-- {#false-appeal-process} -->
Adresy IP lub zachowania błędnie uznane za podejrzane są weryfikowane i mogą zostać odblokowane po analizie.
Jeśli Użytkownik uważa, że otrzymał niesłusznego bana, może złożyć odwołanie poprzez [system ticketów](https://patrons.sefinek.net/tickets).

Każde odwołanie jest rozpatrywane **ręcznie i indywidualnie**, aby uniknąć niesprawiedliwego blokowania.


## Prawa Użytkownika zgodnie z RODO <!-- {#gdpr-rights} -->
Zgodnie z **Rozporządzeniem Parlamentu Europejskiego i Rady (UE) 2016/679 (RODO)** Użytkownik ma prawo do:
- **dostępu** do swoich danych osobowych,
- **sprostowania** nieprawidłowych danych,
- **usunięcia** swoich danych ("prawo do bycia zapomnianym"),
- **ograniczenia przetwarzania** danych,
- **wniesienia sprzeciwu** wobec przetwarzania danych.

Wszelkie żądania dotyczące danych można zgłaszać bezpośrednio na adres contact@sefinek.net.


## Kontakt <!-- {#contact} -->
W sprawach związanych z prywatnością, dostępem do danych lub ich usunięciem prosimy o kontakt z Autorem: **Sefinek** <<contact@sefinek.net>> ([https://sefinek.net](https://sefinek.net))


<br>
<i>Ostatnia aktualizacja: 2 listopada 2025 r.</i>