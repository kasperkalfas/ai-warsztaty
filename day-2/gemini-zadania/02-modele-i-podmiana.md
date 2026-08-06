# Zadanie 2: Modele Gemini i przełączanie między nimi

**Cel:** zrozumieć, że Gemini oferuje kilka modeli o różnej szybkości i
"głębi" myślenia, oraz nauczyć się świadomie przełączać między nimi
zależnie od zadania.
**Poziom:** podstawowy / średniozaawansowany

## Materiały

Konto Gemini z [zadania 1](01-pierwsza-rozmowa.md).

## Kroki

1. Znajdź selektor modelu w interfejsie Gemini – zwykle w górnej części
   ekranu, obok nazwy aplikacji, albo w ustawieniach rozmowy. Nazewnictwo
   bywa zmieniane przez Google, ale zazwyczaj znajdziesz co najmniej dwie
   opcje: wariant **szybszy** (np. "Flash") i wariant **dokładniejszy /
   z rozumowaniem** (np. "Pro" lub "Thinking").
2. Ustaw model szybszy i zadaj proste pytanie faktograficzne, np.
   *"Jaka jest stolica Australii?"*. Zwróć uwagę na czas odpowiedzi.
3. Przełącz na model dokładniejszy/z rozumowaniem i zadaj pytanie
   wymagające wieloetapowego rozumowania, np.:
   *"Mam 3 osoby: Anna jest starsza od Basi, Basia jest starsza od Celiny.
   Kto jest najmłodszy i skąd to wiadomo?"* albo zagadkę logiczną
   dotyczącą planowania budżetu czy harmonogramu.
4. Zadaj **to samo** pytanie z kroku 3 na modelu szybszym i porównaj obie
   odpowiedzi – jakość rozumowania, ewentualne błędy, długość odpowiedzi.
5. Sprawdź, czy w trakcie jednej rozmowy można zmienić model bez utraty
   kontekstu (Gemini pamięta wcześniejsze wiadomości nawet po zmianie
   modelu).

## Na co zwrócić uwagę

- **Szybszy model** (np. Flash) sprawdza się do prostych, codziennych
  zadań: krótkich pytań, streszczeń, szybkich szkiców tekstu – odpowiada
  niemal natychmiast.
- **Wolniejszy model z rozumowaniem** (np. Pro/Thinking) lepiej radzi sobie
  z zadaniami wymagającymi analizy, planowania lub wieloetapowej logiki –
  kosztem dłuższego czasu odpowiedzi i (w planach płatnych) wyższego
  zużycia limitu.
- Dobór modelu do zadania to ważna umiejętność praktyczna – używanie
  najmocniejszego modelu do każdego, nawet najprostszego pytania,
  niepotrzebnie wydłuża czekanie i szybciej zużywa dzienny limit
  darmowego planu.
- Ta sama zasada (różne modele do różnych zadań) obowiązuje też w innych
  narzędziach AI, np. w Claude czy w Gemini CLI (zadanie 4) – warto
  zapamiętać ją jako ogólną regułę, nie tylko dla Gemini.

## Notatki własne

- Przy jakich swoich zadaniach wybrałbyś/wybrałabyś szybszy model, a przy
  jakich – wolniejszy?
- Czy zauważyłeś/aś różnicę w jakości odpowiedzi na pytanie logiczne
  między oboma modelami?
