# Web pre-launch checklist

Praktyczny checklist do sprawdzania stron internetowych przed publikacją, stworzony na podstawie wytycznych Nielsen Norman Group, Webflow, Smashing Magazine oraz WCAG.

---

## WEB-01 · Touch targets (Strefy dotyku)

- **Dotyczy** · Urządzenia mobilne, responsywny web
- **Jak testować** · Zmierz rzeczywiste pole klikalne przycisków, ikon i linków na telefonie. Sprawdź, czy nie są zbyt blisko siebie.
- **Sugerowane rozwiązanie** · Zadbaj o minimum 44 × 44 pt (standard Apple) lub 48 × 48 dp (standard Google). Zwiększ padding wokół przycisków i dodaj minimum 8 px odstępu między linkami.
- **Źródła** · [Apple HIG](https://developer.apple.com/design/human-interface-guidelines/), [Google web.dev](https://web.dev/accessible-tap-targets/)

## WEB-02 · Horizontal overflow (Przewijanie w poziomie)

- **Dotyczy** · Widok mobilny i tablet
- **Jak testować** · Otwórz stronę w narzędziach deweloperskich przeglądarki na szerokościach 375 px, 390 px i 414 px. Spróbuj przesunąć stronę w lewo i w prawo.
- **Sugerowane rozwiązanie** · Strona nie może przesuwać się w poziomie. Sprawdź elementy ze sztywną szerokością (np. `width: 500px`), za duże zdjęcia lub za duże marginesy i zamień je na wartości procentowe lub `max-width: 100%`.
- **Źródła** · [Webflow Responsive](https://university.webflow.com/lesson/intro-to-responsive-design)

## WEB-03 · Headings scale (Skalowanie nagłówków)

- **Dotyczy** · Smartfony (ekrany poniżej 480 px)
- **Jak testować** · Zobacz, jak duży nagłówek H1 z komputera wygląda na małym ekranie telefonu.
- **Sugerowane rozwiązanie** · Zmniejsz wielkość liter na małym ekranie (np. z 48 px do 28–32 px). Unikaj sytuacji, w której jedno słowo łamie się w połowie lub zajmuje cały ekran.
- **Źródła** · [Smashing Magazine](https://www.smashingmagazine.com/2021/03/complete-website-launch-checklist/)

## WEB-04 · Mobile navigation (Nawigacja mobilna)

- **Dotyczy** · Menu hamburger na telefonie
- **Jak testować** · Otwórz menu, kliknij w link do sekcji i zobacz, czy menu samo się zamyka oraz czy da się je łatwo zamknąć krzyżykiem lub kliknięciem w tło.
- **Sugerowane rozwiązanie** · Menu po kliknięciu w link powinno przenieść użytkownika do sekcji i automatycznie się schować, żeby nie zasłaniało treści.
- **Źródła** · [NN/g Mobile Navigation](https://www.nngroup.com/articles/hamburger-menus/)

---

## UX-01 · System status & feedback (Stan systemu)

- **Dotyczy** · Formularze, przyciski akcji, ładowanie danych
- **Jak testować** · Wypełnij formularz na stronie i kliknij wyślij. Zobacz, czy strona od razu daje znać, że coś się dzieje.
- **Sugerowane rozwiązanie** · Zastosuj pierwszą heurystykę Nielsena (Visibility of System Status). Pokaż animację ładowania (spinner) na przycisku podczas wysyłania, a po zakończeniu wyświetl wyraźny komunikat z podziękowaniem.
- **Źródła** · [NN/g Heuristics](https://www.nngroup.com/articles/ten-usability-heuristics/)

## UX-02 · User freedom & modals (Zamykanie okienek)

- **Dotyczy** · Okienka pop-up, banery, powiększone zdjęcia
- **Jak testować** · Otwórz okienko na stronie i spróbuj je zamknąć klawiszem Esc, kliknięciem w ciemne tło lub krzyżykiem.
- **Sugerowane rozwiązanie** · Użytkownik musi mieć pełną kontrolę (User Control and Freedom). Dodaj wyraźny przycisk zamknięcia `×` w prawym górnym rogu i pozwól zamknąć okno kliknięciem poza nim.
- **Źródła** · [NN/g Heuristics](https://www.nngroup.com/articles/ten-usability-heuristics/)

## UX-03 · Error prevention (Zapobieganie błędom)

- **Dotyczy** · Formularze kontaktowe i pola do wpisywania tekstu
- **Jak testować** · Wpisz błędny numer telefonu lub e-mail bez znaku `@` i spróbuj wysłać.
- **Sugerowane rozwiązanie** · Waliduj dane na bieżąco. Wyświetlaj krótką i pomocną podpowiedź pod polem (np. „Podaj poprawny adres e-mail, np. jan@domena.pl”), zamiast ogólnego napisu „Błąd”.
- **Źródła** · [NN/g Heuristics](https://www.nngroup.com/articles/ten-usability-heuristics/), [Webflow Launch QA](https://webflow.com/blog/website-launch-checklist)

## UX-04 · Custom 404 page (Strona błędu 404)

- **Dotyczy** · Nieistniejące podstrony
- **Jak testować** · Wpisz w przeglądarce adres strony z losowym ciągiem liter na końcu (np. `/asdfgh`).
- **Sugerowane rozwiązanie** · Zamiast pustego systemowego błędu serwera przygotuj przyjazną stronę 404 z krótkim tekstem i dużym przyciskiem powrotu na stronę główną.
- **Źródła** · [Smashing Magazine](https://www.smashingmagazine.com/2021/03/complete-website-launch-checklist/)

---

## TXT-01 · Font pairing & hierarchy (Hierarchia fontów)

- **Dotyczy** · Wszystkie podstrony serwisu
- **Jak testować** · Sprawdź w stylach, ile różnych krojów pisma zostało użytych na stronie.
- **Sugerowane rozwiązanie** · Ogranicz się do maksymalnie 2 fontów (jeden wyrazisty na nagłówki, drugi prosty i czytelny na zwykły tekst). Zadbaj o wyraźną różnicę wielkości między H1, H2 i tekstem zwykłym.
- **Źródła** · [Webflow Typography](https://university.webflow.com/lesson/intro-to-responsive-design)

## TXT-02 · Line length & height (Długość wiersza i interlinia)

- **Dotyczy** · Akapity i bloki tekstu
- **Jak testować** · Policz średnią liczbę znaków w jednej linijce tekstu na komputerze. Sprawdź, czy tekst nie zlewa się w pionie.
- **Sugerowane rozwiązanie** · Utrzymuj długość linii w przedziale od 45 do 75 znaków. Ustaw interlinię (`line-height`) na około 150%–165% dla zwykłego tekstu, a dla dużych nagłówków zmniejsz do około 110%–120%.
- **Źródła** · [NN/g Text Scannability](https://www.nngroup.com/articles/how-little-do-users-read/)

## TXT-03 · Scannability & paragraphs (Skanowalność treści)

- **Dotyczy** · Artykuły, opisy oferty, sekcje O nas
- **Jak testować** · Rzuć okiem na stronę przez 5 sekund. Czy da się zrozumieć najważniejsze punkty bez czytania całego tekstu?
- **Sugerowane rozwiązanie** · Ludzie czytają według wzorca litery F (F-Shaped Pattern). Dziel długi tekst na krótkie akapity (maksymalnie 3–4 linijki), używaj śródtytułów, list punktowanych i pogrubiaj słowa kluczowe.
- **Źródła** · [NN/g F-Pattern](https://www.nngroup.com/articles/f-shaped-pattern-reading-web-content/)

## TXT-04 · Hanging prepositions (Wiszące spójniki)

- **Dotyczy** · Teksty w języku polskim
- **Jak testować** · Przejrzyj końce linijek w nagłówkach i akapitach.
- **Sugerowane rozwiązanie** · Nie zostawiaj pojedynczych małych liter (a, i, o, u, w, z) na końcu wiersza. Przenieś je do nowej linii za pomocą twardej spacji (`&nbsp;` lub `Shift + Enter`).
- **Źródła** · [PWN Typografia](https://sjp.pwn.pl/)

---

## A11Y-01 · Color contrast (Kontrast tekstu do tła)

- **Dotyczy** · Wszystkie teksty, etykiety, przyciski i ikony
- **Jak testować** · Użyj narzędzia WebAIM Contrast Checker lub wtyczki WAVE, aby zmierzyć współczynnik kontrastu.
- **Sugerowane rozwiązanie** · Współczynnik kontrastu tekstu do tła musi wynosić minimum 4.5:1 (poziom WCAG AA) dla zwykłego tekstu oraz minimum 3:1 dla dużych nagłówków. Unikaj jasnoszarego tekstu na jasnym tle.
- **Źródła** · [W3C WCAG 2.2](https://www.w3.org/WAI/WCAG21/Understanding/contrast-minimum.html), [WebAIM Checker](https://webaim.org/resources/contrastchecker/)

## A11Y-02 · Color independence (Informacja nie tylko kolorem)

- **Dotyczy** · Linki w tekście, stany błędów, wykresy
- **Jak testować** · Sprawdź stronę w skali szarości (symulacja daltonizmu).
- **Sugerowane rozwiązanie** · Kolor nie może być jedynym sposobem przekazania informacji. Linki wewnątrz tekstu powinny mieć podkreślenie, a komunikaty błędów w formularzu muszą mieć ikonkę ostrzegawczą i czytelny tekst.
- **Źródła** · [The A11Y Project](https://www.a11yproject.com/checklist/)

## A11Y-03 · Image alt text (Teksty alternatywne dla zdjęć)

- **Dotyczy** · Wszystkie znaczniki `<img>` na stronie
- **Jak testować** · Sprawdź w kodzie strony, czy obrazki posiadają atrybut `alt`.
- **Sugerowane rozwiązanie** · Każde zdjęcie, które przekazuje treść (np. produkt, schemat, zdjęcie lokalu), powinno mieć krótki i rzeczowy opis w `alt="..."`. Zdjęcia czysto dekoracyjne powinny mieć pusty atrybut `alt=""`.
- **Źródła** · [W3C Alt Text](https://www.w3.org/WAI/tutorials/images/)

## A11Y-04 · Keyboard navigation (Nawigacja klawiaturą)

- **Dotyczy** · Menu, linki, przyciski, formularze
- **Jak testować** · Przejdź przez całą stronę używając wyłącznie klawisza `Tab` (oraz `Enter` i `Spacja` do aktywacji).
- **Sugerowane rozwiązanie** · Każdy aktywny element musi mieć widoczną ramkę zaznaczenia (focus ring). Użytkownik nie może „utknąć” w żadnym elemencie strony.
- **Źródła** · [The A11Y Project](https://www.a11yproject.com/checklist/)

---

## PERF-01 · Modern image formats (Optymalizacja zdjęć)

- **Dotyczy** · Wszystkie pliki graficzne na stronie
- **Jak testować** · Sprawdź wagę plików w zakładce Network w narzędziach deweloperskich.
- **Sugerowane rozwiązanie** · Konwertuj pliki PNG i JPG do formatów WebP lub AVIF. Skompresuj grafiki tak, aby pojedyncze zdjęcie nie ważyło więcej niż 150–200 KB.
- **Źródła** · [Google Fast Web](https://web.dev/explore/fast), [Squoosh](https://squoosh.app/)

## PERF-02 · Lazy loading (Odłożone ładowanie)

- **Dotyczy** · Grafiki i ramki iframe poniżej pierwszego ekranu
- **Jak testować** · Odśwież stronę i sprawdź, czy zdjęcia z dolnych sekcji ładują się od razu, czy dopiero po przewinięciu.
- **Sugerowane rozwiązanie** · Dodaj atrybut `loading="lazy"` do zdjęć umieszczonych poniżej zgięcia strony (below the fold), aby przyspieszyć początkowe wczytywanie.
- **Źródła** · [web.dev Lazy Loading](https://web.dev/lazy-loading-images/)

## PERF-03 · Cumulative Layout Shift (Stabilność układu CLS)

- **Dotyczy** · Zdjęcia, banery, fonty webowe
- **Jak testować** · Otwórz stronę przy wolnym łączu i obserwuj, czy elementy nie „skaczą” w dół podczas wczytywania obrazków.
- **Sugerowane rozwiązanie** · Zawsze podawaj atrybuty `width` i `height` w kodzie HTML dla zdjęć i wideo. Używaj `font-display: swap` dla fontów internetowych.
- **Źródła** · [Google Web Vitals](https://web.dev/explore/fast)

---

## SEO-01 · Title & Meta Description (Tytuł i opis w Google)

- **Dotyczy** · Sekcja `<head>` każdej podstrony
- **Jak testować** · Użyj narzędzia do podglądu wyników Google (np. metatags.io) lub sprawdź kod źródłowy.
- **Sugerowane rozwiązanie** · Tytuł `<title>` powinien być unikalny, zawierać słowa kluczowe i mieć maksymalnie 55–60 znaków. Opis `<meta name="description">` powinien zachęcać do kliknięcia i mieć od 130 do 160 znaków.
- **Źródła** · [Google SEO Starter Guide](https://developers.google.com/search/docs/fundamentals/seo-starter-guide)

## SEO-02 · OpenGraph preview cards (Podgląd w social media)

- **Dotyczy** · Linki udostępniane na Facebooku, Messengerze, LinkedIn, Slacku
- **Jak testować** · Wklej link do strony w debugerze Facebook Sharing Debugger lub wyślij link na czacie.
- **Sugerowane rozwiązanie** · Ustaw tagi `og:title`, `og:description` oraz przygotuj grafikę `og:image` o wymiarach 1200 × 630 px, żeby link wyglądał profesjonalnie w mediach społecznościowych.
- **Źródła** · [Open Graph Protocol](https://ogp.me/)

## SEO-03 · Favicon & Touch Icon (Ikonka w zakładce)

- **Dotyczy** · Zakładka przeglądarki i skróty na telefonie
- **Jak testować** · Spójrz na kartę w przeglądarce i dodaj stronę do ekranu początkowego w smartfonie.
- **Sugerowane rozwiązanie** · Wgraj plik `favicon.ico` / `favicon.png` (32 × 32 px) oraz ikonę `apple-touch-icon.png` (180 × 180 px), aby strona nie wyświetlała domyślnego pustego symbolu.
- **Źródła** · [Webflow Launch QA](https://webflow.com/blog/website-launch-checklist)

---

## SEC-01 · SSL & HTTPS (Bezpieczne połączenie)

- **Dotyczy** · Cała domena serwisu
- **Jak testować** · Sprawdź pasek adresu przeglądarki — czy obok adresu wyświetla się symbol kłódki `https://`.
- **Sugerowane rozwiązanie** · Zainstaluj bezpłatny certyfikat SSL (np. Let's Encrypt) i ustaw automatyczne przekierowanie 301 z protokołu `http://` na `https://`.
- **Źródła** · [Google Web Security](https://developers.google.com/search/docs/fundamentals/seo-starter-guide)

## SEC-02 · Privacy policy & cookies (Polityka prywatności i ciasteczka)

- **Dotyczy** · Zgodność prawna (RODO / GDPR)
- **Jak testować** · Sprawdź, czy w stopce znajduje się link do Polityki Prywatności i czy przy pierwszej wizycie pojawia się informacja o plikach cookies.
- **Sugerowane rozwiązanie** · Jeśli na stronie działają skrypty śledzące (np. Google Analytics, Pixel Mety) lub formularz zbiera dane osobowe, dodaj podstronę Polityki Prywatności z danymi administratora oraz baner zgody na cookies.
- **Źródła** · [Smashing Magazine QA](https://www.smashingmagazine.com/2021/03/complete-website-launch-checklist/)
