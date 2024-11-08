# **Laboratorium 6: Projektowanie systemu z wykorzystaniem polimorfizmu**.

Laboratorium 6 jest poświęcone praktycznemu wykorzystaniu **polimorfizmu** w C++ i Java. Studenci uczą się, jak zastosować polimorfizm do tworzenia systemów, w których obiekty różnych klas mogą być traktowane jednolicie, a ich specyficzne zachowanie jest realizowane przez funkcje nadpisane w klasach pochodnych. To laboratorium wzmacnia umiejętność projektowania elastycznych i skalowalnych systemów obiektowych.

---

### **Cele laboratorium**:
1. Zrozumienie i zastosowanie **polimorfizmu** w C++.
2. Implementacja polimorfizmu poprzez **funkcje wirtualne** i **klasy bazowe**.
3. Tworzenie systemu, w którym różne obiekty mogą być traktowane jako typy bazowe, ale mają różne zachowanie.

---

### **Przegląd polimorfizmu**

**Polimorfizm** to mechanizm w programowaniu obiektowym, który pozwala na traktowanie obiektów różnych klas w jednolity sposób, jeśli dziedziczą one po wspólnej klasie bazowej. Dzięki temu można wywoływać metody obiektów bez znajomości ich konkretnego typu, co umożliwia większą elastyczność i rozszerzalność kodu.

---

## **Część 1: Projektowanie systemu z wykorzystaniem polimorfizmu w C++**

W C++ polimorfizm jest często realizowany poprzez:
- **Funkcje wirtualne** w klasie bazowej.
- **Nadpisywanie metod** w klasach pochodnych.

---

### **Opis zadania: Projekt systemu do zarządzania pojazdami**

W ramach tego laboratorium zaprojektujemy system do zarządzania różnymi typami pojazdów: **Samochodami**, **Rowerami** i **Motocyklami**. Wszystkie pojazdy mają pewne wspólne cechy (mogą przyspieszać i zatrzymywać się), ale sposób ich działania różni się w zależności od typu pojazdu.

---

### **Zadanie 1: Stworzenie klasy bazowej `Pojazd` z funkcjami wirtualnymi**

1. Stwórz klasę bazową `Pojazd`, która będzie zawierać wspólne cechy dla wszystkich pojazdów.
2. Dodaj funkcje wirtualne, które zostaną nadpisane przez klasy pochodne:
   - `virtual void przyspiesz()`
   - `virtual void zatrzymaj()`
3. Zdefiniuj destruktor wirtualny `~Pojazd()`, aby zapewnić poprawne usuwanie obiektów przez wskaźniki klasy bazowej.

### **Zadanie 2: Stworzenie klas pochodnych `Samochod`, `Rower`, i `Motocykl`**

1. Stwórz klasy pochodne `Samochod`, `Rower` i `Motocykl`, które dziedziczą po klasie `Pojazd`.
2. Każda klasa powinna nadpisywać metody `przyspiesz()` i `zatrzymaj()`, aby wyświetlały specyficzne komunikaty dla każdego pojazdu.

---

### **Zadanie 3: Implementacja polimorfizmu przy użyciu wskaźników do klasy bazowej**

1. Stwórz wektor wskaźników `std::unique_ptr<Pojazd>`, w którym można przechowywać różne typy pojazdów (`Samochod`, `Rower`, `Motocykl`).
2. Dodaj do wektora kilka obiektów różnych typów.
3. Użyj pętli `for`, aby wywołać metody `przyspiesz()` i `zatrzymaj()` dla każdego pojazdu w sposób polimorficzny.

#### **Opis działania**:
- Wektor `pojazdy` przechowuje wskaźniki do obiektów różnych klas pochodnych (`Samochod`, `Rower`, `Motocykl`), traktując je wszystkie jako `Pojazd`.
- Dzięki polimorfizmowi, dla każdego obiektu wywoływane są odpowiednie wersje metod `przyspiesz()` i `zatrzymaj()` zdefiniowane w klasach pochodnych.

---

### **Zadanie 4: Dodanie nowej klasy pochodnej `Skuter`**

1. Dodaj klasę `Skuter`, która dziedziczy po klasie `Pojazd`.
2. Zdefiniuj metody `przyspiesz()` i `zatrzymaj()` specyficzne dla `Skuter`.
3. Dodaj obiekt `Skuter` do wektora `pojazdy` i przetestuj, czy wywoływane są odpowiednie metody.

---

## **Część 2: Java - Projektowanie systemu z wykorzystaniem polimorfizmu**

### **Opis zadania:** Projekt systemu do zarządzania pojazdami
Podobnie jak w C++, w tej części projektu stworzymy system zarządzania pojazdami, wykorzystując polimorfizm do różnicowania zachowań obiektów w klasach pochodnych.

---

### **Zadanie 5: Stworzenie klasy bazowej Pojazd z metodami abstrakcyjnymi**

1. Stwórz abstrakcyjną klasę `Pojazd`, która będzie zawierać metody wspólne dla wszystkich pojazdów.
2. Dodaj metody abstrakcyjne:
  `public abstract void przyspiesz()`;
  `public abstract void zatrzymaj()`;

---

### **Zadanie 6: Stworzenie klas pochodnych Samochod, Rower, i Motocykl**

1. Stwórz klasy `Samochod`, `Rower` i `Motocykl`, które dziedziczą po klasie `Pojazd`.
2. Każda klasa powinna implementować metody `przyspiesz()` i `zatrzymaj()` z odpowiednimi komunikatami.

---

### **Zadanie 7: Implementacja polimorfizmu przy użyciu listy obiektów klasy bazowej**

1. Stwórz `ArrayList<Pojazd>`, w której przechowywane będą obiekty różnych typów (`Samochod`, `Rower`, `Motocykl`).
2. Dodaj kilka obiektów do listy i użyj pętli for do wywołania metod `przyspiesz()` i `zatrzymaj()` dla każdego pojazdu.

---

## **Podsumowanie Laboratorium**

W trakcie tego laboratorium studenci zapoznali się z następującymi zagadnieniami:
1. **Polimorfizm**: Użycie wskaźników klasy bazowej `Pojazd` do wywoływania metod w sposób polimorficzny.
2. **Funkcje wirtualne i nadpisywanie metod**: Definiowanie funkcji wirtualnych i ich implementacja w klasach pochodnych.
3. **Zwiększanie elastyczności kodu**: Możliwość rozszerzania systemu o nowe klasy, takie jak `Skuter`, bez konieczności modyfikacji kodu bazowego.
4. **Java**: Studenci nauczyli się stosować klasy abstrakcyjne i listy obiektów klasy bazowej do realizacji polimorfizmu.
5. **Uniwersalność:** Dzięki polimorfizmowi kod jest bardziej elastyczny i pozwala na łatwe dodawanie nowych typów pojazdów, takich jak Motocykl, bez modyfikacji istniejącej logiki.

---

Laboratorium 6 pozwala studentom na praktyczne zrozumienie polimorfizmu i jego znaczenia w projektowaniu oprogramowania. Dzięki zastosowaniu abstrakcyjnych klas bazowych i dynamicznego wiązania, studenci uczą się, jak projektować bardziej modularny i rozszerzalny kod, który łatwo można dostosować do przyszłych zmian lub rozszerzeń.

