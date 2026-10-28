# Podolog CitiMedic · strona internetowa

Strona gabinetów podologicznych **Podolog CitiMedic** w Gdańsku (ul. dr. Władysława Biegańskiego 10/7) i w Straszynie (ul. Starogardzka 42, lok. 8, C.H. Kremer).

Podgląd: **https://thepadi.github.io/CITIMEDIC-Podologia/**

## Co jest na stronie

- Przełącznik gabinetu Gdańsk / Straszyn. Telefon, adres, godziny i link do rezerwacji zmieniają się na całej stronie.
- Rysunek stopy z góry, podeszwy i dłoni z numerami. Kliknięcie numeru albo pozycji z listy pokazuje opis problemu i pasujące zabiegi z cenami.
- Cennik według kategorii, zespół, gabinet i sterylizacja, opinie, pytania i odpowiedzi, kontakt z mapą.
- Na telefonie dolny pasek „Zadzwoń” i „Umów”.

## Struktura

```
index.html   cała strona (HTML, CSS i JS w jednym pliku)
img/         zdjęcia gabinetu i zespołu, logo, favicon, obrazek podglądu linku
.nojekyll    wyłącza przetwarzanie Jekyll na GitHub Pages
```

Strona nie wymaga instalacji ani budowania.

## Dane

| Element | Wartość |
|---|---|
| Telefon Gdańsk | 695 082 381 |
| Telefon Straszyn | 727 169 899 |
| Rezerwacja Gdańsk | https://booksy.com/pl-pl/134942_podolog-citimedic-hanna-grebla-gdansk_podologia_20383_gdansk |
| Rezerwacja Straszyn | https://booksy.com/pl-pl/286056_podolog-citimedic-straszyn_podologia_20102_pomorskie |
| ZnanyLekarz | https://www.znanylekarz.pl/placowki/podologia-citimedic |

Ceny są w skrypcie w `index.html`, w obiekcie `PRICES`. Dane gabinetów (telefon, adres, godziny) są w obiekcie `LOC`.

## Przed przeniesieniem na własną domenę

1. Usunąć z `<head>` linię `<meta name="robots" content="noindex, nofollow">`.
2. Zmienić adresy `og:url` i `og:image` na docelową domenę.
3. Dodać plik `CNAME` z domeną i ustawić rekordy DNS.
