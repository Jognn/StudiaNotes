## Monolit
Definicja: Cały kod jest brany z jednego repozytorium i kompilowany w pojedyńczy artefakt (chodzi tu o pakowanie i dystrybucje).

![[Monolit.png]]
<p style="text-align:center; font-style:italic"> Zobrazowanie braku faktycznej hermetyzacji kodu (warstwa widoku może się i tak dostać do warstwy danych) </p>

**Zalety:**
-Łatwa i szybka implementacja
-Mała złożoność infrastruktury

**Wady:**
-Ciężko zmienić technologie
-Ograniczona skalowalność
-Wymaga znajomości większości kodu (mała izolacja obowiązków)

<br>
<br>

## Modularny monolit
Różni się od monolitu tym, że konkretne komponenty pakowane są w oddzielne moduły. Powoduję to faktyczną hermetyzacje kodu (np warstwa widoku nie ma bezpośredniego dostępu do warstwy danych).

![[Modularny monolit.png]]
<p style="text-align:center; font-style:italic"> W tym przypadku można zauważyć, że warstwa widoku nie może bezpośrednio odwołać się do warstwy danych. Są one odizolowane </p>