## Dostępne rodzaje technologi

### 1) Bare metal:
- Węzeł fizyczny = węzeł logiczny
- Komponenty oprogramowania zainstalowane bezpośrednio na OS

**Zalety:**
-Możliwość mocnej <ins>izolacji komponentów</ins>. Mogą one nie dzielić żadnej wspólnej przestrzeni

**Wady:**
-Mała elastyczność
<br>
<br>

### 2) Maszyna wirtualna:
Istnieją dwa typy Hypervisorów:
1) Działający na systemie operacyjnym
2) Będący samym w sobie również systemem operacyjnym


**Zalety:**
-Wprowadzenie większej elastyczności
 <br>
 <br>

### 3) Kontener:
- Dzielenie zasobów na namespacy
- Zaleca się, że jeden kontener to jeden proces! 

**Zalety:**
-Duża elastyczność
-Wymaga mniejszej ilości zasobów w stosunku do VM

**Wady:**
-Istnieje o wiele mniejsza izolacja (dzielony system operacyjny)
<br>
<br>

### 4) Servless computing:
Model, w którym dostawca na żądanie przydziela klientą daną moc obliczeniową. Nie posiadają oni żadnego dedykowanego serwera


