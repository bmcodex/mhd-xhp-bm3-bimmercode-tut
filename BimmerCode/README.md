# BimmerCode - Kompletny Przewodnik

## 1. Wprowadzenie do BimmerCode

**BimmerCode** to aplikacja umożliwiająca kodowanie modułów sterujących w samochodach BMW, Mini i Rolls-Royce. Pozwala na aktywację ukrytych funkcji, zmianę ustawień fabrycznych oraz personalizację samochodu bez konieczności posiadania zaawansowanej wiedzy programistycznej (w przeciwieństwie do E-Sys/ISTA).

## 2. Wymagania Wstępne i Sprzęt

| Wymaganie | Szczegóły |
| :--- | :--- |
| **Adapter OBD** | **OBDLink CX+** (zalecany, bardzo stabilny i szybki) lub kabel **ENET/OBD2** (wymaga adaptera Ethernet do USB/Lightning). |
| **Urządzenie** | Smartfon lub tablet z systemem Android lub iOS. |
| **Licencja** | Zakupiona pełna wersja aplikacji BimmerCode. |
| **Akumulator** | Zalecane jest, aby akumulator był naładowany. Kodowanie jest szybkie, ale stabilne napięcie jest zawsze kluczowe. |

## 3. Proces Kodowania

Proces kodowania w BimmerCode jest intuicyjny i opiera się na prostym interfejsie użytkownika.

1.  **Podłącz adapter:** Wepnij adapter OBD (np. OBDLink CX+) do portu OBD.
2.  **Włącz zapłon:** Wciśnij przycisk START bez wciskania pedału hamulca/sprzęgła.
3.  **Połącz z aplikacją:** Uruchom BimmerCode, wybierz adapter i nawiąż połączenie.
4.  **Wybierz moduł:** Aplikacja automatycznie odczyta wszystkie dostępne moduły (np. FEM_BODY, HU_NBT, KOMBI). Wybierz moduł, który chcesz kodować.
5.  **Wybierz funkcję:** Wybierz funkcję, którą chcesz zmienić (np. "Wyłącz Start/Stop", "Cyfrowy prędkościomierz").
6.  **Kodowanie:** Po wybraniu opcji, naciśnij przycisk **"Koduj"**. Aplikacja wykona kopię zapasową oryginalnych ustawień, a następnie wgra nowe.
7.  **Zakończenie:** Po zakończeniu kodowania, moduł zostanie zresetowany, a na desce rozdzielczej mogą pojawić się tymczasowe błędy, które znikną po chwili.

## 4. Popularne Modyfikacje (Przykłady)

| Moduł | Funkcja | Opis |
| :--- | :--- | :--- |
| **FEM_BODY** | Automatyczne składanie lusterek | Zmiana czasu reakcji na przytrzymanie przycisku zamykania. |
| **HU_NBT/HU_EVO** | Video in Motion (VIM) | Oglądanie filmów/TV podczas jazdy. |
| **KOMBI** | Cyfrowy prędkościomierz | Wyświetlanie prędkości cyfrowo w dolnej części zegarów. |
| **ACSM** | Wyłączenie ostrzeżenia o pasach | Wyłączenie dźwiękowego i wizualnego ostrzeżenia o niezapiętych pasach. |
| **FEM_BODY** | Wyłączenie Start/Stop | Zapamiętanie ostatniego stanu systemu Start/Stop lub całkowite wyłączenie. |
| **Licht** | Zmiana świateł powitalnych | Aktywacja dodatkowych świateł (np. halogenów) w sekwencji powitalnej. |

## 5. Wskazówki i Najlepsze Praktyki

*   **Kopia Zapasowa:** BimmerCode automatycznie tworzy kopię zapasową przed każdym kodowaniem. Zawsze upewnij się, że masz dostęp do tych kopii.
*   **Tryb Eksperta:** Aplikacja oferuje **Tryb Eksperta**, który pozwala na bezpośrednią zmianę parametrów (FDL-Coding). Używaj go tylko, jeśli wiesz, co robisz, ponieważ nieprawidłowe zmiany mogą spowodować błędy.
*   **Stabilne Połączenie:** Chociaż kodowanie jest szybkie, stabilne połączenie jest kluczowe. OBDLink CX+ jest tu bardzo dobrym wyborem ze względu na niezawodność Bluetooth.
*   **Reset Modułu:** Jeśli po kodowaniu funkcja nie działa, spróbuj zresetować moduł w aplikacji lub wyłączyć i włączyć zapłon.

---
*Zobacz także: [Sprzęt](../Sprzet/README.md) - Porównanie adapterów OBDLink CX+ i ENET.*
*Zobacz także: [Rozwiązywanie Problemów](../Rozwiazywanie_Problemow/README.md) - Błędy kodowania i komunikacji.*
