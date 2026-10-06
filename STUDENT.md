# Moje wykonanie Lab00

- Login GitHub / pseudonim: Piotr-Falkowski1
- System i terminal (np. Windows + WSL Ubuntu): Windows
- Edytor / IDE: Windows PowerShell oraz MSYS2 (UCRT64)
- Wersja Git: 2.56.0.windows.1
- Wersja kompilatora C++: (zainstalowany przez MSYS2 / UCRT64)
- Wersje java i javac: openjdk 25.0.4.1
- Link do pierwszego PR (uzupełnij w zadaniu 5): https://github.com/Piotr-Falkowski1/oop-lab00-Piotr-Falkowski1/pull/1

## Uruchomienie lokalne
Wynik programu C++:
```text
Hello from C++! Author: Piotr-Falkowski1
```
Wynik programu Java:
```text
Hello from Java! Author: Piotr-Falkowski1
```

## Błąd i poprawka (zadanie 5)
- Krótki fragment komunikatu błędu i numer linii: cpp/main.cpp:5:68: error: expected ‘;’ before ‘return’
    5 |     std::cout << "Hello from C++! Author: Piotr-Falkowski1" << '\n'
      |                                                                    ^
      |                                                                    ;
    6 |     return 0;
      |     ~~~~~~                                                          
Error: Process completed with exit code 1.
- Przyczyna oraz sposób naprawy: Celowe usunięcie średnika na końcu instrukcji wypisującej tekst. Naprawa polegała na ponownym dopisaniu średnika (';') na końcu tej linii
- Commit z błędem (SHA lub link): c06794a
- Czy Actions pokazały błąd, a po naprawie sukces? Tak, GitHub Actions początkowo zgłosił błąd kompilacji, a po wysłaniu poprawionego kodu proces zakończył się sukcesem na zielono

## Krótkie odpowiedzi
1. Co różni commit od push? ...
    'commit' zapisuje paczkę zmian wyłącznie w lokalnej historii na moim komputerze. Z kolei 'push' wysyła te lokalne zapisy na zdalny serwer (repozytorium GitHub).
2. Dlaczego po scaleniu PR wykonuję lokalnie pull? ...
    Operacja "scalenie" odbywa się na serwerze GitHuba, więc lokalny folder na dysku jeszcze o niej nie wie. Polecenie 'pull' pobiera te zaktualizowane zmiany z serwera na dysk komputera.
3. Co potwierdza zielony wynik naszego CI, a czego nie potwierdza? ...
    Środowisko CI (GitHub Actions) sprawdza jedynie, czy kod z sukcesem się kompiluje i uruchamia na ich serwerach. Nie potwierdza ono jednak wykonania wszystkich poleceń z instrukcji, ani tego, czy środowisko na moim lokalnym komputerze jest poprawnie skonfigurowane

## Ewentualne problemy środowiska
Brak / opis problemu i sposób rozwiązania: ...
