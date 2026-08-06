# Zadanie 3: Connections – podłączenie usług i praca z Gmailem

**Cel:** podłączyć do Claude pierwszą usługę zewnętrzną (Gmail) i wykonać
realne zadanie na własnej skrzynce – wyszukanie wiadomości i przygotowanie
odpowiedzi.
**Poziom:** średniozaawansowany

## Materiały

- Konto Claude z [zadania 1](01-formula-pkzo.md).
- Konto Gmail (to samo, którego używasz do NotebookLM).

**Connections działają na darmowym planie** – podlegają jedynie zwykłym
limitom wiadomości opisanym w [zadaniu 2](02-plany-i-limity.md).

## Zanim zaczniesz – zasady bezpieczeństwa

Podłączenie usługi daje Claude dostęp do Twoich prywatnych danych. Zanim
klikniesz "Połącz":

1. **Podłączaj wyłącznie własne konta** – nigdy cudzej skrzynki ani konta
   służbowego bez zgody pracodawcy.
2. **Przeczytaj ekran zgód** – zobaczysz tam, do czego dokładnie
   przyznajesz dostęp. To ten sam mechanizm, co przy logowaniu przez Google
   do innych aplikacji.
3. **Po szkoleniu odłącz usługi**, jeśli ćwiczysz na komputerze, który nie
   jest Twój – instrukcja na końcu tego zadania.

## Kroki

### Część 1: Podłączenie Gmaila

1. W oknie rozmowy kliknij przycisk **"Search and tools"** (w lewym dolnym
   rogu, przy polu wpisywania wiadomości).
2. Wybierz **"Add connectors"** – zobaczysz katalog dostępnych usług.
   Możesz też wejść bezpośrednio na
   [claude.ai/customize/connectors](https://claude.ai/customize/connectors).
3. Znajdź **Gmail** i kliknij **"Connect"**.
4. Zaloguj się kontem Google i zaakceptuj zakres uprawnień.
5. Wróć do rozmowy – w menu "Search and tools" Gmail powinien być
   zaznaczony jako aktywny.

### Część 2: Realne zadanie na skrzynce

6. Poproś Claude o przeszukanie skrzynki, np.:
   *"Znajdź w mojej skrzynce wiadomości z ostatnich 7 dni, na które jeszcze
   nie odpowiedziałem/am, i wypisz je w tabeli: nadawca, temat, czego
   dotyczy."*
7. Wybierz jedną wiadomość i poproś o przygotowanie odpowiedzi, używając
   formuły P.K.Z.O. z zadania 1, np.:

   > **P:** Jesteś asystentem pomagającym w prowadzeniu korespondencji.
   > **K:** Odpowiadam na wiadomość dotyczącą organizacji wolontariatu.
   > **Z:** Przygotuj wersję roboczą odpowiedzi w Gmailu.
   > **O:** Ton uprzejmy, ale konkretny, maksymalnie 150 słów, po polsku.

8. Otwórz Gmaila i sprawdź, czy wersja robocza (draft) faktycznie się
   pojawiła.
9. Przeczytaj ją uważnie, popraw co trzeba – i dopiero wtedy zdecyduj, czy
   ją wysłać.

## Na co zwrócić uwagę

- **Claude nie wyśle e-maila za Ciebie.** Integracja z Gmailem pozwala
  czytać wiadomości i tworzyć wersje robocze, ale wysyłkę zawsze wykonujesz
  samodzielnie w Gmailu. To celowe zabezpieczenie – ostatnie słowo należy
  do człowieka.
- Zawsze przeczytaj wygenerowaną wersję roboczą przed wysłaniem. AI może
  źle zrozumieć kontekst wiadomości albo pominąć coś ważnego.
- Wyniki zależą od tego, jak precyzyjnie opiszesz, czego szukasz –
  formuła P.K.Z.O. działa tu tak samo dobrze jak w zwykłej rozmowie.

## Jak odłączyć usługę

1. Wejdź w **Ustawienia → Connectors** na [claude.ai](https://claude.ai)
   i kliknij **"Disconnect"** przy wybranej usłudze.
2. Dodatkowo możesz cofnąć dostęp po stronie Google:
   [myaccount.google.com/permissions](https://myaccount.google.com/permissions).

Zrób to koniecznie, jeśli ćwiczyłeś/aś na komputerze szkoleniowym lub
współdzielonym.

## Notatki własne

- Ile czasu zajęłoby Ci ręczne znalezienie tych samych wiadomości?
- Czy wersja robocza nadawała się do wysłania bez poprawek, czy wymagała
  zmian? Jakich?
