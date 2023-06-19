# 2. Zmienne

Zmienne są podstawowym elementem każdego języka programowania. W języku C++ zmienne są miejscem w pamięci, gdzie możemy przechowywać dane. Przy deklarowaniu zmiennej, określamy jej typ, co pozwala kompilatorowi na zaalokowanie odpowiedniej ilości pamięci dla tej zmiennej.

## 2.1. Deklaracja i inicjalizacja

W języku C++ zmienną deklarujemy, podając najpierw jej typ, a potem nazwę. Możemy również od razu przypisać jej wartość, co nazywamy inicjalizacją.

```cpp
int liczba;          // Deklaracja
liczba = 10;         // Inicjalizacja

double liczba2 = 20.0;    // Deklaracja i inicjalizacja
```

## 2.2. Typy zmiennych

C++ jest językiem statycznie typowanym, co oznacza, że typ każdej zmiennej musi być znany w czasie kompilacji. Istnieje wiele typów zmiennych w C++, w tym:

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

## 2.3. Zakres zmiennych

Zakres zmiennej określa, gdzie zmienna jest dostępna w kodzie. W C++ mamy trzy podstawowe zakresy:

- Lokalny: Zmienne zadeklarowane wewnątrz bloku lub listy parametrów funkcji są lokalne dla tego bloku lub funkcji.
- Globalny: Zmienne zadeklarowane poza wszystkimi funkcjami są globalne.
- Formalny: Zmienne używane w listach parametrów funkcji są formalnymi parametrami.

## 2.4. Stałe i definicje

Stałe są typem zmiennej, której wartość nie może być zmieniona po inicjalizacji. Możemy zadeklarować stałe używając słowa kluczowego `const`.

```cpp
const int LICZBA = 10;
```

Definicje (`#define`) są również używane do deklarowania stałych, ale są przetwarzane przez preprocesor, a nie przez kompilator, i nie mają określonego typu.

```cpp
#define LICZBA 10
```

Te są podstawowe informacje na temat zmiennych w C++. Jest jeszcze wiele do nauczenia się na temat zmiennych, w

tym modyfikatory typów, kwalifikatory typów, wskaźniki, referencje i wiele innych.