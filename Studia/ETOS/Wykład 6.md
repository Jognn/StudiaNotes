## Wykład 6 etos
Moda rozkładu - wartośc występująca z największym prawdopodobieństwem

**Estymator obciążony wariancji - $n$ w mianowniku**
$$\sigma^2 = \frac{1}{n}\sum$$
<br>

Estymator nieobciążony wariancji - ten z $n-1$ w mianowniku

<br>

**Współczynnik zmienności (wariancji)**
$$V_t = \frac{\sqrt{VAR(N_t)}}{E(N_t)}$$
- Dla rozkładu punktowego $V_t = 0$ 
- Dla rozkładu wykładniczego $V_t = 1$

<br>

**Kwantyl**
$$q_p = min\{x: F(x) \geq p\}$$

- 10 percentyl = 0.1 kwantyl
- *Kwartyle*
	Q1 - 0.25 kwantyl
	Q2 - 0.5 kwantyl
	Q3 - 0.75 kwantyl

<br>

**Przedziały ufności:**
Jeżeli przedziały ufności na siebie nachodzą to można 
- Trzeba wyznaczać przedziały ufności!!

Prawidłowy pomiar:
-Powtarzamy pomiar n razy i wyznaczamy średnią oraz przedziały ufności

$$Pr\{c_1 \leq u \leq c_2 \} = 1 - \alpha$$
- Wyznaczamy przedział tak aby mięc przedział na poziomie 95%/99%

<br>

**Centralne Twierdzeni Graniczne (CTG)**
Zwykle dla 30 eksperymentów (N>30) używamy **CTG**, dla mnieszych używamy rorzkład **t-studenta**
 