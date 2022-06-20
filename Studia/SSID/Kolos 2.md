## Kolos 2
Czas trwania okna:
$$t_O = 2*A*100 \micro s + max(t_R) + t_d$$
$t_O$ - czas trwania okna
A - czas propagacji
$t_R$ - opoźnienie zmienne
$t_d$ - czas nadawania

**Czas propagacji wariant 1:**
$$A = \frac{L[km]}{20 [km]}$$
**Czas propagacji wariant 2:**
$$A = \frac{L_2 - L_1 [km]}{20 [km]}$$
$L_2$ - najdłuższa droga do ONU
$L_1$ - nakrótsza droga do ONU


Wirtualne opoźnienie czasowe, pozwala aby każde urządzenie ONU dostawało z takim samym opóźnieniem wiadomości. Działanie to wprowadza synchronizacje i zapobiega kolizją na odcinku Splitter - OLT w przypadku uplinku.
