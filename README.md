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

**Ćwiczenie: Tworzenie Strony Internetowej dla Restauracji "Smakosz"**

---

### **Część I: Tutorial krok po kroku**

*Zostaje zachowana jako część poprzedniego ćwiczenia, zawierająca szczegółowe instrukcje, kod HTML i CSS oraz wyjaśnienia poszczególnych linijek kodu. Przypominam, że część ta została już przygotowana wcześniej.*

---

### **Część II: Ćwiczenia do samodzielnej realizacji**

Twoim zadaniem jest stworzenie strony internetowej dla fikcyjnej restauracji "Smakosz" zgodnie z poniższymi wytycznymi. Strona powinna być estetyczna, funkcjonalna i zgodna z określonymi założeniami, jakbyś otrzymał ją od zleceniodawcy. Nie otrzymujesz gotowych rozwiązań – musisz samodzielnie zaimplementować wszystkie elementy zgodnie z podanymi parametrami. Pamiętaj o wykonywaniu commitów z opisami po każdym etapie i zapisywaniu zmian w swoim repozytorium na GitHub.

---

#### **Zadanie 1: Struktura Strony Głównej**

**Koncepcja:**
Stwórz stronę główną dla restauracji "Smakosz", która będzie zawierała nagłówek, menu nawigacyjne, sekcję główną z informacjami o restauracji, galerię zdjęć, tabelę z menu oraz stopkę z informacjami kontaktowymi.

**Wytyczne:**

1. **Nagłówek (`header`):**
   - **Tekst:** "Restauracja Smakosz"
   - **Kolor tła:** #8B0000 (ciemny czerwony)
   - **Kolor tekstu:** #FFFFFF (biały)
   - **Czcionka:** 'Georgia, serif'
   - **Rozmiar czcionki:** 36px
   - **Wysokość:** 150px
   - **Wyśrodkowanie tekstu zarówno w pionie, jak i poziomie**

2. **Menu nawigacyjne (`nav`):**
   - **Tło:** #D2691E (ciemnobrązowy)
   - **Linki:**
     - "Strona główna" – link do `index.html`
     - "Menu" – link do `menu.html`
     - "Galeria" – link do `galeria.html`
     - "Kontakt" – link do `kontakt.html`
     - "Zarezerwuj stolik" – link do `rezerwacja.html`
   - **Kolor tekstu linków:** #FFFFFF (biały)
   - **Rozmiar czcionki linków:** 18px
   - **Czcionka linków:** 'Arial, sans-serif'
   - **Efekt przy najechaniu:** zmiana koloru tła linku na #A0522D (brązowy) i tekstu na #FFD700 (złoty)
   - **Układ:** poziomy, elementy wyświetlane obok siebie z równym odstępem

3. **Sekcja główna (`main`):**
   - **Podział na dwie kolumny:**
     - **Lewa kolumna (70% szerokości):** Informacje o restauracji
       - **Nagłówek:** "O Nas"
         - **Kolor tekstu:** #8B0000 (ciemny czerwony)
         - **Rozmiar czcionki:** 28px
         - **Czcionka:** 'Georgia, serif'
       - **Paragraf:** Opis restauracji (minimum 3 zdania)
         - **Kolor tekstu:** #333333 (ciemny szary)
         - **Rozmiar czcionki:** 16px
         - **Interlinia:** 1.5
         - **Tekst wyjustowany**
     - **Prawa kolumna (30% szerokości):** Galeria zdjęć
       - **Dodaj dwa zdjęcia z opisami:**
         - **Zdjęcie 1:** `wejscie.jpg` – "Eleganckie wejście do restauracji"
         - **Zdjęcie 2:** `wnetrze.jpg` – "Przytulne wnętrze"
         - **Szerokość zdjęć:** 100%
         - **Obramowanie zdjęć:** 2px solid #8B0000
         - **Opis zdjęć:** widoczny pod zdjęciem, czcionka: 'Arial, sans-serif', rozmiar: 14px, kolor: #555555

4. **Tabela z Menu (`section.menu`):**
   - **Nagłówek tabeli:** "Nasze Specjały"
     - **Kolor tła nagłówków:** #A0522D (brązowy)
     - **Kolor tekstu nagłówków:** #FFFFFF (biały)
     - **Czcionka nagłówków:** 'Arial, sans-serif'
     - **Rozmiar czcionki nagłówków:** 20px
   - **Kolory wierszy:**
     - **Naprzemiennie białe i #F5F5F5 (jasny szary)**
   - **Kolor tekstu w komórkach:** #333333 (ciemny szary)
   - **Czcionka w komórkach:** 'Verdana, sans-serif'
   - **Rozmiar czcionki w komórkach:** 16px
   - **Przykładowe dane w tabeli:**
     - **Kolumny:** "Danie", "Opis", "Cena"
     - **Wiersze:** Minimum 3 różne dania z opisem i ceną

