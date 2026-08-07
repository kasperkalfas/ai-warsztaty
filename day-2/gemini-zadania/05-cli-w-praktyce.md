# Zadanie 5: Gemini CLI w praktyce

**Cel:** wykorzystać Gemini CLI do realnego zadania na plikach – analizy
zawartości folderu i wygenerowania nowego pliku – oraz poznać tryb, w
którym CLI proponuje zmiany do zatwierdzenia.
**Poziom:** średniozaawansowany

## Materiały

Działające Gemini CLI z [zadania 4](04-cli-instalacja.md).

## Kroki

1. W terminalu przejdź do folderu z materiałami z zadań NotebookLM, np.
   `notebooklm-zadania/materialy/` (albo dowolnego innego folderu z
   dokumentami, do którego masz dostęp).
2. Poproś Gemini CLI o podsumowanie zawartości jednego z plików:

   > Podsumuj w 5 punktach, o czym jest plik
   > 01-zdrowy-tryb-zycia.pdf.

3. Poproś o wygenerowanie nowego pliku na podstawie rozmowy, np.:

   > Na podstawie tego pliku stwórz krótką checklistę (max. 8 punktów) i
   > zapisz ją jako nowy plik checklista.md w tym folderze.

   Zanim Gemini CLI zapisze lub zmieni plik, zwykle poprosi o
   potwierdzenie – przeczytaj proponowaną zmianę przed zaakceptowaniem.

4. Sprawdź, czy plik rzeczywiście powstał (np. poleceniem `dir` w
   PowerShell) i otwórz go, żeby ocenić jakość wyniku.
5. Jeśli masz czas, sprawdź polecenie pomocy w CLI (zwykle `/help` albo
   `--help`), żeby zobaczyć inne dostępne opcje i tryby pracy.

## Na co zwrócić uwagę

- **Zawsze czytaj proponowane zmiany przed ich zaakceptowaniem** – CLI
  może tworzyć, nadpisywać i usuwać pliki, więc świadome zatwierdzanie
  każdej akcji jest kluczowe, szczególnie w folderach z ważnymi danymi.
- To samo narzędzie (analiza plików + generowanie nowych na podstawie
  poleceń w naturalnym języku) można wykorzystać do wielu zadań
  biurowych: porządkowania notatek, tworzenia podsumowań ze spotkań,
  wstępnej analizy danych w plikach tekstowych czy CSV.
- Efektywność pracy z CLI rośnie z konkretnością poleceń – podobnie jak
  przy formule P.K.Z.O. w Claude, im dokładniej opiszesz, czego
  oczekujesz (format, długość, nazwa pliku), tym mniej poprawek będzie
  potrzebnych.

## Notatki własne

- Jaki wynik uzyskałeś/aś i czy wymagał poprawek?
- Do jakiego zadania w swojej pracy mógłbyś/mogłabyś wykorzystać CLI do
  pracy na plikach?
