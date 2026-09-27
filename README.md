# TransportFlow 360

**Problem:** w transporcie informacje o zapytaniu, wycenie, aucie, dokumentach i płatności łatwo rozchodzą się między telefonem, Excelem i wiadomościami.

**Rozwiązanie:** demonstracja jednego procesu od zapytania ofertowego i kalkulacji stawki do realizacji przewozu, dokumentów, faktury oraz płatności.

[Otwórz działające demo](https://lukaszst-cz.github.io/transportflow-360/)

## Szybki podgląd

- [Portal operacyjny](https://lukaszst-cz.github.io/transportflow-360/portal/)
- [Widok właściciela / administratora](https://lukaszst-cz.github.io/transportflow-360/portal/?role=manager)
- [Kalkulator stawki](https://lukaszst-cz.github.io/transportflow-360/kalkulator.html)
- [Case study](https://lukaszst-cz.github.io/transportflow-360/case-study.html)

Uzupełniający backend demonstracyjny Python + SQLite: https://github.com/lukaszst-cz/transportflow-control-center

## Architektura demonstracji

- **TransportFlow 360** — publiczny frontend procesu, portal PWA, kalkulator, case study i skoroszyt demonstracyjny;
- **TransportFlow Control Center** — osobny backend demonstracyjny Python + SQLite z API i modelem danych;
- dane publiczne są syntetyczne, a frontend portfolio nie zapisuje ich do zewnętrznej bazy;
- część publiczna pokazuje przebieg procesu i role, a Control Center pokazuje warstwę aplikacyjną i dane.

## Co działa

- portal PWA z przebiegiem zlecenia;
- kalkulator, widok floty i kontrola dokumentów;
- skoroszyt `TransportFlow_360_demo.xlsx`;
- materiały kontroli jakości i dane demonstracyjne.

## Wartość biznesowa

- mniej ręcznego przepisywania danych między etapami;
- szybsza wycena i kompletowanie wymaganych informacji;
- prostsza kontrola marży, terminów oraz dokumentów;
- jeden, czytelny punkt odniesienia dla dyspozytora i właściciela.

## Dla kogo

Dla firm transportowych, spedycyjnych i usług z własną flotą.

## Ważne

Trasy, kwoty, identyfikatory i dane operacyjne są syntetyczne. Projekt to demonstracja procesu, nie gotowy system produkcyjny.

## Kontrola jakości

Repozytorium sprawdza składnię JavaScript oraz kompletność kluczowych stron, ról, modułów i lokalnych odsyłaczy w GitHub Actions.

## Uruchomienie

Otwórz `index.html` w przeglądarce. Pełny przykład Excel znajduje się w `assets/`. Portal PWA najlepiej testować przez działające demo HTTPS, ponieważ service worker wymaga bezpiecznego kontekstu.
