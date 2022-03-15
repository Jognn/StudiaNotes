## CQRS *(Command and Query Responsibility Segregation)*

Jest to wzorzec, który polega na oddzieleniu **zapisywania danych (command/komenda)** od **odczytywania danych (query/zapytanie)**. Rozwiązanie to jest używane przy skomplikowanych systemach, gdzie zapisywanie i odczytywanie danych jest używane w niesymetrycznej skali. 

![[CQRS_model.png]]

- Wzorzec zakłada używanie bardziej *task-based*, niż *data-centric* komend ("Book hotel room" not "set Reservation Status to Reserved")


**Zalety**
-Niezależne skalowanie, można lepiej skalować odczytywanie od zapisywania
-Optymalizacja schematu odczytywania pod najlepszy odczyt jak i optymalizacja schematu zapisywania pod najlepszy zapis (niezależnie)
-Prostsze queries (można uniknąć skomplikowanych)

<br>

---------------------
### Links
[[Asynchronous Messaging]]