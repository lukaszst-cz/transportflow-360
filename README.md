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

Projekt rozwijany jest w trzech czytelnie rozdzielonych warstwach:

- **TransportFlow 360 — publiczne demo 20/26**: frontend procesu, 9 widoków ról, portal PWA, kalkulator stawki, case study i skoroszyt demonstracyjny dla 20 zestawów oraz 26 kierowców;
- **TransportFlow Python/SQLite — prototyp backendu 20/26**: osobne repozytorium z API, modelem danych SQLite i automatycznymi testami dla tego samego modelu operacyjnego;
- **TransportFlow Control Center — rozszerzony model 50/58**: rozwijany w głównym portfolio wariant React/TypeScript/Cloudflare dla 50 zestawów i 58 kierowców, z CRM, dokumentami, finansami, rolami i KPI.

Dane publiczne są syntetyczne. Warstwy demonstracyjne pokazują proces, architekturę i zakres odpowiedzialności użytkowników, ale nie zastępują produkcyjnego TMS z uwierzytelnianiem, RBAC i integracjami z systemami zewnętrznymi.

## Co działa

- portal PWA z 9 widokami ról i deep-linkami do wybranej roli;
- przebieg zlecenia, kalkulator stawki, flota, dokumenty i KPI;
- skoroszyt `TransportFlow_360_demo.xlsx`;
- automatyczne QA w GitHub Actions: składnia JS, mobile, role, PWA, kalkulator i lokalne odsyłacze;
- osobny backend Python/SQLite oraz rozszerzony Control Center jako kolejne etapy rozwoju koncepcji.

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
