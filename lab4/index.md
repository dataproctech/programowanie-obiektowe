# **Laboratorium 4: Praktyka ukrywania danych i enkapsulacji w Java i C++**

## **Cele:**

1. Zrozumienie pojęć **ukrywania danych** oraz **enkapsulacji** w programowaniu obiektowym.
2. Implementacja klas w językach **C++** oraz **Java**, które stosują ukrywanie danych i enkapsulację.
3. Praktyczne zastosowanie **getterów** i **setterów** w celu zarządzania dostępem do prywatnych atrybutów klasy.

---

## **Część 1: Wprowadzenie do ukrywania danych i enkapsulacji**

- **Ukrywanie danych**: Ukrywanie wewnętrznych szczegółów klasy poprzez oznaczenie atrybutów jako prywatnych (**private**). Zapewnia to, że dane nie będą bezpośrednio dostępne poza klasą.
  
- **Enkapsulacja**: Technika polegająca na łączeniu danych i metod, które te dane modyfikują, wewnątrz jednej klasy, a także ograniczaniu dostępu do tych danych poprzez stosowanie prywatnych atrybutów oraz publicznych metod dostępowych (**gettery** i **settery**).

---

## **Część 2: Zadanie 1 – Implementacja klasy `Osoba` z prywatnymi atrybutami i metodami dostępowymi**

### **Opis**:
Utwórz klasę `Osoba` w językach C++ i Java, która będzie posiadała prywatne atrybuty oraz publiczne metody dostępu (gettery i settery). 

#### **Kroki**:
1. Stwórz prywatne atrybuty:
   - **C++ i Java**: `imię` (string), `nazwisko` (string), `wiek` (int).

2. Stwórz publiczne metody dostępu:
   - **Gettery**: Metody pozwalające na odczytanie wartości prywatnych atrybutów.
   - **Settery**: Metody pozwalające na ustawienie wartości prywatnych atrybutów.
     
---

## **Część 3: Zadanie 2 – Rozbudowa klasy z dodatkowymi atrybutami i walidacją danych**

### **Opis**:
Rozbuduj klasę `Osoba`, dodając nowe prywatne atrybuty i metody dostępu oraz wprowadź dodatkowe zasady walidacji danych.

#### **Kroki**:
1. Dodaj prywatne atrybuty:
   - **C++ i Java**: `email` (string), `telefon` (string).

2. Zaimplementuj walidację w setterach:
   - Sprawdź, czy adres email zawiera znak '@'.
   - Sprawdź, czy numer telefonu ma odpowiednią długość (np. 9 cyfr).
     
--- 

## **Część 4: Zadanie 3 – Użycie modyfikatora protected w klasach dziedziczących**

### **Opis**:
Utwórz hierarchię klas, w której zastosujesz modyfikator protected do ochrony atrybutów dziedziczonych przez klasy potomne. Zaimplementuj klasę bazową Pracownik, a następnie utwórz klasy pochodne Nauczyciel i Administracja, które będą dziedziczyć atrybuty chronione.

### **Kroki**:
1. Stwórz klasę bazową `Pracownik`:

  - Zastosuj modyfikator **protected** do atrybutów `stanowisko` (string) i `wynagrodzenie` (float).
    
2. Stwórz klasy dziedziczące `Nauczyciel` i `Administracja`, które dziedziczą atrybuty klasy `Pracownik`.

3. Zaimplementuj metodę `pokazDane()` w każdej klasie potomnej, która korzysta z chronionych atrybutów.

---

## Podsumowanie laboratorium
W ramach tego laboratorium studenci:

1. Zrozumieli koncepcję **ukrywania danych** oraz **enkapsulacji**, chroniąc prywatne dane za pomocą getterów i setterów.
   
2. Nauczyli się używać modyfikatora dostępu protected w kontekście dziedziczenia klas, umożliwiając dostęp do chronionych atrybutów w klasach potomnych.
   
3. Zrozumieli, w jakich sytuacjach stosuje się różne modyfikatory dostępu (private, protected, public) i jak wpływają one na bezpieczeństwo danych i dziedziczenie.

To laboratorium umożliwi studentom praktyczne zrozumienie i zastosowanie **ukrywania danych** oraz **enkapsulacji** w językach C++ i Java.

