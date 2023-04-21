<h1>Typy zmienne</h1>
W języku C++ istnieją różne typy zmiennych, które mogą przechowywać różne rodzaje danych. Poniżej przedstawiamy najważniejsze typy zmiennych w C++:

<br>
<br>
Liczby całkowite (int):
Liczby całkowite to liczby bez części dziesiętnej. W C++ można je przechowywać w zmiennych typu "int". Na przykład:

```
int liczba = 10;
```
<br>

Liczby zmiennoprzecinkowe (float i double):
Liczby zmiennoprzecinkowe to liczby z częścią dziesiętną. W C++ można je przechowywać w zmiennych typu "float" lub "double". Typ "double" jest bardziej precyzyjny niż "float", ale zajmuje więcej pamięci. Na przykład:

```
float cena = 4.99;
double dokladna_cena = 4.9975;
```
<br>
Znaki (char):
Znaki to pojedyncze litery, cyfry lub znaki specjalne. W C++ można je przechowywać w zmiennych typu "char". Na przykład:

```
char litera = 'a';
```
<br>
Ciągi znaków (string):
Ciągi znaków to ciągi liter, cyfr lub znaków specjalnych. W C++ można je przechowywać w zmiennych typu "string". Na przykład:

```
string imie = "Anna";
```
<br>
Wartości logiczne (bool):
Wartości logiczne to wartości "prawda" lub "fałsz". W C++ można je przechowywać w zmiennych typu "bool". Na przykład:

```
bool czy_poprawne = true;
```
<br>
Wskaźniki (pointer):
Wskaźniki to zmienne przechowujące adres pamięci komputera. W C++ można je przechowywać w zmiennych typu "pointer". Na przykład:

```
int *wskaznik = nullptr;
```
<br>
Pamiętaj, że w C++ musisz określić typ zmiennej przed użyciem. Możesz także zmieniać wartość zmiennych w dowolnym momencie programu.


W C++ istnieje wiele konkretnych typów zmiennych, z których każdy ma swoją wielkość, zakres wartości i miejsce na dysku. Poniżej przedstawiam kilka najpopularniejszych typów zmiennych:

### Typy całkowite

Typy całkowite to zmienne, które przechowują liczby całkowite (bez części dziesiętnej). Najpopularniejszymi typami całkowitymi w C++ są:

- **int**: zmienna całkowita o wielkości 4 bajtów (32 bity) i zakresie wartości od -2 147 483 648 do 2 147 483 647 (włącznie).
- **short int**: zmienna całkowita o wielkości 2 bajtów (16 bitów) i zakresie wartości od -32 768 do 32 767 (włącznie).
- **long int**: zmienna całkowita o wielkości 4 lub 8 bajtów (32 lub 64 bity) i zakresie wartości od -2 147 483 648 do 2 147 483 647 (dla 32-bitowej architektury) lub od -9 223 372 036 854 775 808 do 9 223 372 036 854 775 807 (dla 64-bitowej architektury).
- **unsigned int**: zmienna całkowita o wielkości 4 bajtów (32 bity) i zakresie wartości od 0 do 4 294 967 295 (włącznie).
- **unsigned short int**: zmienna całkowita o wielkości 2 bajtów (16 bitów) i zakresie wartości od 0 do 65 535 (włącznie).
- **unsigned long int**: zmienna całkowita o wielkości 4 lub 8 bajtów (32 lub 64 bity) i zakresie wartości od 0 do 4 294 967 295 (dla 32-bitowej architektury) lub od 0 do 18 446 744 073 709 551 615 (dla 64-bitowej architektury).

### Typy zmiennoprzecinkowe

Typy zmiennoprzecinkowe to zmienne, które przechowują liczby zmiennoprzecinkowe (z częścią dziesiętną). Najpopularniejszymi typami zmiennoprzecinkowymi w C++ są:

- **float**: zmienna zmiennoprzecinkowa o wielkości 4 bajtów (32 bity) i zakresie wartości około ±3.4 × 10^-38 do ±3.4 × 10^38.
- **double**: zmienna zmiennoprzecinkowa o wielkości 8 bajtów (64 bity) i zakresie wartości około ±1.7 × 10^-308 do ±1.7 × 10^308.
- **long double**: zmienna zmiennoprzecinkowa o większej precyzji niż double, o wielkości 8 lub 16 bajtów (64 lub 128 bitów) i zakresie wartości około ±1.- 1.1 × 10^-4932 do ±1.1 × 10^4932.

### Typy logiczne

Typy logiczne to zmienne, które przechowują wartość logiczną true (prawda) lub false (fałsz). W C++ istnieje jeden typ logiczny, który nazywa się bool. Bool zajmuje 1 bajt na dysku i może przyjąć tylko dwie wartości: true lub false.

### Typy znakowe

Typy znakowe to zmienne, które przechowują pojedyncze znaki, np. litery alfabetu, cyfry, znaki interpunkcyjne itp. W C++ istnieją dwa typy znakowe:

- **char**: zmienna znakowa o wielkości 1 bajta i zakresie wartości od -128 do 127 (dla typu signed char) lub od 0 do 255 (dla typu unsigned char).
- **wchar_t**: zmienna znakowa o większej pojemności niż char, o wielkości 2 lub 4 bajtów (16 lub 32 bity) i zakresie wartości od 0 do 65 535 (dla typu wchar_t).

### Podsumowanie

W C++ istnieje wiele konkretnych typów zmiennych, z których każdy ma swoją wielkość, zakres wartości i miejsce na dysku. Warto wybierać odpowiedni typ zmiennej w zależności od jej przeznaczenia, aby uniknąć nieprzewidywalnych efektów i zapewnić poprawne działanie programu.