# Bootmod3 (BM3) - Kompletny Przewodnik

## 1. Wprowadzenie do Bootmod3

**Bootmod3 (BM3)** to zaawansowana platforma do tuningu silników BMW, oferująca szeroki zakres gotowych map (OTS - Off The Shelf) oraz możliwość tworzenia niestandardowych map (Custom Tune). W przeciwieństwie do MHD, BM3 jest platformą opartą na chmurze, która wymaga stałego połączenia z Internetem do zarządzania mapami i licencjami.

## 2. Wymagania Sprzętowe i Licencje

| Element | Wymaganie | Uwagi |
| :--- | :--- | :--- |
| **Adapter OBD** | **ENET/OBD2** (dla F/G Series) lub **K-DCAN** (dla E Series). **OBDLink CX+** jest kompatybilny, ale kabel ENET jest często preferowany ze względu na szybkość i stabilność połączenia. | Wymagany jest adapter Wi-Fi lub kabel ENET podłączony do laptopa/tabletu. |
| **Urządzenie** | Laptop (Windows/macOS) lub urządzenie mobilne (iOS/Android) z dostępem do Internetu. | Laptop jest zalecany do pierwszego flashowania (tzw. **Initial Flash**). |
| **Licencje** | **BM3 License** (do aktywacji platformy) oraz ewentualnie **Map Pack** lub **Custom Tune**. | Licencja jest przypisana do numeru VIN samochodu. |
| **Zasilanie** | **Kluczowe!** Podobnie jak w MHD, wymagany jest stabilny prostownik (13.5V+) podczas flashowania, zwłaszcza przy Initial Flash, który może trwać do 30-40 minut. | |

## 3. Proces Flashowania

### 3.1. Initial Flash (Pierwsze Flashowanie)

Pierwsze wgranie BM3 jest najdłuższe, ponieważ platforma musi wgrać swój własny bootloader do ECU.

1.  **Podłącz zasilanie:** Upewnij się, że prostownik jest podłączony i dostarcza stabilne napięcie.
2.  **Podłącz adapter:** Podłącz kabel ENET do portu OBD i do laptopa/tabletu.
3.  **Włącz zapłon:** Wciśnij przycisk START bez wciskania pedału hamulca/sprzęgła.
4.  **Uruchom aplikację/portal:** Zaloguj się do portalu BM3 na laptopie lub w aplikacji mobilnej.
5.  **Wybierz mapę:** Wybierz mapę OTS (np. Stage 1 98RON) i opcje dodatkowe (np. Cold Start Delete, GTS Roar).
6.  **Rozpocznij flash:** Rozpocznij proces. **NIE PRZERYWAJ!**

### 3.2. Map Change (Zmiana Mapy)

Po Initial Flash, zmiana mapy jest znacznie szybsza (zwykle 1-3 minuty), ponieważ bootloader BM3 jest już wgrany.

1.  Wybierz nową mapę lub zmodyfikuj opcje.
2.  Rozpocznij flash.

## 4. Funkcje Specjalne BM3

| Funkcja | Opis |
| :--- | :--- |
| **Custom Tune** | Możliwość współpracy z tunerem w celu stworzenia mapy idealnie dopasowanej do modyfikacji sprzętowych (np. hybrydowe turbo). |
| **Live Adjustments** | Zmiana niektórych parametrów (np. głośność strzałów, ciśnienie doładowania) w czasie rzeczywistym, bez konieczności ponownego flashowania. |
| **Datalogging** | Zaawansowane logowanie parametrów pracy silnika, dostępne bezpośrednio w aplikacji i na portalu. |
| **GTS/CS Features** | Wgrywanie fabrycznych funkcji z modeli M (np. GTS DCT/Diff Flash, GTS Roar). |
| **Code Reading/Clearing** | Odczyt i kasowanie kodów błędów DTC. |

## 5. Wskazówki i Najlepsze Praktyki

*   **Korzystaj z portalu:** Portal internetowy BM3 oferuje więcej opcji i jest bardziej stabilny niż aplikacja mobilna.
*   **Sprawdź stan połączenia:** Upewnij się, że masz stabilne połączenie z Internetem, ponieważ BM3 pobiera mapy z chmury.
*   **Zawsze loguj:** Po wgraniu nowej mapy, wykonaj logi, aby upewnić się, że silnik pracuje w bezpiecznych parametrach.
*   **Wybór adaptera:** Jeśli używasz kabla ENET, upewnij się, że masz odpowiedni adapter do swojego urządzenia (np. USB-C do Ethernet).

---
*Zobacz także: [Sprzęt](../Sprzet/README.md) - Porównanie adapterów OBDLink CX+ i ENET.*
