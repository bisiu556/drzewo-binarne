# Drzewo binarne (BST) w C++

Program w języku C++ wczytujący liczby całkowite z pliku `dane.txt`, budujący binarne drzewo poszukiwań (BST), prezentujący krok po kroku kierunek wstawiania elementów, rysujący strukturę drzewa od góry w dół, wypisujący elementy w kolejności rosnącej (*in-order*) oraz zwalniający pamięć dynamiczną wraz z weryfikacją liczby wykonanych operacji `delete`.

## Funkcjonalności

* Wczytywanie liczb całkowitych po jednej z pliku tekstowego `dane.txt`.
* Wstawianie elementów do drzewa BST (`liczba > korzen->liczba` na prawo, pozostałe na lewo) z podglądem ścieżki przejścia.
* Rysowanie schematu zbudowanego drzewa z podziałem na lewe (`L`) i prawe (`P`) poddrzewa.
* Wypisywanie posortowanych liczb z wykorzystaniem przejścia *in-order*.
* Rekurencyjne usuwanie drzewa (*post-order*) i zliczanie wywołań `delete` w zmiennej globalnej `licznik_delete`.
* Porównanie liczby wczytanych rekordów z liczbą zwolnionych węzłów.

## Format pliku wejściowego (`dane.txt`)

Plik powinien znajdować się w katalogu roboczym programu i zawierać liczby całkowite oddzielone spacjami lub nowymi liniami, np.:

```text
5 2 8 1 3 6 7 9 11
