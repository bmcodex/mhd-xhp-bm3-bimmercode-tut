# Rozwiązywanie Problemów (Troubleshooting)

Poniżej przedstawiono najczęściej spotykane problemy podczas używania MHD, Bootmod3, xHP i BimmerCode oraz sposoby ich rozwiązania.

## 1. Problemy z Połączeniem (Adapter OBDLink CX+ / ENET)

| Problem | Możliwa Przyczyna | Rozwiązanie |
| :--- | :--- | :--- |
| **Brak połączenia z OBDLink CX+** | Adapter nie jest wybrany w aplikacji lub nie jest w trybie BLE. | Upewnij się, że w ustawieniach aplikacji (MHD, xHP, BimmerCode) wybrano **OBDLink CX+**. Nie paruj go ręcznie w ustawieniach Bluetooth telefonu. |
| **Brak połączenia z kablem ENET** | Nieprawidłowa konfiguracja IP na laptopie. | Ustaw ręcznie adres IP na **169.254.1.1** (Maska podsieci: 255.255.0.0). Wyłącz Wi-Fi. |
| **Połączenie zrywa się** | Słaba jakość adaptera ENET lub problem z portem USB/adapterem OTG. | Użyj kabla ENET wyższej jakości. Sprawdź, czy adapter OTG/USB-C działa poprawnie. Upewnij się, że telefon nie przechodzi w tryb uśpienia. |

## 2. Problemy z Flashowaniem (MHD, Bootmod3, xHP)

| Problem | Możliwa Przyczyna | Rozwiązanie |
| :--- | :--- | :--- |
| **Flashowanie nie rozpoczyna się / błąd na początku** | Niskie napięcie akumulatora. | **Podłącz prostownik!** Upewnij się, że napięcie jest stabilne (min. 12.5V, zalecane 13.5V+). |
| **Flashowanie przerwane (błąd komunikacji)** | Utrata połączenia OBD lub spadek napięcia. | Użyj stabilniejszego adaptera (np. OBDLink CX+ lub ENET). Powtórz flashowanie z podłączonym prostownikiem. |
| **"Choinka" na desce rozdzielczej po flashu** | Normalny objaw. Moduły są resetowane. | Wyłącz i włącz zapłon. Odczekaj 5 minut. Jeśli błędy nie znikną, użyj aplikacji do skasowania kodów DTC. |
| **Błąd Check Engine (CEL) po flashu** | Błąd katalizatora (P0420/P0430) lub błąd czujnika tlenu. | Jeśli masz usunięty katalizator (downpipe), upewnij się, że w opcjach mapy (MHD/BM3) wybrano opcję **Catless Downpipe** (wyłączenie kontroli). Skasuj błąd. |

## 3. Problemy z Kodowaniem (BimmerCode)

| Problem | Możliwa Przyczyna | Rozwiązanie |
| :--- | :--- | :--- |
| **BimmerCode nie widzi modułu** | Moduł jest niekompatybilny lub adapter nie ma dostępu do magistrali. | Sprawdź listę kompatybilności BimmerCode dla swojego modelu. Upewnij się, że adapter jest poprawnie podłączony i wybrany. |
| **Błąd kodowania (Coding Failed)** | Niestabilne połączenie lub próba kodowania zbyt wielu funkcji naraz. | Upewnij się, że adapter jest stabilny. Spróbuj zakodować funkcje pojedynczo. Użyj funkcji **Restore** (Przywróć) z kopii zapasowej. |
| **Funkcja zakodowana, ale nie działa** | Wymagany reset modułu lub nieprawidłowa konfiguracja. | Wyłącz i włącz zapłon. W niektórych przypadkach (np. zmiana regionu) wymagany jest reset iDrive (przytrzymanie przycisku głośności przez 30 sekund). |

## 4. Wskazówki Ogólne

*   **Zawsze miej kopię zapasową:** Przed każdym flashowaniem lub kodowaniem upewnij się, że aplikacja wykonała kopię zapasową oryginalnego oprogramowania/ustawień.
*   **Tryb Samolotowy:** Podczas flashowania/kodowania na urządzeniu mobilnym włącz **Tryb Samolotowy** (z włączonym Bluetooth), aby uniknąć przerwanych połączeń spowodowanych przychodzącymi połączeniami lub powiadomieniami.
*   **Chłodzenie:** Upewnij się, że ECU nie jest przegrzane (np. po długiej, agresywnej jeździe). Najlepiej flashować na zimnym lub lekko rozgrzanym silniku.

---
*Zobacz także: [MHD](../MHD/README.md), [Bootmod3](../Bootmod3/README.md), [xHP](../xHP/README.md), [BimmerCode](../BimmerCode/README.md)*
