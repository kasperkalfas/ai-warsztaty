# Zadanie 8: Skills – gotowe umiejętności z repozytorium Anthropic

**Cel:** włączyć gotowe Skills w Claude, zainstalować skill z publicznego
repozytorium i wykorzystać go do realnego zadania (dokument, prezentacja,
arkusz).
**Poziom:** średniozaawansowany

## Czym są Skills?

**Skill** to spakowany zestaw instrukcji, szablonów i skryptów, który uczy
Claude wykonywania konkretnego zadania w powtarzalny sposób. Zamiast za
każdym razem tłumaczyć w promptcie, jak ma wyglądać efekt, raz instalujesz
skill – a Claude sam sięga po niego, gdy jest potrzebny.

Różnica wobec wcześniejszych zadań:

| Mechanizm | Do czego służy |
|---|---|
| **Prompt P.K.Z.O.** (zadanie 1) | jednorazowe, dokładne polecenie |
| **Connections** (zadania 3–7) | dostęp do Twoich danych i usług zewnętrznych |
| **Skills** (to zadanie) | powtarzalny sposób *wykonania* zadania |

## Materiały

- Konto Claude z [zadania 1](01-formula-pkzo.md).
- Publiczne repozytorium Anthropic:
  [github.com/anthropics/skills](https://github.com/anthropics/skills).

**Skills działają na darmowym planie** (Free, Pro, Max, Team, Enterprise).
Warunek: w **Ustawieniach → Capabilities** musi być włączone wykonywanie
kodu i tworzenie plików (*code execution and file creation*) – bez tego
Skills się nie uruchomią.

## Kroki

### Część 1: Włączenie gotowych Skills

1. Wejdź w **Ustawienia → Capabilities** i upewnij się, że wykonywanie kodu
   i tworzenie plików jest włączone.
2. Przejdź do **Customize → Skills**. Zobaczysz listę gotowych skilli
   dostarczonych przez Anthropic.
3. Włącz przełącznikiem skille do pracy z dokumentami: **docx** (Word),
   **pptx** (PowerPoint), **xlsx** (Excel), **pdf**.
4. Sprawdź działanie – poproś o dokument, nie wspominając o skillu:

   > **P:** Jesteś specjalistą przygotowującym materiały szkoleniowe.
   > **K:** Prowadzę warsztat o ergonomii pracy dla 20 wolontariuszy.
   > **Z:** Przygotuj prezentację podsumowującą zasady ergonomii
   > stanowiska pracy.
   > **O:** 6 slajdów, plik PowerPoint do pobrania, prosty język, po polsku.

5. Pobierz wygenerowany plik i otwórz go. Zwróć uwagę, że Claude sam
   rozpoznał, iż potrzebny jest skill `pptx` – nie trzeba go wywoływać
   z nazwy.

### Część 2: Instalacja skilla z repozytorium

6. Wejdź na [github.com/anthropics/skills](https://github.com/anthropics/skills)
   i otwórz folder [`skills/`](https://github.com/anthropics/skills/tree/main/skills).
   Znajdziesz tam m.in.:

   | Skill | Co robi |
   |---|---|
   | `brand-guidelines` | pilnuje spójnej identyfikacji wizualnej w tworzonych materiałach |
   | `doc-coauthoring` | wspiera wspólne pisanie i redagowanie dokumentów |
   | `internal-comms` | szablony komunikacji wewnętrznej (ogłoszenia, maile do zespołu) |
   | `canvas-design` | projekty graficzne na płótnie (plakaty, grafiki) |
   | `algorithmic-art` | generatywna grafika tworzona kodem |
   | `skill-creator` | pomaga zbudować własny skill od zera |

7. Pobierz wybrany skill jako folder ZIP. Najprościej: przycisk **Code →
   Download ZIP** na stronie repozytorium, a następnie spakuj **pojedynczy
   folder skilla** (ten, który zawiera plik `SKILL.md`) do osobnego ZIP-a.
8. W Claude przejdź do **Customize → Skills**, kliknij **"+"**, wybierz
   **"Upload a skill"** i wgraj przygotowany plik ZIP.
9. Włącz nowy skill przełącznikiem na liście.

### Część 3: Wykorzystanie zainstalowanego skilla

10. Zleć zadanie odpowiadające zainstalowanemu skillowi. Przykład dla
    `internal-comms`:

    > **P:** Jesteś koordynatorem komunikacji w organizacji pozarządowej.
    > **K:** Za dwa tygodnie odbywa się kolejny dzień szkolenia dla
    > wolontariuszy; część osób nie odebrała jeszcze materiałów.
    > **Z:** Przygotuj ogłoszenie do wysłania wolontariuszom.
    > **O:** Do 200 słów, ton przyjazny, z wyraźnym wezwaniem do działania
    > i terminem, po polsku.

11. Porównaj wynik z tym, co Claude wygenerowałby **bez** skilla – wyłącz
    skill i wyślij ten sam prompt jeszcze raz. Zapisz różnice.

## Na co zwrócić uwagę

- **Skille uruchamiają się automatycznie.** Claude sam ocenia, czy dany
  skill pasuje do zadania, na podstawie jego opisu. Nie musisz pisać
  "użyj skilla X" – wystarczy dobrze opisać zadanie.
- Kopie skilli dokumentowych (`docx`, `pptx`, `xlsx`, `pdf`) w folderze
  `skills/` repozytorium to **migawki w czasie**, nieaktualizowane na
  bieżąco – ich wersje są już wbudowane w Claude. Traktuj je jako przykłady do nauki, nie jako
  najnowszą wersję.
- **Instaluj tylko skille ze źródeł, którym ufasz.** Skill może zawierać
  skrypty wykonywane w środowisku Claude. Repozytorium `anthropics/skills`
  jest oficjalne; przy skillach od nieznanych autorów zajrzyj najpierw do
  pliku `SKILL.md` i zobacz, co skill faktycznie robi.
- Jeśli skill się nie uruchamia, sprawdź w pierwszej kolejności, czy
  wykonywanie kodu jest włączone w **Ustawieniach → Capabilities** – to
  najczęstsza przyczyna.
- Największy zysk ze skilli mają zadania, które **powtarzasz regularnie**
  w tej samej formie: raporty, ogłoszenia, materiały szkoleniowe. Dla
  jednorazowego zadania wystarczy dobry prompt P.K.Z.O.

## Notatki własne

- Który gotowy skill najbardziej przydałby się w Twojej pracy lub
  wolontariacie?
- Czym różnił się wynik z włączonym i wyłączonym skillem?
- Jakie zadanie wykonujesz na tyle często, że warto byłoby zbudować dla
  niego własny skill (`skill-creator`)?
