# Zadanie 2: Plany i limity – darmowa wersja Claude a Claude Code

**Cel:** zrozumieć, co obejmuje darmowy plan claude.ai, czym różni się od
planów płatnych oraz czym jest Claude Code (narzędzie CLI dla
programistów) i dlaczego nie jest dostępne za darmo.
**Poziom:** podstawowy

## Materiały

- Przeglądarka i strona [claude.ai/pricing](https://claude.ai/pricing).
- Własne konto Claude (z zadania 1).

## Kroki

1. Wejdź na [claude.ai/pricing](https://claude.ai/pricing) i porównaj
   dostępne plany (Free, Pro, Max, Team, Enterprise).
2. W swoim koncie sprawdź, na jakim planie obecnie pracujesz (ikona/avatar
   w lewym dolnym rogu).
3. Przeczytaj poniższą ściągawkę i zastanów się, czy Twoje dotychczasowe
   użycie Claude mieściło się w limitach darmowego planu.

## Ściągawka: co obejmuje darmowa wersja Claude (claude.ai)

**Objęte:**

- Czat na web/iOS/Android/desktop, dostęp do modeli **Sonnet i Haiku**
  (najmocniejszy model Opus wymaga planu płatnego) – z wyraźnie niższymi
  limitami niż w planach płatnych.
- Okno kontekstu: **200k tokenów** (tyle samo co w planach płatnych).
- Web search, pamięć między rozmowami, tworzenie plików i wykonywanie
  kodu, generowanie treści/wizualizacji danych.
- Rozszerzone myślenie (extended thinking) do trudniejszych zadań.
- Integracje ze Slack, Google Workspace, konektory MCP, rozszerzenia
  desktopowe.

**Limity liczby wiadomości:** Anthropic nie podaje sztywnej liczby (np.
"X wiadomości dziennie") – limity są dynamiczne i zależą od obciążenia
serwerów. Plan Pro ma limity wielokrotnie wyższe niż plan darmowy; limit
odnawia się co kilka godzin.

**Czego NIE ma w darmowym planie:** dostępu do Claude Code CLI – to
zaczyna się dopiero od planu **Pro**.

## Ściągawka: Claude Code CLI – ile tokenów?

Nie ma jednej odpowiedzi "X tokenów" – zależy od sposobu autoryzacji:

| Sposób dostępu | Jak liczone są limity |
|---|---|
| **Plan Pro/Max/Team/Enterprise** (logowanie przez `/login`) | Limit "miejsca" (seat allowance) w oknie **5-godzinnym** i **tygodniowym**, współdzielony z czatem Claude i Cowork. Konkretna liczba tokenów zależy od poziomu miejsca (Standard/Premium) i nie jest podana jako sztywna liczba – zużycie widać komendą `/usage` w CLI. |
| **Klucz API** (Claude Console, pay-as-you-go) | Brak górnego limitu poza budżetem, który sam ustawisz (workspace spend limits); płacisz za każdy token wg cennika API. |
| **Amazon Bedrock / Vertex / Foundry** | Rozliczane per token przez dostawcę chmury. |

Orientacyjny koszt dla firm (dane Anthropic): ok. **13 USD/dzień** i
**150–250 USD/miesiąc** na aktywnego developera (90% użytkowników poniżej
30 USD/dzień) – to zużycie tokenów API, nie darmowy limit.

**Podsumowanie:** Claude Code nie działa w ogóle na darmowym koncie –
wymaga minimum planu Pro (limity odnawiane w oknach 5-godzinnych
i tygodniowych, bez sztywnej liczby tokenów) albo płatnego klucza API
(bez górnego limitu, płatność za tokeny).

## Na co zwrócić uwagę

- Darmowy plan w zupełności wystarcza do zadań z tego warsztatu (czat,
  analiza dokumentów, pisanie) – limit dotyczy liczby wiadomości, nie
  funkcji.
- Limity i ceny zmieniają się – warto zawsze sprawdzić aktualny stan na
  [claude.ai/pricing](https://claude.ai/pricing) przed szkoleniem.

## Notatki własne

- Na jakim planie pracujesz na co dzień?
- Czy limit wiadomości darmowego planu kiedykolwiek Ci przeszkodził?
