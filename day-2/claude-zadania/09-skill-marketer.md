# Zadanie 9: Gotowy skill marketingowy z internetu

**Cel:** znaleźć gotowy skill w internecie, sprawdzić go przed instalacją,
zainstalować w Claude i wykorzystać do realnego zadania promocyjnego.
**Poziom:** średniozaawansowany

## Skąd bierze się skille?

W [zadaniu 8](08-skills-gotowe.md) korzystaliśmy z oficjalnego repozytorium
Anthropic. Nie ma tam jednak skilla marketingowego – takie tworzy
społeczność i publikuje w serwisie GitHub. W tym zadaniu zainstalujemy
jeden z nich.

Skill, którego użyjemy:
[**marketing-research**](https://github.com/ishwarjha/claude-marketing-research-skill)
– prowadzi uporządkowane badanie marketingowe: analizę konkurencji, profil
odbiorcy, pozycjonowanie i propozycję wartości.

## ⚠️ Zanim zainstalujesz cokolwiek z internetu

Skill może zawierać skrypty uruchamiane w środowisku Claude. Instalowanie
skilla od nieznanego autora to podobna decyzja jak instalowanie programu
z nieznanej strony. **Zawsze sprawdź cztery rzeczy:**

| Co sprawdzić | Gdzie | Dla naszego skilla |
|---|---|---|
| Czy jest licencja? | plik `LICENSE` w repozytorium | Apache 2.0 – wolno używać i modyfikować |
| Czy zawiera skrypty? | lista plików w folderze skilla | Nie – tylko instrukcja tekstowa |
| Co skill faktycznie robi? | plik `SKILL.md` | Widoczny w całości, do przeczytania |
| Czy autor jest wiarygodny? | historia i aktywność konta | Projekt publiczny, opisany, z przykładami |

Ten skill wybraliśmy właśnie dlatego, że **nie zawiera żadnych skryptów** –
to wyłącznie instrukcja w formie tekstu. To najbezpieczniejszy rodzaj
skilla. Przy skillach zawierających kod zachowaj znacznie większą
ostrożność.

## Materiały

- Konto Claude z włączonym wykonywaniem kodu (**Ustawienia →
  Capabilities**) – zob. [zadanie 8](08-skills-gotowe.md).
- Repozytorium
  [github.com/ishwarjha/claude-marketing-research-skill](https://github.com/ishwarjha/claude-marketing-research-skill).

## Kroki

### Część 1: Punkt odniesienia – bez skilla

1. Upewnij się, że skill nie jest jeszcze zainstalowany.
2. Poproś o materiał promocyjny:
   *„Pomóż mi zaplanować kampanię naboru wolontariuszy do naszej
   organizacji."*
3. Zachowaj wynik – to Twoje „przed".

### Część 2: Sprawdzenie i instalacja

4. Wejdź na
   [stronę repozytorium](https://github.com/ishwarjha/claude-marketing-research-skill)
   i przejdź przez tabelę kontrolną powyżej – otwórz plik `LICENSE`
   i zajrzyj do folderu `marketing-research/`, żeby zobaczyć, że jest tam
   tylko `SKILL.md`.
5. Otwórz `SKILL.md` i przeczytaj **opis skilla** na samej górze pliku
   (sekcja `description`). To zdanie decyduje, kiedy Claude sięgnie po
   skill.
6. Pobierz skill z zakładki **Releases** – plik z rozszerzeniem
   **`.skill`**.

   *Gdyby nie było gotowego pliku:* pobierz całe repozytorium
   (**Code → Download ZIP**), rozpakuj i spakuj sam folder
   `marketing-research/` do osobnego ZIP-a – tak jak w zadaniu 8.

7. W Claude przejdź do **Customize → Skills → „+" → „Upload a skill"**
   i wgraj pobrany plik.
8. Włącz skill przełącznikiem na liście.

### Część 3: Wykorzystanie do realnego zadania

9. Wyślij **to samo polecenie** co w kroku 2 i porównaj wynik.
10. Teraz zadanie właściwe – prompt P.K.Z.O. dopasowany do organizacji
    pozarządowej:

    > **P:** Jesteś specjalistą od komunikacji w organizacji pozarządowej.
    > **K:** Prowadzimy program szkoleń z kompetencji cyfrowych dla
    > wolontariuszy. Chcemy pozyskać nowych uczestników, głównie osoby
    > dorosłe, które nie czują się pewnie z technologią.
    > **Z:** Przygotuj profil odbiorcy i propozycję wartości naszego
    > programu.
    > **O:** Odpowiedz po polsku, w tabelach, maksymalnie 500 słów.

11. Poproś o materiał końcowy na podstawie tej analizy:
    *„Na podstawie powyższego profilu napisz post na Facebooka
    zapraszający do udziału w programie. Do 150 słów, po polsku."*
12. Porównaj ten post z tym, co dostałeś/aś w kroku 2, przed instalacją
    skilla.

## Na co zwrócić uwagę

- **Skill jest po angielsku, ale odpowiedzi mogą być po polsku.** Instrukcja
  wewnątrz `SKILL.md` jest anglojęzyczna – wystarczy w promptcie napisać
  „odpowiedz po polsku". Warto to pokazać uczestnikom, bo obcojęzyczny
  skill bywa odrzucany jako „nie dla nas".
- Skill został napisany z myślą o firmach (konkurencja, propozycja
  wartości, pozycjonowanie). W organizacji pozarządowej te pojęcia też
  mają sens: konkurujecie o **czas i uwagę** wolontariuszy, a propozycja
  wartości to odpowiedź na pytanie „dlaczego warto przyjść akurat do was".
- **Skill porządkuje myślenie, nie zastępuje wiedzy o odbiorcach.** Jeśli
  nie wiesz, kim są Twoi wolontariusze, skill tego nie odgadnie – wymyśli
  prawdopodobnie brzmiący profil. Zweryfikuj go z rzeczywistością, zanim
  na nim oprzesz kampanię.
- Uważaj na dane w analizie konkurencji – skill może korzystać
  z wyszukiwania internetowego. Nie wpisuj do promptu informacji
  poufnych o swojej organizacji.
- Jeśli skill przestanie być potrzebny, wyłącz go przełącznikiem lub usuń
  w **Customize → Skills**. Warto zrobić to po szkoleniu, jeśli pracujesz
  na komputerze współdzielonym.

## Notatki własne

- Czym różnił się plan kampanii „przed" i „po" instalacji skilla?
- Czy profil odbiorcy zgadzał się z tym, co wiesz o swoich wolontariuszach?
  Co skill zmyślił?
- Którą z czterech rzeczy z tabeli kontrolnej sprawdzasz zwykle przed
  instalacją czegokolwiek – i czy po tym zadaniu coś się zmieni?
