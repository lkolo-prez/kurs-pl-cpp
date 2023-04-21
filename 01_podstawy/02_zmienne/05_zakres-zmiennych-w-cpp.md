W C++ istnieją różne poziomy zakresów zmiennych, a ich zasięg (czyli obszar, w którym zmienna jest dostępna) zależy od miejsca, w którym została zdefiniowana. Poniżej przedstawiam kilka rodzajów zakresów zmiennych:

### Zakres globalny

Zmienne zdefiniowane na poziomie globalnym są dostępne w całym programie. Ich zasięg rozciąga się od momentu ich definicji do końca programu:

```cpp
#include <iostream>

int zmienna_globalna = 10; // zmienna globalna

int main() {
    std::cout << "Zmienna globalna: " << zmienna_globalna << std::endl;
    return 0;
}
```

W powyższym przykładzie zmienna zmienna_globalna jest dostępna w całym programie, a jej wartość może być odczytana w funkcji main().

### Zakres lokalny

Zmienne zdefiniowane wewnątrz bloku (np. funkcji) są dostępne tylko w obrębie tego bloku. Ich zasięg rozciąga się od momentu ich definicji do końca bloku:

```cpp
#include <iostream>

void funkcja() {
    int zmienna_lokalna = 20; // zmienna lokalna
    std::cout << "Zmienna lokalna: " << zmienna_lokalna << std::endl;
}

int main() {
    funkcja();
    return 0;
}
```

W powyższym przykładzie zmienna zmienna_lokalna jest dostępna tylko wewnątrz funkcji funkcja(), a jej wartość może być odczytana tylko wewnątrz tej funkcji.

### Zakres blokowy

W C++ można również definiować zmienne wewnątrz bloków kodu (np. pętli), co pozwala na bardziej precyzyjne kontrolowanie ich zasięgu. Zmienne zdefiniowane wewnątrz bloku są dostępne tylko wewnątrz tego bloku:

```cpp
#include <iostream>

int main() {
    for (int i = 1; i <= 5; i++) {
        int zmienna_blokowa = i * 2; // zmienna blokowa
        std::cout << "Zmienna blokowa: " << zmienna_blokowa << std::endl;
    }
    return 0;
}
```

W powyższym przykładzie zmienna zmienna_blokowa jest dostępna tylko wewnątrz pętli for, a jej wartość zmienia się w każdym obiegu pętli.

### Zakres przestrzeni nazw

W C++ można również definiować zmienne wewnątrz przestrzeni nazw, co pozwala na uniknięcie konfliktów nazw i zapewnienie czytelności kodu. Zmienne zdefiniowane wewnątrz przestrzeni nazw są dostępne tylko w obrębie tej przestrzeni:

```cpp
#include <iostream>

namespace moja_przestrzen_nazw {
    int zmienna = 30; // zmienna w przestrzeni nazw
}

int main() {
    std::cout << "Zmienna w przestrzeni nazw: " << moja_przestrzen_nazw::zmienna << std::endl;
    return 0;
}
```

W powyższym przykładzie zmienna zmienna jest dostępna tylko wewnątrz przestrzeni nazw moja_przestrzen_nazw, a jej wartość może być odczytana tylko po zaimportowaniu tej przestrzeni nazw do programu.

### Zakres argumentów funkcji

Argumenty funkcji są zmiennymi zdefiniowanymi na poziomie lokalnym wewnątrz funkcji. Ich zasięg rozciąga się od momentu wywołania funkcji do momentu jej zakończenia:

```cpp
#include <iostream>

void funkcja(int argument) {
    std::cout << "Argument funkcji: " << argument << std::endl;
}

int main() {
    int zmienna_lokalna = 40;
    funkcja(zmienna_lokalna);
    return 0;
}
```

W powyższym przykładzie argument funkcji jest zmienną lokalną wewnątrz funkcji funkcja(), a jego wartość zostaje przekazana podczas wywołania funkcji.

### Podsumowanie

Zasięg zmiennych w C++ zależy od miejsca, w którym zostały zdefiniowane. Zmienne zdefiniowane na poziomie globalnym są dostępne w całym programie, zmienne zdefiniowane wewnątrz bloku lub funkcji są dostępne tylko w obrębie tego bloku lub funkcji, zmienne zdefiniowane w przestrzeni nazw są dostępne tylko w obrębie tej przestrzeni, a argumenty funkcji są dostępne tylko wewnątrz funkcji, w której zostały zdefiniowane. Wszystkie zmienne mają swoje zasięgi, których przestrzeganie jest ważne dla poprawnego działania programu i uniknięcia nieprzewidywalnych efektów.