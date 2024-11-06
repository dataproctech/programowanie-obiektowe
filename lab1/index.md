# Laboratorium 1: Podstawowa Struktura Klasy w C++ i Java

## Przegląd

W tym laboratorium będziesz ćwiczyć podstawowe pojęcia programowania obiektowego (OOP) poprzez stworzenie prostych klas w językach **C++** oraz **Java**. Dzięki temu zrozumiesz podstawy definicji klas, obiektów, atrybutów oraz metod, które są kluczowymi elementami OOP.

Zaimplementujesz klasę `Car` zarówno w C++, jak i w Javie, aby poćwiczyć pisanie prostych definicji klas, konstruktorów i metod.

## Cele

Pod koniec tego laboratorium będziesz w stanie:
- Zrozumieć i zaimplementować prostą klasę z atrybutami i metodami.
- Użyć konstruktorów do inicjalizacji atrybutów klasy.
- Utworzyć obiekty z klasy.
- Wywołać metody na obiekcie i wyświetlić wartości atrybutów.
- Zapoznać się z IDE dla C++ i Java.

## Instrukcje

## Zadanie 1: 

### Część 1: Implementacja w C++

1. **Skonfiguruj środowisko**:
   - Otwórz swoje IDE (np. Visual Studio lub dowolne środowisko C++).
   - Utwórz nowy projekt o nazwie `Lab1_CPP`.

2. **Utwórz klasę `Car`**:
   - Zdefiniuj klasę o nazwie `Car` z następującymi atrybutami:
     - `string make` (Marka samochodu, np. Toyota, Honda).
     - `string model` (Model samochodu, np. Corolla, Civic).
     - `int year` (Rok produkcji, np. 2020, 2019).

3. **Metody klasy**:
   - Utwórz konstruktor, który zainicjalizuje atrybuty klasy.
   - Napisz metodę `void displayInfo()`, aby wyświetlić szczegóły samochodu.

4. **Napisz funkcję główną (main)**:
   - W funkcji `main()` utwórz obiekt klasy `Car`.
   - Wywołaj metodę `displayInfo()`, aby wyświetlić szczegóły samochodu.

### Część 2: Implementacja w Javie

1. **Skonfiguruj środowisko**:
  - Otwórz swoje IDE dla Javy (np. IntelliJ IDEA lub Eclipse).
  - Utwórz nowy projekt o nazwie `Lab1_Java`.

2. **Utwórz klasę Car**:
  - Zdefiniuj klasę o nazwie `Car` z następującymi atrybutami:
    - `String make` (Marka samochodu, np. Toyota, Honda).
    - `String model` (Model samochodu, np. Corolla, Civic).
    - `int year` (Rok produkcji, np. 2020, 2019).

3. **Metody klasy**:
  - Utwórz konstruktor, aby zainicjalizować atrybuty klasy.
  - Napisz metodę `void displayInfo()`, aby wyświetlić szczegóły samochodu.

4. **Napisz metodę główną (main)**:
  - W metodzie `main()` utwórz obiekt klasy `Car`.
  - Wywołaj metodę `displayInfo()`, aby wyświetlić szczegóły samochodu.
    
### Część 3: Refleksja i Pytania

Po ukończeniu zadań, zastanów się nad następującymi pytaniami:
  1. Dlaczego ważne jest używanie specyfikatorów dostępu private dla atrybutów?
  2. Co się stanie, jeśli zmienisz specyfikator dostępu atrybutów na public? Spróbuj to zrobić i zaobserwuj zmiany.
  3. Czy możesz utworzyć wiele obiektów klasy Car? Jeśli tak, jak każdy obiekt przechowuje swoje własne atrybuty?

## Zadanie 2: Dodanie metod i obliczanie atrybutów

### Zadanie C++ 
### Cel:
Rozszerz klasę `Car`, dodając nowe atrybuty oraz metodę do obliczania wieku samochodu.

   1. Zmodyfikuj klasę `Car`, dodając:
      Atrybut `int currentYear` reprezentujący obecny rok.
   2. Dodaj metodę:
      `int getCarAge()`, która oblicza i zwraca wiek samochodu na podstawie różnicy między `currentYear` a rokiem produkcji samochodu (`year`).
   3. Zaktualizuj funkcję `main()`:
      Utwórz obiekt klasy `Car`.
      Wywołaj `getCarAge()` i wyświetl wiek samochodu.
      
### Zadanie Java 
### Cel:
Rozszerz klasę `Car`, dodając metodę do obliczania wieku samochodu.

   1. Zmodyfikuj klasę `Car`, dodając:
      Atrybut `int currentYear` reprezentujący obecny rok.
   2. Dodaj metodę:
      `int getCarAge()`, która oblicza i zwraca wiek samochodu na podstawie różnicy między `currentYear` a rokiem produkcji samochodu (`year`).
   3. Zaktualizuj metodę `main()`:
      Utwórz obiekt klasy `Car`.
      Wywołaj `getCarAge()` i wyświetl wiek samochodu.
      
## Zadanie 3: Porównywanie obiektów (sprawdzanie równości)

### Zadanie C++ 
### Cel:
Dodaj funkcjonalność, która porównuje dwa obiekty `Car` i sprawdza, czy są takie same (na podstawie `make`, `model` oraz `year`).
   1. Dodaj metodę:
      `bool isSameCar(Car otherCar)`, która porównuje make, model i year dwóch obiektów klasy `Car` i zwraca `true`, jeśli są takie same, w przeciwnym razie `false`.
   2. Zaktualizuj funkcję `main()`:
      Utwórz dwa obiekty klasy `Car`.
      Wywołaj metodę `isSameCar()` i sprawdź, czy dwa samochody są takie same, a następnie wyświetl wynik.
      
### Zadanie Java 
### Cel:
Dodaj funkcjonalność, która porównuje dwa obiekty `Car` i sprawdza, czy są takie same (na podstawie `make`, `model` oraz `year`).
   1. Dodaj metodę:
      `boolean isSameCar(Car otherCar)`, która porównuje `make`, `model` i `year` dwóch obiektów klasy `Car` i zwraca `true`, jeśli są takie same, w przeciwnym razie `false`.
   2. Zaktualizuj metodę `main()`:
      Utwórz dwa obiekty klasy `Car`.
      Wywołaj metodę `isSameCar()` i sprawdź, czy dwa samochody są takie same, a następnie wyświetl wynik.
      
## Zadanie 4:

Wykonaj zadanie krok po kroku w C++ i Javie (utwórz dwa nowe pliki dla tego zadania):
   1. Zbuduj klasę `Parrot`, która potrafi wypowiadać frazę, która jest predefiniowana w opisie klasy (metoda `say`).
   2. Zmodyfikuj klasę z zadania `1.` tak, aby fraza była ustawiana podczas tworzenia konkretnej instancji.
   3. Zmodyfikuj klasę z zadania `2.` tak, aby fraza mogła być zmieniana podczas działania programu.
   4. Zmodyfikuj klasę z zadania `3.` tak, aby można było określić liczbę powtórzeń podczas wywoływania metody say.
   5. Zmodyfikuj klasę z zadania `4.` tak, aby można było dodawać frazy do zbioru fraz, które zna papuga. Gdy wywoływana jest metoda `say`, papuga wypowiada losową frazę ze swojego zbioru.
