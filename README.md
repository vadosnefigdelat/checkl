# 🚀 The Ultimate Website Launch Checklist
### Kompletny Przewodnik i Checklist Przed Publikacją Strony WWW
> Zbiór najlepszych praktyk, heurystyk i metod audytu stron internetowych zebranych ze sprawdzonych źródeł: **Nielsen Norman Group (NN/g)**, **Webflow Pre-Launch QA**, **Smashing Magazine**, **The A11Y Project (WCAG 2.2)** oraz **Google Web Vitals**.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/vadosnefigdelat/checkl/pulls)
[![Web Standards](https://img.shields.io/badge/Standards-WCAG%202.2%20%7C%20Core%20Web%20Vitals-blue.svg)](#)

---

## 🧭 Spis treści (Table of Contents)
1. [📱 1. UI & Responsywność (Mobile, Tablet, Desktop)](#-1-ui--responsywno%C5%9B%C4%87)
2. [👁️ 2. UX i 10 Heurystyk Nielsena Normana](#-%EF%B8%8F-2-ux-i-10-heurystyk-nielsena-normana)
3. [✍️ 3. Typografia, Treść i Skanowalność](#-%EF%B8%8F-3-typografia-tre%C5%9B%C4%87-i-skanowalno%C5%9B%C4%87)
4. [🎨 4. Kolory, Kontrast i Dostępność (WCAG 2.2 / A11y)](#-4-kolory-kontrast-i-dost%C4%99pno%C5%9B%C4%87-wcag-22)
5. [🖱️ 5. Interakcje, Formularze i Doświadczenie Użytkownika](#-%EF%B8%8F-5-interakcje-formularze-i-stany-ui)
6. [⚡ 6. Wydajność, Obrazy i Prędkość (Core Web Vitals)](#-6-wydajno%C5%9B%C4%87-obrazy-i-core-web-vitals)
7. [🔍 7. SEO i Widoczność w Wyszukiwarkach](#-7-seo-i-social-media-opengraph)
8. [🔒 8. Bezpieczeństwo i Prawo (RODO, Cookies, HTTPS)](#-8-bezpiecze%C5%84stwo-i-aspekty-prawne)
9. [🧰 9. Najlepsze Darmowe Narzędzia do Audytu](#-9-niezb%C4%99dnik-najlepsze-darmowe-narz%C4%99dzia)

---

## 📱 1. UI & Responsywność

Przetestuj stronę na co najmniej 4 szerokościach ekranu: **Mobile (375–420px)**, **Tablet (768–1024px)**, **Laptop (1280–1440px)**, **Duży monitor (1920px+)**.

* [ ] **Brak poziomego paska przewijania (No Horizontal Overflow):** Strona na telefonie nie może przesuwać się w lewo/prawo. Nic nie może wystawać poza krawędź ekranu (`overflow-x: hidden` to tylko ostateczność, szukaj elementów o sztywnej szerokości `width: ...px`).
* [ ] **Minimalna strefa dotyku (Touch Target Size):** Według standardów Google i Apple, każdy klikalny element na telefonie (przycisk, ikona menu, link) musi mieć minimum **44 × 44 px** (lub **48 × 48 px**), aby użytkownik nie klikał przypadkowo sąsiednich rzeczy.
* [ ] **Odstępy między elementami klikalnymi:** Pomiędzy dwoma linkami lub ikonami na telefonie zachowaj minimum **8–12 px** marginesu.
* [ ] **Skalowanie nagłówków:** Upewnij się, że wielkie nagłówki z wersji komputerowej (np. 56px) na telefonie zmniejszają się (np. do 28–34px) i nie dzielą słów w nienaturalnych miejscach.
* [ ] **Test obrotu ekranu (Landscape):** Sprawdź, czy po obróceniu telefonu poziomo nagłówek i menu nie zasłaniają całego ekranu.
* [ ] **Zamykanie menu mobilnego:** Czy menu "hamburger" po kliknięciu w link automatycznie się zwija i nie blokuje ekranu?

---

## 👁️ 2. UX i 10 Heurystyk Nielsena Normana

Zasady użyteczności stworzone przez **Nielsen Norman Group (NN/g)** — światowy autorytet w dziedzinie User Experience:

* [ ] **Widoczność stanu systemu (Visibility of System Status):** Użytkownik w każdej chwili wie, co się dzieje. Jeśli formularz wysyła dane — pojawia się animacja ładowania (spinner / pasek postępu), a po wysłaniu jasny komunikat sukcesu.
* [ ] **Dopasowanie do prawdziwego świata (Match with the Real World):** Język strony jest prosty i naturalny dla odbiorcy. Brak hermetycznego żargonu i trudnych skrótów technicznych.
* [ ] **Kontrola i wolność użytkownika (User Control and Freedom):** Użytkownik może w każdej chwili zamknąć okno pop-up / modal (klawiszem `Esc`, wyraźnym krzyżykiem `×` lub kliknięciem w tło).
* [ ] **Spójność i standardy (Consistency and Standards):** 
  * Logo w lewym górnym rogu zawsze prowadzi do strony głównej.
  * Koszyk i profil znajdują się w prawym górnym rogu.
  * Linki wyglądają jak linki (są podkreślone lub mają odróżniający się kolor).
* [ ] **Zapobieganie błędom (Error Prevention):** W polach formularza (np. telefon, e-mail) z góry podpowiedz poprawny format (np. placeholder: `twoj@email.pl`).
* [ ] **Rozpoznawanie zamiast przypominania (Recognition rather than Recall):** Informacje potrzebne do podjęcia decyzji (np. cena, czas dostawy, godziny otwarcia) są widoczne od razu, a nie ukryte głęboko w podstronach.
* [ ] **Estetyka i minimalizm:** Usunięto wszystkie zbędne elementy, które tylko zaśmiecają stronę i odciągają uwagę od głównego celu (Call to Action).
* [ ] **Własna strona błędu 404 (Custom 404 Page):** Zamiast systemowego błędu serwera, strona posiada dedykowaną, przyjazną stronę 404 z przyciskiem *„Wróć na stronę główną”* i wyszukiwarką.

---

## ✍️ 3. Typografia, Treść i Skanowalność

Użytkownicy w internecie **nie czytają tekstu od deski do deski — oni go skanują** (tzw. F-Pattern).

* [ ] **Maksymalnie 2 rodziny fontów:** Jeden krój na nagłówki (np. szeryfowy lub wyrazisty display) i jeden neutralny krój na treść (np. *Inter*, *Plus Jakarta Sans*, *Roboto*).
* [ ] **Hierarchia wielkości (Modular Scale):** Wyraźna różnica skali między H1 (główny tytuł), H2 (sekcja), H3 (kafelki) i tekstem akapitowym.
* [ ] **Optymalna interlinia (*line-height*):**
  * Zwykły tekst: **1.5 – 1.65 (150%–165%)** — zapewnia swobodny oddech dla oka.
  * Wielkie nagłówki: **1.05 – 1.20 (105%–120%)** — zapobiega rozpadaniu się tytułu.
* [ ] **Długość wiersza (Line Length):** Szerokość kolumny tekstu powinna wynosić od **45 do 75 znaków na wiersz** (ok. 600–700 px). Zbyt szerokie linijki męczą wzrok.
* [ ] **Krótkie akapity:** Maksymalnie **3–4 linijki w akapicie**. Dziel tekst śródtytułami, pogrubieniami i listami punktowanymi.
* [ ] **Likwidacja „bękartów” i „sierot” (Wiszące spójniki):** Samotne litery (*a, i, o, u, w, z*) na końcach linijek przeniesione do nowego wiersza za pomocą twardej spacji (`&nbsp;` lub `Shift + Enter`).
* [ ] **Brak tekstów tymczasowych:** Usunięte wszystkie fragmenty *„Lorem Ipsum”*, *„test test”*, a także domyślne napisy szablonów.
* [ ] **Sprawdzenie danych kontaktowych:** Prawdziwy i działający numer telefonu, adres e-mail, aktualne godziny otwarcia i adres z linkiem do Map Google.

---

## 🎨 4. Kolory, Kontrast i Dostępność (WCAG 2.2)

Dostępność cyfrowa (*Accessibility / a11y*) to gwarancja, że z Twojej strony skorzystają również osoby słabowidzące, starsze lub korzystające z czytników ekranu.

* [ ] **Zasada podziału 60 – 30 – 10:**
  * **60%:** Kolor dominujący (tło, baza).
  * **30%:** Kolor struktury (karty, teksty, linie).
  * **10%:** Wyrazisty kolor akcentu (przyciski CTA, najważniejsze komunikaty).
* [ ] **Minimalny współczynnik kontrastu tekstu (WCAG AA / AAA):**
  * Zwykły tekst do tła: minimum **4.5:1** (zalecane **7:1** dla poziomu AAA).
  * Duży tekst (od 24px) lub pogrubiony (od 18.5px): minimum **3:1**.
* [ ] **Kolor to nie jedyny nośnik informacji:** Nie wyróżniaj linków w tekście wyłącznie kolorem — dodaj podkreślenie. Komunikaty błędów oprócz czerwonego koloru muszą mieć ikonkę ostrzegawczą i jasny tekst.
* [ ] **Miękkie tło zamiast ostrej bieli:** Zamiast agresywnego `#FFFFFF` warto stosować złamaną biel, kość słoniową lub subtelny krem (np. `#FAF7F2`, `#F8F9FA`), co zmniejsza zmęczenie oczu.
* [ ] **Teksty alternatywne dla grafik (`alt="..."`):** Wszystkie zdjęcia niosące treść mają krótki, opisowy znacznik alt (np. `alt="Filiżanka świeżo parzonego cappuccino z cynamonem"`). Grafiki czysto ozdobne mają pusty atrybut `alt=""`.
* [ ] **Nawigacja klawiaturą (Tab Navigation):** Możliwość przejścia przez całą stronę wyłącznie klawiszem `Tab` (widoczny focus outline wokół klikalnych elementów).

---

## 🖱️ 5. Interakcje, Formularze i Stany UI

* [ ] **Stany interaktywne (Hover, Active, Focus):**
  * Każdy przycisk i link reaguje na najechanie kursorem myszy (*hover*).
  * Widoczny stan wciśnięcia (*active*).
  * Widoczne obramowanie dla osób nawigujących klawiaturą (*focus-visible*).
* [ ] **Walidacja formularza na żywo (Inline Validation):** Użytkownik widzi błąd od razu po wpisaniu złego maila, a nie dopiero po przeładowaniu całej strony.
* [ ] **Pola formularza dostosowane do urządzeń mobilnych:**
  * W polu na telefon klawiatura przełącza się na numeryczną (`type="tel"`).
  * W polu e-mail klawiatura pokazuje małpę `@` (`type="email"`).
* [ ] **Test wysłania formularza:** 
  * Czy po wysłaniu e-mail trafia do skrzynki odbiorczej właściciela strony?
  * Czy e-maile nie wpadają do folderu SPAM?
* [ ] **Sprawdzenie wszystkich linków zewnętrznych:** Linki do Instagrama, Facebooka, LinkedIn otwierają się w nowej karcie (`target="_blank" rel="noopener noreferrer"`).
* [ ] **Płynne przewijanie (Smooth Scroll):** Kotwice w menu (np. `#kontakt`, `#menu`) płynnie przewijają widok do sekcji.

---

## ⚡ 6. Wydajność, Obrazy i Core Web Vitals

Szybkość ładowania decyduje o tym, czy użytkownik zostanie na stronie, czy zamknie ją po 3 sekundach.

* [ ] **Nowoczesne formaty grafik:** Wszystkie zdjęcia skompresowane i zapisane w formatach **WebP** lub **AVIF** (zamiast ciężkich PNG/JPG).
* [ ] **Właściwe wymiary grafik:** Zdjęcie wyświetlane w rozmiarze 400 × 400 px nie powinno mieć w pliku 4000 × 4000 px i ważyć 8 MB. Plik powinien ważyć poniżej **150–250 KB**.
* [ ] **Opóźnione ładowanie (`loading="lazy"`):** Zdjęcia poniżej pierwszego ekranu ładują się dopiero wtedy, gdy użytkownik do nich przewinie.
* [ ] **Optymalizacja fontów:** Fonty w formacie `.woff2` z parametrem `font-display: swap`, aby tekst pojawiał się natychmiast bez białego ekranu (*FOIT*).
* [ ] **Wynik Google PageSpeed Insights:** Strona osiąga minimum **85+ punktów** na urządzeniach mobilnych i **95+** na komputerach.
* [ ] **Brak przesunięć układu (CLS - Cumulative Layout Shift):** Wszystkie obrazki i ramki wideo mają określone atrybuty `width` i `height`, aby strona nie „skakała” podczas wczytywania.

---

## 🔍 7. SEO i Social Media (OpenGraph)

* [ ] **Unikalny znacznik `<title>` na każdej podstronie:** Maksymalnie **55–60 znaków** (np. `Chwila | Sąsiedzka kawiarnia i ciasto domowe Poznań`).
* [ ] **Meta opis (`<meta name="description">`):** Chwytliwy opis pod wynik wyszukiwania w Google o długości **130–160 znaków** z jasnym wezwaniem do odwiedzin.
* [ ] **Tylko jeden nagłówek `<h1>` na stronę:** Stanowiący główną frazę i temat strony.
* [ ] **Karty Social Media (Open Graph & Twitter Cards):**
  * Zdefiniowany tag `og:title`, `og:description`, `og:url`.
  * Wgrana dedykowana grafika `og:image` (o wymiarach **1200 × 630 px**), która wyświetla się przy wklejaniu linku na Facebooku, Messengerze, Slacku czy Twitterze/X.
* [ ] **Wgrana ikona Favicon i Webclip:**
  * Standardowa ikonka do zakładki przeglądarki (`favicon.ico` / `.png` 32 × 32 px).
  * Ikonka Apple Touch Icon (180 × 180 px) dla skrótów na ekranie smartfona.
* [ ] **Pliki `robots.txt` i mapa strony `sitemap.xml`:** Upewnij się, że strona nie ma włączonej blokady indeksowania (`noindex`), jeśli ma być widoczna w Google.

---

## 🔒 8. Bezpieczeństwo i Aspekty Prawne

* [ ] **Aktywny certyfikat SSL (Protokół HTTPS):** W pasku adresu wyświetla się kłódka `https://`. Automatyczne przekierowanie z `http://` na `https://`.
* [ ] **Pasek zgody na pliki Cookies (RODO / GDPR / ePrivacy):** Jeśli strona korzysta z Google Analytics, pikseli reklamowych lub zewnętrznych skryptów śledzących — użytkownik musi mieć możliwość wyrażenia zgody przed ich uruchomieniem.
* [ ] **Polityka Prywatności i Regulamin:** Podstrona opisująca, kto jest administratorem danych, jak dane są przetwarzane i jak się skontaktować.
* [ ] **Prawa autorskie w stopce:** Aktualny rok (np. `© 2026 Nazwa Firmy. Wszelkie prawa zastrzeżone.`).

---

## 🧰 9. Niezbędnik: Najlepsze Darmowe Narzędzia

Oto zestaw najpopularniejszych narzędzi online, którymi specjaliści testują strony:

| Narzędzie | Zastosowanie | Link |
| :--- | :--- | :--- |
| **Google PageSpeed Insights** | Test prędkości, optymalizacji i wskaźników Core Web Vitals | [pagespeed.web.dev](https://pagespeed.web.dev/) |
| **WAVE Accessibility Tool** | Automatyczny audyt błędów dostępności i kontrastu WCAG | [wave.webaim.org](https://wave.webaim.org/) |
| **WebAIM Contrast Checker** | Precyzyjny kalkulator kontrastu tekstu do tła | [webaim.org/resources/contrastchecker](https://webaim.org/resources/contrastchecker/) |
| **Squoosh / TinyPNG** | Błyskawiczna kompresja i konwersja grafik do formatu WebP | [squoosh.app](https://squoosh.app/) |
| **Metatags.io** | Podgląd jak strona prezentuje się w Google, na Facebooku i Twitterze | [metatags.io](https://metatags.io/) |
| **Responsively App** | Narzędzie do testowania strony na kilkunastu ekranach naraz | [responsively.app](https://responsively.app/) |
| **Coolors Contrast** | Sprawdzanie palet kolorystycznych pod kątem daltonizmu | [coolors.co/contrast-checker](https://coolors.co/contrast-checker) |

---

### 💡 Prosty trik na koniec: „Test zmrużonych oczu” (*Squint Test*)
Odsuń się od monitora na krok i mocno zmruż oczy, aby obraz się rozmył:
1. Czy od razu widzisz 2–3 najważniejsze elementy na ekranie?
2. Jeśli wszystko zlewa się w jedną szarą plamę — dodaj więcej pustej przestrzeni (white space) i wzmocnij kontrast kluczowych przycisków!

---
*Projekt otwarty na rozwój. Jeśli masz pomysł na dodatkowe punkty kontrolne, stwórz Pull Request lub zgłoś Issue!*
