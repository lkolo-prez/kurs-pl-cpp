<h1>Podstawy C++</h1>

**Wprowadzenie do języka C++**
C++ to wszechstronny język programowania, który znalazł zastosowanie w wielu dziedzinach, w tym w tworzeniu aplikacji komputerowych, gier, systemów operacyjnych i oprogramowania wbudowanego. W tym szkoleniu nauczysz się podstaw języka C++, w tym składni, typów danych, instrukcji warunkowych i pętli, funkcji, klas i obiektów, szablonów i algorytmów i struktur danych.
   <br>

**Podstawy programowania w C++**
Składnia języka
Składnia języka C++ obejmuje deklaracje zmiennych, instrukcje warunkowe, pętle, funkcje i wiele innych konstrukcji. W języku C++, kod źródłowy jest zapisywany w plikach z rozszerzeniem .cpp. Aby skompilować i uruchomić kod w C++, potrzebujesz kompilatora, takiego jak GCC lub Clang.
   <br>

Najpopularniejszy kod ***Hello World!***
```
#include <iostream>

int main() {
    std::cout << "Witaj świecie!";
    return 0;
}
```
<br>

***Podstawowe operacje werjścia/wyjścia***
W języku C++ obiekt cout jest obiektem strumienia wyjściowego (ang. output stream), który służy do wyświetlania tekstu i innych wartości na standardowym wyjściu, czyli na ekranie. Obiekt cout jest częścią biblioteki iostream.

Do wyświetlenia wartości na ekranie za pomocą obiektu cout, korzystamy z operatora wstrzykiwania (<<). Przykładowo, jeśli chcemy wyświetlić napis "Hello world" na ekranie, możemy to zrobić w następujący sposób:
```
std::cout << "Hello world" << std::endl;
```

W tym przykładzie, napis "Hello world" jest przekazywany do obiektu cout za pomocą operatora wstrzykiwania (<<), a następnie kończymy linię za pomocą std::endl.
<br>

Z kolei obiekt cin jest obiektem strumienia wejściowego (ang. input stream), który służy do wczytywania danych z wejścia standardowego, czyli od użytkownika lub z pliku. Do wczytania danych za pomocą obiektu cin, korzystamy z operatora wyciągania (>>). Przykładowo, jeśli chcemy wczytać liczbę od użytkownika, możemy to zrobić w następujący sposób:

```
int liczba;
std::cin >> liczba;
```
W tym przykładzie, zmienna "liczba" jest wczytywana z obiektu cin za pomocą operatora wyciągania (>>).
<br>
```
#include <iostream>

int main() {
    int liczba;

    std::cout << "Podaj liczbę całkowitą: ";
    std::cin >> liczba;

    std::cout << "Wczytana liczba to: " << liczba << std::endl;

    return 0;
}
```


<br>

**Zmienne**
Zmienne to podstawowe elementy programowania w C++. Mogą przechowywać różne typy danych, takie jak liczby całkowite, liczby zmiennoprzecinkowe, znaki, łańcuchy znaków i wiele innych. W języku C++, zmienne muszą być zadeklarowane przed ich użyciem, a ich wartości mogą być przypisane za pomocą operatora przypisania (=).
   <br>
```
#include <iostream>
using namespace std;

int main() {
    // Zmienna typu char
    char znak = 'A';
    cout << "Zmienna znakowa: " << znak << endl;

    // Zmienna typu short
    short liczbaShort = 1234;
    cout << "Zmienna short: " << liczbaShort << endl;

    // Zmienna typu int
    int liczbaInt = 123456;
    cout << "Zmienna int: " << liczbaInt << endl;

    // Zmienna typu long
    long liczbaLong = 123456789;
    cout << "Zmienna long: " << liczbaLong << endl;

    // Zmienna typu long long
    long long liczbaLongLong = 1234567890123;
    cout << "Zmienna long long: " << liczbaLongLong << endl;

    // Zmienna typu float
    float liczbaFloat = 3.14f;
    cout << "Zmienna float: " << liczbaFloat << endl;

    // Zmienna typu double
    double liczbaDouble = 3.14159265358979323846;
    cout << "Zmienna double: " << liczbaDouble << endl;

    // Zmienna typu bool
    bool czyPrawda = true;
    cout << "Zmienna bool: " << czyPrawda << endl;

    return 0;
}
```
   <br>

**Pętle**
Pętle umożliwiają powtarzanie określonych czynności w kodzie. W języku C++ istnieją trzy rodzaje pętli: for, while i do-while. Każda z tych pętli ma swoje zastosowanie i wymaga określenia warunku zakończenia pętli.
   <br>
