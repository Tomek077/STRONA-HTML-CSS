**Ćwiczenie: Tworzenie strony internetowej salonu kosmetycznego**

---

### **Część I: Tutorial krok po kroku**

W tym ćwiczeniu stworzymy kompletną stronę internetową dla salonu kosmetycznego. Wykonaj poniższe kroki, pamiętając o wykonywaniu commitów z opisami po każdym etapie.

---

#### **Krok 1: Inicjalizacja projektu**

1. **Utwórz nowy folder projektu o nazwie `SalonKosmetyczny`.**

2. **W folderze projektu utwórz plik `index.html`.**

3. **Dodaj do `index.html` podstawową strukturę HTML:**

   ```html
   <!DOCTYPE html>
   <html lang="pl">
   <head>
       <meta charset="UTF-8">
       <title>Salon Kosmetyczny BeautySpa</title>
       <link rel="stylesheet" href="style.css">
   </head>
   <body>

   </body>
   </html>
   ```

   **Wyjaśnienie kodu:**

   - `<!DOCTYPE html>` – deklaruje, że dokument jest w formacie HTML5.
   - `<html lang="pl">` – otwiera element HTML i ustawia język dokumentu na polski.
   - `<head>` – sekcja nagłówkowa zawierająca metadane dokumentu.
     - `<meta charset="UTF-8">` – ustawia kodowanie znaków na UTF-8.
     - `<title>Salon Kosmetyczny BeautySpa</title>` – tytuł strony wyświetlany na karcie przeglądarki.
     - `<link rel="stylesheet" href="style.css">` – łączy zewnętrzny arkusz stylów `style.css`.
   - `<body>` – główna sekcja dokumentu, w której będzie zawarta treść strony.
   - `</body>` – zamyka sekcję `<body>`.
   - `</html>` – zamyka element `<html>`.

4. **Utwórz plik `style.css` w tym samym folderze.**

**Commit:** "Inicjalizacja projektu - dodanie plików index.html i style.css z podstawową strukturą"

---

#### **Krok 2: Podział strony na 4 bloki**

1. **W pliku `index.html`, w sekcji `<body>`, dodaj cztery elementy `<div>` z identyfikatorami:**

   ```html
   <div id="header"> <!-- Nagłówek strony -->
       <h1>BeautySpa - Twoje miejsce relaksu</h1>
   </div>

   <div id="menu"> <!-- Menu nawigacyjne -->
       <ul>
           <li><a href="index.html">Strona główna</a></li>
           <li><a href="oferta.html">Oferta</a></li>
           <li><a href="kontakt.html">Kontakt</a></li>
           <li><a href="https://www.facebook.com/BeautySpa" target="_blank">Facebook</a></li>
       </ul>
   </div>

   <div id="content"> <!-- Główna treść strony -->
       <!-- Treść zostanie dodana w kolejnym kroku -->
   </div>

   <div id="footer"> <!-- Stopka strony -->
       <p>&copy; 2023 BeautySpa - Salon Kosmetyczny</p>
   </div>
   ```

   **Wyjaśnienie kodu:**

   - `<div id="header">` – nagłówek strony z identyfikatorem `header`.
     - `<h1>BeautySpa - Twoje miejsce relaksu</h1>` – nagłówek pierwszego poziomu z nazwą salonu i sloganem.
   - `<div id="menu">` – menu nawigacyjne z identyfikatorem `menu`.
     - Lista linków do różnych podstron oraz do strony zewnętrznej (Facebook).
   - `<div id="content">` – sekcja głównej treści strony.
   - `<div id="footer">` – stopka strony z identyfikatorem `footer`.

