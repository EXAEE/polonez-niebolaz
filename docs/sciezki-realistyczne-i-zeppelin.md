# Realistyczne ścieżki: CubeSat, Kapsuła oraz analiza Zeppelina atmosferyczno-orbitalnego

Dokument roboczy oparty na fizyce, istniejących badaniach (HAPS, rockoon, airship-assisted launch) i uczciwej ocenie limitów.

---

## Część A — CubeSat (najbardziej realna ścieżka orbitalna)

### Cel
Wprowadzić projekt Niebołaz realnie na orbitę jako bezzałogowy obiekt edukacyjno-badawczy.

### Ścieżka krok po kroku

1. **Definicja misji**
   - 1U / 2U / 3U CubeSat
   - Ładunek: kamera + proste sensory + beacon open-source
   - Cel orbity: LEO (rideshare)

2. **Budowa**
   - Struktura zgodna ze standardem CubeSat
   - EPS (baterie + solar)
   - OBC + radio (UHF/VHF lub S-band)
   - Testy: vacuum, thermal, vibration (wymagane przez integratora)

3. **Wystrzelenie**
   - Rideshare (SpaceX Transporter, europejskie opcje, inne)
   - Nie budujemy własnej rakiety

4. **Operacje**
   - Stacja naziemna open-source (np. na bazie SatNOGS / własna)
   - Telemetria, komendy, ewentualnie downlink obrazu

### Co jest realne
- Koszt w skali dziesiątek–niskich setek tysięcy EUR (zależnie od ładunku i testów)
- Czas: 1–3 lata przy dobrej organizacji
- Pełna zgodność z duchem open-source i edukacji

### Czego nie robimy
- Własnej rakiety nośnej
- „Garażowego satelity bez kwalifikacji środowiskowych”

---

## Część B — Kapsuła (4–5 osób + ładunek na LEO)

### Realistyczna ocena

Kapsuła załogowa na orbitę to skala:
- Crew Dragon / Starliner / Soyuz / Apollo
- nie kontynuacja deskorolki ani paramotoru

### Wymagania minimalne (fizyka + inżynieria)
- Δv rzędu ~9–10 km/s z powierzchni (orbita + straty)
- Ochrona termiczna przy powrocie
- Systemy life support
- Abort na starcie
- Infrastruktura startowa, kontroli lotu, odzysku
- Niezawodność i certyfikacja na poziomie „nie wolno się mylić”

### Napęd
Sam układ elektryczny ani elektro-wodorowy **nie wystarcza** do wyniesienia 4–5 osób z Ziemi na LEO.  
Potrzebna jest chemia rakietowa o wysokiej gęstości energii (RP-1/LOX, CH₄/LOX, LH₂/LOX) lub równoważny system nośny.

### Realistyczne warstwy podejścia w projekcie

| Warstwa | Co można robić już teraz / w perspektywie | Status |
|---------|-------------------------------------------|--------|
| Symboliczno-badawcza | Studia masy, Δv, architektury, estetyka Kapsuły | otwarte |
| Pośrednia | Suborbitalny demonstrator / ładunek na cudzej rakiecie | trudne, ale wyobrażalne |
| Pełna orbitalna załogowa | Własny system nośny + Kapsuła | skala państwowa/przemysłowa |

**Wniosek:** Kapsułę zostawiamy jako nazwaną wizję pokoleniową. Nie planujemy jej jako kolejnego milestone po wariantach atmosferycznych.

---

## Część C — Zeppelin atmosferyczno-orbitalny (nowy wariant) — analiza wykonalności

### Propozycja użytkownika (w skrócie)
Jednostka typu Zeppelin, która:
- potrafi długo (dni/tygodnie) stabilnie latać w atmosferze (cicho / opcjonalnie stealth),
- potrafi wynieść się na orbitę w celu naprawy i umieszczania satelitów,
- w dalszej wizji: atmosferyczno-orbitalno-międzyplanetarna.

### Werdykt fizyczny (skrót)

**Czysty „Zeppelin orbitalny” (jedna maszyna unosząca się wypornością aż na orbitę) jest niemożliwy.**

Powód podstawowy:
- Wyporność (Archimedes) działa tylko w ośrodku o gęstości > 0.
- Na orbicie i w próżni gęstość atmosfery ≈ 0 → **brak siły nośnej z wyporności**.
- Orbita to nie „wysokość”, tylko **prędkość pozioma** (~7,8 km/s na LEO) + wysokość poza gęstą atmosferą.

Żaden balon / sterowiec nie „wypłynie” na orbitę.  
To nie jest kwestia lepszych materiałów — to kwestia braku medium.

### Co jest realne w pobliżu tej wizji

#### 1. Sterowiec stratosferyczny / HAPS (High-Altitude Pseudo-Satellite)
- Wysokość typowa: **18–25 km** (nie orbitа)
- Czas lotu: dni–tygodnie–miesiące (z solarem + bateriami)
- Zastosowania: obserwacja, łączność, „pseudo-satelita”
- Badania i programy: HAPS airship i fixed-wing (m.in. prace przeglądowe Gonzalo et al., projekty typu Stratobus / Sceye, NASA HAPS)
- **To jest najlepszy realny odpowiednik „długiego, stabilnego, cichego lotu” z wizji Zeppelina**

