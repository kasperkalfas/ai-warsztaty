# Zadanie 7: Microsoft Learn – nauka na wiarygodnych źródłach

**Cel:** podłączyć konektor Microsoft Learn i przekonać się, czym różni się
odpowiedź oparta na oficjalnej dokumentacji od odpowiedzi z ogólnej wiedzy
modelu.
**Poziom:** średniozaawansowany

## Materiały

- Konto Claude z [zadania 1](01-formula-pkzo.md).
- Konektor **Microsoft Learn** z katalogu Connections – nie wymaga
  logowania do konta Microsoft, bo korzysta z publicznej dokumentacji.

## Kroki

1. **Najpierw bez konektora.** W nowej rozmowie, z wyłączonymi
   konektorami, zadaj pytanie techniczne, np.:
   *"Jak w Excelu użyć funkcji WYSZUKAJ.PIONOWO i czym różni się od
   X.WYSZUKAJ?"*
   Zapisz lub zapamiętaj odpowiedź.
2. Podłącz **Microsoft Learn** w menu **"Search and tools" → "Add
   connectors"**.
3. Zadaj **to samo pytanie** ponownie, prosząc wprost o oparcie się na
   dokumentacji:
   *"Odpowiedz na to pytanie na podstawie dokumentacji Microsoft Learn
   i podaj linki do źródeł."*
4. Porównaj obie odpowiedzi: czy różnią się szczegółowością? Czy druga
   zawiera odnośniki, które możesz kliknąć i sprawdzić?
5. Zadaj pytanie o coś, czego nie znasz, w formule P.K.Z.O.:

   > **P:** Jesteś trenerem uczącym osoby nietechniczne obsługi narzędzi
   > Microsoft 365.
   > **K:** Prowadzę zajęcia dla wolontariuszy, którzy zaczynają pracę
   > z OneDrive i nie znają pojęć technicznych.
   > **Z:** Wyjaśnij, na czym polega udostępnianie plików i zarządzanie
   > uprawnieniami w OneDrive, na podstawie dokumentacji Microsoft Learn.
   > **O:** Prosty język, maksymalnie 300 słów, w punktach, z linkami do
   > źródeł na końcu.

6. Kliknij przynajmniej jeden podany link i sprawdź, czy potwierdza treść
   odpowiedzi.

## Na co zwrócić uwagę

- To ćwiczenie pokazuje **najważniejszą zaletę konektorów**: odpowiedź
  przestaje być "z pamięci modelu", a zaczyna opierać się na aktualnym,
  możliwym do sprawdzenia źródle. Ta sama zasada stała za NotebookLM
  (odpowiedzi tylko z wgranych źródeł) i Perplexity (odpowiedzi
  z cytowaniami).
- Wiedza modelu ma **datę graniczną** – o nowszych funkcjach czy zmianach
  w interfejsie model może po prostu nie wiedzieć. Dokumentacja jest
  aktualizowana na bieżąco.
- Konektor obejmuje dokumentację Microsoftu – nie odpowie na pytania spoza
  tego zakresu. To zaleta: wąskie, wiarygodne źródło zamiast całego
  internetu.
- Zawsze klikaj w podane linki przy ważnych informacjach. Sam fakt, że
  odpowiedź zawiera odnośnik, nie gwarantuje, że treść odpowiedzi
  dokładnie mu odpowiada.

## Notatki własne

- Czym różniła się odpowiedź przed podłączeniem konektora i po nim?
- Czy link potwierdzał treść odpowiedzi?
- Do jakich tematów w swojej pracy przydałoby Ci się źródło "tylko
  z oficjalnej dokumentacji"?
