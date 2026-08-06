# Zadanie 6: Podróże – Booking.com i Kiwi.com

**Cel:** wykorzystać konektory podróżnicze do zaplanowania wyjazdu –
wyszukanie lotów i noclegów bez przełączania się między serwisami.
**Poziom:** średniozaawansowany

## Materiały

- Konto Claude z [zadania 1](01-formula-pkzo.md).
- Konektory **Kiwi.com** (wyszukiwanie lotów) i **Booking.com** (noclegi)
  z katalogu Connections.

**Uwaga:** katalog konektorów bywa aktualizowany, a niektóre usługi wymagają
dodatkowego zalogowania się do swojego konta w danym serwisie. Jeśli
któregoś konektora nie znajdziesz na liście, wykonaj zadanie na tym, który
jest dostępny – zasada pracy jest identyczna.

## Kroki

1. Podłącz **Kiwi.com** i **Booking.com** w menu **"Search and tools" →
   "Add connectors"**. Jeśli pojawi się prośba o zalogowanie do serwisu,
   przejdź przez nią tak jak przy Gmailu.
2. Wyszukaj loty promptem P.K.Z.O.:

   > **P:** Jesteś doradcą podróży planującym wyjazdy grupowe.
   > **K:** Planuję wyjazd szkoleniowy dla dwóch osób z Warszawy do
   > Barcelony, na cztery dni w drugiej połowie przyszłego miesiąca.
   > Terminy są elastyczne, budżet ograniczony.
   > **Z:** Znajdź najtańsze połączenia lotnicze w obie strony.
   > **O:** Przedstaw 3 opcje w tabeli: data wylotu i powrotu, godziny,
   > przewoźnik, cena, liczba przesiadek. Ceny w PLN.

3. Poproś o dopasowanie noclegu do wybranego wariantu:
   *"Dla najtańszej opcji znajdź nocleg dla dwóch osób blisko centrum,
   z oceną minimum 8.0 i bezpłatnym anulowaniem. Pokaż 3 propozycje
   w tabeli z ceną za cały pobyt."*
4. Poproś o podsumowanie całości:
   *"Zsumuj koszt wybranego wariantu (loty + nocleg) i przygotuj krótkie
   uzasadnienie wyboru w 3 zdaniach."*
5. Sprawdź jedną z propozycji bezpośrednio w serwisie (Kiwi.com lub
   Booking.com) i porównaj cenę z tą podaną przez Claude.

## Na co zwrócić uwagę

- **Nic nie zostaje zarezerwowane ani opłacone.** Konektory służą do
  wyszukiwania i porównywania; rezerwację zawsze finalizujesz samodzielnie
  w serwisie. To zadanie nie kosztuje ani złotówki.
- **Zawsze zweryfikuj cenę i warunki w serwisie przed rezerwacją.** Ceny
  biletów i pokoi zmieniają się w czasie rzeczywistym, a podana w rozmowie
  kwota może być już nieaktualna. Sprawdź też bagaż, godziny przesiadek
  i warunki anulowania – to elementy, które łatwo przeoczyć w podsumowaniu.
- Realna wartość tego rozwiązania to **porównanie w jednym miejscu**:
  zamiast otwierać kilkanaście kart, opisujesz swoje warunki raz i
  dostajesz zestawienie. Im dokładniejsze ograniczenia (O), tym mniej
  bezużytecznych wyników.
- Planując wyjazd dla organizacji, pamiętaj o wewnętrznych zasadach
  rozliczania kosztów – najtańsza opcja nie zawsze jest tą dopuszczalną.

## Notatki własne

- Czy cena w serwisie zgadzała się z tą podaną przez Claude?
- Ile czasu zajęłoby Ci to samo porównanie ręcznie?
