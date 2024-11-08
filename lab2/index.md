# Laboratorium 2: Tworzenie klas z konstruktorami i destruktorami

W ramach tego laboratorium studenci nauczą się podstaw zarządzania obiektami w programowaniu obiektowym, ze szczególnym uwzględnieniem mechanizmów konstruktorów i destruktorów. 

## Cel laboratorium:

- Zrozumienie roli konstruktorów i destruktorów w programowaniu obiektowym.
- Implementacja klas z konstruktorami i destruktorami w językach C++ i Java.
- Zrozumienie zarządzania zasobami oraz automatycznego zwalniania pamięci (C++).

## Część 1: Wprowadzenie do konstruktorów i destruktorów

Konstruktor: Metoda, która jest automatycznie wywoływana podczas tworzenia obiektu. Jej zadaniem jest inicjalizacja pól klasy.

C++: Konstruktor może być przeciążony (może mieć różne wersje z różnymi parametrami).

Java: Każda klasa ma domyślny konstruktor, ale może mieć również niestandardowe, przeciążone konstruktory.

Destruktor (C++): Specjalna metoda, która jest wywoływana automatycznie, gdy obiekt przestaje być używany. Destruktor służy do zwalniania zasobów (np. pamięci dynamicznej).

## Część 2: Zadanie 1 – Tworzenie klasy Samochód z konstruktorami i destruktorem w C++ i Java

### Cel: Stworzenie klasy Samochód z różnymi wersjami konstruktorów, a w C++ także destruktorem.

#### Wersja w C++:
1. Stwórz klasę `Samochód`:
  - Atrybuty:
    - `string marka`
    - `string model`
    - `int rokProdukcji`
  - Konstruktor: Przyjmujący wartości dla wszystkich atrybutów.
  - Domyślny konstruktor: Inicjalizujący atrybuty domyślnymi wartościami.
  - Destruktor: Wyświetlający komunikat "Destruktor wywołany dla: [marka] [model]".

#### Wersja w Java:
1. Stwórz klasę `Samochód`:
  - Atrybuty:
    - String marka
    - String model
    - int rokProdukcji
  - Konstruktor: Przyjmujący wartości dla wszystkich atrybutów.
  - Domyślny konstruktor: Inicjalizujący atrybuty domyślnymi wartościami.

#### Do zrobienia:
  - Zaimplementowanie klasy `Samochód` z konstruktorami w C++ lub Java.
  - W przypadku C++: Dodanie destruktora, który wyświetla komunikat o usunięciu obiektu.
  - Testowanie kodu poprzez tworzenie różnych obiektów za pomocą konstruktorów.

## Część 3: Zadanie 2 – Przeciążenie konstruktorów i inicjalizacja zasobów
### Cel: Zaimplementuj klasę, która przechowuje dynamicznie alokowane zasoby (np. tablice dynamiczne), wykorzystując przeciążone konstruktory oraz destruktory w C++.

#### Wersja w C++:
1. Stwórz klasę `Tablica`:
  - Atrybut: wskaźnik do dynamicznej tablicy `int`.
  - Konstruktor domyślny: alokuje tablicę o wielkości 10 elementów.
  - Konstruktor z parametrem: alokuje tablicę o podanej wielkości.
  - Destruktor: zwalnia dynamiczną pamięć.

#### Wersja w Java:
W języku Java nie ma potrzeby stosowania destruktorów do zwalniania zasobów, ponieważ tym zajmuje się garbage collector. Możesz jednak zaimplementować finalizer (choć jego użycie jest odradzane).

#### Do zrobienia:
  - Implementacja klasy `Tablica` w C++ i Java.
  - Testowanie działania konstruktorów i destruktorów (w przypadku C++).
  - W C++: Upewnienie się, że pamięć jest prawidłowo zwalniana po zakończeniu programu.

## Wymagania końcowe:
  - Rozumieć różnicę między konstruktorami domyślnymi a konstruktorami przeciążonymi.
  - Nauczyć się tworzyć destruktory w C++ i wiedzieć, kiedy są one wywoływane.
  - W Javie: zrozumienie, jak działa garbage collector i dlaczego destruktory nie są potrzebne.