Opcja stealth/cicho: przy napędzie elektrycznym i dużej wysokości hałas spada; pełne stealth radarowe to osobna, trudna dziedzina (kształt, materiały, rozmiar sterowca działa przeciwko).

#### 2. Rockoon (balon + rakieta)
- Balon stratosferyczny unosi rakietę na ~20–35 km
- Rakieta startuje z wysokości i robi resztę Δv do orbity / suborbity
- Historycznie: Van Allen; współcześnie: testy firm typu B2Space, Zero 2 Infinity, prace akademickie
- Sens: tańszy dostęp dla małych satelitów, mniej oporu i mniejszy wymagany Δv rakiety
- **Nie jest to sterowiec wracający z orbity** — to system startowy

#### 3. Airship-assisted launch
- Duży sterowiec jako pierwszy, wolny „stopień zero”
- Uwalnia rakietę na wysokości z pewną prędkością początkową
- Istnieją studia koncepcyjne (m.in. prace o airship-assisted space launch)
- Nadal rakieta robi robotę orbitalną; sterowiec zostaje w atmosferze

#### 4. „Orbital airship” / vacuum airship w próżni
- Koncepty vacuum balloon są badane teoretycznie, ale:
  - w atmosferze problemem jest wytrzymałość skorupy na ciśnienie zewnętrzne vs masa,
  - w próżni orbitalnej **nie ma czego wypierać** — nie ma sensu wypornościowego.
- Nie rozwiązuje to problemu osiągnięcia orbital velocity.

### Czego brakuje do wizji „Zeppelin sam wchodzi na orbitę i wraca”

| Brak | Dlaczego krytyczne |
|------|--------------------|
| Siła nośna w próżni | Wyporność = 0 poza atmosferą |
| Δv ~9–10 km/s | Sterowiec nie generuje orbital velocity |
| Ochrona termiczna powrotu | Wejście w atmosferę z orbital velocity |
| Masa układu dual-mode | System atmosferyczny + system kosmiczny w jednej maszynie zabija masę |
| Napęd i paliwo orbitalne | Elektryczność/H₂ nie zastępują stopnia nośnego z Ziemi |
| Operacje orbitalne (serwis satelitów) | Wymagają statku kosmicznego z manewrowaniem, manipulatorami, zbliżaniem |

### Lepszy kierunek / rekomendowany mix dla Niebołaza

Zamiast jednego „Zeppelina orbitalno-międzyplanetarnego” — **rozdzielone warstwy**:

1. **Niebołaz HAPS / Sterowiec stratosferyczny**  
   Długi, stabilny, cichy lot w atmosferze (dni–tygodnie).  
   Najbliższy realny odpowiednik atmosferycznej części wizji.

2. **Niebołaz Rockoon / Airship-assist**  
   Sterowiec lub balon jako stopień zero do wynoszenia małych rakiet z CubeSatami.  
   Realny związek z umieszczaniem satelitów — bez udawania, że sterowiec sam jest na orbicie.

3. **Satelita + ewentualnie serwis orbitalny**  
   CubeSat własny; serwis satelitów to osobna klasa misji (OSAM), daleka i przemysłowa.

4. **Kapsuła**  
   Zostaje wizją załogową pokoleniową, nie powiązaną liniowo ze sterowcem.

### Propozycja nazewnicza w rodzinie

- **Niebołaz HAPS** (sterowiec / platforma stratosferyczna) — nowy, realny wariant atmosferyczny dalekiego zasięgu czasowego
- **Niebołaz Rockoon** — system startowy balon/sterowiec + rakieta dla małych satelitów
- Unikać nazwy sugerującej, że ten sam kadłub „płynie na orbitę”

---

## Podsumowanie wykonalności

| Koncept | Wykonalność | Komentarz |
|---------|-------------|-----------|
| CubeSat na rideshare | **Wysoka** | Najlepszy pierwszy krok orbitalny |
| Kapsuła 4–5 os. na LEO | **Ekstremalnie niska w DIY** | Skala przemysłowa/państwowa |
| Sterowiec stratosferyczny (HAPS) tygodnie w powietrzu | **Średnia–wysoka badawczo** | Realny kierunek, aktywne badania |
| Rockoon / airship-assist dla małych satelitów | **Średnia** | Testowane współcześnie |
| Jeden Zeppelin sam wchodzący na orbitę i serwisujący satelity | **Niemożliwy** | Brak wyporności w próżni + brak Δv |
| Zeppelin międzyplanetarny | **Niemożliwy w tej architekturze** | Jeszcze dalej od fizyki wyporności |

---

## Rekomendacja dla repo

1. Rozwijamy **CubeSat** jako konkretną ścieżkę.
2. **Kapsułę** trzymamy jako nazwaną wizję z twardymi limitami.
3. Dodajemy wariant **HAPS / Sterowiec stratosferyczny** jako uczciwe spełnienie atmosferycznej części pomysłu „Zeppelina”.
4. Opcjonalnie dokumentujemy **Rockoon** jako sposób wiązania sterowca z umieszczaniem satelitów — bez mieszania go z orbitą samej platformy.
5. Nie budujemy narracji o sterowcu orbitalno-międzyplanetarnym jako jednym pojeździe.

Fizyka nie jest wrogiem wizji — jest jej filtrem. Po filtrze zostaje więcej realnych projektów, nie mniej.
