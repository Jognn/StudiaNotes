## Usługi sieciowe

**Warstwa transportowa**: HTTP/HTTPS, FTP, STMP itp

**Warstwa komunikacji**: SOAP, dialekt XML definiujący sposób wymiany informacji między konsumentem 

**Kontrakt/Dokumentacja**: dokument WSDL, jest to kontrakt pomiędzy producentem i konsumentem (takie nasze API)

![[Struktura SOAP.png]]

![[Dokument - WSDL.png]]

- Występują jeszcze handlery/filtry
![[Przechwytywacze.png]]


- Pliki binarne w SOAP mogą być zakodowane jako Base64 lub może istnieć załącznik do linku gdzie to pobrać

Zalety SOAP:
1) Dobre wsparcie starszych systemów
2) Sformalizowany kontrakt
3) Możliwość przetwarzania stanowego (jest jakaś sesja)


https://www.developer.net.pl/ogolne/rest-vs-soap/
https://rapidapi.com/blog/api-vs-web-service/