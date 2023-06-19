# C++

## Spis treści
1. [Podstawy](#podstawy)
2. [Zmienne](#zmienne)
3. [Kontrola przepływu](#kontrola_przeplywu)
4. [Funkcje](#funkcje)
5. [Tablice](#tablice)
6. [Wskaźniki](#wskazniki)
7. [Struktury, klasy i obiekty](#struktury_klasy_obiekty)

<a name="podstawy"></a>
## 1. Podstawy

```cpp
#include <iostream>

// Komentarz jednoliniowy

/* 
Komentarz wieloliniowy
*/

int main() {
    std::cout << "Witaj, świecie!" << std::endl;
    return 0;
}
```

<a name="zmienne"></a>
## 2. Zmienne

```cpp
int liczba = 10;          // Integer
double liczba2 = 20.0;    // Double
char znak = 'A';          // Char
bool prawda = true;       // Boolean
std::string napis = "Hello"; // String
```

<a name="kontrola_przeplywu"></a>
## 3. Kontrola przepływu

### If, else if, else

```cpp
int liczba = 10;

if (liczba > 10) {
    std::cout << "Liczba jest większa od 10" << std::endl;
} else if (liczba < 10) {
    std::cout << "Liczba jest mniejsza od 10" << std::endl;
} else {
    std::cout << "Liczba jest równa 10" << std::endl;
}
```

### Pętla for

```cpp
for(int i = 0; i < 10; i++) {
    std::cout << i << std::endl;
}
```

### Pętla while

```cpp
int i = 0;

while(i < 10) {
    std::cout << i << std::endl;
    i++;
}
```

<a name="funkcje"></a>
## 4. Funkcje

```cpp
// Definicja funkcji
void mojaFunkcja() {
    std::cout << "Witaj z funkcji!" << std::endl;
}

// Użycie funkcji
int main() {
    mojaFunkcja();
    return 0;
}
```

<a name="tablice"></a>
## 5. Tablice

```cpp
int tablica[5] = {1, 2, 3, 4, 5};

for(int i = 0; i < 5; i++) {
    std::cout << tablica[i] << std::endl;
}
```

<a name="wskazniki"></a>
## 6. Wskaźniki

```cpp
int liczba = 10;
int *wskaznik = &liczba; // wskaznik do liczby

std::cout << *wskaznik << std::endl; // wyświetl

wartość na którą wskazuje wskaźnik
```

<a name="struktury_klasy_obiekty"></a>
## 7. Struktury, klasy i obiekty

### Struktury

```cpp
struct Osoba {
    std::string imie;
    int wiek;
};

Osoba osoba1 = {"Jan", 20};
```

### Klasy i obiekty

```cpp
class Samochod {
    public:
        std::string marka;
        int rokProdukcji;

        void pokazDane() {
            std::cout << "Marka: " << marka << ", Rok produkcji: " << rokProdukcji << std::endl;
        }
};

Samochod samochod1;
samochod1.marka = "Toyota";
samochod1.rokProdukcji = 2005;
samochod1.pokazDane();
```
To są podstawy składni C++. Jest wiele innych zaawansowanych tematów takich jak dziedziczenie, polimorfizm, szablony, obsługa wyjątków, które nie zostały tutaj uwzględnione. Daj mi znać, jeśli chcesz więcej informacji na te tematy.

# 1. Podstawy

Programy w C++ składają się z funkcji i zmiennych, które są zorganizowane w plikach. 

## 1.1. Struktura programu

```cpp
#include <iostream>

int main() {
    std::cout << "Witaj, świecie!" << std::endl;
    return 0;
}
```

- `#include <iostream>`: Preprocesor C++ wykonuje instrukcje zaczynające się od "#". Instrukcja `#include` kieruje preprocesor do włączenia treści określonego pliku do kodu źródłowego. W tym przypadku `iostream` jest standardową biblioteką wejścia/wyjścia w C++, która umożliwia operacje wejścia/wyjścia.

- `int main()`: C++ wykonuje programy zaczynając od funkcji `main()`. Funkcja ta musi zwracać wartość typu int (która jest zazwyczaj 0 na koniec programu), stąd `int` przed `main`.

- `std::cout << "Witaj, świecie!" << std::endl;`: `std::cout` jest obiektem strumienia wyjścia, który zazwyczaj wypisuje na ekran. Operator `<<` jest operatorem wstawiania, który wstawia ciąg "Witaj, świecie!" do strumienia. `std::endl` jest manipulatorem strumienia, który wstawia nową linię i opróżnia strumień.

- `return 0;`: Instrukcja `return` kończy wykonanie funkcji `main()` i zwraca wartość 0.

## 1.2. Komentarze

```cpp
// Komentarz jednoliniowy

/* 
Komentarz wieloliniowy
*/
```

- Komentarze są używane do wyjaśnienia kodu źródłowego i ignorowane są podczas kompilacji. C++ obsługuje komentarze jedno i wieloliniowe.

## 1.3. Typy danych

C++ posiada następujące typy danych:

- Typy całkowite: `int`, `short`, `long`, `long long`
- Typy zmiennoprzecinkowe: `float`, `double`, `long double`
- Typy znakowe: `char`
- Typy logiczne: `bool`
- Typy złożone: `string`, `array`, `vector`, `class`, `struct`, etc.

```cpp
int liczba = 10;          // Integer
double liczba2 = 20.0;    // Double
char znak = 'A';          // Char
bool prawda = true;       // Boolean
std::string napis = "Hello"; // String
```

## 1.4. Operatory

C++ posiada wiele operatorów, które można użyć do manipulowania zmiennymi, takie jak:

- Operatory arytmetyczne: `+`, `-`, `*`, `/`, `%`
- Operatory przypisania: `=`, `+=`, `-=`, `*=`, `/=`, `%=`
- Operatory porównania:

`==`, `!=`, `<`, `>`, `<=`, `>=`
- Operatory logiczne: `&&`, `||`, `!`

```cpp
int a = 10;
int b = 20;

// Operator arytmetyczny
int c = a + b; // 30

// Operator przypisania
a += b; // a = a + b, a = 30

// Operator porównania
bool wynik = a == b; // false

// Operator logiczny
bool wynik2 = (a == b) || (a > b); // true
```

## 1.5. Wejście / wyjście

Standardowa biblioteka C++ zapewnia metody do obsługi wejścia i wyjścia.

- Wyjście: `std::cout` służy do wyświetlania tekstu na ekranie. Można użyć operatora `<<` do wstawiania danych do `cout`.

```cpp
std::cout << "Witaj, świecie!" << std::endl;
```

- Wejście: `std::cin` służy do odczytywania danych z wejścia klawiatury. Można użyć operatora `>>` do wyjęcia danych z `cin`.

```cpp
int liczba;
std::cout << "Podaj liczbę: ";
std::cin >> liczba;
```

To są podstawowe informacje na temat podstaw C++. C++ jest bardzo bogatym językiem z wieloma funkcjami, więc jest jeszcze wiele do nauczenia się poza tymi podstawami.