# Szczegóły techniczne – Polonez Niebołaz

## 1. Bezzałogowy Niebołaz (dron)

### Cel
Platforma testowa napędów, sterowania, struktur i (w przyszłości) systemów wodorowych bez ryzyka dla człowieka.

### Założenia techniczne
- Układ: multirotor (4–8 wirników) lub konfiguracja hybrydowa
- Masa startowa: zależna od wersji (od małych testowych po większe transportowe lekkie)
- Napęd: elektryczny (baterie Li-ion / LiFePO4)
- Sterowanie: open-source flight stack (ArduPilot / PX4 lub własny)
- Telemetria + failsafe (powrót / lądowanie przy utracie łączności)
- Opcjonalnie: zaczep ładunku, sensory obserwacyjne

### Priorytety
- Redundancja
- Logi z każdego lotu
- Łatwa wymiana silników, ESC i śmigieł

---

## 2. Deskorolka (1 osoba, max 5–10 m)

### Cel
Eksperyment ze sterowaniem balansem ciała tuż nad ziemią.

### Napęd i struktura
- Multirotor o dużej powierzchni nośnej (niższe obciążenie dysku → łatwiejsza stabilizacja)
- Platforma stojąca z powierzchnią antypoślizgową
- Opcjonalne niskie uchwyty / balustrada
- Klatka lub strefy zgniotu chroniące nogi i miednicę przy upadku

### Sterowanie
- IMU + detekcja przechyłu platformy / stóp
- Komputer stabilizuje wysokość i poziom, człowiek zadaje kierunek przez balans
- Twardy limiter wysokości (barometr + lidar/sonar)
- Max wysokość: 5–10 m (programowo + najlepiej sprzętowo)

### Bezpieczeństwo
- Automatyczne zejście przy utracie stabilności
- Przycisk zabijający ciąg (kill switch) łatwo dostępny
- Testy najpierw z manekinem / obciążeniem

### Energia
- Wyłącznie baterie
- Krótki czas lotu (minuty) – akceptowalny przy charakterze eksperymentu

---

## 3. Paramotor / Motorower powietrzny

### Cel
Najbardziej klasyczna i najbezpieczniejsza ścieżka załogowa.

### Układ
- Skrzydło paralotniowe (certyfikowane lub sprawdzone konstrukcje)
- Wózek 1- lub 2-osobowy
- Napęd: silnik elektryczny + śmigło w klatce ochronnej
- Opcja range extendera wodorowego / małego generatora w późniejszej fazie

### Parametry orientacyjne
- Moc: dobrana do masy (typowo kilkanaście–kilkadziesiąt kW przy starcie)
- Czas lotu: zależny od baterii (cel realistyczny: 20–60 min w wersji elektrycznej)
- Start: z rozbiegiem lub z wózka

### Bezpieczeństwo
- Klatka śmigła
- Systemy ratunkowe (spadochron / systemy ultralekkie – do rozważenia)
- Szkolenie i procedury jak w paramotoryzacji

---

## 4. Dwuosobowy multikopter elektro-wodorowy

### Cel
Ambitny VTOL z dwoma osobami.

### Napęd
- Główny ciąg: silniki elektryczne
- Energia: baterie + ogniwo paliwowe wodorowe LUB mały generator wodorowy jako range extender
- Wodór traktowany jako sposób na wydłużenie czasu lotu, nie jako magiczne rozwiązanie wszystkich problemów

### Główne wyzwania techniczne
- Gęstość energii i masa całego układu
- Redundancja wirników i elektroniki
- Zarządzanie ciepłem
- Hałas
- Przechowywanie wodoru (bezpieczeństwo)
- Certyfikacja i prawo

### Status
Daleki cel badawczy. Nie jest najbliższym milestone’em.

---

## Wspólne zasady techniczne dla całej rodziny

1. Failsafe zawsze obecny
2. Logi z każdego testu
3. Najpierw bezzałogowe i nisko, potem wyżej i z człowiekiem
4. Żadnych lotów nad ludźmi i twardymi przeszkodami w fazie eksperymentalnej
5. Dokumentacja otwarta