```
#include <iostream>

int main() {
    // Pętla for
    std::cout << "Pętla for:" << std::endl;
    for (int i = 1; i <= 10; i++) {
        std::cout << i << std::endl;
    }

    // Pętla while
    std::cout << "Pętla while:" << std::endl;
    int j = 1;
    while (j <= 10) {
        std::cout << j << std::endl;
        j++;
    }

    // Pętla do-while
    std::cout << "Pętla do-while:" << std::endl;
    int k = 1;
    do {
        std::cout << k << std::endl;
        k++;
    } while (k <= 10);

    return 0;
}
```
<br>

**Instrukcje warunkowe**
Instrukcje warunkowe pozwalają na wykonywanie różnych działań w zależności od spełnienia określonego warunku. W języku C++ istnieją dwie podstawowe instrukcje warunkowe: if i switch. Instrukcja if umożliwia wykonanie pewnych instrukcji, gdy określony warunek jest spełniony, a instrukcja switch umożliwia wybór różnych przypadków w zależności od wartości zmiennej.
   <br>

```
#include <iostream>

int main() {
    int wynik = 75;

    // Instrukcja warunkowa if
    std::cout << "Instrukcja warunkowa if:" << std::endl;
    if (wynik >= 90) {
        std::cout << "Ocena: A" << std::endl;
    } else if (wynik >= 80) {
        std::cout << "Ocena: B" << std::endl;
    } else if (wynik >= 70) {
        std::cout << "Ocena: C" << std::endl;
    } else if (wynik >= 60) {
        std::cout << "Ocena: D" << std::endl;
    } else {
        std::cout << "Ocena: F" << std::endl;
    }

    // Instrukcja warunkowa switch
    std::cout << "Instrukcja warunkowa switch:" << std::endl;
    switch (wynik / 10) {
        case 10:
        case 9:
            std::cout << "Ocena: A" << std::endl;
            break;
        case 8:
            std::cout << "Ocena: B" << std::endl;
            break;
        case 7:
            std::cout << "Ocena: C" << std::endl;
            break;
        case 6:
            std::cout << "Ocena: D" << std::endl;
            break;
        default:
            std::cout << "Ocena: F" << std::endl;
            break;
    }

    return 0;
}

```
<br>

**Funkcje**
Funkcje są blokami kodu, które mogą być wywoływane z innego miejsca w programie. W języku C++, funkcje mają swoje nazwy, typy zwracane i parametry. Funkcje są często używane do rozdzielenia kodu na mniejsze, bardziej zorganizowane bloki, które są łatwiejsze do utrzymania.
   <br>
```
#include <iostream>

int dodaj(int a, int b) {
    return a + b;
}

int main() {
    int x = 3;
    int y = 5;

    int suma = dodaj(x, y);

    std::cout << "Suma " << x << " i " << y << " to " << suma << std::endl;

    return 0;
}
```
<br>

**Podsumowanie**
W tym szkoleniu nauczysz się podstaw języka C++, ale to tylko wstęp do bardziej zaawansowanych tematów, takich jak programowanie obiektowe, szablony i algorytmy i struktury danych. Zrozumienie podstaw języka C++ jest kluczowe do zrozumienia bardziej zaawansowanych koncepcji, dlatego ważne jest, aby poświęcić odpowiednią ilość czasu na naukę składni i konstrukcji języka C++.

W kolejnych częściach tego szkolenia będziesz uczyć się bardziej zaawansowanych tematów, takich jak tworzenie klas i obiektów, dziedziczenie, polimorfizm, szablony i algorytmy i struktury danych. Będziesz także uczyć się, jak tworzyć aplikacje konsolowe i graficzne, jak debugować kod i jak stosować dobre praktyki programowania. 
<br>

**Zadania do wykonania**
1) Zadeklaruj zmienną typu całkowitego o nazwie "liczba" i przypisz jej wartość 10. Następnie wyświetl wartość tej zmiennej na konsoli.
   <br>
2) Napisz program, który wczytuje liczby od użytkownika i wyświetla ich sumę. Program powinien zakończyć wczytywanie liczb, gdy użytkownik wprowadzi 0.
   <br>
3) Napisz funkcję, która oblicza silnię danej liczby całkowitej. Funkcja powinna zwracać wynik jako wartość typu całkowitego.
   <br>
4) Napisz program, który sortuje tablicę liczb całkowitych w kolejności rosnącej. Użyj algorytmu sortowania przez wybieranie.
   <br>
5) Napisz program, który oblicza pierwiastek kwadratowy liczby całkowitej. Użyj funkcji szablonowej.  
    <br>

**Podsumowanie**
Wprowadzenie do języka C++ to pierwszy krok w nauce programowania w tym języku. Poznanie podstawowych koncepcji, takich jak składnia, zmienne, pętle, instrukcje warunkowe i funkcje, jest kluczowe dla zrozumienia bardziej zaawansowanych koncepcji, takich jak programowanie obiektowe, szablony i algorytmy i struktury danych. Warto poświęcić czas na naukę i praktykę, aby stać się biegłym programistą w języku C++.
