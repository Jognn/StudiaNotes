## Dockerfile

Obraz dockerowy jest budowany na podstawie *Dockerfile* oraz dodatkowego *contextu* (PATH, URL)

- Docker cachuje sobie zbudowane obrazy
- Docker  usuwa komentarze w Dockerfile przy buildowaniu

<br> 


#### Format Dockerfile
  1) **FROM ** - określa parent image, każy Dockerfile musi się zaczynać od tej instrukcji
  2) **RUN**
  3)  **CMD** - wykonywanie czegoś w konsoli, jeżeli dodamy przy buildowaniu kontenera argument zostanie ono pominięte
  4)  **ENTRYPOINT** - tak samo jako **CMD**, ale zawsze zostanie wykonane


<br>

#### Parser directives
Są to dodatkowe dyrektywy definiowane na początku pliku w postaci komentarzy
![[Parser-directive.png]]

<br> 

#### Zmienne środowiskowe replacement
![[env-replacement.png]]


