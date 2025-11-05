# xHP Flashtool - Kompletny Przewodnik

## 1. Wprowadzenie do xHP Flashtool

**xHP Flashtool** to wiodąca platforma do modyfikacji oprogramowania sterownika skrzyni biegów (TCU - Transmission Control Unit) w samochodach BMW wyposażonych w automatyczne skrzynie biegów ZF (np. 6HP i 8HP). Modyfikacje te mają na celu poprawę szybkości i agresywności zmiany biegów, zwiększenie momentu obrotowego oraz optymalizację działania w trybach D, S i M.

## 2. Wymagania Wstępne

| Wymaganie | Szczegóły |
| :--- | :--- |
| **Adapter OBD** | **OBDLink CX+** (zalecany ze względu na stabilność Bluetooth) lub kabel **ENET/OBD2** (dla F/G Series). |
| **Urządzenie** | Smartfon lub tablet z systemem Android lub iOS. |
| **Akumulator** | **Kluczowe!** Wymagany jest stabilny prostownik (13.5V+) podłączony do samochodu. Flashowanie TCU jest bardzo wrażliwe na spadki napięcia i może trwać do 10-15 minut. |
| **Licencje** | Zakupiona licencja xHP (Flashtool License) oraz wybrany pakiet map (Stage 1, 2 lub 3). |

## 3. Dostępne Mapy (Stages)

xHP oferuje zazwyczaj trzy główne mapy, z których każda zapewnia inny poziom agresywności i funkcjonalności:

| Mapa | Opis | Główne Zmiany |
| :--- | :--- | :--- |
| **Stage 1** | Optymalizacja fabrycznej mapy. Szybsze i płynniejsze zmiany biegów, lepsza reakcja na gaz. Idealna dla seryjnych samochodów. | Zoptymalizowane punkty zmiany biegów, szybsze zmiany. |
| **Stage 2** | Znacznie szybsze zmiany biegów, podniesione limity momentu obrotowego. Bardziej sportowe odczucia w trybach S i M. | Zwiększone ciśnienie w skrzyni, szybsze zmiany, twardsze redukcje. |
| **Stage 3** | Najbardziej agresywna mapa. Błyskawiczne zmiany biegów (tzw. "DCT-like"), zoptymalizowane pod kątem jazdy torowej i mocno zmodyfikowanych silników. | Najszybsze zmiany, maksymalne ciśnienie, pełna kontrola momentu obrotowego. |

## 4. Proces Flashowania

1.  **Podłącz zasilanie:** Podłącz prostownik i upewnij się, że napięcie jest stabilne.
2.  **Podłącz adapter:** Wepnij adapter OBD i nawiąż połączenie z aplikacją xHP.
3.  **Wybierz mapę:** Wybierz Stage (np. Stage 3) i ewentualnie dostosuj opcje (np. tryb startu, wskaźnik biegu na desce).
4.  **Rozpocznij flash:** Rozpocznij proces. Aplikacja przeprowadzi Cię przez kroki (np. włączenie/wyłączenie zapłonu).
5.  **NIE PRZERYWAJ!** Podczas flashowania na desce rozdzielczej mogą pojawić się błędy i choinki. To normalne.

## 5. Wskazówki i Najlepsze Praktyki

*   **Zawsze używaj prostownika!** To najważniejsza zasada przy flashowaniu TCU.
*   **Adaptacja:** Po wgraniu nowej mapy, skrzynia biegów potrzebuje czasu na adaptację. Przez pierwsze kilkadziesiąt kilometrów jazdy (zarówno spokojnej, jak i dynamicznej) skrzynia będzie uczyć się nowych parametrów.
*   **Reset Adaptacji:** W aplikacji xHP istnieje opcja resetu adaptacji. Jest to zalecane po wgraniu nowej mapy, aby skrzynia mogła zacząć "uczyć się" od zera.
*   **Wskaźnik Biegu:** xHP umożliwia aktywację wskaźnika biegu na desce rozdzielczej w trybie D (w wielu modelach jest to domyślnie wyłączone).

---
*Zobacz także: [Rozwiązywanie Problemów](../Rozwiazywanie_Problemow/README.md) - Błędy komunikacji i spadki napięcia.*
