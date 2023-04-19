<h1>Kompilowanie w C++ za pomocą wiersza poleceń</h1>

<br>
Otwórz dowolny edytor tekstu i napisz kod programu w języku C++ na przykład.
```
#include <iostream>

int main()
{
    std::cout << "Hello, world!" << std::endl;
    return 0;
}
```
Zapisz plik z kodem programu w odpowiednim formacie (z rozszerzeniem .cpp). Np. nazwij go "hello.cpp".
<br>

Otwórz terminal lub wiersz poleceń.

Przejdź do katalogu, w którym znajduje się plik z kodem programu. Można to zrobić za pomocą polecenia cd (change directory).

Skompiluj program w bashu za pomocą polecenia g++. Np.:


```
g++ -o hello hello.cpp
```
Wyjaśnienie: -o oznacza, że należy skompilować plik wyjściowy, a hello to nazwa pliku wyjściowego. Ostatecznie w tym przypadku plik wyjściowy będzie miał nazwę "hello".

Po skompilowaniu programu w bashu uruchom go za pomocą polecenia ./nazwa_programu (w tym przypadku "./hello"). Np.:

```
./hello
```
<br>
Zobaczysz wynik działania programu na ekranie. W tym przypadku wyświetli się komunikat "Hello, world!".
<br>

To tyle! Teraz możesz eksperymentować z programami napisanymi w języku C++ i kompilować je w terminalu.



