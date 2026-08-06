# Zadanie 5: Google Drive – praca z własnymi dokumentami

**Cel:** podłączyć Dysk Google, przeanalizować własne dokumenty i zapisać
wynik pracy Claude z powrotem na Dysku.
**Poziom:** średniozaawansowany

## Materiały

- Konto Claude z podłączonym kontem Google (zob.
  [zadanie 3](03-connections-gmail.md)).
- Kilka dokumentów na Dysku Google. Jeśli nie masz własnych, wgraj na Dysk
  materiały o zdrowiu i ergonomii z folderu
  [`materialy/`](../notebooklm-zadania/materialy/).

## Kroki

1. Podłącz **Google Drive** w menu **"Search and tools" → "Add
   connectors"**.
2. Zacznij od wyszukiwania:
   *"Znajdź na moim Dysku dokumenty dotyczące ergonomii i wypisz ich nazwy
   wraz z datą modyfikacji."*
3. Poproś o analizę konkretnego pliku:
   *"Przeczytaj dokument [nazwa] i wypisz 5 najważniejszych wniosków."*
4. Zleć zadanie łączące dokumenty – prompt P.K.Z.O.:

   > **P:** Jesteś specjalistą przygotowującym materiały szkoleniowe.
   > **K:** Mam na Dysku kilka dokumentów o zdrowiu i ergonomii pracy.
   > **Z:** Przygotuj na ich podstawie jednostronicowe podsumowanie dla
   > osoby, która nie czytała żadnego z tych dokumentów.
   > **O:** Maksymalnie 400 słów, w punktach, prostym językiem, po polsku.

5. Poproś o zapisanie wyniku na Dysku:
   *"Zapisz to podsumowanie na moim Dysku jako nowy dokument o nazwie
   'TEST – podsumowanie ergonomia'."*
6. Otwórz Dysk Google i sprawdź, czy plik się pojawił i czy treść się
   zgadza.

## Na co zwrócić uwagę

- **Porównaj to z NotebookLM.** Oba narzędzia pracują na Twoich
  dokumentach, ale inaczej: NotebookLM odpowiada wyłącznie na podstawie
  wgranych źródeł i podaje klikalne cytowania, natomiast Claude łączy treść
  dokumentów z własną wiedzą ogólną. Do weryfikowalnych streszczeń lepszy
  jest NotebookLM; do przetwarzania i tworzenia nowych materiałów – Claude.
- Claude nie zawsze poda cytowanie z dokumentu – jeśli fakt jest ważny,
  sprawdź go w oryginalnym pliku.
- Dysk często zawiera dokumenty z danymi osobowymi (listy uczestników,
  umowy, skany). Zanim poprosisz o przeszukanie całego Dysku, zastanów
  się, czy nie lepiej wskazać konkretny folder lub plik.
- Zapisując pliki z Claude na Dysk, używaj rozpoznawalnych nazw (np. z
  przedrostkiem "TEST" na warsztacie), żeby łatwo je potem znaleźć
  i usunąć.

## Notatki własne

- Które narzędzie – NotebookLM czy Claude – wybierzesz do pracy
  z własnymi dokumentami i dlaczego?
- Czy podsumowanie nadawało się do wykorzystania bez poprawek?
