---
title: Classes
weight: 6
---
Tidligere i dette materiale blev det forklaret, hvordan Python adskiller mellem variable gennem variablens *type*.

Mere specifikt er et objekt i Python altid en eller anden *class*. En *class* tillader at både data (attributes) og funktioner (metoder) lagres i et objekt. Når et objekt defineres som fx en string, så er det objekt en "string-class", hvilket dikterer, hvad vi kan gøre med objektet (hvilket attributes og metoder, som der er til rådighed).

Når man bruger Python til dataanalyse, har man sjældent brug for selv at definere classes. Man bør dog være opmærksom på, hvilken class man faktisk laver, når man danner et objekt/en variabel, da denne sætter rammerne for, hvad der er muligt.

## Opbygning af en class

Nedenstående ses et eksempel på opbygning af en class kaldt `greeter`. Denne class indeholder metoder til at lave hilsner. Den har ikke nogen praktisk anvendelighed, og skal blot ses som et eksempel:


```python
class greeter:
    def __init__(self, name):
        self.name = name
    
    def say_hello(self):
        print("Goddag " + self.name + "!")
    
    def say_goodbye(self):
        print("Farvel " + self.name + "!")
```

I ovenstående defineres classen `greeter`. Læg mærke til hvordan classens indhold er en række funktioner. Den første funkion `__init__` kaldes også for "constructor". I denne defineres, hvad der skal ske, når man laver en variabel med denne class. Her defineres også, hvilke argumenter classen kræver. I denne funktion kræves blot ét input (`name`). Derudover skal funktioner i en class (metoder) altid have sig selv med som argument (`self`).

Ligesom en funktion returnerer en class ikke noget, før vi bruger den. I nedenstående laves en variabel med classen `greeter`: 


```python
my_greeter = greeter("Kristian")
```

Ovenstående kommando returnerer ikke noget, da vi blot har defineret en variabel (`my_greeter`) som class `greeter` med navnet `"Kristian"` som input. 

Fordi `my_greeter` nu er af class `greeter`, kan vi tilgå data/information og funktionerne i classen. Data/information i en class kaldes "attributes" og tilgås blot med punktum efterfulgt af attribut-navn.

`greeter`-class indeholder kun ét attribut (`name`):


```python
my_greeter.name
```




    'Kristian'



Funktionerne i en class kaldes metoder ("methods"). Som tidligere forklaret tilgås disse med punktum efterfulgt af metodenavnet efterfulgt af parentes. De to metoder i `greeter`-classen tager kun sig selv som argument, så der skal ikke specificeres yderligere input:


```python
my_greeter.say_hello()
my_greeter.say_goodbye()
```

    Goddag Kristian!
    Farvel Kristian!
    
