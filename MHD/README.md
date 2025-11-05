# MHD Flasher - Kompletny Przewodnik

## 1. Wprowadzenie do MHD Flasher

**MHD Flasher** to jedna z najpopularniejszych platform do modyfikacji oprogramowania sterownika silnika (ECU) w samochodach BMW, szczególnie dla silników N54, N55, B58 i S55. Umożliwia wgrywanie gotowych map (Stage 1, 2, 2+, E30, itp.) oraz logowanie parametrów pracy silnika.

## 2. Wymagania Wstępne

Przed rozpoczęciem flashowania upewnij się, że spełniasz poniższe warunki:

| Wymaganie | Szczegóły |
| :--- | :--- |
| **Adapter OBD** | **OBDLink CX+** (zalecany ze względu na stabilność Bluetooth) lub kabel **ENET/OBD2** z odpowiednim adapterem OTG (dla urządzeń z Androidem/iOS). |
| **Urządzenie** | Smartfon lub tablet z systemem Android lub iOS. |
| **Akumulator** | **Kluczowe!** Akumulator musi być w pełni naładowany (zalecane podłączenie prostownika o stabilnym napięciu 13.5V+). Flashowanie trwa od 5 do 30 minut (w zależności od typu flasha), a spadek napięcia może uszkodzić ECU. |
| **Licencje** | Zakupiona licencja MHD (np. Flasher License, Stage 1/2/3 Map Pack). |

## 3. Proces Flashowania

### 3.1. Przygotowanie

1.  **Podłącz adapter:** Wepnij adapter OBD (np. OBDLink CX+) do portu OBD w samochodzie.
2.  **Włącz zapłon:** Wciśnij przycisk START bez wciskania pedału hamulca/sprzęgła (zapłon włączony, silnik wyłączony).
3.  **Połącz z aplikacją:** Uruchom aplikację MHD, wybierz swój adapter i nawiąż połączenie.

### 3.2. Wybór Mapy i Opcji

1.  Przejdź do sekcji **Flash**.
2.  Wybierz żądaną mapę (np. Stage 2+ dla silnika N55).
3.  Skonfiguruj opcje mapy (tzw. **OTS Options**), takie jak:
    *   **Cold Start Noise Reduction:** Wyciszenie głośnego rozruchu.
    *   **Exhaust Burble:** Ustawienie głośności i czasu trwania strzałów z wydechu.
    *   **Speed Limiter Removal:** Usunięcie ogranicznika prędkości.
    *   **Catless Downpipe:** Wyłączenie kontroli katalizatora (wymagane przy braku katalizatora).

### 3.3. Wgrywanie Mapy

1.  Aplikacja poprosi o potwierdzenie, że akumulator jest naładowany.
2.  Rozpocznie się proces flashowania. **NIE PRZERYWAJ TEGO PROCESU!** Nie dotykaj telefonu, nie wyłączaj zapłonu, nie otwieraj drzwi.
3.  Po zakończeniu, aplikacja poinformuje o sukcesie i poprosi o wyłączenie/włączenie zapłonu.

## 4. Logowanie (Datalogging)

Logowanie jest kluczowe do monitorowania zdrowia silnika i weryfikacji, czy mapa działa poprawnie.

1.  W aplikacji MHD przejdź do sekcji **Monitor/Log**.
2.  Wybierz parametry do logowania (zalecane: **Boost Target**, **Boost Actual**, **AFR Bank 1**, **Timing Correction**, **IAT**, **LPFP**, **HPFP**).
3.  Rozpocznij logowanie, a następnie wykonaj jazdę testową (np. pełne przyspieszenie na 3. biegu od 2500 do 6500 RPM).
4.  Zapisz plik logu (zazwyczaj w formacie CSV) i przeanalizuj go za pomocą narzędzi online (np. Datazap.me).

## 5. Wskazówki i Najlepsze Praktyki

*   **Zawsze używaj prostownika** podczas flashowania, zwłaszcza przy pierwszym flashu, który jest najdłuższy (pełne wgranie).
*   **Sprawdź połączenie:** Upewnij się, że adapter jest stabilnie podłączony i sparowany przed rozpoczęciem.
*   **Odczekaj:** Po flashowaniu odczekaj kilka minut, zanim uruchomisz silnik, aby wszystkie moduły się zresetowały.
*   **Monitoruj korekty zapłonu (Timing Corrections):** Jeśli są wysokie (np. -5 stopni lub więcej), może to oznaczać problem z paliwem (niskie oktanowo) lub świecami/cewkami. Przestań jeździć agresywnie i zrób logi.
*   **Kopiuj oryginalny plik:** MHD automatycznie zapisuje kopię oryginalnego oprogramowania (stock tune) na Twoim urządzeniu. Upewnij się, że masz tę kopię zapasową.
