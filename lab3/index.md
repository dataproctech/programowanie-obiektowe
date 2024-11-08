# **Laboratorium 3: Analiza obiektowa z modelowaniem koncepcyjnym, strukturalnym i projektowaniem**

## **Teoria:**
[Prezentacja z wykladu](analiza_obiektowa.pdf)
<p>Kliknięcie w link otworzy plik PDF w przeglądarce, umożliwiając przeglądanie lub pobranie pliku.

## **Cele:**

1. Zrozumienie i zastosowanie modelowania koncepcyjnego oraz strukturalnego w analizie obiektowej.
2. Stworzenie diagramu UML przedstawiającego relacje: dziedziczenie, asocjacja, agregacja, kompozycja i relacja zwykła.
3. Przeanalizowanie wymagań i zaprojektowanie klas oraz ich relacji w systemie zgodnie z zasadami programowania obiektowego.

---

### **Zadanie: Projekt systemu zarządzania szkołą**

**Opis**:
Twoim zadaniem jest zaprojektowanie systemu zarządzania szkołą, który obejmuje różne typy użytkowników, kursy oraz powiązane zasoby. Na podstawie wymagań stwórz diagram UML, który będzie zawierał klasy oraz relacje między nimi.

#### **Wymagania systemu**:

1. W systemie istnieją różne role, takie jak **Nauczyciel** i **Uczeń**, które są rodzajami klasy bazowej **Osoba**.
2. **Szkoła** oferuje wiele **Kursów**, a każdy kurs może mieć przypisanego jednego nauczyciela i wielu uczniów.
3. Każdy **Uczeń** może być zapisany na wiele **Kursów**, a **Nauczyciel** może prowadzić kilka kursów.
4. **Sala lekcyjna** jest powiązana z kursem, ale sala istnieje niezależnie od kursów.
5. Każdy kurs ma przypisany zestaw **Materiałów**, które nie mogą istnieć bez kursu.

---

## **Część 1: Modelowanie koncepcyjne – Identyfikacja klas i atrybutów**

### **Kroki:**

1. **Zidentyfikuj główne klasy**:
   - Na podstawie wymagań systemu zidentyfikuj główne klasy, takie jak: `Osoba`, `Nauczyciel`, `Uczeń`, `Kurs`, `Sala lekcyjna`, `Materiał`.

2. **Zdefiniuj atrybuty i metody** dla każdej klasy:
   - Przykłady atrybutów:
     - **Osoba**: `imię`, `nazwisko`, `dataUrodzenia`
     - **Kurs**: `nazwaKursu`, `kodKursu`
     - **Sala lekcyjna**: `numerSali`, `pojemność`
     - **Materiał**: `nazwaMateriału`, `typPliku`

3. **Zidentyfikuj role specjalizowane**.
  
---

## **Część 2: Modelowanie strukturalne – Definiowanie relacji między klasami**

### **Kroki:**

1. **Zidentyfikuj relacje między klasami**:
   - **Dziedziczenie**: ?
   - **Asocjacja**: ?
   - **Agregacja**: ?
   - **Kompozycja**: ?
   - **Relacja zwykła**: ?

2. **Określ liczności relacji**.
   
---

## **Część 3: Projektowanie – Stworzenie diagramu UML**

### **Kroki:**

1. **Narysuj diagram UML**:
   - Użyj narzędzia do rysowania diagramów UML (np. **Lucidchart**, **Draw.io**, **StarUML**), aby przedstawić klasy i relacje między nimi.
   - Diagram powinien zawierać:
     - **Dziedziczenie**.
     - **Asocjację**.
     - **Agregację**.
     - **Kompozycję**.
     - **Relację zwykłą**.

2. **Zweryfikuj poprawność diagramu**:
   - Upewnij się, że wszystkie klasy i relacje zostały poprawnie odwzorowane w diagramie.
   - Sprawdź, czy diagram odzwierciedla wszystkie wymagania systemu.

---

## **Podsumowanie Laboratorium:**

W ramach tego laboratorium studenci:
1. Zidentyfikują klasy i atrybuty na podstawie wymagań systemu.
2. Zrozumieją i zastosują różne relacje między klasami: dziedziczenie, asocjacja, agregacja, kompozycja i relacje zwykłe.
3. Stworzą diagram UML, który dokładnie odzwierciedla strukturę systemu zarządzania szkołą.

---

## **Wymagania końcowe**:
- Studenci muszą dostarczyć diagram UML przedstawiający wszystkie zidentyfikowane klasy i relacje.
- Diagram powinien być w pełni poprawny pod względem zastosowania relacji oraz liczności.
- Projekt powinien spełniać wszystkie wymagania funkcjonalne systemu.

---

## **Narzędzia rekomendowane do tworzenia diagramów UML:**
- **Lucidchart**
- **Draw.io**
- **StarUML**
- **Visual Paradigm**

---

To laboratorium pomoże studentom zrozumieć, jak w praktyce wygląda analiza obiektowa, oraz nauczy ich stosowania różnych typów relacji między obiektami w systemach obiektowych.

