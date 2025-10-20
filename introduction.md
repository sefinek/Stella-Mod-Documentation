[//]: # (Title: Wprowadzenie - Dokumentacja Stella Mod)
[//]: # (Description: Kompletny przewodnik po Genshin Stella Mod. Dowiedz się, jak zainstalować, skonfigurować i bezpiecznie korzystać z modów takich jak ReShade, 3DMigoto i FPS Unlocker, aby ulepszyć grafikę i płynność gry Genshin Impact.)
[//]: # (Tags: Genshin Stella Mod, Dokumentacja Stella Mod, Instalacja Stella Mod, Konfiguracja Stella Mod, ReShade, 3DMigoto, Odblokowanie FPS, Mody Genshin Impact, Bezpieczne modowanie, Stella Mod Plus)
[//]: # (Canonical: /genshin-stella-mod/docs?page=introduction)
[//]: # (Contributors: Sefinek)

# Genshin Stella Mod: Wprowadzenie do dokumentacji
<div align="center">
    Zapoznaj się z kompletnym przewodnikiem.
    Niezależnie od tego, czy dopiero zaczynasz, czy korzystasz z projektu od dawna – ta dokumentacja zawiera wszystkie informacje o instalacji, konfiguracji oraz możliwościach Oprogramowania <b>Genshin Stella Mod</b>.
    Przeglądaj interesujące Cię sekcje i odkryj, jak <b>Stella Mod</b> może ulepszyć Twoje wrażenia z gry w Genshin Impact.
</div>
<br>

<div class="mafumafu-container">
    <div class="bottom-image">
        <a href="https://sefinek.net/genshin-stella-mod?download=true&referrer=introduction"><img src="https://sefinek.net/images/stella/mafumafu/download.png" alt="Download Stella Mod" height="148"></a>
        <a href="https://discord.com/invite/k2wfGRq4dT" target="_blank"><img src="https://sefinek.net/images/stella/mafumafu/discord.png" alt="Discord" height="148"></a>
    </div>
</div>

## Definicje <!-- {#definitions} -->
Poniższe definicje stosuje się we wszystkich dokumentach projektu **Genshin Stella Mod**, w tym w **EULA**, **Polityce prywatności** i innych materiałach powiązanych.

- **Oprogramowanie** – Genshin Stella Mod oraz wszystkie jego komponenty, pliki binarne, biblioteki, moduły, skrypty i zasoby potrzebne do działania.
- **Launcher** – aplikacja służąca do uruchamiania, konfiguracji i aktualizacji Oprogramowania, a także do komunikacji z serwerem API Autora.
- **Użytkownik** – osoba fizyczna lub prawna, która instaluje lub korzysta z Oprogramowania.
- **Autor** – Sefinek; właściciel praw autorskich, twórca i licencjodawca Oprogramowania.
- **Licencja** – umowa regulująca zasady korzystania z Oprogramowania (EULA).
- **Serwer prywatny** – infrastruktura należąca do Autora, zlokalizowana fizycznie w Polsce, bez wykorzystania usług chmurowych.
- **Dane techniczne** – informacje generowane przez Oprogramowanie w celach diagnostycznych lub statystycznych (np. ID urządzenia, logi, dane o konfiguracji).
- **Identyfikator urządzenia (ID)** – unikalny skrót generowany lokalnie przez Oprogramowanie na podstawie numerów seryjnych podzespołów; służy do rozpoznawania urządzeń i zapobiegania nadużyciom.
- **API** – interfejs komunikacyjny między Oprogramowaniem a serwerem Autora; odpowiada za aktualizacje, synchronizację oraz weryfikację licencji Stella Plus.
- **Honeypot** – mechanizm bezpieczeństwa służący do wykrywania i rejestrowania prób nieautoryzowanego dostępu.
- **Logi Oprogramowania** – dane diagnostyczne dotyczące działania Oprogramowania; mogą być przesyłane na serwer wyłącznie za zgodą Użytkownika.
- **Dane osobowe** – informacje umożliwiające identyfikację osoby fizycznej; Oprogramowanie ich nie gromadzi ani nie przetwarza.
- **RODO** – Rozporządzenie Parlamentu Europejskiego i Rady (UE) 2016/679 w sprawie ochrony danych osobowych.

W przypadku braku definicji danego terminu należy interpretować go zgodnie z jego znaczeniem prawnym lub kontekstowym w dokumentacji projektu.


### Znaczenie emoji <!-- {#emoji-legend} -->
| Emoji                         | <div align="left">Znaczenie</div> | Emoji                        | <div align="left">Znaczenie</div> | Emoji                       | <div align="left">Znaczenie</div> |
|-------------------------------|-----------------------------------|:-----------------------------|:----------------------------------|:----------------------------|:----------------------------------|
| <div align="center">✔️</div>  | Tak / Obsługiwane                 | <div align="center">❌️</div> | Nie / Nieobsługiwane              | <div align="center">❓</div> | Niepewne                          |
| <div align="center">🎯️</div> | Domyślnie nieobsługiwane          | <div align="center">🤔</div> | Nieprzetestowane                  |                             |                                   |



## Czym jest Stella Mod Launcher? <!-- {#what-is-sml} -->
Jest to oficjalna aplikacja uruchamiająca **Genshin Stella Mod**.
Została ona napisana w języku [C#](https://learn.microsoft.com/dotnet/csharp) przy użyciu platformy [.NET 9.0](https://dotnet.microsoft.com/en-us/download/dotnet/9.0).
Launcher umożliwia Użytkownikowi pobieranie aktualizacji Oprogramowania.
Priorytetem jest **bezpieczeństwo**, dlatego system dystrybucji został zaprojektowany tak, aby zapewnić integralność plików oraz ochronę danych Użytkownika.


## Czym jest Genshin Stella Mod? <!-- {#what-is-gsm} -->
**Genshin Stella Mod** to starannie opracowany zestaw modów, mających na celu ulepszenie wrażeń z gry **Genshin Impact**.
- Oferuje szeroki wybór filtrów, presetów – od kolorowych i dynamicznych po realistyczne i filmowe. Każdy efekt można dostosować za pomocą nakładki **ReShade**.
- Jedną z kluczowych funkcji jest również **odblokowanie limitu FPS**, co umożliwia płynniejszą rozgrywkę, szczególnie na monitorach o wysokiej częstotliwości odświeżania.
- Dla subskrybentów **Stella Mod Plus** dostępne są dodatkowe funkcje, w tym integracja z **3DMigoto**, która pozwala na modyfikacje modeli postaci i wiele innych opcji wizualnych.

Projekt jest stale rozwijany – Autor dba o aktualizacje, optymalizację i wsparcie techniczne dla wszystkich Użytkowników Oprogramowania.


## Czy Stella Mod jest bezpieczny? <!-- {#is-it-safe} -->
**Tak, całkowicie.**
Oprogramowanie zostało zaprojektowane tak, aby **nie modyfikować oryginalnych plików gry**. Działa w niezależnej warstwie, poprawiając efekty wizualne i wydajność bez ingerencji w pliki gry.
Dzięki temu rozgrywka pozostaje nienaruszona, a oryginalny kod gry zachowuje pełną integralność.


## Czy HoYoverse ma z tym coś wspólnego? <!-- {#hoyoverse-affiliation} -->
Nie. Projekt **Genshin Stella Mod** nie jest w jakikolwiek sposób powiązany z **miHoYo**, **COGNOSPHERE**, **HoYoverse**.
Wszystkie znaki towarowe i prawa autorskie należą do ich właścicieli.


## Pomóż ulepszyć dokumentację Genshin Stella Mod <!-- {#contributing} -->
Chcesz pomóc w ulepszaniu tej dokumentacji? Możesz to zrobić, wysyłając [Pull Request](https://github.com/sefinek/Stella-Mod-Documentation/pulls) na GitHub.
Każda poprawka – od korekty błędów po dodanie nowych sekcji – jest mile widziana. Doceniamy każdą pomoc i dążymy do tego, by dokumentacja była jak najbardziej przyjazna i kompletna.


## Do zobaczenia w Stella Mod <!-- {#closing-note} -->
Dziękujemy za zainteresowanie **Genshin Stella Mod**! Jesteśmy pewni, że docenisz ulepszoną grafikę i bardziej immersyjne doświadczenie w świecie **Teyvat**. Miłego dnia!
