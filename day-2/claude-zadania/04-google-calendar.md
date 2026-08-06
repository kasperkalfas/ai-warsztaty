# Zadanie 4: Google Calendar – planowanie spotkań

**Cel:** podłączyć kalendarz Google i zlecić Claude realne zadania
planistyczne: sprawdzenie dostępności, utworzenie i modyfikację wydarzenia.
**Poziom:** średniozaawansowany

## Materiały

- Konto Claude z podłączonym kontem Google (zob.
  [zadanie 3](03-connections-gmail.md)).
- Własny kalendarz Google.

## Zanim zaczniesz

W odróżnieniu od Gmaila, konektor kalendarza ma pełne uprawnienia
**do zapisu**: Claude może tworzyć, zmieniać i **usuwać** wydarzenia.
Ćwicz na wydarzeniach testowych, nie na prawdziwych spotkaniach, i czytaj
uważnie, co Claude proponuje zrobić, zanim potwierdzisz.

## Kroki

1. Podłącz **Google Calendar** w menu **"Search and tools" → "Add
   connectors"** (tak samo jak Gmaila w zadaniu 3).
2. Zacznij od odczytu – poproś o podsumowanie:
   *"Pokaż moje wydarzenia z najbliższych 7 dni w formie listy: data,
   godzina, nazwa. Zaznacz dni, w których nie mam nic zaplanowanego."*
3. Poproś o znalezienie wolnego terminu:
   *"Znajdź w przyszłym tygodniu dwa wolne terminy po 60 minut, między 9:00
   a 15:00, w dni robocze."*
4. Utwórz wydarzenie testowe promptem P.K.Z.O., np.:

   > **P:** Jesteś asystentem organizującym moje spotkania.
   > **K:** Planuję cykliczne spotkanie zespołu wolontariuszy.
   > **Z:** Utwórz w moim kalendarzu wydarzenie testowe.
   > **O:** Nazwa "TEST – spotkanie wolontariuszy", w przyszły wtorek
   > o 10:00, czas trwania 45 minut, z opisem zawierającym trzy punkty
   > agendy.

5. Sprawdź w Google Calendar, czy wydarzenie się pojawiło i czy zgadzają
   się szczegóły.
6. Poproś o modyfikację, np.: *"Przesuń wydarzenie TEST o godzinę później
   i dodaj link do Google Meet."*
7. Na koniec posprzątaj: *"Usuń wydarzenie TEST z mojego kalendarza."*
   Sprawdź w kalendarzu, czy faktycznie zniknęło.

## Na co zwrócić uwagę

- **Zawsze weryfikuj efekt w samym kalendarzu.** Claude potwierdzi, że
  wykonał zadanie – ale to Ty odpowiadasz za to, co znalazło się w Twoim
  kalendarzu.
- Uważaj na polecenia usuwające. Sformułowanie w stylu *"wyczyść mi
  przyszły tydzień"* może usunąć więcej, niż zamierzasz. Bądź konkretny/a
  i najpierw poproś o listę tego, co ma zostać usunięte.
- Kalendarz to dane osobowe także innych osób – nazwy spotkań i listy
  uczestników. Pamiętaj o tym, jeśli podłączasz kalendarz służbowy.
- Największa realna oszczędność czasu to szukanie wspólnych terminów
  i przepisywanie ustaleń z e-maila do kalendarza – warto pokazać to
  osobom, które będziesz szkolić.

## Notatki własne

- Czy Claude poprawnie zrozumiał określenia względne ("przyszły wtorek",
  "za dwa tygodnie")?
- Jakie zadanie kalendarzowe wykonujesz najczęściej i czy dałoby się je
  w ten sposób przyspieszyć?
