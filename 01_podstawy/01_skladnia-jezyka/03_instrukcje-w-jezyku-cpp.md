
<h1>Instrukcje w C++</h1>

Witajcie w lekcji dotyczącej instrukcji w języku C++!
Instrukcje w języku C++ pozwalają na kontrolowanie przepływu programu i wykonywanie różnych działań w zależności od spełnienia określonych warunków.

<br>

1. Instrukcja warunkowa if: Instrukcja if umożliwia wykonanie pewnych instrukcji, gdy określony warunek jest spełniony. Składnia instrukcji if wygląda następująco:
```
   if (warunek) {
       // kod do wykonania, gdy warunek jest spełniony
   }
```
<br>

2. Instrukcja warunkowa if-else: Instrukcja if-else umożliwia wykonanie pewnych instrukcji, gdy określony warunek jest spełniony, lub wykonanie innych instrukcji, gdy warunek nie jest spełniony. Składnia instrukcji if-else wygląda następująco:
```
   if (warunek) {
       // kod do wykonania, gdy warunek jest spełniony
   } else {
       // kod do wykonania, gdy warunek nie jest spełniony
   }
```
<br>

3. Instrukcja warunkowa switch: Instrukcja switch umożliwia wybór różnych przypadków w zależności od wartości zmiennej. Składnia instrukcji switch wygląda następująco:
```
   switch (zmienna) {
       case wartosc1:
           // kod do wykonania, gdy zmienna ma wartość wartosc1
           break;
       case wartosc2:
           // kod do wykonania, gdy zmienna ma wartość wartosc2
           break;
       default:
           // kod do wykonania, gdy zmienna nie ma wartości odpowiadającej żadnemu case
           break;
   }
```
<br>
4. Pętla for: Pętla for umożliwia powtarzanie określonych czynności przez określoną liczbę razy. Składnia pętli for wygląda następująco:
```
   for (inicjalizacja; warunek; zwiększenie) {
       // kod do wykonania w każdej iteracji pętli
   }
```
<br>
5. Pętla while: Pętla while umożliwia powtarzanie określonych czynności, dopóki określony warunek jest spełniony. Składnia pętli while wygląda następująco:
```
   while (warunek) {
       // kod do wykonania w każdej iteracji pętli
   }
```
<br>
6. Pętla do-while umożliwia powtarzanie określonych czynności, dopóki określony warunek jest spełniony. Instrukcje wewnątrz pętli wykonywane są przynajmniej raz, a następnie pętla sprawdza, czy warunek jest spełniony i powtarza operacje, jeśli warunek jest nadal prawdziwy.

```
do {
    // kod do wykonania w każdej iteracji pętli
} while (warunek);
```

<h2>Zadania</h2>

1) Napisz program, który odczytuje liczbę i wyświetla komunikat "Liczba jest dodatnia" lub "Liczba jest ujemna" w zależności od znaku liczby.

2) Napisz program, który sprawdza, czy podana liczba jest parzysta czy nieparzysta i wyświetla odpowiedni komunikat.

3) Napisz program, który odczytuje trzy liczby i wyświetla największą z nich.

4) Napisz program, który pobiera od użytkownika dwie liczby i wykonuje jedno z działań matematycznych (dodawanie, odejmowanie, mnożenie lub dzielenie) na podstawie wyboru użytkownika. Wyświetl wynik.

5) Napisz program, który sprawdza, czy podany rok jest rokiem przestępnym i wyświetla odpowiedni komunikat.

6) Napisz program, który sprawdza, czy podana liczba jest liczbą pierwszą i wyświetla odpowiedni komunikat.

7) Napisz program, który odczytuje wiek użytkownika i wyświetla komunikat "Możesz głosować" lub "Nie możesz głosować" w zależności od wieku.

8) Napisz program, który sprawdza, czy podane trzy liczby tworzą trójkę pitagorejską i wyświetla odpowiedni komunikat.

9) Napisz program, który odczytuje ocenę z przedmiotu i wyświetla odpowiedni komunikat (np. "Bardzo dobry", "Dobry", "Dostateczny", "Niedostateczny").

10) Napisz program, który sprawdza, czy podany ciąg znaków jest palindromem (czytany tak samo od lewej jak i od prawej strony) i wyświetla odpowiedni komunikat.
