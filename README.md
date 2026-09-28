# TransportFlow 360

W transporcie część informacji zwykle żyje w Excelu, część w telefonie, a część w wiadomościach. TransportFlow 360 zbiera to w jeden prosty model: od wyceny i przydziału auta po dokumenty, realizację, dostawę i rozliczenie.

[Otwórz działające demo](https://lukaszst-cz.github.io/transportflow-360/)

## Szybki podgląd

- [Portal operacyjny](https://lukaszst-cz.github.io/transportflow-360/portal/)
- [Widok właściciela / administratora](https://lukaszst-cz.github.io/transportflow-360/portal/?role=manager)
- [Kalkulator stawki](https://lukaszst-cz.github.io/transportflow-360/kalkulator.html)
- [Case study](https://lukaszst-cz.github.io/transportflow-360/case-study.html)

Uzupełniający backend demonstracyjny Python + SQLite: https://github.com/lukaszst-cz/transportflow-control-center

## Jak projekt jest podzielony

- **TransportFlow 360** — publiczne demo dla 20 zestawów i 26 kierowców. Zawiera portal PWA, 9 widoków ról, kalkulator, case study i skoroszyt Excel.
- **TransportFlow Python/SQLite** — prosty backend demo dla tej samej wersji 20/26, z API i testami.
- **TransportFlow Control Center** — większa wersja w React/TypeScript/Cloudflare dla 50 zestawów i 58 kierowców, z CRM, dokumentami, finansami i KPI.

Wszystkie dane są przykładowe. To demonstracja procesu i architektury, a nie gotowy TMS do pracy na danych firmowych.

## Co działa

- portal PWA z 9 widokami ról i deep-linkami do wybranej roli;
- przebieg zlecenia, kalkulator stawki, flota, dokumenty i KPI;
- skoroszyt `TransportFlow_360_demo.xlsx`;
- automatyczne QA w GitHub Actions: składnia JS, mobile, role, PWA, kalkulator i lokalne odsyłacze;
- osobny backend Python/SQLite oraz rozszerzony Control Center jako kolejne etapy rozwoju koncepcji.

## Po co ten projekt

- mniej przepisywania tych samych danych w kilku miejscach;
- prostsza wycena i kontrola kosztu zlecenia;
- terminy i dokumenty w jednym miejscu;
- wspólny widok dla dyspozytora i osoby zarządzającej.

## Dla kogo

Dla firm transportowych, spedycyjnych i usług z własną flotą.

## Ważne

Trasy, kwoty, identyfikatory i dane operacyjne są syntetyczne. Projekt to demonstracja procesu, nie gotowy system produkcyjny.

## Kontrola jakości

Repozytorium sprawdza składnię JavaScript oraz kompletność kluczowych stron, ról, modułów i lokalnych odsyłaczy w GitHub Actions.

## Uruchomienie

Otwórz `index.html` w przeglądarce. Pełny przykład Excel znajduje się w `assets/`. Portal PWA najlepiej testować przez działające demo HTTPS, ponieważ service worker wymaga bezpiecznego kontekstu.
