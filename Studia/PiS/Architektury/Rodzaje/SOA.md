## SOA *(Service oriented Architecture)*
![[SOA.png]]
- Rozwiązanie w postaci rozproszonych usług sieciowych
- Posiada ono własną szynę ESB (Enterprise Service Bus), na podstawie której scentralizowany komponent przeprowadza integracje z systemami backendowymi. Udostępnia im różne usługi do ponownego wykorzystania dla aplikacji 
- Często wykorzystuje protokół *SOAP*  do komunikacji (ale nie zawsze)

**Zalety:**
-Standaryzacja
-Mniej czasu na integracje


**Wady:**
-Magistrala ESB staję się często "wąskim gardłem"
-Zmiany w magistrali ESB mogą niekorzystnie odziaływać na aplikacje 