5. **Stopka (`footer`):**
   - **Kolor tła:** #8B0000 (ciemny czerwony)
   - **Kolor tekstu:** #FFFFFF (biały)
   - **Czcionka:** 'Arial, sans-serif'
   - **Rozmiar czcionki:** 14px
   - **Zawartość:**
     - **Adres:** ul. Smakosza 10, 00-001 Warszawa
     - **Telefon:** 123-456-789
     - **Email:** kontakt@smakosz.pl
     - **Link do pobrania pliku PDF:** "Pobierz menu w PDF" – link do `menu.pdf`, z atrybutem `download`
     - **Styl linku:** kolor #FFD700 (złoty), bez podkreślenia, podkreślenie przy najechaniu kursorem

6. **Ogólne Style:**
   - **Tło strony:** #FFF8DC (kukurydziany)
   - **Marginesy:** 0 dla wszystkich elementów
   - **Font-family całej strony:** 'Arial, sans-serif'
   - **Responsive Design:** Upewnij się, że strona jest czytelna na różnych rozdzielczościach ekranów (minimum: 1024px szerokości)

**Commit:** "Zadanie 1: Stworzenie struktury strony głównej dla restauracji 'Smakosz' z określonymi stylami"

---

#### **Zadanie 2: Dodanie Treści do Sekcji "O Nas"**

**Koncepcja:**
W sekcji "O Nas" opisz krótko historię restauracji, jej misję oraz wartości, jakie reprezentuje.

**Wytyczne:**

1. **Nagłówek:** "O Nas"
   - **Kolor tekstu:** #8B0000 (ciemny czerwony)
   - **Rozmiar czcionki:** 28px
   - **Czcionka:** 'Georgia, serif'

2. **Paragraf:**
   - **Treść:** Opis restauracji (minimum 3 zdania). Możesz użyć następującego przykładu:
     > "Restauracja Smakosz została założona w 2010 roku z pasji do wyśmienitej kuchni i wyjątkowej obsługi. Naszym celem jest zapewnienie gościom niezapomnianych doznań kulinarnych w przytulnej atmosferze. Dbamy o najwyższą jakość składników i innowacyjne podejście do tradycyjnych dań."
   - **Kolor tekstu:** #333333 (ciemny szary)
   - **Rozmiar czcionki:** 16px
   - **Interlinia:** 1.5
   - **Tekst wyjustowany**

**Commit:** "Zadanie 2: Dodanie treści do sekcji 'O Nas'"

---

#### **Zadanie 3: Dodanie Tabeli z Menu**

**Koncepcja:**
Przedstaw w tabeli różnorodne dania oferowane przez restaurację wraz z opisem i ceną.

**Wytyczne:**

1. **Nagłówek tabeli:** "Nasze Specjały"
   - **Kolor tła nagłówków:** #A0522D (brązowy)
   - **Kolor tekstu nagłówków:** #FFFFFF (biały)
   - **Czcionka nagłówków:** 'Arial, sans-serif'
   - **Rozmiar czcionki nagłówków:** 20px

2. **Kolumny tabeli:** "Danie", "Opis", "Cena"

3. **Przykładowe dane:**

   | Danie               | Opis                                      | Cena  |
   |---------------------|-------------------------------------------|-------|
   | Pierogi Ruskie      | Tradycyjne pierogi z serem i ziemniakami  | 25 zł |
   | Zupa Pomidorowa     | Aromatyczna zupa z dojrzałych pomidorów  | 18 zł |
   | Stek Wołowy         | Soczysty stek z dodatkiem warzyw          | 60 zł |

4. **Stylizacja tabeli:**
   - **Szerokość:** 100%
   - **Obramowanie:** 1px solid #ddd dla tabeli, nagłówków i komórek
   - **Padding:** 10px dla nagłówków i komórek
   - **Wyrównanie tekstu:** wyśrodkowany
   - **Naprzemienne kolory wierszy:** co drugi wiersz ma tło #F9F9F9 (jasny szary)

**Commit:** "Zadanie 3: Dodanie tabeli z menu restauracji"

---

#### **Zadanie 4: Dodanie Galerii Zdjęć**

**Koncepcja:**
Pokaż atmosferę restauracji oraz przykładowe dania poprzez galerię zdjęć.

**Wytyczne:**

1. **Sekcja:** "Galeria"
   - **Nagłówek:** "Galeria"
     - **Kolor tekstu:** #8B0000 (ciemny czerwony)
     - **Rozmiar czcionki:** 28px
     - **Czcionka:** 'Georgia, serif'

