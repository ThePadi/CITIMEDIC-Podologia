# Podolog CitiMedic · strona internetowa

Strona gabinetu podologicznego **Podolog CitiMedic** (Gdańsk, ul. dr. Władysława Biegańskiego 10/7 oraz Straszyn, ul. Starogardzka 42, C.H. Kremer).

Podgląd: **https://thepadi.github.io/CITIMEDIC-Podologia/**

## Co jest na stronie

- **Interaktywna stopa** (widok paznokci i podeszwy). Pacjent klika kropkę w miejscu problemu i widzi opis, objawy oraz zabiegi z cennikiem dobrane do tego problemu.
- **Cennik** 7 zabiegów z przyciskiem „Umów” prowadzącym do kalendarza na ZnanyLekarz.
- **O nas** i lista specjalizacji gabinetu.
- Sprzęt, zespół, zdjęcia gabinetu, dwa gabinety z mapami, pytania i odpowiedzi, opinie.
- Klikalne numery telefonów, link do ZnanyLekarz i Instagrama, pasek „Zadzwoń / Umów online” na telefonie.

## Struktura

```
index.html            cała strona (HTML, CSS i JS w jednym pliku)
assets/logo-white.svg logo na niebieskim tle
assets/logo-blue.svg  logo na jasnym tle
assets/favicon.svg    ikona karty przeglądarki
assets/og-image.png   obrazek podglądu linku (Messenger, WhatsApp, SMS)
```

Strona nie wymaga instalacji ani budowania. Wystarczy otworzyć `index.html` w przeglądarce.

## Dane na stronie

| Element | Wartość |
|---|---|
| Kolor marki | `#3A6FB3` |
| Telefon Gdańsk | 695 082 381 |
| Telefon Straszyn | 727 169 899 |
| Rezerwacja | https://www.znanylekarz.pl/placowki/podologia-citimedic |
| Instagram | https://www.instagram.com/podologcitimedic/ |

Ceny w `index.html` znajdują się w sekcji `PRICE LIST` oraz w obiekcie `SERVICES` w skrypcie (używanym przez interaktywną stopę). Przy zmianie ceny trzeba poprawić oba miejsca.

## Przed uruchomieniem na własnej domenie

1. Usunąć z `<head>` linię `<meta name="robots" content="noindex, nofollow">`, żeby Google mógł zaindeksować stronę.
2. Zdjęcia gabinetu są teraz ładowane z profilu ZnanyLekarz. Podmienić je na własne pliki w `assets/`.
3. Zaktualizować adresy `og:url` i `og:image` na docelową domenę.
4. Dodać plik `CNAME` z domeną i ustawić rekordy DNS.

Informacje medyczne na stronie mają charakter ogólny i nie zastępują konsultacji ze specjalistą.
