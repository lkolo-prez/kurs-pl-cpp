<h1>Struktura programu</h1>

Witajcie w lekcji dotyczącej struktury programu w języku C++!

Program w C++ składa się z jednego lub wielu plików źródłowych, które muszą być skompilowane przy użyciu kompilatora C++. Wynikowy plik wykonywalny może być następnie uruchomiony na systemie operacyjnym.

***Struktura programu w C++ składa się z następujących elementów:***

1) Dyrektywy preprocesora: Dyrektywy preprocesora rozpoczynają się od znaku # i są przetwarzane przed właściwą kompilacją programu. Mogą one służyć do definiowania stałych, włączania bibliotek, itp.

2) Deklaracje zmiennych i funkcji: W tym miejscu programista deklaruje zmienne i funkcje, które będą używane w programie. Deklaracje zmiennych określają typ zmiennej oraz jej nazwę, a deklaracje funkcji określają jej nazwę, typ zwracany i listę parametrów.

3) Funkcja main: Funkcja main jest punktem wejścia do programu. W niej umieszczany jest kod, który zostanie wykonany przy uruchomieniu programu.

4) Definicje funkcji: Definicje funkcji zawierają kod, który zostanie wykonany, gdy funkcja zostanie wywołana.

***Oto przykładowy szkielet programu w C++, który zawiera wszystkie powyższe elementy:***

```
// definicja biblioteki
#include <iostream>
// Dyrektywy preprocesora
#define PI 3.14

// Deklaracje zmiennych i funkcji globalnych
int dodaj(int a, int b);

//definicja głównej funkcji 'main'
int main() {
    // Kod programu
    int x = 3; //definicja zmiennych wewnątrz funkcji
    int y = 5;
    int suma = dodaj(x, y); //odwołanie się do funkcji 
    std::cout << "Suma " << x << " i " << y << " to " << suma << std::endl;

    return 0;
}

// Definicje funkcji
int dodaj(int a, int b) {
    return a + b;
}
```
<br>

***Wytłuamczenie czym jest STD***
std:: to nazwa przestrzeni nazw (ang. namespace) w języku C++, która służy do grupowania różnych klas, funkcji i zmiennych w jednej przestrzeni nazw. Nazwa przestrzeni nazw "std" pochodzi od standardowej biblioteki C++, która zawiera wiele gotowych funkcji i klas, takich jak strumienie wejścia/wyjścia (cout, cin), kontenery STL (vector, list, map) czy algorytmy STL (sort, find, count_if).


Dzięki wykorzystaniu przestrzeni nazw, programista może uniknąć konfliktów nazw między różnymi klasami, funkcjami lub zmiennymi. Przykładowo, jeśli dwie klasy miałyby tę samą nazwę, to programista mógłby odwołać się do każdej z tych klas poprzez nazwę przestrzeni, w której się znajdują.


Aby korzystać z elementów znajdujących się w przestrzeni nazw "std", programista musi dodać dyrektywę "using namespace std" na początku programu lub przed wykorzystaniem elementów przestrzeni nazw w kodzie. Przykładowo, jeśli chcemy skorzystać z funkcji cout i cin, możemy to zrobić w następujący sposób:
<br>

```
#include <iostream>

int main() {
    using namespace std;

    int liczba;
    cout << "Podaj liczbę całkowitą: ";
    cin >> liczba;
    cout << "Wczytana liczba to: " << liczba << endl;

    return 0;
}
```
<br>
W tym kodzie, za pomocą dyrektywy "using namespace std" definiujemy, że będziemy korzystać z przestrzeni nazw "std" w naszej funkcji main. Dzięki temu, możemy korzystać z funkcji cout i cin bez konieczności używania przedrostka "std::".
<br>
<br>

***Zadania***
1) Napisz program, który prosi użytkownika o wprowadzenie dwóch liczb całkowitych, a następnie wyświetla wynik ich dodawania, odejmowania, mnożenia i dzielenia.
<br>
2) Napisz program, który prosi użytkownika o wprowadzenie dwóch liczb całkowitych, a następnie wyświetla większą z nich.
<br>
3) Napisz program, który oblicza i wyświetla sumę liczb naturalnych od 1 do 100.
<br>
4) Napisz program, który pyta użytkownika o wprowadzenie liczby całkowitej n, a następnie wyświetla wszystkie liczby naturalne od 1 do n.
<br>
5) Napisz program, który pyta użytkownika o wprowadzenie liczby całkowitej n, a następnie oblicza i wyświetla silnię tej liczby.
<br>
6) Napisz program, który pobiera od użytkownika serię liczb, a następnie wyświetla największą i najmniejszą z tych liczb.
<br>
7) Napisz program, który pobiera od użytkownika serię liczb, a następnie wyświetla sumę i średnią arytmetyczną tych liczb.
<br>
8) Napisz program, który pobiera od użytkownika dwie liczby całkowite a i b, a następnie wyświetla wszystkie liczby całkowite między a i b (włącznie z a i b).
<br>
9) Napisz program, który pobiera od użytkownika serię liczb, a następnie wyświetla tylko te liczby, które są podzielne przez 3 lub 5.
<br>
10) Napisz program, który pobiera od użytkownika serię liczb, a następnie wyświetla tylko te liczby, które są liczbami pierwszymi.
<br>
Zadania te mają na celu ćwiczenie różnych aspektów programowania w języku C++, takich jak wprowadzanie danych, wykonywanie operacji matematycznych, pętle, instrukcje warunkowe i funkcje. Można je dostosować do poziomu zaawansowania uczniów, dodając bardziej zaawansowane elementy lub ograniczając je do podstawowych funkcjonalności.