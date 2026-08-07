# Zadanie 1: Pierwsza rozmowa z Gemini

**Cel:** poznać podstawowy przepływ pracy w Gemini – zalogowanie się,
zadanie pierwszych pytań, wgranie pliku – i porównać styl odpowiedzi z
Claude z wcześniejszego zadania.
**Poziom:** podstawowy

## Materiały

Konto Google i przeglądarka – instrukcja logowania znajduje się w
[README](README.md#jak-zacząć-pracę-z-gemini-przeglądarka).

## Co jest darmowe: przeglądarka i CLI

Gemini ma dwie postacie i **obie działają bez płacenia**:

| | Gdzie | Co daje darmowy plan |
|---|---|---|
| **Gemini w przeglądarce** | [gemini.google.com](https://gemini.google.com) | Rozmowa, wgrywanie plików, generowanie obrazów. Limit wiadomości i obrazów odnawia się cyklicznie. |
| **Gemini CLI** | terminal na własnym komputerze | Logowanie osobistym kontem Google daje **1000 zapytań dziennie**, bez karty płatniczej. Model dobierany jest automatycznie z rodziny Gemini. |

Do zadań z tego warsztatu limity w zupełności wystarczą – 1000 zapytań
dziennie to znacznie więcej, niż wykorzystasz podczas nauki.

**Warto zapamiętać to porównanie:** Claude Code (terminalowy odpowiednik
u konkurencji, zob.
[zadanie 2 z Claude](../claude-zadania/02-plany-i-limity.md)) wymaga
minimum płatnego planu Pro. Gemini CLI ma realny darmowy próg – to jedna
z niewielu takich ofert wśród narzędzi terminalowych i dobry argument, by
pokazać je osobom, które dopiero zaczynają.

Gemini CLI wymaga jednak zainstalowanego Node.js i pracy w terminalu –
dlatego zaczynamy od przeglądarki, a do CLI wracamy w
[zadaniu 4](04-cli-instalacja.md).

## Kroki

1. Wejdź na [gemini.google.com](https://gemini.google.com) i zaloguj się
   kontem Google.
2. Zadaj to samo pytanie, którego użyłeś/aś w zadaniu P.K.Z.O. z Claude
   (albo dowolne pytanie na temat związany z Twoją pracą lub
   wolontariatem).
3. Wgraj plik – zdjęcie, PDF lub dokument (może być jeden z materiałów
   NotebookLM z folderu
   [`materialy/`](../notebooklm-zadania/materialy/)) – i zapytaj o jego
   zawartość. Gemini odczytuje treść wgranego pliku i odpowiada na jego
   podstawie.
4. Poproś o krótkie podsumowanie w punktach tego, co zawiera plik.

## Na co zwrócić uwagę

- Gemini jest **multimodalny** – oprócz tekstu przyjmuje obrazy, PDF-y i
  (w aplikacji mobilnej) głos.
- Jeśli jesteś zalogowany/a kontem Google używanym też do Gmaila i Dysku,
  w ustawieniach zobaczysz opcję włączenia dostępu do "aplikacji Google"
  (Gmail, Kalendarz, Dysk) – wracamy do niej w [zadaniu 7](07-inne-mozliwosci.md).
- Porównaj odpowiedź Gemini z odpowiedzią Claude na to samo pytanie – różne
  modele AI mają różny "styl": długość odpowiedzi, ton, sposób
  formatowania. Żaden nie jest uniwersalnie "lepszy" – warto znać kilka
  narzędzi i wybierać do zadania.
- Limity darmowych planów zmieniają się – jeśli będziesz prowadzić
  szkolenie z tego materiału, sprawdź aktualny stan przed zajęciami
  i uruchom CLI dzień wcześniej, żeby potwierdzić, że logowanie kontem
  Google przechodzi bez problemu.

## Notatki własne

- Czym różniła się odpowiedź Gemini od odpowiedzi Claude na to samo
  pytanie?
- Co zaskoczyło Cię w odczytaniu wgranego pliku?
