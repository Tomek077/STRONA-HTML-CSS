**Ćwiczenie: Przypomnienie podstaw HTML i zewnętrznego stylu CSS**

---

### **Część I: Tutorial krok po kroku**

W tym ćwiczeniu odświeżymy podstawy tworzenia strony internetowej za pomocą HTML i CSS. Wykonaj poniższe kroki, pamiętając o wykonywaniu commitów z opisami po każdym etapie.

---

#### **Krok 1: Inicjalizacja projektu**

1. **Utwórz nowy folder projektu.**
2. **W folderze projektu utwórz plik `index.html`.**
3. **Dodaj do `index.html` podstawową strukturę HTML:**

   ```html
   <!DOCTYPE html>
   <html lang="pl">
   <head>
       <meta charset="UTF-8">
       <title>Moja Strona</title>
       <link rel="stylesheet" href="style.css">
   </head>
   <body>

   </body>
   </html>
   ```

4. **Utwórz plik `style.css` w tym samym folderze.**

**Commit:** "Inicjalizacja projektu - dodanie index.html i style.css z podstawową strukturą"

---

#### **Krok 2: Podział strony na 4 bloki**

1. **W pliku `index.html`, w sekcji `<body>`, dodaj cztery elementy `<div>` z klasami:**

   ```html
   <div class="blok1">Blok 1</div>
   <div class="blok2">Blok 2</div>
   <div class="blok3">Blok 3</div>
   <div class="blok4">Blok 4</div>
   ```

2. **W pliku `style.css` dodaj podstawowe style dla tych bloków:**

   ```css
   .blok1, .blok2, .blok3, .blok4 {
       width: 200px;
       height: 100px;
       margin: 10px;
       display: inline-block;
   }
   ```

**Commit:** "Dodanie 4 bloków na stronie"

---

#### **Krok 3: Ustawienie szerokości, wysokości, kolorów, marginesów**

1. **Dodaj indywidualne style dla każdego bloku w `style.css`:**

   ```css
   .blok1 {
       background-color: red;
   }

   .blok2 {
       background-color: blue;
   }

   .blok3 {
       background-color: green;
   }

   .blok4 {
       background-color: yellow;
   }
   ```

**Commit:** "Ustawienie stylów dla bloków - kolory i rozmiary"

---

#### **Krok 4: Ustawienie koloru czcionki i wielkości**

1. **Dodaj style dla tekstu wewnątrz bloków w `style.css`:**

   ```css
   .blok1, .blok2, .blok3, .blok4 {
       color: white;
       font-size: 16px;
       text-align: center;
       line-height: 100px; /* Centrowanie tekstu w pionie */
   }
   ```

**Commit:** "Ustawienie stylów dla tekstu - kolor i rozmiar czcionki"

---

#### **Krok 5: Dodanie linku do podstrony**

1. **Utwórz nowy plik `podstrona.html` z podstawową strukturą HTML:**

   ```html
   <!DOCTYPE html>
   <html lang="pl">
   <head>
       <meta charset="UTF-8">
       <title>Podstrona</title>
   </head>
   <body>
       <h1>To jest podstrona</h1>
   </body>
   </html>
   ```

2. **Dodaj link do podstrony w `index.html`:**

   ```html
   <a href="podstrona.html">Przejdź do podstrony</a>
   ```

**Commit:** "Dodanie linku do podstrony"

---

#### **Krok 6: Dodanie linku do strony zewnętrznej**

1. **Dodaj link do strony zewnętrznej w `index.html`:**

   ```html
   <a href="https://www.google.com" target="_blank">Przejdź do Google</a>
   ```

**Commit:** "Dodanie linku do strony zewnętrznej"

---

#### **Krok 7: Dodanie dwóch zdjęć z opisami**

1. **Utwórz folder `images` i umieść w nim dwa zdjęcia, np. `obraz1.jpg` i `obraz2.jpg`.**
2. **Dodaj obrazy z opisami w `index.html`:**

   ```html
   <img src="images/obraz1.jpg" alt="Opis pierwszego zdjęcia">
   <img src="images/obraz2.jpg" alt="Opis drugiego zdjęcia">
   ```

3. **Dodaj stylizację w `style.css` (opcjonalnie):**

   ```css
   img {
       width: 200px;
       height: auto;
       margin: 10px;
   }
   ```

**Commit:** "Dodanie zdjęć z opisami"

---

#### **Krok 8: Dodanie tabeli**

