Celem projektu było stworzenie kompletnego systemu zarządzania biblioteką z uwzględnieniem:

  - poprawnego modelowania danych,
  - implementacji logiki biznesowej po stronie bazy danych,
  - automatyzacji procesów (kary, dostępność egzemplarzy),
  - przygotowania zapytań analitycznych wspierających raportowanie.

Zaimplementowana logika biznesowa
**1. Funkcje**
Funkcja obliczająca średnią długość wypożyczenia.
Funkcja "oblicz_kare" naliczająca karę za przetrzymanie książki (po 30 dniach, 1% ceny książki za każdy dzień opóźnienia).

**2.Procedury składowane**
Statystyka wypożyczeń w wybranym okresie (z podziałem na biblioteki).
Dodawanie nowego czytelnika z walidacją unikalności adresu e-mail.
Sprawdzanie dostępności książki w bibliotekach.

**3.Widoki**
Ranking najczęściej wypożyczanych gatunków.
Pracownik z największą liczbą transakcji.
Najczęściej wypożyczana książka.

**4.Wyzwalacze (triggery)**
Automatyczna korekta minimalnej ceny książki (min. 10 PLN).
Automatyczne uzupełnianie daty zwrotu.
Dynamiczna aktualizacja statusu dostępności egzemplarza (Dostępny/Niedostępny).
