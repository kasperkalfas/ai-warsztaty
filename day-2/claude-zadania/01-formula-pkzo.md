# Zadanie 1: Formuła P.K.Z.O. – prompting dla każdego

**Cel:** nauczyć się budować skuteczne zapytania (prompty) według prostej
formuły P.K.Z.O. i zobaczyć na własnym przykładzie, jak bardzo poprawia to
jakość odpowiedzi.
**Poziom:** podstawowy

Dobry prompt to klucz do uzyskania precyzyjnych i użytecznych odpowiedzi od
AI. Formuła P.K.Z.O. to prosta metoda, która pomoże Ci konstruować skuteczne
zapytania.

## Schemat P.K.Z.O.

| Litera | Element | Co zawiera | Przykład |
|--------|---------|------------|----------|
| **P** | Persona (Rola) | Nadaj Claude konkretną rolę eksperta, który ma Ci pomóc. | *"Jesteś ekspertem finansowym…", "Jesteś doświadczonym nauczycielem…", "Jesteś specjalistą HR…"* |
| **K** | Kontekst (Sytuacja) | Opisz sytuację, w której się znajdujesz. Podaj tło i ważne szczegóły. | *"Pracujemy nad budżetem na 2027 rok…", "Organizuję szkolenie dla 20 osób…", "Przygotowuję się do rozmowy kwalifikacyjnej…"* |
| **Z** | Zadanie (Cel) | Określ konkretny cel – co dokładnie ma zrobić Claude? | *"Stwórz tabelę…", "Napisz e-mail…", "Przygotuj listę kroków…", "Wygeneruj pomysły…"* |
| **O** | Ograniczenia (Ramy i format) | Określ format odpowiedzi, długość, styl, język lub inne wymagania. | *"Użyj PLN, max 10 pozycji, format tabeli", "W punktach, maksymalnie 5 punktów", "Ton formalny, do 200 słów"* |

## Materiały

Konto na [claude.ai](https://claude.ai) – instrukcja logowania znajduje się
w [README](README.md#jak-zacząć-pracę-z-claude).

## Kroki

1. Zaloguj się na [claude.ai](https://claude.ai) i rozpocznij nową rozmowę.
2. **Zadaj najpierw "słabe" pytanie** – celowo ogólne, bez formuły, np.:
   *"Napisz coś o ergonomii pracy."*
   Przeczytaj odpowiedź i oceń, na ile jest przydatna w Twojej sytuacji.
3. **Teraz zbuduj prompt według P.K.Z.O.** – możesz wykorzystać poniższy
   przykład lub napisać własny na ten sam temat:

   > **P:** Jesteś specjalistą BHP z doświadczeniem w szkoleniu osób
   > pracujących biurowo.
   > **K:** Prowadzę warsztat dla 20 wolontariuszy, którzy pracują przy
   > komputerze po kilka godzin dziennie i nie mają wiedzy technicznej.
   > **Z:** Przygotuj checklistę dobrych praktyk ergonomii stanowiska pracy,
   > którą uczestnicy powiesią przy biurku.
   > **O:** Maksymalnie 8 punktów, każdy w jednym zdaniu, prostym językiem,
   > po polsku, w formie listy do odhaczenia.

4. **Porównaj obie odpowiedzi.** Która jest bardziej konkretna? Która
   nadaje się do użycia bez poprawek?
5. **Zmień jedno ograniczenie** i wyślij prompt ponownie – np. zamiast
   8 punktów poproś o 4, albo zmień ton na bardziej swobodny. Zobacz, jak
   jeden element formuły zmienia efekt.
6. **Napisz własny prompt P.K.Z.O.** dotyczący Twojej pracy lub
   wolontariatu i sprawdź wynik.


## 💡 Przykład 1: Przygotowanie ogłoszenia o pracę

### ❌ Słaby prompt:
```
Napisz ogłoszenie o pracę dla sekretarki.
```

### ✅ Dobry prompt (P.K.Z.O.):
```
PERSONA: Jesteś specjalistą HR z 10-letnim doświadczeniem w rekrutacji.

KONTEKST: Nasza szkoła poszukuje osoby na stanowisko sekretarki/sekretarza 
do obsługi sekretariatu szkolnego. Praca na pełen etat, wymagana obsługa 
programu Vulcan, kontakt z rodzicami i nauczycielami.

ZADANIE: Stwórz profesjonalne ogłoszenie o pracę, które przyciągnie 
odpowiednich kandydatów.

OGRANICZENIA:
- Długość: do 300 słów
- Struktura: stanowisko, opis, wymagania, oferujemy, kontakt
- Ton: profesjonalny ale przyjazny
- Wynagrodzenie: 4500-5500 zł brutto (podaj widełki)
```

---

## 💡 Przykład 2: Planowanie budżetu firmowego

### ❌ Słaby prompt:
```
Pomóż mi z budżetem firmy.
```

### ✅ Dobry prompt (P.K.Z.O.):
```
PERSONA: Jesteś doświadczonym doradcą finansowym dla małych firm.

KONTEKST: Prowadzę małą firmę usługową (5 pracowników). Planuję budżet 
na 2025 rok. Roczny przychód to około 600 000 zł. Chcę lepiej kontrolować 
wydatki i zaplanować oszczędności na rozwój firmy.

ZADANIE: Stwórz szablon prostego budżetu rocznego z podstawowymi kategoriami 
kosztów, które powinienem monitorować.

OGRANICZENIA:
- Format: tabela w markdown
- Waluta: PLN
- Maksymalnie 12 kategorii kosztów
- Podziel na: koszty stałe i zmienne
- Dodaj kolumnę z procentowym udziałem w budżecie
- Dodaj krótki komentarz (2-3 zdania) do każdej kategorii
```



## Na co zwrócić uwagę

- Nie każdy prompt musi mieć wszystkie cztery elementy – ale im bardziej
  złożone zadanie, tym bardziej się opłacają. Najczęściej pomijanym, a
  najbardziej przydatnym elementem są **Ograniczenia** (O).
- Kontekst (K) to miejsce, w którym łatwo nieświadomie podać **dane
  osobowe** – nie wklejaj do promptu imion, adresów, numerów PESEL ani
  danych innych osób. Opisz sytuację ogólnie ("uczestnik szkolenia"
  zamiast konkretnego nazwiska).
- Rozmowa z Claude jest **kontekstowa** – nie musisz powtarzać całego
  promptu, żeby coś poprawić. Wystarczy dopisać *"Skróć to do 4 punktów"*
  albo *"Napisz to prostszym językiem"*.
- Jeśli odpowiedź nie trafia w Twoje potrzeby, zwykle szybciej jest
  **doprecyzować prompt**, niż wielokrotnie prosić o poprawki – to także
  oszczędza limit wiadomości na bezpłatnym planie.

## Notatki własne

- Czym różniła się odpowiedź na "słabe" pytanie od odpowiedzi na prompt
  P.K.Z.O.?
- Który element formuły (P, K, Z czy O) najbardziej zmienił wynik w Twoim
  przypadku?
- Zapisz tutaj swój najlepszy prompt P.K.Z.O., żeby móc go użyć ponownie:


