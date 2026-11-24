# Wikibox Studio

Samodzielny kreator infoboksów do alternatywnej historii. Przykładowe dane są fikcyjne. Nie wymaga instalacji, serwera, konta ani bibliotek zewnętrznych.

## Uruchomienie lokalne
Otwórz `index.html` w przeglądarce. Dostępne są szablony, edycja bloków, zdjęcia z dysku, PNG (1–4×), zapis i odczyt JSON oraz eksport tabeli w wikikodzie. Dane są lokalne. Automatyczny zapis podlega limitowi localStorage; większe projekty zapisuj jako JSON. Przeglądarki mogą ograniczać localStorage i schowek dla plików lokalnych; w takim przypadku użyj GitHub Pages, a kod wiki zostanie pobrany jako plik, jeśli kopiowanie nie będzie dostępne.

## Publikacja w GitHub Pages
1. Utwórz publiczne repozytorium `wikibox-builder` w GitHubie (https://github.com/new).
2. Wgraj `index.html`, `README.md` i `.nojekyll` do głównego katalogu repozytorium. Wystarczy również sam `index.html`.
3. Zatwierdź pliki (Commit changes).
4. Wejdź w Settings → Pages. Wybierz Deploy from a branch, gałąź main oraz /(root), a następnie Save.
5. GitHub wyświetli adres strony po wdrożeniu: `https://TWOJ-LOGIN.github.io/wikibox-builder/`.

Dokumentacja: https://docs.github.com/en/pages/quickstart

## Uwagi
- PNG powstaje lokalnie na canvasie. Wczytane obrazy są pomniejszane do maksymalnie 1000 px na dłuższym boku. GIF jest statyczny.
- Wikikod to ogólna tabela MediaWiki, a nie kod konkretnego szablonu Wikipedii. Obrazy trzeba osobno przesłać do docelowej wiki i podać ich nazwy. Wygląd może różnić się zależnie od CSS wiki.
- Porównanie kandydatów zawiera dwie kolumny; można dodawać kolejne bloki. Pola z separatorem ` | ` rozdzielają wyniki na dwie wartości.

## English Wikipedia edition 2.0
13 edytowalnych szablonów (w tym pusty), angielskie etykiety, oddzielny kolor tytułu, opcjonalne niebieskie wartości oraz pogrubienie tekstu. Wygląd bazuje na parametrach wizualnych enwiki i szablonach officeholder / Christian leader, lecz silnik Canvas jest autorski i nie wykonuje MediaWiki ani Lua. Nie jest gwarantowaną kopią piksel w piksel. Przykładowe treści są fikcyjne. Zapis v2 jest odseparowany od v1; wcześniejszy plik JSON można otworzyć ręcznie.

Wzorce:
- https://en.wikipedia.org/wiki/Module:Infobox/styles.css
- https://en.wikipedia.org/wiki/Template:Infobox_officeholder
- https://en.wikipedia.org/wiki/Template:Infobox_Christian_leader
