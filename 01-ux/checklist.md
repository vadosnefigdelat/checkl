# UX and usability

[Start here](../README.md) · [Source register](../06-sources/sources.md)

## UX-01 · System status & feedback

- **Dotyczy** · Formularze, przyciski akcji, ładowanie danych
- **Jak testować** · Wypełnij formularz na stronie i kliknij wyślij. Zobacz, czy strona od razu daje znać, że coś się dzieje.
- **Sugerowane rozwiązanie** · Zastosuj pierwszą heurystykę Nielsena (Visibility of System Status). Pokaż animację ładowania (spinner) na przycisku podczas wysyłania, a po zakończeniu wyświetl wyraźny komunikat z podziękowaniem.
- **Źródła** · [NN/g](https://www.nngroup.com/articles/ten-usability-heuristics/)

## UX-02 · User freedom & modals

- **Dotyczy** · Okienka pop-up, banery, powiększone zdjęcia
- **Jak testować** · Otwórz okienko na stronie i spróbuj je zamknąć klawiszem Esc, kliknięciem w ciemne tło lub krzyżykiem.
- **Sugerowane rozwiązanie** · Użytkownik musi mieć pełną kontrolę (User Control and Freedom). Dodaj wyraźny przycisk zamknięcia `×` w prawym górnym rogu i pozwól zamknąć okno kliknięciem poza nim.
- **Źródła** · [NN/g](https://www.nngroup.com/articles/ten-usability-heuristics/)

## UX-03 · Error prevention & validation

- **Dotyczy** · Formularze kontaktowe i pola do wpisywania tekstu
- **Jak testować** · Wpisz błędny numer telefonu lub e-mail bez znaku `@` i spróbuj wysłać.
- **Sugerowane rozwiązanie** · Waliduj dane na bieżąco. Wyświetlaj krótką i pomocną podpowiedź pod polem (np. „Podaj poprawny adres e-mail, np. jan@domena.pl”), zamiast ogólnego napisu „Błąd”.
- **Źródła** · [NN/g](https://www.nngroup.com/articles/ten-usability-heuristics/), [Webflow](https://webflow.com/blog/website-launch-checklist)

## UX-04 · Custom 404 page

- **Dotyczy** · Nieistniejące podstrony
- **Jak testować** · Wpisz w przeglądarce adres strony z losowym ciągiem liter na końcu (np. `/nieistniejacy-adres`).
- **Sugerowane rozwiązanie** · Zamiast pustego systemowego błędu serwera przygotuj przyjazną stronę 404 z krótkim tekstem i dużym przyciskiem powrotu na stronę główną.
- **Źródła** · [Smashing Magazine](https://www.smashingmagazine.com/2021/03/complete-website-launch-checklist/)

## UX-05 · Consistency & standard placement

- **Dotyczy** · Globalna nawigacja i układ
- **Jak testować** · Sprawdź, czy logo, koszyk, wyszukiwarka i linki znajdują się w przewidywalnych miejscach.
- **Sugerowane rozwiązanie** · Logo w lewym górnym rogu zawsze prowadzi do strony głównej. Koszyk i profil znajdują się w prawym górnym rogu. Nie zmuszaj użytkownika do zgadywania.
- **Źródła** · [NN/g](https://www.nngroup.com/articles/ten-usability-heuristics/)
