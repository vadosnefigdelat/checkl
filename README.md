# Web UI/UX Knowledge Base

Baza wiedzy i ustrukturyzowany checklist audytu stron internetowych przed publikacją. Każdy punkt posiada stały identyfikator (ID), metodę testowania, rekomendowane rozwiązanie oraz bezpośrednie odnośniki do oficjalnych źródeł branżowych.

## Jak przeprowadzić audyt strony

1. Otwórz stronę na komputerze oraz na rzeczywistym telefonie (lub w narzędziach deweloperskich przeglądarki).
2. Przejdź przez kolejne działy bazy wiedzy według tabeli poniżej.
3. Dla każdego punktu sprawdź stan na stronie:
   - **Zgodne (Pass)** — element spełnia kryteria.
   - **Niezgodne (Fail)** — element wymaga poprawy według sekcji *Sugerowane rozwiązanie*.
   - **Nie dotyczy (N/A)** — strona nie posiada danego elementu (np. brak formularza).
4. Po wdrożeniu poprawek powtórz testy na tym samym urządzeniu.

---

## Checklist według działów (Checklist by topic)

| Dział tematyczny | Ścieżka do listy | Liczba punktów |
| :--- | :--- | :---: |
| **01. Doświadczenie użytkownika (UX)** | [01-ux/checklist.md](01-ux/checklist.md) | 5 |
| **02. Interfejs i responsywność (UI & Mobile)** | [02-ui-responsive/checklist.md](02-ui-responsive/checklist.md) | 4 |
| **03. Typografia i czytelność tekstu** | [03-typography/checklist.md](03-typography/checklist.md) | 5 |
| **04. Dostępność cyfrowa (WCAG 2.2)** | [04-accessibility/checklist.md](04-accessibility/checklist.md) | 4 |
| **05. Wydajność, SEO i Bezpieczeństwo** | [05-performance-seo/checklist.md](05-performance-seo/checklist.md) | 7 |
| **06. Wykaz oficjalnych źródeł** | [06-sources/sources.md](06-sources/sources.md) | 11 |

---

## Szybki przegląd (Quick review)

Jeśli masz tylko 5 minut przed oddaniem projektu, sprawdź te najważniejsze punkty krytyczne:

1. **WEB-01** — Czy przyciski na telefonie mają minimum 44 × 44 px i nie są zbyt blisko siebie?
2. **WEB-02** — Czy strona na telefonie nie przesuwa się w prawo i w lewo?
3. **UX-01** — Czy po kliknięciu „Wyślij” w formularzu widać potwierdzenie lub animację ładowania?
4. **TXT-01** — Czy na stronie nie ma więcej niż 2 różnych fontów i czy usunięto wszystkie teksty *Lorem ipsum*?
5. **A11Y-01** — Czy tekst jest mocno kontrastowy względem tła (minimum 4.5:1)?
6. **PERF-01** — Czy zdjęcia są skompresowane i nie ważą po kilka megabajtów?
7. **SEC-01** — Czy strona ma aktywny certyfikat SSL (kłódka `https://`)?

---

## Oficjalne źródła (Sources overview)

Projekt bazuje wyłącznie na powszechnie uznanych standardach branżowych:
- **Nielsen Norman Group (NN/g)** — [Heurystyki ergonomii i użyteczności](06-sources/sources.md)
- **Webflow** — [Wytyczne techniczne przed wdrożeniem](06-sources/sources.md)
- **Smashing Magazine** — [Kompletna kontrola jakości stron www](06-sources/sources.md)
- **W3C / Web Accessibility Initiative** — [Wytyczne dostępności WCAG 2.2](06-sources/sources.md)
- **Google Developers** — [Wskaźniki Core Web Vitals i SEO](06-sources/sources.md)
- **Apple Human Interface Guidelines** — [Standardy stref dotykowych](06-sources/sources.md)

---

### 💡 Prosty trik na koniec: „Test zmrużonych oczu” (*Squint Test*)
Odsuń się od monitora na krok i mocno zmruż oczy, aby obraz się rozmył:
1. Czy od razu widzisz 2–3 najważniejsze elementy na ekranie?
2. Jeśli wszystko zlewa się w jedną szarą plamę — dodaj więcej pustej przestrzeni (white space) i wzmocnij kontrast kluczowych przycisków!