2. **Utwórz styl w `style.css` dla podstawowego układu strony:**

   ```css
   body {
       margin: 0;
       font-family: Arial, sans-serif;
       background-color: #f9f9f9;
   }

   #header, #menu, #content, #footer {
       width: 100%;
   }

   #header {
       background-color: #e0acd5;
       color: #fff;
       padding: 40px 20px;
       text-align: center;
   }

   #menu {
       background-color: #333;
   }

   #menu ul {
       list-style-type: none;
       margin: 0;
       padding: 0;
       overflow: hidden;
   }

   #menu li {
       float: left;
   }

   #menu li a {
       display: block;
       color: white;
       text-align: center;
       padding: 14px 20px;
       text-decoration: none;
   }

   #menu li a:hover {
       background-color: #111;
   }

   #content {
       padding: 20px;
   }

   #footer {
       background-color: #e0acd5;
       color: #fff;
       text-align: center;
       padding: 20px;
   }
   ```

   **Wyjaśnienie kodu:**

   - `body` – ustawia marginesy na 0, rodzinę fontów na Arial i tło strony na jasnoszare.
   - `#header` – ustawia tło nagłówka na kolor różowy (#e0acd5), kolor tekstu na biały, wewnętrzne odstępy i wyśrodkowanie tekstu.
   - `#menu` i jego elementy – tworzy poziome menu nawigacyjne z ciemnoszarym tłem i białym tekstem.
   - `#content` – wewnętrzne odstępy dla treści.
   - `#footer` – styl stopki z tym samym tłem co nagłówek.

**Commit:** "Dodanie 4 bloków strony z podstawowym stylem dla salonu kosmetycznego"

---

#### **Krok 3: Dodanie treści do sekcji "content"**

1. **W sekcji `<div id="content">`, dodaj treści związane z salonem kosmetycznym:**

   ```html
   <h2>O nas</h2>
   <p>BeautySpa to wyjątkowe miejsce, gdzie możesz zrelaksować się i zadbać o swoje piękno. Oferujemy szeroką gamę zabiegów kosmetycznych i relaksacyjnych.</p>

   <h2>Nasze usługi</h2>
   <ul>
       <li>Masaż relaksacyjny</li>
       <li>Zabiegi na twarz</li>
       <li>Manicure i pedicure</li>
       <li>Depilacja laserowa</li>
   </ul>

   <h2>Godziny otwarcia</h2>
   <p>Poniedziałek - Piątek: 9:00 - 19:00<br>
      Sobota: 10:00 - 16:00<br>
      Niedziela: Nieczynne</p>
   ```

   **Wyjaśnienie kodu:**

   - **Sekcja "O nas":**
     - `<h2>` – nagłówek drugiego poziomu.
     - `<p>` – paragraf z opisem salonu.
   - **Sekcja "Nasze usługi":**
     - `<ul>` – lista nienumerowana z oferowanymi usługami.
     - `<li>` – elementy listy z nazwami usług.
   - **Sekcja "Godziny otwarcia":**
     - `<p>` – paragraf z informacjami o godzinach otwarcia, używający znacznika `<br>` do łamania linii.

**Commit:** "Dodanie treści związanych z salonem kosmetycznym do sekcji content"

---

#### **Krok 4: Dodanie linku do podstrony "Oferta"**

1. **Utwórz nowy plik `oferta.html` z podstawową strukturą HTML podobną do `index.html`.**

2. **W pliku `oferta.html`, w sekcji `<div id="content">`, dodaj szczegółowy opis oferty:**

   ```html
   <h2>Oferta</h2>
   <p>Zapoznaj się z naszą pełną ofertą zabiegów kosmetycznych i masaży.</p>
   <!-- Dodaj szczegółowe opisy poszczególnych usług -->
   ```

3. **Upewnij się, że w menu nawigacyjnym link do `oferta.html` działa poprawnie.**

**Commit:** "Dodanie podstrony 'Oferta' z opisem usług"

---

#### **Krok 5: Dodanie linku do podstrony "Kontakt"**

1. **Utwórz nowy plik `kontakt.html` z podstawową strukturą HTML.**

2. **W pliku `kontakt.html`, w sekcji `<div id="content">`, dodaj dane kontaktowe:**

   ```html
   <h2>Kontakt</h2>
   <p>BeautySpa - Salon Kosmetyczny<br>
      ul. Piękna 1, 00-000 Warszawa<br>
      Telefon: 123 456 789<br>
      Email: kontakt@beautyspa.pl</p>

   <h3>Formularz kontaktowy</h3>
   <form action="#" method="post">
       <label for="name">Imię:</label><br>
       <input type="text" id="name" name="name"><br>
       <label for="email">Email:</label><br>
       <input type="email" id="email" name="email"><br>
       <label for="message">Wiadomość:</label><br>
       <textarea id="message" name="message"></textarea><br>
       <input type="submit" value="Wyślij">
   </form>
   ```

   **Wyjaśnienie kodu:**

   - **Dane kontaktowe:**
     - Użycie `<p>` i `<br>` do wyświetlenia adresu, telefonu i emaila.
   - **Formularz kontaktowy:**
     - `<form>` – rozpoczyna formularz.
     - `<label>` i `<input>` – pola formularza dla imienia, emaila i wiadomości.
     - `<textarea>` – pole tekstowe dla wiadomości.
     - `<input type="submit">` – przycisk do wysłania formularza.

**Commit:** "Dodanie podstrony 'Kontakt' z danymi kontaktowymi i formularzem"

---

#### **Krok 6: Dodanie linku do strony zewnętrznej (Facebook)**

1. **W menu nawigacyjnym mamy już link do strony zewnętrznej (Facebook). Upewnij się, że link otwiera się w nowej karcie:**

   ```html
   <li><a href="https://www.facebook.com/BeautySpa" target="_blank">Facebook</a></li>
   ```

   **Wyjaśnienie kodu:**

   - `href="https://www.facebook.com/BeautySpa"` – adres profilu salonu na Facebooku.
   - `target="_blank"` – powoduje otwarcie linku w nowej karcie przeglądarki.

**Commit:** "Sprawdzenie i potwierdzenie działania linku do Facebooka"

---

#### **Krok 7: Dodanie dwóch zdjęć z opisami**

1. **W folderze projektu utwórz folder `images` i umieść w nim dwa obrazy związane z kosmetyką, np. `masaż.jpg` i `zabieg.jpg`.**

2. **W sekcji `#content` na stronie głównej (`index.html`), dodaj obrazy z opisami:**

   ```html
   <h2>Galeria</h2>
   <figure>
       <img src="images/masaż.jpg" alt="Masaż relaksacyjny" width="300">
       <figcaption>Masaż relaksacyjny</figcaption>
   </figure>

   <figure>
       <img src="images/zabieg.jpg" alt="Zabieg na twarz" width="300">
       <figcaption>Zabieg na twarz</figcaption>
   </figure>
   ```

   **Wyjaśnienie kodu:**

   - **Element `<figure>`** – grupuje obraz z podpisem.
   - **Element `<img>`** – wstawia obraz.
     - `src` – ścieżka do obrazu.
     - `alt` – tekst alternatywny dla obrazu.
     - `width` – szerokość obrazu w pikselach.
   - **Element `<figcaption>`** – dodaje podpis pod obrazem.

3. **Dodaj style do obrazów i opisów w `style.css`:**

   ```css
   figure {
       display: inline-block;
       margin: 10px;
       text-align: center;
   }

   figure img {
       width: 300px;
       height: auto;
       border-radius: 10px;
   }

   figcaption {
       margin-top: 5px;
       font-style: italic;
   }
   ```

   **Wyjaśnienie kodu:**

   - `figure` – ustawia elementy obok siebie z marginesami.
   - `figure img` – ustawia szerokość obrazów i zaokrągla rogi.
   - `figcaption` – dodaje odstęp i kursywę do podpisu.

**Commit:** "Dodanie zdjęć usług z opisami do strony głównej"

---

#### **Krok 8: Dodanie tabeli z cennikiem**

1. **W sekcji `#content` na stronie `oferta.html`, dodaj tabelę prezentującą cennik usług:**

   ```html
   <h2>Cennik usług</h2>
   <table>
       <tr>
           <th>Usługa</th>
           <th>Czas trwania</th>
           <th>Cena</th>
       </tr>
       <tr>
           <td>Masaż relaksacyjny</td>
           <td>60 min</td>
           <td>150 zł</td>
       </tr>
       <tr>
           <td>Zabieg na twarz</td>
           <td>45 min</td>
           <td>120 zł</td>
       </tr>
       <tr>
           <td>Manicure</td>
           <td>30 min</td>
           <td>70 zł</td>
       </tr>
   </table>
   ```

   **Wyjaśnienie kodu:**

   - **Tabela `<table>`** – przedstawia dane w formie tabelarycznej.
   - **Wiersze `<tr>`** – reprezentują wiersze tabeli.
   - **Nagłówki `<th>`** – komórki nagłówkowe tabeli.
   - **Dane `<td>`** – komórki z danymi.

2. **Dodaj style do tabeli w `style.css`:**

   ```css
   table {
       width: 100%;
       border-collapse: collapse;
       margin-bottom: 20px;
   }

   table, th, td {
       border: 1px solid #ddd;
   }

   th, td {
       padding: 10px;
       text-align: center;
   }

   th {
       background-color: #e0acd5;
       color: #fff;
   }

   tr:nth-child(even) {
       background-color: #f9f9f9;
   }
   ```

   **Wyjaśnienie kodu:**

   - `border-collapse: collapse;` – usuwa odstępy między komórkami.
   - `tr:nth-child(even)` – zmienia tło co drugiego wiersza, tworząc efekt paskowania.

**Commit:** "Dodanie tabeli cennika usług na stronie 'Oferta'"

---

#### **Krok 9: Dodanie linku do pobrania pliku tekstowego (np. cennika w PDF)**

1. **Umieść plik `cennik.pdf` w folderze projektu.**

2. **W sekcji `#content` na stronie `oferta.html`, dodaj link do pobrania pliku:**

   ```html
   <p>Pełny cennik usług dostępny jest w pliku PDF:</p>
   <a href="cennik.pdf" download>Pobierz cennik usług (PDF)</a>
   ```

   **Wyjaśnienie kodu:**

   - **Element `<a>` z atrybutem `download`** – umożliwia pobranie pliku po kliknięciu linku.
   - `href="cennik.pdf"` – ścieżka do pliku PDF z cennikiem.

**Commit:** "Dodanie linku do pobrania cennika usług w PDF"

---

### **Podsumowanie**

Gratulacje! Ukończyłeś tworzenie kompletnej strony internetowej salonu kosmetycznego. Strona zawiera wszystkie niezbędne elementy, takie jak nagłówek, menu, treść, obrazy, tabela z cennikiem i formularz kontaktowy.

---

**Przypomnienie:**

- **Po każdym etapie pamiętaj o wykonaniu commita z odpowiednim opisem.**
- **Zapisz wszystkie zmiany w swoim repozytorium na GitHub.**

---

**Powodzenia!**

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
