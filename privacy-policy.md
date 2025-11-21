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
1. **Identyfikator urządzenia (Device ID)** – unikalny hash generowany na podstawie identyfikatorów sprzętowych podzespołów komputera. Służy do weryfikacji licencji, anonimowych statystyk oraz zapobiegania nadużyciom.
2. **Identyfikatory sprzętowe** – w celu weryfikacji urządzenia i zapobiegania nadużyciom zbierane są:
   - identyfikator procesora (CPU ID),
   - identyfikator płyty głównej (Motherboard ID),
   - identyfikator dysku systemowego (Disk ID),
   - adres MAC karty sieciowej,
   - pełna nazwa komputera (Full Computer Name).
3. **Podstawowe informacje** – adres IP, wersja systemu operacyjnego, region systemowy, numer build Windows.
4. **Dane anty-fraudowe** – wyniki detekcji maszyn wirtualnych oraz debuggerów (w celu ochrony przed nadużyciami). Analiza ta odbywa się lokalnie na komputerze Użytkownika.

Każde dane są **szyfrowane za pomocą kryptografii** przed wysłaniem ich na serwer.

### Dane dla subskrybentów Stella Mod Plus
W przypadku posiadania aktywnej subskrypcji Stella Mod Plus, zbierane są dodatkowo:
1. **Dane konta** – adres email, nazwa użytkownika.
2. **Awatar użytkownika**:
   - jeśli Użytkownik loguje się przez dostawców OAuth2, w bazie danych zapisywany jest wyłącznie **link do awatara** udostępniony przez danego dostawcę (Discord, Google, Twitter, Twitch, Microsoft). Sam plik obrazu **nie jest pobierany ani przechowywany** na serwerze Autora,
   - jeśli Użytkownik prześle **własny awatar** (custom avatar), plik jest przesyłany i przechowywany na serwerze Autora.
3. **Dane z dostawców OAuth2** – jeśli Użytkownik zdecyduje się zalogować przez zewnętrzne usługi (Discord, Google, Twitter, Twitch lub Microsoft), zbierane są dane profilowe udostępnione przez tych dostawców, takie jak:
   - nazwa użytkownika,
   - adres email.
4. **Integracja z Discord** – w przypadku połączenia konta z Discord, serwer API może zarządzać rolami na serwerze Discord oraz wysyłać powiadomienia (za zgodą Użytkownika).
5. **Dane płatności** – token subskrypcji jest powiązany z adresem email użytym podczas zakupu. Płatności są przetwarzane przez Stripe. Autor nie ma dostępu do danych płatniczych.
6. **Preferencje użytkownika** – wybór preferowanego serwera mirror, preferencje korespondencji (email, Discord), język, region.
7. **Historia korespondencji** – zapisywane są informacje o mailach wysłanych przez system (temat, data, status odczytania) w celu prowadzenia historii komunikacji z Użytkownikiem.

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
Dostęp do logów posiada wyłącznie Autor. Dane nie są przekazywane osobom trzecim, z wyjątkiem sytuacji wymaganych przepisami prawa (np. na żądanie organów ścigania).
Wszystkie dane są przechowywane na prywatnym serwerze w Polsce, bez użycia zewnętrznych usług chmurowych lub innych serwerów VPS/dedykowanych.
Żaden inny podmiot zewnętrzny nie ma dostępu do nich.

### Czy zbieramy dane osobowe?
- **Wersja darmowa**: Oprogramowanie **nie zbiera danych osobowych** w standardowym użyciu. Device ID sam w sobie nie pozwala na identyfikację konkretnej osoby.
  Jednak **adres IP** może być uznany za daną osobową w rozumieniu RODO, dlatego jest on przetwarzany wyłącznie w celach technicznych opisanych powyżej.
- **Stella Mod Plus**: W przypadku aktywnej subskrypcji zbierane są następujące dane osobowe:
  - adres email i nazwa użytkownika,
  - dane profilowe z dostawców OAuth2 (jeśli użyte),
  - identyfikatory sprzętowe połączone z kontem użytkownika,
  - token subskrypcji i dane płatności (przetwarzane przez Stripe),
  - historia korespondencji i preferencje użytkownika.

  Dane te są przetwarzane wyłącznie w celu weryfikacji licencji, zarządzania subskrypcją, świadczenia usługi oraz komunikacji z Użytkownikiem.
  Podczas procesu płatności dane użytkownika (nazwa, email) są przekazywane do Stripe zgodnie z ich polityką prywatności.
- **Dostawcy OAuth2**: Jeśli Użytkownik loguje się przez Discord, Google, Twitter, Twitch lub Microsoft, dane są zbierane zgodnie z polityką prywatności tych dostawców. Autor przetwarza tylko te dane, które są niezbędne do uwierzytelnienia i zarządzania kontem.

Oprogramowanie **nie monitoruje aktywności Użytkownika** podczas grania w Genshin Impact i **nie zapisuje historii działań w grze**.
Oprogramowanie **nie wykorzystuje plików cookie ani narzędzi analitycznych** do śledzenia zachowań użytkownika.


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
- Logi Oprogramowania mają wyłącznie cel diagnostyczny. Ich przesłanie może pomóc w wykrywaniu błędów lub problemów technicznych, jednak decyzja o ich analizie należy w pełni do Autora.
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
<i>Ostatnia aktualizacja: 21 listopada 2025 r.</i>
