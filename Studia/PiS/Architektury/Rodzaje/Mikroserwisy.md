## Mikroserwisy
Definicja: Polegają one na rozbijaniu komponentów na oddzielne,  małe części, które można poddawać niezależnym zmianom, skalowaniu i administracją
![[Mikroserwisy.png]]

- Wprowadzają one również swoje problemy: *Odnajdywanie serwisów*, *logowanie wiadomości*, *zarządzanie transakcjami*

**Zalety:**
-Większe możliwości skalowalności
-Niezależność technologiczna (każdy może być napisany przy użyciu innych technologii)


**Wady:**
-Opóźnienie w komunikacji (wysyłamy żądania restowe)
-Wyszukiwanie błędów jest trudniejsze niż w Monolicie

<br> 
<br>

### Wzorzec Saga
Jest to wzorzec, który rozwiązuje problem spójności transkacji w rozproszonej architekturze. Opiera się on na *local transactions* w każdym w każdym serwisie. Jeżeli jedno z lokalnych transkacji zakończy się niepowodzeniem wtedy wzorzec uruchamia mechanizm odrwacania.

Istnieją dwa rodzaje organizacji Saga:
1) Choreografia 
2) Okiestracja 
<br>

#### 1) Choreografia (rozproszone)
![[Saga_Choreografia.png]]
Polega ono na na ciągu przesyłaniu zdarzeń przez każdy z serwisów. Jeżeli, któryś w kolejce powie, że wystąpił błąd wtedy wszystkie transakcje są wycofywowane

#### 2) Orkiestracja (scentralizowane)
![[Saga_Orkiestracja.png]]
Istniej jeden główny komponent, który jest odpowiedzialny za incijalizację kolejki transakcji. W momencie wystąpienia błedu, wszystkie transakcje są wycofywane i zwraca on klientowi odpowiedź.


<br>
<br>

### LINKS:
https://docs.microsoft.com/en-us/azure/architecture/reference-architectures/saga/saga
