# UI & Responsive web

[Start here](../README.md) · [Source register](../06-sources/sources.md)

## WEB-01 · Touch targets

- **Dotyczy** · Urządzenia mobilne, responsywny web
- **Jak testować** · Zmierz rzeczywiste pole klikalne przycisków, ikon i linków na telefonie. Sprawdź, czy nie są zbyt blisko siebie.
- **Sugerowane rozwiązanie** · Zadbaj o minimum 44 × 44 pt (standard Apple) lub 48 × 48 dp (standard Google). Zwiększ padding wokół przycisków i dodaj minimum 8 px odstępu między linkami.
- **Źródła** · [Apple HIG](https://developer.apple.com/design/human-interface-guidelines/), [Google web.dev](https://web.dev/accessible-tap-targets/)

## WEB-02 · Horizontal overflow

- **Dotyczy** · Widok mobilny i tablet
- **Jak testować** · Otwórz stronę w narzędziach deweloperskich przeglądarki na szerokościach 375 px, 390 px i 414 px. Spróbuj przesunąć stronę w lewo i w prawo.
- **Sugerowane rozwiązanie** · Strona nie może przesuwać się w poziomie. Sprawdź elementy ze sztywną szerokością (np. `width: 500px`), za duże zdjęcia lub za duże marginesy i zamień je na wartości procentowe lub `max-width: 100%`.
- **Źródła** · [Webflow Responsive](https://university.webflow.com/lesson/intro-to-responsive-design)

## WEB-03 · Headings scale

- **Dotyczy** · Smartfony (ekrany poniżej 480 px)
- **Jak testować** · Zobacz, jak duży nagłówek H1 z komputera wygląda na małym ekranie telefonu.
- **Sugerowane rozwiązanie** · Zmniejsz wielkość liter na małym ekranie (np. z 48 px do 28–32 px). Unikaj sytuacji, w której jedno słowo łamie się w połowie lub zajmuje cały ekran.
- **Źródła** · [Smashing Magazine](https://www.smashingmagazine.com/2021/03/complete-website-launch-checklist/)

## WEB-04 · Mobile navigation

- **Dotyczy** · Menu hamburger na telefonie
- **Jak testować** · Otwórz menu, kliknij w link do sekcji i zobacz, czy menu samo się zamyka oraz czy da się je łatwo zamknąć krzyżykiem lub kliknięciem w tło.
- **Sugerowane rozwiązanie** · Menu po kliknięciu w link powinno przenieść użytkownika do sekcji i automatycznie się schować, żeby nie zasłaniało treści.
- **Źródła** · [NN/g Mobile Navigation](https://www.nngroup.com/articles/hamburger-menus/)
