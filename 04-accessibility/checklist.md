# Accessibility & WCAG 2.2

[Start here](../README.md) · [Source register](../06-sources/sources.md)

## A11Y-01 · Color contrast

- **Dotyczy** · Wszystkie teksty, etykiety, przyciski i ikony
- **Jak testować** · Użyj narzędzia WebAIM Contrast Checker lub wtyczki WAVE, aby zmierzyć współczynnik kontrastu.
- **Sugerowane rozwiązanie** · Współczynnik kontrastu tekstu do tła musi wynosić minimum 4.5:1 (poziom WCAG AA) dla zwykłego tekstu oraz minimum 3:1 dla dużych nagłówków. Unikaj jasnoszarego tekstu na jasnym tle.
- **Źródła** · [W3C WCAG 2.2](https://www.w3.org/WAI/WCAG21/Understanding/contrast-minimum.html), [WebAIM Checker](https://webaim.org/resources/contrastchecker/)

## A11Y-02 · Color independence

- **Dotyczy** · Linki w tekście, stany błędów, wykresy
- **Jak testować** · Sprawdź stronę w skali szarości (symulacja daltonizmu).
- **Sugerowane rozwiązanie** · Kolor nie może być jedynym sposobem przekazania informacji. Linki wewnątrz tekstu powinny mieć podkreślenie, a komunikaty błędów w formularzu muszą mieć ikonkę ostrzegawczą i czytelny tekst.
- **Źródła** · [The A11Y Project](https://www.a11yproject.com/checklist/)

## A11Y-03 · Image alt text

- **Dotyczy** · Wszystkie znaczniki `<img>` na stronie
- **Jak testować** · Sprawdź w kodzie strony, czy obrazki posiadają atrybut `alt`.
- **Sugerowane rozwiązanie** · Każde zdjęcie, które przekazuje treść (np. produkt, schemat, zdjęcie lokalu), powinno mieć krótki i rzeczowy opis w `alt="..."`. Zdjęcia czysto dekoracyjne powinny mieć pusty atrybut `alt=""`.
- **Źródła** · [W3C Alt Text](https://www.w3.org/WAI/tutorials/images/)

## A11Y-04 · Keyboard navigation

- **Dotyczy** · Menu, linki, przyciski, formularze
- **Jak testować** · Przejdź przez całą stronę używając wyłącznie klawisza `Tab` (oraz `Enter` i `Spacja` do aktywacji).
- **Sugerowane rozwiązanie** · Każdy aktywny element musi mieć widoczną ramkę zaznaczenia (focus ring). Użytkownik nie może „utknąć” w żadnym elemencie strony.
- **Źródła** · [The A11Y Project](https://www.a11yproject.com/checklist/)
