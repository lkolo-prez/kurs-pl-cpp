Witajcie w lekcji dotyczącej operacji matematycznych w języku C++!
<h1>Operacje Matematyczne</h1>
W języku C++ istnieją podstawowe operacje matematyczne, które pozwalają na wykonywanie różnych działań na liczbach.

1. Dodawanie (+): Służy do dodawania dwóch liczb. 
 Przykład: `int a = 5, b = 3; int c = a + b;` 
 (zmienna c będzie miała wartość 8).
<br>

2. Odejmowanie (-): Służy do odejmowania jednej liczby od drugiej. 
   Przykład: `int a = 5, b = 3; int c = a - b;` 
   (zmienna c będzie miała wartość 2).
<br>

3. Mnożenie (*): Służy do mnożenia dwóch liczb. 
   Przykład: `int a = 5, b = 3; int c = a * b;` 
   (zmienna c będzie miała wartość 15).
<br>

4. Dzielenie (/): Służy do dzielenia jednej liczby przez drugą. 
   Przykład: `int a = 10, b = 2; int c = a / b;` 
(zmienna c będzie miała wartość 5).
<br>

5. Reszta z dzielenia (%): Służy do obliczania reszty z dzielenia dwóch liczb. 
   Przykład: `int a = 10, b = 3; int c = a % b;` 
    (zmienna c będzie miała wartość 1, ponieważ reszta z dzielenia 10 przez 3 wynosi 1).
<br>

W języku C++ dostępne są również inne operacje matematyczne, takie jak potęgowanie (pow), pierwiastkowanie (sqrt), funkcje trygonometryczne (sin, cos, tan) czy logarytmy (log, log10). Aby korzystać z tych funkcji, należy dołączyć bibliotekę \<cmath>.
<br>

Przykładowy kod wykorzystujący funkcję potęgowania:
```cpp
#include <iostream>
#include <cmath>

int main() {
    double a = 2, b = 3;
    double c = pow(a, b); // potęgowanie
    std::cout << "Wynik potęgowania " << a << " do potęgi " << b << " to " << c << std::endl;

    return 0;
}
```

<h2></h2>

1) Napisz program, który odczytuje długość podstawy i wysokość trójkąta i oblicza jego pole.

2) Napisz program, który odczytuje długość boków prostokąta i oblicza jego pole i obwód.

3) Napisz program, który odczytuje długość promienia koła i oblicza jego pole i obwód.

4) Napisz program, który odczytuje długość boku kwadratu i oblicza jego pole i obwód.

5) Napisz program, który odczytuje dwie liczby i wykonuje na nich jedno z działań matematycznych (dodawanie, odejmowanie, mnożenie lub dzielenie). Wyświetl wynik.

6) Napisz program, który odczytuje dwie liczby i wyświetla większą z nich.

7) Napisz program, który odczytuje trzy liczby i wyświetla średnią arytmetyczną.

8) Napisz program, który odczytuje liczbę i oblicza jej pierwiastek kwadratowy.

9) Napisz program, który odczytuje trzy liczby i wyświetla największą i najmniejszą z nich.

10) Napisz program, który odczytuje długość boków trójkąta i oblicza jego obwód i pole za pomocą wzoru Herona.
