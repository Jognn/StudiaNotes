## BIOS
BIOS (Basic Input Output System) - sytem wlaczany po uruchomieniu komputera, sprawdza podlaczeone peryferia i komponenty komputerowe (w obecnych systemach wlaczone sa na poczatku sterowniki/dziala to troche inaczej)

- Nie ma on systemu plików
- Rozpoczyna prace od wczytania *boot sectora (Cylinder 0, Head 0, Sector 0)* - sprawdza czy ostatnie bajty to **0xaa55**. Jeżeli tak znaczy, że jest to kod służacy do bootwania

Przykładowy boot sector (little-endian format):

![[Przyklad boot sectora.png]]

- **BIOS** ustawia *Interrupt Vector Table* na początku pamięci (fizyczny adres 0x0)


## Odwołania
- [[Interrupts]]