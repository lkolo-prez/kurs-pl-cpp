# 3. Instrukcje sterujące

Instrukcje sterujące są fundamentalnym elementem każdego języka programowania. Pozwalają one na kontrolowanie przepływu programu i podejmowanie decyzji w zależności od spełnienia określonych warunków.

## 3.1. Instrukcja warunkowa `if`

Instrukcja `if` pozwala na wykonanie określonego bloku kodu, jeśli spełniony jest dany warunek.

```cpp
int a = 10;
if (a > 5) {
    std::cout << "a jest większe od 5" << std::endl;
}
```

## 3.2. Instrukcja `else`

Instrukcja `else` służy do wykonania bloku kodu, gdy warunek w instrukcji `if` nie jest spełniony.

```cpp
int a = 10;
if (a > 15) {
    std::cout << "a jest większe od 15" << std::endl;
} else {
    std::cout << "a jest mniejsze lub równe 15" << std::endl;
}
```

## 3.3. Instrukcja `else if`

Instrukcja `else if` umożliwia dodanie dodatkowych warunków do instrukcji `if`.

```cpp
int a = 10;
if (a > 15) {
    std::cout << "a jest większe od 15" << std::endl;
} else if (a > 5) {
    std::cout << "a jest większe od 5, ale mniejsze lub równe 15" << std::endl;
} else {
    std::cout << "a jest mniejsze lub równe 5" << std::endl;
}
```

## 3.4. Instrukcja `switch`

Instrukcja `switch` jest alternatywą dla instrukcji `if`, która pozwala na porównanie jednej zmiennej/ wyrażenia z wieloma wartościami.

```cpp
int a = 2;
switch (a) {
    case 1:
        std::cout << "a jest równe 1" << std::endl;
        break;
    case 2:
        std::cout << "a jest równe 2" << std::endl;
        break;
    default:
        std::cout << "a nie jest równe ani 1, ani 2" << std::endl;
        break;
}
```

## 3.5. Pętle

Pętle są używane do wielokrotnego wykonania bloku kodu. C++ obsługuje trzy rodzaje pętli: `for`, `while` i `do while`.

- Pętla `for`

```cpp
for (int i = 0; i < 10; i++) {
    std::cout << i << std::endl;
}
```

- Pętla `while`

```cpp
int i = 0;
while (i < 10) {
    std::cout << i << std::endl;
    i++;
}
```

- Pętla `do while`

```cpp
int i = 0;
do {
    std::cout << i << std::endl;


    i++;
} while (i < 10);
```

Wszystkie te pętle mogą być kontrolowane za pomocą instrukcji `break` (kończy pętlę przedwcześnie) i `continue` (przechodzi do następnej iteracji pętli).

Te podstawowe instrukcje sterujące są niezbędne do tworzenia skomplikowanych programów w C++. Istnieje jednak wiele bardziej zaawansowanych technik sterowania przepływem, takich jak obsługa wyjątków i skoki goto.