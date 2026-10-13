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
- za pomocą `expect()` sprawdzić, czy wyświetlana jest wartość `rocket`,
- uruchomić testy i upewnić się, że nowy test oraz pozostałe testy projektu przechodzą poprawnie.
Test powinien sprawdzać rezultat widoczny w DOM-ie, a nie bezpośrednio wartość przekazaną do inputu `card`.

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
