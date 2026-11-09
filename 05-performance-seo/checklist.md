# Performance, SEO & Security

[Start here](../README.md) · [Source register](../06-sources/sources.md)

## PERF-01 · Modern image formats

- **Dotyczy** · Wszystkie pliki graficzne na stronie
- **Jak testować** · Sprawdź wagę plików w zakładce Network w narzędziach deweloperskich.
- **Sugerowane rozwiązanie** · Konwertuj pliki PNG i JPG do formatów WebP lub AVIF. Skompresuj grafiki tak, aby pojedyncze zdjęcie nie ważyło więcej niż 150–200 KB.
- **Źródła** · [Google Fast Web](https://web.dev/explore/fast), [Squoosh](https://squoosh.app/)

## PERF-02 · Lazy loading

- **Dotyczy** · Grafiki i ramki iframe poniżej pierwszego ekranu
- **Jak testować** · Odśwież stronę i sprawdź, czy zdjęcia z dolnych sekcji ładują się od razu, czy dopiero po przewinięciu.
- **Sugerowane rozwiązanie** · Dodaj atrybut `loading="lazy"` do zdjęć umieszczonych poniżej zgięcia strony (below the fold), aby przyspieszyć początkowe wczytywanie.
- **Źródła** · [web.dev Lazy Loading](https://web.dev/lazy-loading-images/)

## PERF-03 · Cumulative Layout Shift (CLS)

- **Dotyczy** · Zdjęcia, banery, fonty webowe
- **Jak testować** · Otwórz stronę przy wolnym łączu i obserwuj, czy elementy nie „skaczą” w dół podczas wczytywania obrazków.
- **Sugerowane rozwiązanie** · Zawsze podawaj atrybuty `width` i `height` w kodzie HTML dla zdjęć i wideo. Używaj `font-display: swap` dla fontów internetowych.
- **Źródła** · [Google Web Vitals](https://web.dev/explore/fast)

## SEO-01 · Title & Meta Description

- **Dotyczy** · Sekcja `<head>` każdej podstrony
- **Jak testować** · Użyj narzędzia do podglądu wyników Google (np. metatags.io) lub sprawdź kod źródłowy.
- **Sugerowane rozwiązanie** · Tytuł `<title>` powinien być unikalny, zawierać słowa kluczowe i mieć maksymalnie 55–60 znaków. Opis `<meta name="description">` powinien zachęcać do kliknięcia i mieć od 130 do 160 znaków.
- **Źródła** · [Google SEO Starter Guide](https://developers.google.com/search/docs/fundamentals/seo-starter-guide)

## SEO-02 · OpenGraph preview cards

- **Dotyczy** · Linki udostępniane na Facebooku, Messengerze, LinkedIn, Slacku
- **Jak testować** · Wklej link do strony w debugerze Facebook Sharing Debugger lub wyślij link na czacie.
- **Sugerowane rozwiązanie** · Ustaw tagi `og:title`, `og:description` oraz przygotuj grafikę `og:image` o wymiarach 1200 × 630 px, żeby link wyglądał profesjonalnie w mediach społecznościowych.
- **Źródła** · [Open Graph Protocol](https://ogp.me/)

## SEC-01 · SSL & HTTPS

- **Dotyczy** · Cała domena serwisu
- **Jak testować** · Sprawdź pasek adresu przeglądarki — czy obok adresu wyświetla się symbol kłódki `https://`.
- **Sugerowane rozwiązanie** · Zainstaluj bezpłatny certyfikat SSL (np. Let's Encrypt) i ustaw automatyczne przekierowanie 301 z protokołu `http://` na `https://`.
- **Źródła** · [Google Web Security](https://developers.google.com/search/docs/fundamentals/seo-starter-guide)

## SEC-02 · Privacy policy & cookies

- **Dotyczy** · Zgodność prawna (RODO / GDPR)
- **Jak testować** · Sprawdź, czy w stopce znajduje się link do Polityki Prywatności i czy przy pierwszej wizycie pojawia się informacja o plikach cookies.
- **Sugerowane rozwiązanie** · Jeśli na stronie działają skrypty śledzące (np. Google Analytics, Pixel Mety) lub formularz zbiera dane osobowe, dodaj podstronę Polityki Prywatności z danymi administratora oraz baner zgody na cookies.
- **Źródła** · [Smashing Magazine QA](https://www.smashingmagazine.com/2021/03/complete-website-launch-checklist/)
