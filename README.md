# Nasz Dom — PWA na GitHub Pages

## Publikacja

1. Rozpakuj ZIP.
2. W repozytorium GitHub `nasz-dom` **zastąp** dotychczasowy plik `index.html` nowym.
3. Wgraj także `manifest.webmanifest`, `sw.js` oraz cały folder `icons` (z zachowaniem struktury katalogów).
4. Zatwierdź zmiany (Commit changes). GitHub Pages powinien wdrożyć je automatycznie.
5. Otwórz stronę w **Chrome** na Xiaomi, najlepiej po odświeżeniu strony. Z menu ⋮ wybierz **Dodaj do ekranu głównego** / **Zainstaluj aplikację**.
6. Jeśli wcześniej był na ekranie zwykły skrót, usuń go i zainstaluj ponownie.

## Ważne

- Używaj HTTPS GitHub Pages. Otwarcie pliku `index.html` z dysku (file://) nie uruchomi PWA.
- Aplikacja ma ikonę i tryb `standalone`; Chrome może wyświetlić przycisk instalacji albo opcję dodania skrótu zależnie od wersji przeglądarki.
- Service worker zapisuje w pamięci podręcznej tylko pliki interfejsu; danych z Supabase **nie** przechowuje offline. Logowanie i aktualizacja wpisów wymagają internetu.
- Po kolejnych aktualizacjach aplikacji zwiększ wersję `CACHE_NAME` w `sw.js`, jeżeli zmienisz zasoby statyczne.
- Jeżeli Chrome uparcie pokazuje starą wersję, zamknij aplikację, odśwież stronę w Chrome lub usuń stare dane witryny (uwaga: wyloguje to z aplikacji).
- Nie przesyłaj na GitHub kluczy `service_role`, haseł ani innych sekretów.
