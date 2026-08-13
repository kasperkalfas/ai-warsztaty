# Zadanie 7: „CENTRUM KREATYWNOŚCI" – galeria stylów

**Cel:** każdy uczestnik tworzy grafikę z napisem **CENTRUM KREATYWNOŚCI**
w innym stylu – a następnie oglądamy wszystkie prace obok siebie i widzimy,
jak bardzo sam styl zmienia wymowę tego samego hasła.
**Poziom:** podstawowy (zadanie zespołowe, na zakończenie bloku)
**Budżet:** 1–2 kredyty AI na osobę

## Dlaczego akurat napis?

To zadanie celowo dotyka **najsłabszego miejsca generatorów grafiki**:
modele źle radzą sobie z tekstem na obrazie, a polskie znaki (**Ś**
w „KREATYWNOŚCI") psują wynik jeszcze częściej. Zamiast to omijać,
sprawdzimy to na własne oczy, a potem zrobimy to porządnie.

Kolejność jest częścią lekcji: **najpierw zobacz, jak AI sobie nie radzi,
potem naucz się obejścia.**

## Materiały

Zalogowany [Microsoft Designer](https://designer.microsoft.com) z
[zadania 1](01-konto-microsoft-i-pierwsza-grafika.md).

## Krok 1: Wybierz swój styl

Żeby galeria była ciekawa, **każda osoba bierze inny styl**. Rozlosujcie je
albo rozdzielcie po kolei:

| # | Styl | # | Styl |
|---|------|---|------|
| 1 | akwarela | 11 | vintage, plakat z lat 60. |
| 2 | ilustracja wektorowa, płaskie kolory | 12 | neon, ciemne tło |
| 3 | fotografia studyjna | 13 | kolaż z wyciętego papieru |
| 4 | szkic ołówkiem | 14 | witraż |
| 5 | grafika 3D, miękkie światło | 15 | mozaika |
| 6 | komiks, wyraźny kontur | 16 | haft / tkanina |
| 7 | minimalizm, dużo bieli | 17 | graffiti, mur miejski |
| 8 | art déco, złote zdobienia | 18 | origami, papierowe formy |
| 9 | pixel art | 19 | blueprint, rysunek techniczny |
| 10 | pastelowa kreda | 20 | druk sitodrukowy, 2 kolory |

## Krok 2: Spróbuj wygenerować napis (1 kredyt)

1. Wygeneruj obraz, prosząc **wprost o napis**, np.:

   `Plakat z dużym napisem "CENTRUM KREATYWNOŚCI", styl: akwarela,
   jasne tło, kadr kwadratowy`

   (wstaw swój styl zamiast „akwarela")

2. Przeczytaj uważnie, co model napisał. Najczęściej zobaczysz:
   przekręcone litery, brakujący ogonek przy **Ś**, powtórzone lub
   wymyślone znaki, czasem napis w ogóle nieczytelny.
3. **Nie generuj drugi raz w nadziei, że tym razem wyjdzie.** To nie kwestia
   szczęścia, tylko ograniczenia modelu – kolejne próby zużyją kredyty
   i skończą się podobnie.

## Dlaczego AI przekręca litery?

Warto to zrozumieć, bo wtedy przestaje dziwić:

- **Model maluje piksele, nie pisze liter.** Jak pokazywał film z
  [zadania 0](00-jak-dziala-generowanie-obrazow.md), obraz powstaje przez
  stopniowe "odszumianie" losowych pikseli. Model nie ma pojęcia "litera Ś" –
  ma tylko wyuczone wrażenie, **jak zwykle wygląda coś, co przypomina
  napis**. Rysuje więc kształty przypominające pismo, tak jak rysuje kształty
  przypominające drzewo. Dla drzewa "mniej więcej" wystarczy, dla liter nie –
  każdy najmniejszy błąd od razu widać.
- **Opis jest rozumiany jako całość, nie litera po literze.** Zanim model
  zacznie malować, Twój opis zostaje zamieniony na ogólne "znaczenie"
  (skompresowaną reprezentację). W tej kompresji dokładna kolejność znaków
  w napisie często się gubi – zostaje informacja "duży napis na plakacie",
  a nie precyzyjna sekwencja C-E-N-T-R-U-M.
- **Napis to jedno – ale poprawny napis to zupełnie co innego.** W milionach
  obrazów treningowych model widział mnóstwo plakatów i szyldów, ale uczył
  się ich wyglądu, nie ortografii. Dlatego wynik wygląda "jak napis"
  z daleka, a z bliska rozpada się na wymyślone znaki.
- **Polskie znaki mają najgorzej.** Ogonki i kreski (ą, ć, ś, ż) występują
  w danych treningowych wielokrotnie rzadziej niż tekst angielski, więc
  model "widział" ich za mało, by je pewnie odtworzyć. Stąd **Ś** gubiące
  kreskę częściej niż litery łacińskie.

Nowsze modele radzą sobie z krótkimi angielskimi napisami coraz lepiej, ale
zasada pozostaje: **generator to malarz, nie maszyna do pisania** – dlatego
tekst nakładamy polem tekstowym, co zrobimy w następnym kroku.

## Krok 3: Zrób to porządnie (0–1 kredytów)

4. Wygeneruj (lub wykorzystaj obraz z kroku 2 albo z
   [zadania 2](02-jak-pisac-opisy-obrazow.md)) **tło bez tekstu** w swoim
   stylu – dopisz do opisu `bez tekstu, bez napisów`.
5. Przejdź do edytora projektu i **dodaj napis jako pole tekstowe** –
   tak jak w [zadaniu 3](03-plakat-z-szablonu.md). Wpisz:
   **CENTRUM KREATYWNOŚCI**.
6. Dobierz krój i kolor liter tak, żeby pasowały do stylu tła, ale
   pozostały czytelne. Sprawdź, czy **Ś** wyświetla się poprawnie – część
   krojów dekoracyjnych nie zawiera polskich znaków i podmienia je na
   „S" albo puste pole.
7. Pobierz gotowy plik jako PNG.

## Krok 4: Galeria

8. Pokażcie wszystkie prace obok siebie – na rzutniku, we wspólnym folderze
   albo wydrukowane i rozłożone na stole.
9. Omówcie wspólnie:
   - Który styl najlepiej pasuje do hasła „Centrum Kreatywności" i dlaczego?
   - Który napis jest czytelny z odległości, a który ginie na tle?
   - Czy dałoby się rozpoznać, że to ta sama nazwa, gdyby nie było podpisu?

## Na co zwrócić uwagę

- **Tekst dodawaj zawsze jako pole tekstowe, nie przez generowanie.** To
  najważniejszy wniosek z tego zadania i zasada, która oszczędzi Wam
  najwięcej kredytów i nerwów w przyszłości.
- Polskie znaki diakrytyczne (ą, ć, ę, ł, ń, ó, ś, ź, ż) to częsty problem –
  zarówno w generowaniu obrazu, jak i w krojach ozdobnych w edytorze.
  Zawsze sprawdzaj napis po podmianie czcionki.
- Ten sam napis w dwudziestu stylach to gotowa lekcja o tym, że **styl
  niesie znaczenie**: pixel art mówi co innego niż witraż, choć słowa są
  identyczne. To bezpośrednio przygotowuje do Dnia 3 („Grafika AI
  i Wystąpienia Publiczne").
- Jeśli materiał miałby trafić do publikacji, wróć do
  [zadania 6](06-prawa-i-oznaczanie-tresci-ai.md) – oznaczanie treści
  wygenerowanych przez AI obowiązuje także grafiki z napisem.

## Notatki własne

- Jak model poradził sobie z napisem w kroku 2? Zapisz, co dokładnie
  przekręcił:
- Który styl z galerii wybrał(a)byś na materiały swojej organizacji?
- Czy Twój krój pisma poprawnie pokazał literę **Ś**?
