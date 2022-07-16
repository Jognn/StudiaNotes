## Class terminology

**data members** - atrybuty funkcji
**member functions** - metody funkcji (w tym konstruktor i destruktor)

#### Konstruktor
- W celu użycia domyślnego konstruktora należy pominąć nawiasy


1) **Functional form** (nawiasy)

Przykład:
`Rectangle rect`  - domyślny konstruktor zostanie użyty'
`Rectange rect()` - domyślny konstruktor nie zostanie użytym kompilator potraktuje to jako próba wywołania funckji *rect()*


2) **Uniform initialization**  (curly braces/brackets)

Przykład:
`Rectangle rect = width` - pojedybcza wartosc
`Rectangle rect {height = 3, width=2}` - wiele wartości

3) **Member initialization in constructors**
Inicjalizacja w ten sposób pozwala na zdefiniowanie konstruktorów obiektów podanych w parametrach (domyśłnie używany jest default konstruktor). Dzięki temu parametr będzie tylko raz iniclajizowany

Przykład:
`Rectangle(std::string name, FooObject bar) : bar(name) {}`

