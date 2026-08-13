# Zadanie 4: Gemini CLI – instalacja i pierwsze polecenia

**Cel:** zainstalować od zera Gemini CLI – wersję Gemini działającą w
terminalu – i wykonać pierwsze polecenia. Zadanie zawiera wyjaśnienie
wszystkich pojęć (terminal, CLI, Node.js, npm), więc nie musisz mieć
żadnego doświadczenia z programowaniem.
**Poziom:** średniozaawansowany (wymaga terminala)

## Słowniczek – co będziemy instalować i po co

Zanim cokolwiek zainstalujemy, wyjaśnijmy cztery pojęcia, które pojawią
się w tym zadaniu:

**Terminal** (inaczej: konsola, wiersz poleceń) to program, w którym
komunikujesz się z komputerem **tekstem** zamiast klikaniem. Wpisujesz
polecenie, naciskasz Enter, komputer wykonuje je i wypisuje odpowiedź.
Terminal jest wbudowany w każdy system: na Windows to **PowerShell**
lub aplikacja **Terminal**, na Macu – aplikacja **Terminal**.

**CLI** (ang. *Command Line Interface*, interfejs wiersza poleceń) to
każdy program obsługiwany z terminala – bez okien i przycisków, samym
tekstem. „Gemini CLI" to więc po prostu Gemini w wersji na terminal:
zamiast pisać w okienku przeglądarki, piszesz w konsoli. Brzmi to mniej
wygodnie, ale ma jedną wielką zaletę – CLI działa **w konkretnym
folderze na Twoim dysku** i może pracować na Twoich plikach.

**Node.js** to środowisko, które pozwala uruchamiać na komputerze
programy napisane w języku JavaScript – takie jak właśnie Gemini CLI.
Traktuj Node.js jak „silnik": sam z siebie nic nie robi, ale bez niego
Gemini CLI nie wystartuje. Dlatego instalujemy go w pierwszej
kolejności.

**npm** (ang. *Node Package Manager*) to menedżer pakietów instalowany
**razem z Node.js** – osobno nie trzeba go pobierać. Działa jak sklep
z aplikacjami dla programów w JavaScript: jednym poleceniem pobiera
program z internetu i instaluje go na komputerze. Użyjemy go do
zainstalowania Gemini CLI. Spotkasz też polecenie `npx` – to „młodszy
brat" npm, który uruchamia program **bez instalowania go na stałe**
(przydatne, gdy chcesz coś tylko wypróbować).

Kolejność jest więc taka:

| Krok | Co instalujemy | Po co |
|---|---|---|
| 1 | Node.js (a z nim npm) | „silnik", bez którego nic nie ruszy |
| 2 | Gemini CLI (przez npm) | właściwe narzędzie |
| 3 | klucz API z Google AI Studio | dostęp do modelu Gemini |

## Materiały

- Komputer z Windows, macOS lub Linux i uprawnieniami do instalowania
  programów.
- Połączenie z internetem.
- Konto Google (to samo, którego używasz do Gmaila).

**Jeśli podczas szkolenia to zadanie jest pokazem prowadzącego** –
obserwuj kroki na ekranie i wróć do samodzielnej instalacji po zajęciach.

## Kroki

### Część 1: Otwarcie terminala i podstawy nawigacji

1. Otwórz terminal:
   - **Windows:** naciśnij klawisz Windows, wpisz `powershell`
     i naciśnij Enter. Otworzy się okno z migającym kursorem –
     to właśnie terminal.
   - **macOS:** naciśnij Cmd+Spacja, wpisz `terminal` i naciśnij Enter.
2. Oswój się z terminalem – wpisz swoje pierwsze polecenie i naciśnij
   Enter:

   ```
   whoami
   ```

   Komputer wypisze nazwę Twojego użytkownika. Tak wygląda cała praca
   w terminalu: polecenie → Enter → odpowiedź.

