# Zadanie 4: Gemini CLI – instalacja i pierwsze polecenia

**Cel:** uruchomić Gemini CLI – wersję Gemini działającą w terminalu – i
wykonać pierwsze polecenia.
**Poziom:** średniozaawansowany (wymaga terminala)

## Materiały

- Terminal (Windows: PowerShell lub Terminal).
- Zainstalowany [Node.js](https://nodejs.org) w wersji 20 lub nowszej.
- Konto Google.

**Jeśli podczas szkolenia to zadanie jest pokazem prowadzącego** –
obserwuj kroki na ekranie i wróć do samodzielnej instalacji po zajęciach.

## Kroki

1. Sprawdź, czy masz zainstalowany Node.js:

   ```
   node -v
   ```

   Jeśli polecenie zwróci błąd albo wersję niższą niż 20, zainstaluj
   aktualną wersję ze strony [nodejs.org](https://nodejs.org) (wersja
   LTS) przed dalszymi krokami.

2. Uruchom Gemini CLI bez trwałej instalacji, żeby wypróbować narzędzie:

   ```
   npx https://github.com/google-gemini/gemini-cli
   ```

   Albo zainstaluj je na stałe:

   ```
   npm install -g @google/gemini-cli
   ```

   a potem uruchamiaj poleceniem `gemini`.

3. Przy pierwszym uruchomieniu narzędzie poprosi o zalogowanie się kontem
   Google w przeglądarce – potwierdź dostęp.

4. W trybie czatu w terminalu zadaj proste pytanie, np.:

   > Wyjaśnij w 3 zdaniach, czym różni się CLI od aplikacji w
   > przeglądarce.

5. Przejdź do folderu z materiałami warsztatu (np. folder z tym
   repozytorium) i poproś Gemini CLI, żeby powiedziało, co znajduje się w
   bieżącym katalogu:

   > Co znajduje się w tym folderze? Podsumuj krótko.

## Na co zwrócić uwagę

- Darmowy plan Gemini CLI ma limit zapytań (odnawiany cyklicznie – co
  minutę i co dobę) – wystarczający do zadań z tego warsztatu, ale nie do
  pracy ciągłej przez cały dzień.
- **Gemini CLI ma dostęp do plików w folderze, w którym je uruchomisz** –
  uruchamiaj je w bezpiecznych, znanych sobie katalogach, nie w miejscach
  z poufnymi danymi, których nie chcesz udostępniać.
- CLI to pierwszy krok w stronę "agentów AI" – narzędzi, które nie tylko
  odpowiadają na pytania, ale mogą też wykonywać działania (np. czytać i
  edytować pliki). Do tego tematu wrócimy szerzej w Dniu 6 programu
  ("Systemy AI, Agenci z n8n").

## Notatki własne

- Czy instalacja przebiegła bez problemów? Jeśli nie – co sprawiło
  trudność?
- Czym różniło się dla Ciebie zadawanie pytań w terminalu od zadawania
  ich w przeglądarce?
