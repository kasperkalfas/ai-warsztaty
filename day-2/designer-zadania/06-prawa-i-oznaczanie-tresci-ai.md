# Zadanie 6: Prawa, oznaczanie treści AI i granice narzędzia

**Cel:** wiedzieć, czego **nie wolno** generować, jak oznaczać materiały
tworzone przez AI i co dzieje się z Twoimi danymi w narzędziu.
**Poziom:** dyskusyjny (bez generowania grafiki)
**Budżet:** 0 kredytów AI – pracujesz na plikach pobranych wcześniej

## Materiały

Materiały przygotowane w zadaniach 1–5 oraz notatki z Bloku 2 (Regulacje AI).

## Kroki

1. Otwórz jeden z pobranych plików i sprawdź, czy zawiera **Content
   Credentials** (metadane C2PA – informację, że obraz powstał z użyciem AI).
   Microsoft dodaje takie oznaczenia do generowanych obrazów; sprawdzisz je
   we właściwościach pliku lub w weryfikatorze
   [contentcredentials.org/verify](https://contentcredentials.org/verify).
2. To samo oznaczenie znajdziesz też **ręcznie, bez weryfikatora**:
   - **Właściwości pliku:** prawy przycisk → **Właściwości → Szczegóły**.
     Uwaga: dla plików z generatorów ta karta bywa niemal pusta – manifest
     C2PA nie jest tam pokazywany, a brak danych w "Szczegółach" **nie**
     oznacza, że plik nie ma oznaczenia AI.
   - **PowerShell (Windows):** manifest C2PA zawiera widoczny tekst `c2pa`,
     więc wykrywa go jedna komenda:
     `Select-String -Path .\obraz.jpg -Pattern "c2pa" -Quiet`
     Wynik `True` = plik ma osadzony manifest. Analogicznie można poszukać
     wzorca `trainedAlgorithmicMedia` – to oficjalny znacznik IPTC
     "utworzone przez algorytm AI". Ta metoda tylko wykrywa oznaczenie;
     treść i podpis pokaże dopiero weryfikator z kroku 1.
3. Oznaczenie sprawdzisz też **w aplikacji Gemini** (gemini.google.com lub
   aplikacja mobilna, po zalogowaniu): wgraj obraz i zapytaj wprost
   *"Czy ten obraz został wygenerowany przez AI?"*. Gemini sprawdza dwie
   rzeczy: niewidzialny znak wodny **SynthID** oraz metadane **Content
   Credentials (C2PA)**. Ważne ograniczenie: SynthID wykrywa tylko treści
   z narzędzi AI **Google** – obraz z Designera rozpozna więc po metadanych
   C2PA, a nie po znaku wodnym. Odpowiedź "nie wykryto SynthID" **nie
   oznacza**, że obraz nie jest z AI.
4. Sprawdź, co się stanie z metadanymi po wysłaniu pliku przez komunikator
   lub wrzuceniu na portal społecznościowy – wgraj go ponownie do
   weryfikatora. Czy oznaczenie przetrwało?
5. Sformułuj **jedno zdanie**, którym oznaczysz materiał w publikacji,
   np. *"Grafika wygenerowana przy pomocy AI (Microsoft Designer)"*.
   Ustal z grupą, gdzie je umieszczać: w podpisie, w stopce, w opisie posta.
6. Przeanalizujcie w grupie cztery sytuacje – w każdej odpowiedzcie: wolno,
   nie wolno, czy "wolno pod warunkiem":
   - plakat z wygenerowaną postacią wyglądającą jak konkretny znany polityk,
   - logo organizacji wygenerowane w Designerze i zgłoszone do rejestracji
     jako znak towarowy,
   - zdjęcie "z akcji charytatywnej", której w rzeczywistości nie było,
     użyte w sprawozdaniu dla sponsora,
   - portret uczestniczki warsztatów wgrany do edytora, żeby podmienić tło,
     bez pytania jej o zgodę.
7. Sprawdź w [warunkach usługi Microsoft](https://www.microsoft.com/servicesagreement),
   czego dotyczy sekcja o usługach opartych na AI – zwróć uwagę na zakaz
   generowania treści szkodliwych i na to, że narzędzie jest przeznaczone
   do użytku zgodnego z prawem.
8. Zapisz dla siebie krótką zasadę: **czego nigdy nie wpiszesz w opis obrazu**
   (dane osobowe, informacje wrażliwe, dane podopiecznych).

## Na co zwrócić uwagę

- Oznaczanie treści generowanych przez AI to nie tylko dobra praktyka –
  **AI Act** wprowadza obowiązki przejrzystości wobec odbiorców treści
  syntetycznych (m.in. deepfake'ów). Szczegóły omawiane są w Bloku 2.
- Metadane C2PA łatwo zgubić: kompresja, zrzut ekranu czy przepuszczenie
  pliku przez niektóre portale usuwa oznaczenie. Dlatego oznaczenie **słowne
  w podpisie** jest pewniejsze niż samo poleganie na metadanych.
- Oznaczenia AI działają tylko **w jedną stronę**: obecność manifestu C2PA
  lub znaku wodnego potwierdza pochodzenie z AI, ale ich **brak niczego nie
  dowodzi** – oznaczenie mogło zostać usunięte, a wiele generatorów w ogóle
  go nie dodaje. Znaki wodne (np. SynthID Google czy niewidzialny znak
  Microsoftu) siedzą w samych pikselach i przetrwają więcej niż metadane,
  ale każdy wykrywa tylko treści "swojego" dostawcy.
- Wizerunek konkretnej, rozpoznawalnej osoby (także wygenerowany) to
  osobna kwestia prawna – dobra osobiste chronione są niezależnie od tego,
  jakim narzędziem powstał obraz.
- Grafika wygenerowana przez AI ma niejasny status w prawie autorskim –
  w wielu porządkach prawnych wytwór bez wkładu człowieka nie jest chroniony.
  Przy logo i znakach firmowych to realne ryzyko: możesz nie być w stanie
  zabronić innym używania takiego znaku. Do identyfikacji wizualnej
  organizacji bezpieczniej zamówić projekt u człowieka.
- Wszystko, co wpisujesz w opis i wgrywasz do edytora, trafia na serwery
  dostawcy. Dane podopiecznych, wrażliwe zdjęcia i informacje objęte
  tajemnicą nie mają tam czego szukać.

## Notatki własne

- Jak brzmi Twoja formuła oznaczania materiałów AI?
- Która z czterech sytuacji z punktu 6 wywołała największą różnicę zdań
  w grupie i dlaczego?
