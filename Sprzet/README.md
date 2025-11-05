# Sprzęt - OBDLink CX+ vs. Kabel ENET/OBD2

Wybór odpowiedniego adaptera jest kluczowy dla stabilności i bezpieczeństwa operacji flashowania i kodowania. Poniżej znajduje się porównanie dwóch najczęściej używanych rozwiązań: **OBDLink CX+** i kabla **ENET/OBD2**.

## 1. Porównanie Adapterów

| Cecha | OBDLink CX+ | Kabel ENET/OBD2 |
| :--- | :--- | :--- |
| **Typ Połączenia** | Bluetooth 5.1 (BLE) | Ethernet (wymaga adaptera) |
| **Kompatybilność** | MHD, xHP, BimmerCode, BimmerLink | Bootmod3, BimmerCode, E-Sys, ISTA |
| **Szybkość Flashowania** | Bardzo szybki (dzięki BLE), ale wolniejszy niż ENET. | Najszybszy, szczególnie przy Initial Flash (Bootmod3). |
| **Stabilność** | Bardzo wysoka. Połączenie Bluetooth jest stabilne. | Bardzo wysoka. Połączenie przewodowe jest niezawodne. |
| **Wymagane Urządzenie** | Smartfon/Tablet (iOS/Android) | Laptop (Windows/macOS) lub Tablet/Smartfon z adapterem Ethernet. |
| **Wygoda Użycia** | Najwyższa. Bezprzewodowy, łatwe podłączenie. | Niższa. Wymaga kabla i często dodatkowego adaptera. |
| **Zalecany do** | BimmerCode, xHP, MHD (codzienne użycie) | Bootmod3 (Initial Flash), E-Sys, ISTA (zaawansowana diagnostyka) |

## 2. OBDLink CX+ - Instrukcja Użycia

### 2.1. Parowanie

1.  Wepnij OBDLink CX+ do portu OBD.
2.  Włącz zapłon.
3.  W przeciwieństwie do starszych adapterów, **OBDLink CX+ nie wymaga ręcznego parowania w ustawieniach Bluetooth urządzenia**.
4.  Uruchom aplikację (MHD, xHP, BimmerCode).
5.  W ustawieniach aplikacji wybierz **OBDLink CX+** jako adapter. Aplikacja sama nawiąże połączenie przez Bluetooth Low Energy (BLE).

### 2.2. Wskazówki

*   **Tryb Niskiego Poboru Mocy:** CX+ automatycznie przechodzi w tryb uśpienia po wyłączeniu zapłonu, minimalizując ryzyko rozładowania akumulatora.
*   **Stabilność:** Jest to obecnie najbardziej zalecany adapter do aplikacji mobilnych ze względu na stabilność połączenia BLE.

## 3. Kabel ENET/OBD2 - Instrukcja Użycia

Kabel ENET jest niezbędny do komunikacji z samochodami serii F, G i I.

### 3.1. Podłączenie

1.  Podłącz wtyczkę OBD2 do portu w samochodzie.
2.  Podłącz wtyczkę Ethernet (RJ45) do laptopa lub do adaptera Ethernet-USB/Lightning/USB-C.
3.  **Konfiguracja Sieci (Laptop):**
    *   Ustaw ręcznie adres IP karty sieciowej na **169.254.1.1** (Maska podsieci: 255.255.0.0).
    *   **Ważne:** Wyłącz Wi-Fi na czas połączenia, aby uniknąć konfliktów sieciowych.

### 3.2. Wskazówki

*   **Szybkość:** Kabel ENET jest najszybszym sposobem na flashowanie, co jest kluczowe przy dużych plikach (np. Initial Flash w Bootmod3).
*   **Adaptery:** Upewnij się, że używasz wysokiej jakości adaptera Ethernet, jeśli podłączasz kabel do urządzenia mobilnego. Tanie adaptery mogą powodować niestabilność.

---
*Zobacz także: [Rozwiązywanie Problemów](../Rozwiazywanie_Problemow/README.md) - Problemy z połączeniem adaptera.*
