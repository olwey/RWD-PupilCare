# ZASADY PROJEKTU (wklej na początku każdej rozmowy z AI)

Pracujesz nad istniejącym serwisem statycznym. Te zasady są stałe. Nie zmieniaj ich, nawet jeśli uważasz, że coś byłoby lepsze. Jeśli zadanie wymaga złamania zasady, napisz to i zapytaj, zamiast zmieniać.

## Marka (z karty projektu, ZMIEŃ na swoje)
- Nazwa: Nazwa marki
- Kolory: primary #1d3557, secondary #457b9d, CTA #b5172b, tekst #222222
- Kroje: nagłówki "Lora", tekst "Inter" (Google Fonts)
- Język treści: polski. Ton: (np. rzeczowy, przyjazny)

## Technologia
1. HTML + CSS + Bootstrap 5.3.3 z CDN jsDelivr (CSS w <head>, bootstrap.bundle.min.js przed </body>). Żadnych innych frameworków CSS (bez Tailwinda, Bulmy itp.) i bez kroków budowania (npm, Vite, React).
2. Układ wyłącznie siatką Bootstrapa: container → row → col-*. Komponenty Bootstrapa (navbar, card, breadcrumb, pagination, form-control, table) zamiast pisania ich od zera.
3. Jeden plik własnych stylów: style.css. Nie twórz nowych plików CSS, nie dodawaj bloków <style> ani atrybutów style="".
4. Kolory marki i kroje tylko przez zmienne z sekcji :root w style.css. Poza :root wolno użyć tylko białego (#fff) i czarnego (#000).
5. Menu (<nav>) i stopka (<footer>) są identyczne na każdej stronie. Zmiana w menu = ta sama zmiana na wszystkich stronach. Na każdej stronie zmienia się tylko klasa active.
6. Nazwy plików są stałe: index.html, blog.html, single.html, sklep.html, produkt.html, koszyk.html, zamowienie.html, konto.html, kontakt.html, polityka-prywatnosci.html, 404.html.

## Wymagania na każdej stronie
- <meta name="viewport" content="width=device-width, initial-scale=1">, własny <title> i <meta name="description">, og:title, og:description, og:image.
- Blok JSON-LD schema.org (index: Organization lub podtyp; single: Article; produkt: Product).
- header, nav, main, footer; dokładnie jeden h1; każdy <img> z opisowym alt; każde pole formularza z <label for>.
- Przyciski i linki menu min. 44 × 44 px (reguły w sekcji 3 style.css zostają). Kontrast tekstu min. 4.5:1.
- Brak przewijania w bok przy 360, 768 i 1280 px. Linki tylko do istniejących plików, bez href="#".

## Jak odpowiadasz
Pokazuj tylko zmieniane fragmenty i nazwę pliku. Przy każdej zmianie napisz, której zasady dotyczy.