1. **Dodaj tabelę w `index.html`:**

   ```html
   <table border="1">
       <tr>
           <th>Imię</th>
           <th>Nazwisko</th>
           <th>Wiek</th>
       </tr>
       <tr>
           <td>Jan</td>
           <td>Kowalski</td>
           <td>30</td>
       </tr>
       <tr>
           <td>Anna</td>
           <td>Nowak</td>
           <td>25</td>
       </tr>
   </table>
   ```

2. **Dodaj style do tabeli w `style.css`:**

   ```css
   table {
       width: 50%;
       border-collapse: collapse;
       margin: 20px 0;
   }

   th, td {
       padding: 8px 12px;
       text-align: left;
   }
   ```

**Commit:** "Dodanie tabeli z danymi"

---

#### **Krok 9: Dodanie linku do pobrania pliku tekstowego**

1. **Umieść plik `dokument.txt` w folderze projektu.**
2. **Dodaj link do pobrania pliku w `index.html`:**

   ```html
   <a href="dokument.txt" download>Pobierz plik tekstowy</a>
   ```

**Commit:** "Dodanie linku do pobrania pliku tekstowego"

---

### **Podsumowanie**

Gratulacje! Ukończyłeś tutorial przypominający podstawy HTML i CSS. Wszystkie zmiany zapisz w swoim repozytorium na GitHub.

---

**Ćwiczenie: Przypomnienie podstaw HTML i zewnętrznego stylu CSS**

---

### **Część II: Ćwiczenia do samodzielnej realizacji (z konkretnymi parametrami)**

Twoim zadaniem jest stworzenie strony internetowej zgodnie z poniższymi, szczegółowymi wytycznymi. Ćwiczenie to ma na celu utrwalenie umiejętności potrzebnych do egzaminu kwalifikacyjnego INF.03. Pamiętaj o wykonywaniu commitów z opisami po każdym etapie i zapisywaniu zmian w swoim repozytorium na GitHub.

---

#### **Zadanie 1: Struktura strony**

- **Utwórz plik `index.html` z podstawową strukturą HTML.**