2. **Zdjęcia:**
   - **Ilość:** 3 zdjęcia
   - **Nazwy plików:** `salon.jpg`, `danie1.jpg`, `danie2.jpg`
   - **Opis zdjęć:**
     - `salon.jpg` – "Eleganckie wnętrze restauracji"
     - `danie1.jpg` – "Pierogi Ruskie z dodatkami"
     - `danie2.jpg` – "Soczysty stek wołowy"
   - **Szerokość zdjęć:** 30% szerokości kontenera
   - **Obramowanie zdjęć:** 2px solid #8B0000
   - **Opis zdjęć:** widoczny pod zdjęciem, czcionka: 'Arial, sans-serif', rozmiar: 14px, kolor: #555555
   - **Efekt przy najechaniu:** przyciemnienie zdjęcia do 80% przez zmianę `opacity` na 0.8

3. **Stylizacja galerii:**
   - **Użyj flexbox do ułożenia zdjęć obok siebie z równymi odstępami**
   - **Dodaj marginesy wokół zdjęć: 10px**
   - **Zaokrągl rogi zdjęć: border-radius: 5px**

**Commit:** "Zadanie 4: Dodanie galerii zdjęć restauracji"

---

#### **Zadanie 5: Dodanie Formularza Kontaktowego**

**Koncepcja:**
Umożliw klientom kontakt z restauracją poprzez prosty formularz.

**Wytyczne:**

1. **Sekcja:** "Kontakt"
   - **Nagłówek:** "Kontakt"
     - **Kolor tekstu:** #8B0000 (ciemny czerwony)
     - **Rozmiar czcionki:** 28px
     - **Czcionka:** 'Georgia, serif'

2. **Dane kontaktowe:**
   - **Adres:** ul. Smakosza 10, 00-001 Warszawa
   - **Telefon:** 123-456-789
   - **Email:** kontakt@smakosz.pl
   - **Stylizacja tekstu:** 
     - **Kolor:** #333333 (ciemny szary)
     - **Rozmiar czcionki:** 16px

3. **Formularz:**
   - **Nagłówek:** "Formularz kontaktowy"
     - **Kolor tekstu:** #8B0000 (ciemny czerwony)
     - **Rozmiar czcionki:** 22px
     - **Czcionka:** 'Arial, sans-serif'
   - **Pola formularza:**
     - **Imię:**
       - **Element:** `<input type="text" id="name" name="name">`
       - **Placeholder:** "Twoje imię"
     - **Email:**
       - **Element:** `<input type="email" id="email" name="email">`
       - **Placeholder:** "Twój email"
     - **Wiadomość:**
       - **Element:** `<textarea id="message" name="message" rows="5" placeholder="Twoja wiadomość"></textarea>`
   - **Przycisk wysyłania:**
     - **Element:** `<input type="submit" value="Wyślij">`
     - **Stylizacja przycisku:** 
       - **Tło:** #8B0000
       - **Kolor tekstu:** #FFFFFF
       - **Padding:** 10px 20px
       - **Border:** none
       - **Border-radius:** 5px
       - **Efekt przy najechaniu:** tło zmienia się na #A0522D

4. **Stylizacja formularza w CSS:**
   - **Elementy formularza:**
     - **Pola input i textarea:**
       - **Width:** 100%
       - **Padding:** 10px
       - **Margin-bottom:** 15px
       - **Border:** 1px solid #ccc
       - **Border-radius:** 4px
   - **Przycisk:**
     - **Dodaj hover effect w CSS:**
       ```css
       form input[type="submit"]:hover {
           background-color: #A0522D;
           cursor: pointer;
       }
       ```

**Commit:** "Zadanie 5: Dodanie formularza kontaktowego"

---

#### **Zadanie 6: Dodanie Linku do Pobrania Pliku PDF z Menu**

**Koncepcja:**
Udostępnij klientom możliwość pobrania pełnego menu w formacie PDF.

**Wytyczne:**

1. **Plik PDF:**
   - **Nazwa pliku:** `menu.pdf`
   - **Zawartość:** Pełne menu restauracji "Smakosz"

2. **Link do pobrania:**
   - **Tekst linku:** "Pobierz pełne menu (PDF)"
   - **Umiejscowienie:** w sekcji "Menu" poniżej tabeli z menu
   - **Atrybuty:** `href="menu.pdf"` oraz `download`
   - **Stylizacja linku:** 
     - **Kolor tekstu:** #FFD700 (złoty)
     - **Brak podkreślenia**
     - **Efekt przy najechaniu:** tekst jest podkreślony

   - **Przykład kodu HTML:**
     ```html
     <p>Pobierz pełne menu:</p>
     <a href="menu.pdf" download class="download-link">Pobierz pełne menu (PDF)</a>
     ```

