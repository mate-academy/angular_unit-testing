# Moonbase Control: Testy jednostkowe

Zadanie z modułu Angular. Repozytorium zawiera kod startowy aplikacji Moonbase Control dla tej lekcji.

## Zadanie

Rozszerz testy komponentu `Card` o sprawdzenie kolejnego elementu jego widoku.

Komponent otrzymuje przez input również nazwę ikony i wykorzystuje ją podczas renderowania karty. W przygotowanych danych testowych wartość `icon` została ustawiona na `rocket`. Dodaj test, który sprawdzi, czy ta informacja została poprawnie wyrenderowana w UI.

Student powinien:

- utworzyć nowy przypadek testowy w `card.spec.ts`,
- wykorzystać dane przygotowane już w `beforeEach()`,
- za pomocą `fixture.nativeElement` uzyskać dostęp do wyrenderowanego widoku,
- odnaleźć element odpowiedzialny za wyświetlenie ikony,
- za pomocą `expect()` sprawdzić, czy element `mat-icon` ma atrybut `fonticon` o wartości `rocket`,
- uruchomić testy i upewnić się, że nowy test przechodzi poprawnie,
- przejść po pozostałych plikach `*.spec.ts` w aplikacji i spróbować naprawić testy, które nie przechodzą.

Test powinien sprawdzać rezultat widoczny w DOM-ie, a nie bezpośrednio wartość przekazaną do inputu `card`.

💡 Komponent `mat-icon` otrzymuje nazwę ikony przez `[fontIcon]`, a nie jako tekst elementu. Angular Material zapisuje ją w atrybucie `fonticon`, który możesz odczytać za pomocą `getAttribute()`.

💡 Pliki testów wygenerowane przez Angular CLI nie były aktualizowane podczas rozwijania aplikacji. Najczęstsze przyczyny błędów to brakujące zależności komponentu (np. `provideHttpClient()` lub `provideRouter([])` w `providers`) oraz wymagane inputy, którym test nie przekazał wartości (`fixture.componentRef.setInput()`).

## Jak zacząć

1. Zrób fork tego repozytorium na swoje konto GitHub.
2. Sklonuj swój fork na komputer.
3. Zainstaluj zależności: `npm install`.
4. Uruchom aplikację: `npm start`.
5. Jeśli zadanie korzysta z danych z API, uruchom w drugim terminalu mock API: `npm run api`.

## Jak oddać zadanie

1. Zapisz zmiany w commicie i wypchnij je do swojego forka.
2. Otwórz Pull Request z forka do repozytorium `mate-academy/angular_unit-testing`, do brancha `main`.
3. Platforma uruchomi review Twojego Pull Requesta.