- **Podziel stronę na 5 bloków za pomocą elementów `<div>` lub semantycznych znaczników HTML5, z następującymi identyfikatorami i stylami:**

  1. **Nagłówek (`header`):**
     - Szerokość: 100%
     - Wysokość: 120 pikseli
     - Kolor tła: niebieski (#1E90FF)

  2. **Menu nawigacyjne (`nav`):**
     - Szerokość: 100%
     - Wysokość: 40 pikseli
     - Kolor tła: stalowy niebieski (#4682B4)

  3. **Główna zawartość (`main`):**
     - Szerokość: 70%
     - Minimalna wysokość: 400 pikseli
     - Kolor tła: alabastrowy (#F0F8FF)
     - Umieszczony po lewej stronie

  4. **Panel boczny (`aside`):**
     - Szerokość: 30%
     - Minimalna wysokość: 400 pikseli
     - Kolor tła: jasny stalowy niebieski (#B0C4DE)
     - Umieszczony po prawej stronie

  5. **Stopka (`footer`):**
     - Szerokość: 100%
     - Wysokość: 60 pikseli
     - Kolor tła: niebieski (#1E90FF)

**Commit:** "Dodanie struktury strony z 5 blokami o określonych parametrach"

---

#### **Zadanie 2: Stylizacja bloków**

- **Ustaw style dla każdego bloku w zewnętrznym pliku CSS `style.css`, zgodnie z następującymi wytycznymi:**

  - **Nagłówek (`header`):**
    - Wyśrodkowany tekst w pionie i poziomie
    - Kolor tekstu: biały
    - Rozmiar czcionki: 32 piksele
    - Czcionka: Arial, sans-serif

  - **Menu nawigacyjne (`nav`):**
    - Lista pozioma z linkami
    - Linki bez podkreślenia
    - Kolor tekstu linków: biały
    - Przy najechaniu kursorem na link, zmienia się kolor tekstu na jasny niebieski (#ADD8E6)

  - **Główna zawartość (`main`):**
    - Wewnętrzny odstęp (padding): 20 pikseli
    - Tekst wyrównany do lewej
    - Kolor tekstu: granatowy (#000080)
    - Rozmiar czcionki: 18 pikseli

  - **Panel boczny (`aside`):**
    - Wewnętrzny odstęp (padding): 20 pikseli
    - Kolor tekstu: granatowy (#000080)
    - Rozmiar czcionki: 16 pikseli

  - **Stopka (`footer`):**
    - Wyśrodkowany tekst w pionie i poziomie
    - Kolor tekstu: biały
    - Rozmiar czcionki: 14 pikseli

**Commit:** "Ustawienie stylów dla każdego bloku zgodnie z wytycznymi"

---

#### **Zadanie 3: Treść strony**

- **W bloku głównej zawartości (`main`) dodaj artykuł składający się z:**

  - **Tytułu (np. "Witamy na naszej stronie")**
    - Kolor tekstu: midnight blue (#191970)
    - Rozmiar czcionki: 28 pikseli

  - **Paragrafu z tekstem (możesz użyć tekstu zastępczego)**
    - Interlinia: 1.6
    - Tekst wyjustowany

- **W panelu bocznym (`aside`) dodaj sekcję z nagłówkiem (np. "Nawigacja") i listą linków do różnych sekcji strony (mogą to być linki do fragmentów na tej samej stronie).**
  - Kolor tekstu nagłówka: midnight blue (#191970)
  - Rozmiar czcionki nagłówka: 22 piksele

**Commit:** "Dodanie treści do bloków main i aside zgodnie z wytycznymi"

---

#### **Zadanie 4: Menu i podstrony**

- **W menu nawigacyjnym (`nav`) dodaj linki do następujących stron:**
  - **"Strona Główna" (link do `index.html`)**
  - **"Galeria" (link do `galeria.html`)**
  - **"Kontakt" (link do `kontakt.html`)**

- **Utwórz plik `galeria.html` z tą samą strukturą co `index.html`. W bloku głównej zawartości umieść nagłówek "Galeria".**

- **W panelu bocznym (`aside`) dodaj link do strony zewnętrznej (np. "Ministerstwo Edukacji" z linkiem `https://www.gov.pl/web/edukacja`), który otwiera się w nowej karcie.**

**Commit:** "Dodanie menu z linkami do podstron i strony zewnętrznej"

---

#### **Zadanie 5: Galeria obrazów**

- **W pliku `galeria.html` w bloku głównej zawartości (`main`) dodaj trzy obrazy:**

  - **Obrazy o szerokości 250 pikseli, zachowujące proporcje wysokości**
  - **Obrazy umieszczone obok siebie w jednym rzędzie**
  - **Dodaj do obrazów atrybuty `alt` z opisem każdego obrazu**
  - **Ustaw, aby po najechaniu kursorem na obraz, wyświetlał się efekt przyciemnienia oraz opis (za pomocą CSS i pseudo-klasy `:hover`)**

**Commit:** "Dodanie galerii obrazów z efektami hover"

---

#### **Zadanie 6: Tabela**

- **W pliku `index.html` w bloku głównej zawartości (`main`) dodaj tabelę przedstawiającą plan lekcji:**

  - **Tabela powinna zawierać:**
    - **5 kolumn dla dni tygodnia (poniedziałek - piątek)**
    - **8 wierszy dla godzin lekcyjnych (1 - 8)**
  - **Wypełnij tabelę przykładowymi przedmiotami**

- **Stylizacja tabeli:**

  - **Szerokość tabeli: 100%**
  - **Obramowanie tabeli oraz komórek: 1 piksel, solid, kolor szary (#ccc)**
  - **Nagłówki tabeli (`th`) powinny mieć:**
    - **Kolor tła: stalowy niebieski (#4682B4)**
    - **Kolor tekstu: biały**
    - **Wewnętrzny odstęp (padding): 8 pikseli**
  - **Komórki tabeli (`td`):**
    - **Wewnętrzny odstęp (padding): 8 pikseli**
    - **Tekst wyśrodkowany**
  - **Naprzemienne kolory wierszy (co drugi wiersz ma inny kolor tła, np. jasnoszary)**

**Commit:** "Dodanie tabeli z planem lekcji i jej stylizacja"

---

#### **Zadanie 7: Link do pobrania pliku**

- **W stopce (`footer`) dodaj link do pobrania pliku PDF (np. `regulamin.pdf`):**

  - **Tekst linku: "Pobierz regulamin strony"**
  - **Link powinien pobierać plik po kliknięciu (użyj atrybutu `download`)**

- **Stylizacja linku:**

  - **Kolor tekstu linku: biały**
  - **Brak podkreślenia**
  - **Przy najechaniu kursorem na link, tekst jest podkreślony**

**Commit:** "Dodanie linku do pobrania pliku PDF w stopce"

---

### **Przypomnienie**

- **Po każdym etapie pamiętaj o wykonaniu commita z odpowiednim opisem.**
- **Zapisz wszystkie zmiany w swoim repozytorium na GitHub.**

---

**Powodzenia w realizacji zadania!**
