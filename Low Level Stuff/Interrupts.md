## Interrupts

- Przerwania zostają wywołane z konkretnym indexem w tablicy *Interrupt Vector Table*. Zawiera ona pointery do pamięci zawierającej *Interrupt Service Routine (ISR)* obsługującej przerwanie
  
- Tablica *Interrupt Vector Table* jest ustawiana przez **BIOS** z początku pamięci (fizyczny adres 0x0)
  
 - Dodatkowo *ISR* sczytuje wartość rejestru **ax** w celu ustalenia dodatkowych parametrów obsługi (jaki znak będzie wyświetlony na monitorze itp)


## Odwołania
- [[BIOS]]