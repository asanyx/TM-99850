# Raport bezpieczeństwa – ApiDemos_Security_Check

**Status:** Wymaga przeglądu

---

## Flagi

- `debuggable=true` — tryb debugowania jest włączony. W wersji produkcyjnej pozwala atakującym na podłączenie się do procesu aplikacji i podgląd wrażliwych danych.

## Ryzykowne uprawnienia

| Uprawnienie | Ryzyko |
|---|---|
| `READ_CONTACTS` | Dostęp do listy kontaktów użytkownika |
| `INTERNET` | Możliwość wysyłania danych na zewnętrzne serwery |
| `WRITE_EXTERNAL_STORAGE` | Zapis plików na zewnętrznym nośniku |
| `RECORD_AUDIO` | Dostęp do mikrofonu — ryzyko podsłuchu |
| `CAMERA` | Dostęp do kamery — ryzyko nagrywania bez wiedzy użytkownika |

---

## Podsumowanie

Aplikacja ma włączony tryb debugowania (`debuggable=true`), co w wersji produkcyjnej pozwala atakującym na podłączenie się do procesu i podgląd danych. Posiada też zestaw wrażliwych uprawnień — dostęp do kontaktów, mikrofonu, kamery, internetu i zewnętrznego storage — co przy złośliwym użyciu umożliwia kradzież danych osobowych lub szpiegowanie użytkownika.

---

**Tester:** Piotr Dymianowicz

**Data:** 09.05.2026