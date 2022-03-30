## LAB2 - Przetworniki ADC
W przetwornikach ADC wartość napięcia wejściowego $U_{we}$ porównywana jest do napięcia referencyjnego $U_{ref}$

![[Schema przetwornika ADC.png]]

<br>

### Kwantyzacja
![[Krzywa przetwarzania.png]]
- Na krzywej przetwarzania można zobaczyć, że oś pozioma to stosunek $\frac{U_{we}}{U_{ref}}$

**Wartość cyfrowa napięcia**
![[Wartosc cyfrowa napiecia.png]]

**Szerokość jednego schodka**
![[Szerokosc jednego schodka.png]]

- *Błąd kwantyzacji* to odchylenie zarejestrowanej wartości cyfrowej od wartości rzeczywistej. Spowodowany jest on skończoną rozdzielczością przetwornika

**Maksymalna wartość błędu kwantyzacji**
![[Najwiekszy blad kwantyzacji.png]]

![[Wykres bledu kwantyzacji.png]]

**Rodzaje przetworników**:
1) Przetwarzanie bezpośrednie (Flash)
2) Kompensacyjno-wagowe (SAR)
3) Modulacji sygnału (sigma-delta)


- **Zdolność rozdzielcza** = $\frac{U}{2^n}$

- Twierdzenie o próbkowaniu  - częstotliwośc próbkowania musi być conajmniej większa od dwukrotności sygnału

### Parametry dokładności przetwarzania
1) Nieliniowość całkowa
2) Nieliniowość różniczkowa
3) Błąd przesunięcia zegara
4) Współczynnik zmian cieplnych
5) Błąd kwantyzacji

**Czas pomiaru:**
$$T_{CONV} = T_{probkowania} + T_{konwertowanie}$$





