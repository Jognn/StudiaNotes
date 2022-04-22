## Wyklad 5

Jitter - zmiana sygnału fizycznego (faza, częstotliwość itp). Często używane w innych odniesieniach :)

## Pomiary Jedno i dwupunktowe
### One point IP Packet Delay Variation 
Metoda polega na padaniu IPDV tylko w odbiorniku. Bada różnice pomiędzy teoretycznym czasie przyjścia, a rzeczywisty czas przyjścia.

Jeżeli jest mocne opoźnienie to czas rzeczywistym staje się punktem odniesienia.

1) Pakiety wysyłane w stałych odstępach T
2) Nie wymaga synchronizacji (odbiornika i zegara)
3) Metoda pozwala estymować wartość IPDV



## Rodzaje pomiarów
**Pomiar offline** - pomiary wykonywane po tym jak usługa przestanie być używana (w laboratorium po czasie)

**Pomiar online** - pomiary w czasie rzeczywsitym (podczas trwania usługi)

**Pomiar in service** - wysyłane są pakiety w strumieniu użytkownika, które monitorują jakość usługi

**Pomiar out of service** - sztucznie dodane połączenie, które udaje użytkownika i sprawdza dla niego jak by się zachowało

## Metody pomiarow
### Pasywne
### Pomar AvB metodą dyspersji par pakietów
C - przepływnośc

Przypadek 1: 
$C_1=C_2 => \Delta_{in} = \Delta_{out}$

Przypadek 2:
$C_1>C_2 => \Delta_{in} < \Delta_{out}$

Przypadek 3:
$C_1<C_2 => \Delta_{in} = \Delta_{out}$
(Dziwne :D)

Wniosek: Z szybszego łącza jak przechodze na wolniejsze to się rozszerza $\Delta_{out}$

- Wprowadzenie Cross Traffic powoduje że metoda nie wiadomo co mierzy

#### Pociągi pakietów (packet Trains)

$$R_s = \frac{L}{\Delta_s}$$
<h2 style="border: 1px solid black">wzoryyyyy</h2>

wykresss


## Analiza wyników
- Wynik pomiaru to zmienna losowa (powtórzenie w tym samych warunkach może dać inną wartość)

Dystrybuanta
$F_s(a) = P(x < a)$

Funkcja gęstości prawdopodobieństwa
$f(x) = \frac{dF(x)}{dx}$

Wartość oczekiwana
$u = E[X]= \sum x_i * p_i$

Wariancja
$\sigma ^2 = \sum(x_i - u)^2 * f(x_i)$

Średnia arytmetyczna (estymator wartości oczekiwanej populacji)

Średnia geometryczna


















