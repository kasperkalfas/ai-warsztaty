# Zadanie 8: Własny skill – posty na LinkedIn (AIDA i 5W)

**Cel:** zbudować od zera własny skill w Claude (przez przeglądarkę, bez
programowania), który pisze posty na LinkedIn według formuł AIDA i 5W –
na przykładzie marki osobistej fryzjera strzygącego dyrektorów i prezesów.
**Poziom:** średniozaawansowany

## Po co własny skill?

**Skill** to spakowany zestaw instrukcji, który uczy Claude wykonywania
konkretnego zadania w powtarzalny sposób. W tym zadaniu **zapisujemy
własny, powtarzalny sposób pracy** w formie skilla. Zamiast za każdym
razem tłumaczyć Claude, jak ma wyglądać post na LinkedIn, robimy to raz –
i od tej pory każdy prompt „napisz post" daje wynik w naszym stylu.

Dwie formuły, które skill będzie znał:

| Formuła | Rozwinięcie | Do czego służy |
|---|---|---|
| **AIDA** | Attention (uwaga) → Interest (zainteresowanie) → Desire (pragnienie) → Action (działanie) | posty sprzedażowe i promocyjne – prowadzą czytelnika od nagłówka do kliknięcia |
| **5W** | Who (kto), What (co), When (kiedy), Where (gdzie), Why (dlaczego) | posty informacyjne – ogłoszenia, zaproszenia, relacje z wydarzeń |

Nasz bohater: **fryzjer premium**, który strzyże dyrektorów i prezesów.
Buduje markę osobistą na LinkedIn – tam, gdzie są jego klienci. To celowo
wyrazisty przykład: łatwo ocenić, czy post „brzmi jak on", czy jak
generyczna reklama.

## Materiały

