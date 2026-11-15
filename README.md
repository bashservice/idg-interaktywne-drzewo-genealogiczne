Gotowy opis projektu w formacie Markdown, który możesz bezpośrednio wkleić do pliku `README.md` w swoim repozytorium na GitHubie.

---

# 🌳 IDG — Interaktywne Drzewo Genealogiczne

**IDG (Interaktywne Drzewo Genealogiczne)** to lekka, działająca w całości w przeglądarce aplikacja webowa (Single-File App) służąca do budowania, wizualizacji i zarządzania historią rodziny. Projekt został stworzony z myślą o maksymalnej prywatności i prostocie — wszystkie dane, zdjęcia oraz dokumenty zapisywane są lokalnie w przeglądarce użytkownika za pomocą **IndexedDB**, bez potrzeby konfigurowania zewnętrznych serwerów czy baz danych.

---

## ✨ Główne funkcjonalności

* **Interaktywna mapa (Pan & Zoom):** Swobodne przesuwanie obszaru roboczego, przybliżanie/oddalanie (również za pomocą gestów dotykowych *pinch-to-zoom* na urządzeniach mobilnych) oraz szybkie centrowanie widoku.
* **Zarządzanie strukturą drzewa:**
* Dodawanie protoplastów oraz bezpośrednich krewnych (ojciec, matka, partner/ka, dziecko).
* Przepinanie rodziców i modyfikowanie istniejących relacji.
* Przesuwanie pojedynczych kafelków lub całych gałęzi potomków jednocześnie.
* Blokowanie pozycji kafelków na mapie, aby uniknąć przypadkowych zmian układu.
* Zwijanie i rozwijanie wybranych odnóg drzewa oraz opcja ukrywania osób zmarłych.


* **Bogate profile członków rodziny:**
* Przechowywanie podstawowych danych (imię, nazwisko, nazwisko rodowe, płeć, daty urodzenia i śmierci, biogram).
* **Galeria zdjęć:** Dodawanie zdjęć przez adres URL lub wgrywanie z dysku (z automatyczną obsługą formatu WebP) oraz szybki podgląd po najechaniu kursorem na kafelek.
* **Archiwum dokumentów:** Możliwość załączania plików (np. akty urodzenia, zaświadczenia w formacie PDF, DOC, obrazy) bezpośrednio do profilu osoby (zapisywane w Base64).


* **Widok tabelaryczny i wyszukiwarka:** Przejrzysta lista wszystkich członków rodziny z możliwością sortowania i filtrowania po danych osobowych.
* **Powiadomienia i statystyki:**
* Podgląd statystyk drzewa na żywo (łączna liczba osób, podział na płeć).
* Kalendarz nadchodzących wydarzeń przypominający o urodzinach oraz rocznicach śmierci w najbliższych 30 dniach.


* **Struktura katalogów i kopie zapasowe:**
* Pełny **eksport i import** drzewa (wraz ze zdjęciami i dokumentami) do jednego pliku `.json`.
* Generator logicznej struktury folderów dla zdjęć i dokumentów z podziałem na pokolenia oraz możliwością pobrania manifestu JSON.



---

## 🛠️ Technologie

Aplikacja została napisana w czystym **Vanilla JavaScript**, **HTML5** oraz **CSS3** bez zewnętrznych frameworków i bibliotek:

* **IndexedDB API** — trwałe przechowywanie dużych ilości danych (zdjęć i plików PDF) po stronie klienta.
* **SVG** — dynamiczne rysowanie połączeń między węzłami drzewa oraz wektorowy zestaw ikon interfejsu.
* **Pointer Events API** — płynna obsługa myszy oraz ekranów dotykowych.
* **Responsive Web Design (RWD)** — interfejs dostosowany do ekranów komputerów, tabletów i smartfonów.

---

## 🚀 Jak uruchomić?

Projekt nie wymaga instalacji ani procesu budowania (*zero-build*):

1. Sklonuj repozytorium lub pobierz plik `index.html`:
```bash
git clone https://github.com/twoja-nazwa-uzytkownika/nazwa-repozytorium.git

```


2. Otwórz plik `index.html` bezpośrednio w dowolnej nowoczesnej przeglądarce internetowej (Chrome, Firefox, Edge, Safari).

*(Opcjonalnie)* Możesz udostępnić aplikację za pomocą **GitHub Pages** w ustawieniach repozytorium (`Settings -> Pages`), ponieważ cały kod znajduje się w jednym pliku.

---

## 💾 Prywatność i bezpieczeństwo danych

Aplikacja działa w 100% lokalnie (**Offline-First**). Żadne wprowadzone dane osobowe, zdjęcia ani dokumenty nie są wysyłane na zewnętrzne serwery. Aby nie utracić danych przy czyszczeniu pamięci przeglądarki, zaleca się regularne korzystanie z funkcji **Eksportuj (JSON)** w celu utworzenia lokalnej kopii zapasowej.

---

## 📄 Licencja

Ten projekt jest udostępniany na licencji MIT — możesz go dowolnie modyfikować i wykorzystywać do własnych celów.
