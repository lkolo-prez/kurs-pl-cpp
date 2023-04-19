Komentarze w języku C++ umożliwiają wprowadzenie dodatkowych informacji do kodu, które są ignorowane przez kompilator. Komentarze można używać do wyjaśnienia, co robi dany fragment kodu lub do umieszczenia notatek, które pomogą Ci później zrozumieć, co robił kod.

W języku C++ istnieją dwa rodzaje komentarzy: jednoliniowe i wieloliniowe.

Jednoliniowe komentarze zaczynają się od dwóch ukośników "//" i obejmują tylko jeden wiersz tekstu. Np.

```
// To jest jednoliniowy komentarz
```
<br>
Wieloliniowe komentarze zaczynają się od "/" i kończą na "/". Np.
```
/*
To jest wieloliniowy komentarz.
Można tutaj wprowadzić więcej tekstu.
*/
```
<br>
Komentarze można umieszczać w dowolnym miejscu w kodzie. Np.
```
#include <iostream>

int main()
{
    // To jest komentarz
    std::cout << "Hello, world!" << std::endl; // To jest inny komentarz
    /*
    To jest jeszcze inny komentarz.
    Można umieszczać je w dowolnym miejscu.
    */
    return 0;
}
```
<br>

Komentarze są bardzo przydatne, ponieważ pozwalają na lepszą czytelność kodu i ułatwiają jego późniejsze zrozumienie.
<br>

Należy pamiętać, że komentarze nie są wykonywane przez program i nie mają wpływu na jego działanie. Dlatego warto stosować je w umiarkowany sposób i umieszczać tylko najważniejsze informacje.


<h2>Zalecenia</h2>

1) Ułatwiają zrozumienie kodu - Komentarze pozwalają na lepsze zrozumienie kodu przez inne osoby, które mogą nie mieć pełnej wiedzy na temat danego problemu lub języka programowania.

2) Ułatwiają późniejsze modyfikacje - Komentarze umożliwiają łatwiejsze późniejsze wprowadzanie zmian w kodzie. Osoba, która będzie zmieniać kod po Tobie, będzie miała łatwiejsze zadanie, jeśli komentarze jasno opiszą, co dany fragment kodu robi.

3) Są pomocne podczas debugowania - Komentarze mogą być pomocne podczas debugowania programu, ponieważ pozwalają zrozumieć, co robi dany fragment kodu i jakie są oczekiwane wyniki.

4) Poprawiają czytelność kodu - Komentarze zwiększają czytelność kodu poprzez umieszczenie w nim dodatkowych informacji.

5) Ułatwiają współpracę - Komentarze pomagają w lepszej współpracy pomiędzy programistami pracującymi nad tym samym kodem.

6) Są dobrym nawykiem programistycznym - Używanie komentarzy jest dobrym nawykiem programistycznym, ponieważ pozwala na tworzenie bardziej czytelnego i zrozumiałego kodu.

Warto jednak pamiętać, że komentarze nie powinny zastępować jasnego i czytelnego kodu. Należy pisać kod zrozumiale, stosować nazwy zmiennych i funkcji zgodnie z ich przeznaczeniem oraz unikać zbyt skomplikowanych konstrukcji.