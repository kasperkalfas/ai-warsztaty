# Zadanie 6: Gemini CLI – podstawowa strona HTML

**Cel:** wykorzystać Gemini CLI do wygenerowania prostej strony
internetowej (HTML + CSS) i otworzyć ją w przeglądarce – pierwszy kontakt
z tworzeniem stron z pomocą AI.
**Poziom:** podstawowy / średniozaawansowany

## Materiały

Działające Gemini CLI z [zadania 4](04-cli-instalacja.md).

## Kroki

1. Utwórz nowy, pusty folder na stronę i przejdź do niego:

   ```
   mkdir moja-strona
   cd moja-strona
   ```

2. Uruchom w nim Gemini CLI (`gemini`) i poproś o wygenerowanie prostej
   strony wizytówkowej, np.:

   > Stwórz plik index.html z prostą stroną wizytówką: nagłówek z moim
   > imieniem, krótki akapit "o mnie" i sekcja kontakt. Użyj prostego,
   > czytelnego stylu CSS w tym samym pliku.

3. Zaakceptuj propozycję zapisania pliku, gdy CLI o to poprosi.
4. Otwórz plik `index.html` w przeglądarce – w Eksploratorze plików
   kliknij go dwukrotnie, albo w terminalu (PowerShell) wpisz:

   ```
   start index.html
   ```

5. Poproś Gemini CLI o jedną zmianę w stronie, np. inny kolor tła albo
   dodanie ikony/emoji, i odśwież stronę w przeglądarce (F5), żeby
   zobaczyć efekt.
6. **(Opcjonalnie)** Poproś o dodanie kolejnej sekcji, np. listy
   umiejętności albo linków do mediów społecznościowych.

## Na co zwrócić uwagę

- To pierwszy kontakt z tworzeniem stron internetowych z pomocą AI –
  szerzej temat programowania (w tym HTML) wraca w **Dniu 5** programu
  ("Podstawy Programowania: Python, HTML, SQL, Hosting").
- Zanim poprosisz o większą zmianę, warto zerknąć na zawartość
  wygenerowanego pliku (np. poleceniem `type index.html` w PowerShell) –
  to dobry nawyk przy każdej pracy z kodem generowanym przez AI, nie
  tylko w tym ćwiczeniu.
- Jeśli efekt zmiany Cię nie zadowala, możesz po prostu poprosić Gemini
  CLI o cofnięcie ostatniej zmiany albo opisać, co dokładnie chcesz
  poprawić – nie musisz pisać kodu ręcznie.
- Gotową stronę można później umieścić w internecie (hosting) – ten temat
  również pojawi się w Dniu 5.

## Notatki własne

- Jak wyglądała Twoja pierwsza strona HTML wygenerowana przez Gemini CLI?
- Jaką jedną zmianę udało Ci się wprowadzić poleceniem w naturalnym
  języku?
