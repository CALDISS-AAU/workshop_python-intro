---
title: Logiske værdier (booleans)
weight: 8
---
youtube Vm8gu-hJV68 >}}

En stor del af programmeringsarbejde involverer at arbejde med logiske værdier; også kaldt booleanske værdier. Disse lagres som typen `bool`.

Variable af typen `bool` kan *kun* antage værdien sandt (`True`) eller falsk (`False`). Python har en række operatorer, som altid returnerer en booleansk værdi:


```python
a = 10
b = 12

a == b
```




    False



I ovenstående bruges `==` til at spørge: "Er a lig med b?" (`=` bruges selvfølgelig ikke, da denne bruges til at danne variable).

En booleansk værdi kan tilskrives en variabel ligesom alle mulige andre værdier. Sådanne variable bliver typen boolean, som altså kun kan være sand (`True`) eller falsk (`False`).


```python
check = a == b

print(check, 
      type(check))
```

    False <class 'bool'>
    

Her er en række operatorer, som altid returnerer en booleansk værdi:

```
a == b  # Lig med
a != b  # Ikke lig med
a > b   # Større end
a >= b  # Større end eller lig med
a < b   # Mindre end
a <= b  # Mindre end eller lig med
```

Mange funktioner og metoder returnerer også booleanske værdier. Fx returnerer metoden `.startswith()` en booleansk værdi afhængig af, om en tekststreng starter med et vis stykke tekst eller ej:


```python
words = "Hello there!"

print(words.startswith("Hello"))
```

    True
    

Booleanske værdier har mange formål:

- Check af resultat: Værdier checkes op imod et sæt af gyldige værdier
- Filtrering: Værdier udvælges efter bestemte betingelser
- Betinget udførelse: Dele af kode udføres kun, hvis en bestemt betingelse er mødt (noget er "sandt" eller "falsk")
- Fejlhåndtering: Visse fejl kan forventes ved at sætte betingelser op for derefter at håndtere dem

---
## VIDENSCHECK

Tag et kig på nedenstående kode:


```python
a = 7
b = 17
c = a < b
```

*Hvilken variabel indeholder en booleansk værdi?*

{{%expand "Løsning" %}} `c` indeholder en booleansk værdi (`True`), da det er resultatet af testen af, hvorvidt `a` er mindre end `b`.
{{%/expand%}} 

---