3. **Stylizacja linku w CSS:**
   - **Dodaj do `style.css`:**
     ```css
     .download-link {
         color: #FFD700;
         text-decoration: none;
     }

     .download-link:hover {
         text-decoration: underline;
     }
     ```

**Commit:** "Zadanie 6: Dodanie linku do pobrania menu w PDF"

---

#### **Zadanie 7: Stylizacja Ogólna Strony**

**Koncepcja:**
Ulepsz wygląd strony, dbając o spójność kolorystyczną, czcionki oraz responsywność.

**Wytyczne:**

1. **Czcionki:**
   - **Nagłówki (`h1`, `h2`, `h3`):** 'Georgia, serif'
   - **Teksty paragrafów i list:** 'Arial, sans-serif'
   - **Linki:** 'Arial, sans-serif'

2. **Kolory:**
   - **Tło strony:** #FFF8DC (kukurydziany)
   - **Nagłówki:** #8B0000 (ciemny czerwony)
   - **Tekst paragrafów:** #333333 (ciemny szary)
   - **Linki:** #FFFFFF (biały) w menu, #FFD700 (złoty) w stopce
   - **Przy najechaniu na linki w menu:** tło #A0522D (brązowy), tekst #FFD700 (złoty)

3. **Rozmiary czcionek:**
   - **Nagłówki:**
     - `h1`: 36px
     - `h2`: 28px
     - `h3`: 22px
   - **Tekst paragrafów i list:** 16px
   - **Linki w menu:** 18px
   - **Opis zdjęć:** 14px

4. **Marginesy i odstępy:**
   - **Sekcje:** 20px padding wewnętrzny
   - **Elementy list i tabel:** odpowiednie marginesy dla czytelności
   - **Galeria:** marginesy 10px między zdjęciami

5. **Responsive Design:**
   - **Użyj media queries w CSS, aby dostosować układ na urządzeniach mobilnych:**
     - **Menu nawigacyjne:** zmiana z poziomego na pionowy układ
     - **Galeria zdjęć:** ułożenie zdjęć jeden pod drugim na mniejszych ekranach

   - **Przykład media query:**
     ```css
     @media screen and (max-width: 768px) {
         #menu li {
             float: none;
             width: 100%;
         }

         .gallery {
             display: block;
         }

         .gallery img {
             width: 100%;
             margin-bottom: 10px;
         }
     }
     ```

**Commit:** "Zadanie 7: Stylizacja ogólna strony dla restauracji 'Smakosz'"

---

#### **Zadanie 8: Dodanie Linku do Pobrania Pliku PDF w Stopce**

**Koncepcja:**
Ułatw klientom dostęp do menu poprzez link w stopce.

**Wytyczne:**

1. **Link do pobrania:**
   - **Tekst linku:** "Pobierz pełne menu (PDF)"
   - **Atrybuty:** `href="menu.pdf"` oraz `download`
   - **Stylizacja linku:**
     - **Kolor tekstu:** #FFD700 (złoty)
     - **Brak podkreślenia**
     - **Efekt przy najechaniu:** tekst jest podkreślony

2. **Umiejscowienie:** w sekcji `footer` poniżej danych kontaktowych

3. **Przykład kodu HTML:**
   ```html
   <p>Pobierz pełne menu:</p>
   <a href="menu.pdf" download class="download-link">Pobierz pełne menu (PDF)</a>
   ```

4. **Stylizacja linku w CSS:**
   - **Dodaj do `style.css`:**
     ```css
     .download-link {
         color: #FFD700;
         text-decoration: none;
     }

     .download-link:hover {
         text-decoration: underline;
     }
     ```

**Commit:** "Zadanie 8: Dodanie linku do pobrania menu w PDF w stopce"

---

### **Przypomnienie**

- **Po każdym etapie pamiętaj o wykonaniu commita z odpowiednim opisem.**
- **Zapisz wszystkie zmiany w swoim repozytorium na GitHub.**

---

**Powodzenia w realizacji zadania! Twój profesjonalny projekt strony internetowej restauracji "Smakosz" czeka na wykonanie.**

---

### **Dodatkowe Wskazówki:**

- **Używaj semantycznych znaczników HTML5** (np. `<header>`, `<nav>`, `<main>`, `<section>`, `<footer>`) zamiast `<div>` tam, gdzie to możliwe.
- **Optymalizuj obrazy** pod kątem webu, aby strona ładowała się szybko.
- **Sprawdzaj poprawność kodu** za pomocą walidatora HTML i CSS.
- **Testuj stronę na różnych przeglądarkach i urządzeniach**, aby upewnić się, że wygląda dobrze wszędzie.

---

**Powodzenia! Twój profesjonalny projekt strony internetowej czeka na realizację.**
