## UART
UART jest modułem odpowiedzialnym za obsługę **asynchronicznej** komunikacji (nie ma zegara synchronizującego odbiornik) **szeregowej** pomiędzy dwoma urządzeniami. 

Na zajęciach zaś używamy konkretnej odmiany *USART (Universal Synchronous Asynchronous Reciever-Transmitter*, którzy posiada opcje synchronicznej komunikacji

![[UART.png]]

*Data Bus* równolegle przesyła bit po bitcie do interfejsu UART

Aby moduły UART mogły się ze soba porozumiewiać powinny one mieć ustawiony taki sam baud-rate (maksymalna ilość bitów na sekunde). Dzięki temu nie musimy synchronizować modułów UART, ponieważ przesyłają z taką samą prędkością dane.

### Przesył danych
	![[Pakiet UART.png]]

1) Start bit - Podczas gdy nie są przesyłane dane zwykle moduł UART jest w stanie wysokim (napięcie jak dla 1). W momencie gdy chce zacząć przesyłać dane przełącza się z 1 na 0 w celu zasygnalizowania nowej ramki.

2) Data Frame - może zawierać od 5 do 9 (gdy nie ma bitów parzystości) bitów danych
3) Parity Bits - bit parzystości tak aby była parzysta liczba 0 i 1 (modulo 2 = 0)
4) Stop bits - moduł UART sygnalizuje zakończenie transmisji poprzez przejście ze stanu niskiego do wysokiego (restartuje się żeby mógl potem znowu  zacząć od Start Bit)


## Przerwania 

1) **Interrupts** - Dostajemy przerwanie, które sygnalizuje, żę coś się zadziało
2) **Polling** - Odczytywanie co jakiś czas stanu w celu zobaczenia czy jakieś zdarzenie wystąpiło