- Konto na [claude.ai](https://claude.ai) z włączonym wykonywaniem kodu
  i tworzeniem plików (**Ustawienia → Capabilities** – *code execution
  and file creation*). **Skills działają także na darmowym planie.**
- Notatnik (lub dowolny edytor tekstu) i możliwość spakowania folderu do
  ZIP – na Windows: prawy przycisk myszy → **Kompresuj do pliku ZIP**.

## Kroki

### Część 1: Punkt odniesienia – bez skilla

1. Upewnij się, że żaden skill marketingowy nie jest włączony.
2. Wyślij do Claude:
   *„Napisz post na LinkedIn promujący usługi fryzjera, który strzyże
   dyrektorów i prezesów."*
3. Zachowaj wynik – to Twoje „przed". Zwykle wychodzi poprawny, ale
   generyczny post, który mógłby napisać każdy.

### Część 2: Zbudowanie skilla

Skill to folder z jednym obowiązkowym plikiem: `SKILL.md`. Na górze pliku
znajduje się krótki opis (sekcja między `---`), po którym Claude
rozpoznaje, kiedy sięgnąć po skill. Reszta to instrukcja pisana zwykłym
językiem.

4. Utwórz na pulpicie folder o nazwie `linkedin-fryzjer-premium`.
5. W folderze utwórz plik tekstowy `SKILL.md` i wklej poniższą treść
   (możesz ją potem dowolnie zmieniać – to Twój skill):

   ```markdown
   ---
   name: linkedin-fryzjer-premium
   description: Pisze posty na LinkedIn budujące markę osobistą fryzjera
     premium, który strzyże dyrektorów i prezesów. Używaj, gdy użytkownik
     prosi o post na LinkedIn, treść promocyjną salonu fryzjerskiego lub
     materiał budujący markę osobistą fryzjera/barbera.
   ---

   # Posty na LinkedIn: fryzjer klasy premium

   ## Kim jest autor postów

   Fryzjer z wieloletnim doświadczeniem, którego klientami są dyrektorzy,
   prezesi i menedżerowie wyższego szczebla. Strzyże ludzi, którzy
   codziennie występują publicznie: na zarządach, konferencjach, w
   mediach. Sprzedaje nie strzyżenie, lecz pewność siebie i profesjonalny
   wizerunek. Dyskrecja jest częścią usługi.

   ## Ton i styl

   - Pewny siebie, ale nie przechwalający się. Konkret zamiast przymiotników.
   - Język biznesowy, zrozumiały dla kadry zarządzającej – zero żargonu
     fryzjerskiego bez wyjaśnienia.
   - Krótkie akapity (1–3 zdania), między akapitami pusta linia –
     tak czyta się posty na LinkedIn.
   - Bez emotikonów lub maksymalnie jeden. Bez wykrzykników w co drugim
     zdaniu.
   - Nigdy nie podawaj nazwisk ani firm klientów – dyskrecja to fundament
     tej marki. Pisz „prezes spółki technologicznej", nie „prezes firmy X".

   ## Formuła AIDA – posty promocyjne

   Gdy post ma sprzedawać (usługę, pakiet, wolny termin), użyj struktury:

   1. **Attention** – pierwsze zdanie musi zatrzymać przewijanie.
      Obserwacja, liczba albo przewrotne stwierdzenie związane z
      wizerunkiem ludzi biznesu. Nie zaczynaj od „Czy wiesz, że...".
   2. **Interest** – rozwiń: dlaczego fryzura ma znaczenie w pracy
      na wysokim stanowisku (pierwsze wrażenie, spójność wizerunku,
      wystąpienia publiczne).
   3. **Desire** – pokaż, co klient zyskuje: oszczędność czasu (dojazd do
      biura, stała godzina co 3 tygodnie), dyskrecję, fryzurę „odporną"
      na cały dzień spotkań.
   4. **Action** – jedno konkretne wezwanie do działania: wiadomość
      prywatna, link do kalendarza, telefon. Jedno, nie trzy.

   ## Formuła 5W – posty informacyjne

   Gdy post informuje (nowa usługa, zmiana adresu, udział w wydarzeniu),
   upewnij się, że treść odpowiada na pięć pytań:

   - **Who** – kto? (fryzjer i dla kogo jest usługa)
   - **What** – co dokładnie się dzieje lub jest oferowane?
   - **When** – kiedy? (daty, godziny, od kiedy obowiązuje)
   - **Where** – gdzie? (adres, dzielnica, „u klienta w biurze")
   - **Why** – dlaczego to ma znaczenie dla odbiorcy?

   Kolejność może być dowolna, ale żadne z pięciu pytań nie może zostać
   bez odpowiedzi.

   ## Zasady wspólne dla obu formuł

   - Długość: 120–200 słów. LinkedIn ucina dłuższe posty za „...więcej".
   - Pierwsze 2 linijki muszą działać samodzielnie – tyle widać przed
     rozwinięciem posta.
   - Na końcu maksymalnie 3 hasztagi, po polsku lub branżowe, np.
     #markaosobista #wizerunekbiznesowy #fryzjermeski.
   - Jeśli użytkownik nie wskazał formuły, wybierz: AIDA dla treści
     sprzedażowych, 5W dla informacyjnych – i napisz na końcu, której
     formuły użyto i dlaczego.
   ```

6. Zapisz plik. **Uwaga na rozszerzenie:** plik musi nazywać się
   `SKILL.md`, a nie `SKILL.md.txt` – jeśli zapisujesz z Notatnika,
   w oknie zapisu wybierz „Wszystkie pliki" i wpisz nazwę z `.md`.
7. Spakuj **cały folder** `linkedin-fryzjer-premium` do ZIP (prawy
   przycisk → **Kompresuj do pliku ZIP**).
8. W Claude przejdź do **Customize → Skills → „+" → „Upload a skill"**
   i wgraj plik ZIP. Włącz skill przełącznikiem na liście.

### Część 3: Test i porównanie

9. Wyślij **to samo polecenie** co w kroku 2 i porównaj z wersją „przed".
   Post powinien mieć strukturę AIDA, krótkie akapity i jedno wezwanie
   do działania.
10. Sprawdź drugą formułę – poproś o post informacyjny:
    *„Napisz post: od września przyjmuję także w gabinecie na Mokotowie,
    w czwartki i piątki."*
    Claude powinien sam wybrać 5W i odpowiedzieć na wszystkich pięć pytań.
11. Sprawdź granice skilla – poproś o coś spoza jego opisu:
    *„Napisz zaproszenie na urodziny."*
    Skill nie powinien się uruchomić, bo opis (`description`) mówi tylko
    o LinkedIn i marce fryzjera.

### Wariant dla chętnych: skill-creator

Zamiast pisać `SKILL.md` ręcznie, możesz zainstalować skill
**skill-creator** z oficjalnego repozytorium Anthropic
([github.com/anthropics/skills](https://github.com/anthropics/skills))
i poprosić Claude: *„Zbuduj mi skill
do postów na LinkedIn w formułach AIDA i 5W dla fryzjera premium"* –
Claude przeprowadzi Cię przez pytania i sam przygotuje plik do pobrania.
Warto jednak raz zrobić to ręcznie, żeby wiedzieć, co jest w środku.

## Na co zwrócić uwagę

- **Sekcja `description` to najważniejsze zdania całego skilla.** To po
  niej Claude decyduje, czy skill pasuje do zadania. Zbyt ogólny opis
  („pomaga w marketingu") sprawi, że skill będzie się włączał za często;
  zbyt wąski – że wcale.
- **Skill to instrukcja, nie magia.** Wszystko, co umie, sam(a) w niego
  wpisałeś/aś. Jeśli posty wychodzą złe, popraw treść `SKILL.md`, spakuj
  i wgraj ponownie – to normalny cykl pracy nad skillem.
- Formuły AIDA i 5W działają dla **każdej marki**, nie tylko fryzjera.
  Po warsztacie podmień sekcję „Kim jest autor postów" na opis własnej
  organizacji – reszta skilla zostaje bez zmian.
- Zasada dyskrecji w skillu (bez nazwisk klientów) to przykład
  **ograniczenia wpisanego na stałe** – nie musisz o nim pamiętać w
  każdym promptcie. Pomyśl, jakie stałe zasady obowiązują w Twojej
  komunikacji (RODO, wizerunek podopiecznych) i dopisz je do własnych
  skilli.
- Jeśli skill się nie uruchamia, sprawdź kolejno: czy wykonywanie kodu
  jest włączone w **Ustawieniach → Capabilities**, czy skill jest
  włączony przełącznikiem i czy plik nazywa się dokładnie `SKILL.md`.

## Notatki własne

- Czym różnił się post „przed" i „po" wgraniu skilla?
- Czy Claude poprawnie wybrał formułę (AIDA vs 5W) bez podpowiedzi?
- Jaką markę (swoją, organizacji) opisałbyś/opisałabyś w sekcji „Kim
  jest autor postów" i jakie stałe zasady byś dopisał(a)?