3. Sprawdź, gdzie jesteś. Terminal zawsze „stoi" w jakimś folderze na
   dysku – nazywa się go **bieżącym katalogiem**. Wpisz:

   ```
   pwd
   ```

   (skrót od ang. *print working directory* – „pokaż bieżący katalog").
   Zobaczysz ścieżkę, np. `C:\Users\Kasia` – to Twój folder domowy.
   Zawartość bieżącego folderu wypisze polecenie:

   ```
   ls
   ```

   (skrót od ang. *list* – „wypisz"). Zobaczysz znajome nazwy:
   `Documents`, `Downloads`, `Desktop` – te same foldery, które na co
   dzień oglądasz w Eksploratorze plików.

4. Naucz się przechodzić między folderami poleceniem `cd` (ang. *change
   directory* – „zmień katalog"). Wejście do folderu:

   ```
   cd Documents
   ```

   Folder musi istnieć w bieżącym katalogu – jego nazwę podpatrz w
   wyniku `ls`. Powrót o jeden poziom „w górę", do folderu nadrzędnego:

   ```
   cd ..
   ```

   (dwie kropki zawsze oznaczają „folder nadrzędny"). Trzy przydatne
   triki:

   - wpisz początek nazwy folderu i naciśnij **Tab** – terminal sam
     dokończy nazwę;
   - `cd` z pełną ścieżką, np. `cd C:\Users\TwojaNazwa\Documents`,
     przenosi Cię we wskazane miejsce niezależnie od tego, gdzie
     właśnie jesteś;
   - jeśli nazwa folderu zawiera spację, weź ścieżkę w cudzysłów:
     `cd "Moje dokumenty"`.

   Poćwicz chwilę na sucho: wejdź do dowolnego folderu (`cd nazwa`),
   obejrzyj zawartość (`ls`), sprawdź, gdzie jesteś (`pwd`), wróć
   (`cd ..`). Te cztery polecenia wystarczą do całej dalszej pracy –
   także z Gemini CLI i innymi narzędziami w terminalu.

### Część 2: Instalacja Node.js

5. Sprawdź, czy Node.js nie jest już zainstalowany – wpisz:

   ```
   node -v
   ```

   - Jeśli zobaczysz numer wersji, np. `v22.14.0` – Node.js już jest.
     Gdy pierwsza liczba to **20 lub więcej**, przejdź od razu do
     części 3.
   - Jeśli zobaczysz błąd w stylu *„node is not recognized"* lub
     *„command not found"* – Node.js nie jest zainstalowany. Wykonaj
     kroki 6–8.

6. Wejdź na stronę [nodejs.org](https://nodejs.org) i pobierz wersję
   oznaczoną **LTS** (ang. *Long Term Support* – wersja stabilna,
   wspierana długoterminowo; to właściwy wybór dla początkujących).
   Strona sama rozpozna Twój system i podpowie właściwy plik.

7. Uruchom pobrany instalator:
   - **Windows:** otwórz pobrany plik `.msi` i klikaj **Next**,
     akceptując ustawienia domyślne. Niczego nie musisz zmieniać –
     npm zainstaluje się automatycznie razem z Node.js. Na końcu
     kliknij **Install** (system może poprosić o zgodę administratora)
     i **Finish**.
   - **macOS:** otwórz pobrany plik `.pkg` i przejdź przez instalator,
     również zostawiając ustawienia domyślne.

8. **Zamknij terminal i otwórz go ponownie** – to ważne, bo terminal
   „dowiaduje się" o nowych programach dopiero po ponownym
   uruchomieniu. Następnie sprawdź, czy instalacja się powiodła:

   ```
   node -v
   npm -v
   ```

   Obydwa polecenia powinny wypisać numery wersji (np. `v22.14.0`
   i `10.9.2`). Jeśli tak – masz działający Node.js i npm.

### Część 3: Instalacja Gemini CLI

9. W terminalu wpisz polecenie, które każe npm pobrać i zainstalować
   Gemini CLI:

   ```
   npm install -g @google/gemini-cli
   ```

   Rozszyfrujmy je: `npm install` = „zainstaluj", `-g` = „globalnie"
   (czyli dla całego komputera, nie tylko jednego folderu),
   `@google/gemini-cli` = nazwa pakietu w katalogu npm. Instalacja
   potrwa chwilę – poczekaj, aż w terminalu znów pojawi się migający
   kursor.

   *Wariant bez instalacji:* jeśli chcesz tylko wypróbować narzędzie,
   zamiast instalować użyj `npx https://github.com/google-gemini/gemini-cli`
   – uruchomi ono Gemini CLI jednorazowo, bez zostawiania go na dysku.

10. Uruchom narzędzie:

    ```
    gemini
    ```

    Jeśli zobaczysz błąd *„gemini is not recognized"* – zamknij i otwórz
    terminal ponownie (jak w kroku 8) i spróbuj jeszcze raz.

### Część 4: Klucz API i pierwsze polecenia

Przy pierwszym uruchomieniu Gemini CLI pyta o sposób logowania.
**Uwaga:** opcja „Sign in with Google" **nie działa już dla zwykłych
kont indywidualnych** – od czerwca 2026 Google wyłączyło tę ścieżkę
i wyświetla komunikat *„This client is no longer supported for Gemini
Code Assist for individuals"* z odesłaniem do produktu Antigravity.
Użyjemy więc drugiej opcji: **darmowego klucza API**.

Klucz API to długi ciąg znaków, który działa jak hasło do usługi.
**Traktuj go jak hasło:** nie wklejaj go do czatów, nie wysyłaj mailem
i nie publikuj.

11. Utwórz klucz: wejdź na
    [aistudio.google.com/apikey](https://aistudio.google.com/apikey),
    zaloguj się kontem Google i kliknij **Create API key**. Skopiuj
    wygenerowany klucz (przycisk kopiowania obok). Darmowy poziom
    wystarcza do tego warsztatu i nie wymaga karty płatniczej.

12. Wróć do terminala i zapisz klucz w tzw. zmiennej środowiskowej –
    to „schowek", z którego Gemini CLI sam go odczyta:

    ```
    setx GEMINI_API_KEY "tu-wklej-swoj-klucz"
    ```

    (macOS/Linux: dopisz `export GEMINI_API_KEY="tu-wklej-swoj-klucz"`
    do pliku `~/.zshrc` lub `~/.bashrc`.)
    Po tym poleceniu **zamknij terminal i otwórz go ponownie** – tak
    jak przy instalacji Node.js, zmiana działa dopiero w nowym oknie.

13. Uruchom `gemini` jeszcze raz. Gdy pojawi się pytanie o sposób
    logowania, wybierz **Use Gemini API Key**. Narzędzie znajdzie klucz
    w zmiennej środowiskowej i będzie gotowe do rozmowy.

14. Zadaj pierwsze pytanie – pisze się tu tak samo jak w oknie czatu,
    tylko bez myszki:

    > Wyjaśnij w 3 zdaniach, czym różni się CLI od aplikacji w
    > przeglądarce.

15. Teraz największa zaleta CLI – praca na plikach. Zakończ rozmowę
    (wpisz `/quit` lub naciśnij Ctrl+C) i przejdź do folderu z
    materiałami warsztatu poleceniami z części 1, np.:

    ```
    cd Documents\ai-warsztaty
    ```

    Ścieżkę dostosuj do miejsca, gdzie masz materiały – pomagaj sobie
    poleceniem `ls` i klawiszem Tab, a gdy zabłądzisz, wróć wyżej przez
    `cd ..`. Gdy `pwd` pokaże właściwy folder, uruchom `gemini`
    ponownie.

16. Poproś Gemini, żeby powiedziało, co znajduje się w bieżącym
    katalogu:

    > Co znajduje się w tym folderze? Podsumuj krótko.

    Zwróć uwagę: Gemini w przeglądarce nie mogłoby tego zrobić – nie
    widzi Twojego dysku. CLI widzi folder, w którym je uruchomisz.

17. Zakończ rozmowę (wpisz `/quit` lub naciśnij Ctrl+C).

## Najczęstsze problemy

| Objaw | Przyczyna i rozwiązanie |
|---|---|
| `node is not recognized` po instalacji | terminal otwarty przed instalacją – zamknij go i otwórz ponownie |
| `gemini is not recognized` po `npm install` | jak wyżej – nowy terminal; jeśli nie pomoże, powtórz krok 9 |
| npm wypisuje błędy o uprawnieniach | uruchom terminal jako administrator (Windows: prawy przycisk na PowerShell → „Uruchom jako administrator") |
| instalator Node.js blokowany przez system | potwierdź zgodę w oknie kontroli konta użytkownika (UAC) |
| błąd *„This client is no longer supported for Gemini Code Assist for individuals"* | wybrano „Sign in with Google" – ta opcja nie działa już dla kont indywidualnych; użyj klucza API (kroki 11–13) |
| po wyborze „Use Gemini API Key" komunikat o braku klucza | terminal otwarty przed `setx` – zamknij go i otwórz ponownie; sprawdź też, czy klucz wkleił się w całości |

## Na co zwrócić uwagę

- Darmowy klucz API ma limit zapytań (odnawiany cyklicznie – co minutę
  i co dobę; orientacyjnie kilkaset zapytań dziennie) – wystarczający do
  zadań z tego warsztatu, ale nie do pracy ciągłej przez cały dzień.
- **Klucz API to hasło.** Jeśli podejrzewasz, że ktoś mógł go zobaczyć
  (np. na współdzielonym komputerze), wejdź na
  [aistudio.google.com/apikey](https://aistudio.google.com/apikey)
  i usuń klucz – w każdej chwili możesz utworzyć nowy. Po warsztacie na
  cudzym komputerze usuń też zmienną środowiskową:
  `setx GEMINI_API_KEY ""`.
- **Gemini CLI ma dostęp do plików w folderze, w którym je uruchomisz** –
  uruchamiaj je w bezpiecznych, znanych sobie katalogach, nie w miejscach
  z poufnymi danymi, których nie chcesz udostępniać.
- Node.js i npm zostają na komputerze także po warsztacie – to standardowe,
  bezpieczne narzędzia używane przez miliony programistów. Jeśli jednak
  chcesz posprzątać: Gemini CLI odinstalujesz poleceniem
  `npm uninstall -g @google/gemini-cli`, a Node.js – jak każdy program –
  w **Ustawienia → Aplikacje** (Windows).
- CLI to pierwszy krok w stronę "agentów AI" – narzędzi, które nie tylko
  odpowiadają na pytania, ale mogą też wykonywać działania (np. czytać i
  edytować pliki). Do tego tematu wrócimy szerzej w Dniu 6 programu
  ("Systemy AI, Agenci z n8n").

## Notatki własne

- Czy instalacja przebiegła bez problemów? Jeśli nie – co sprawiło
  trudność i który wiersz tabeli „Najczęstsze problemy" pomógł?
- Czym różniło się dla Ciebie zadawanie pytań w terminalu od zadawania
  ich w przeglądarce?
- Jak własnymi słowami wyjaśniłbyś/wyjaśniłabyś koleżance lub koledze,
  czym jest Node.js, a czym npm?
