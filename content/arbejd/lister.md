---
title: Lister og tuples
weight: 1
---
## Lister

Den mest basale datastruktur er en liste. En liste defineres med `[]`:


```python
my_list = [2, 7, 9, 10]
```

I ovenstående defineres listen `my_list` til at indeholde værdierne 2, 7, 9 og 10. En liste kan fremkaldes ligesom hvilken som helst anden variabel:


```python
print(my_list)
```

    [2, 7, 9, 10]


En liste er blot en beholder af forskellige variable. Lister kan derfor indeholde variable af forskellig typer:


```python
my_list2 = [2, "hello", 10, True]

print(my_list2)
```

    [2, 'hello', 10, True]


Lister kan også indeholde andre lister:


```python
my_list3 = [9, 17, [2, 91], 16]

print(my_list3)
```

    [9, 17, [2, 91], 16]


**Variable i lister**

En liste kan bestå af en række variable:


```python
a = 4
b = 9
c = 11

my_list4 = [a, b, c]

print(my_list4)
```

    [4, 9, 11]


Bemærk dog, at når en liste dannes med variable, så er det variablenes værdi(er), der lagres i listen og ikke selve variablen. 

Det kan ses, hvis man ændrer en af variablerne i listen. Herunder ændres variabel `a` fra `4` til `21`. Selvom variablen ændres, så er indholdet af listen (`my_list4`) ikke ændret. 


```python
print(my_list4)   # listen består af værdierne 4, 9 og 11 tilsvarende variable a, b og c

a = 21            # værdien af variabel af ændres

print(my_list4)   # listens indhold er uændret (stadig 4, 9 og 11)
```

    [4, 9, 11]
    [4, 9, 11]


Når listen genereres, lagres den værdi, som `a` har på det tidspunkt, listen generes. Værdiens tilknytning til variabel `a` lagres altså ikke i listen.

**Index**

Hvert element i en liste tildeles et *index*. Et bestemt element kan altid kaldes frem ved at refere til elementets index med `[]`:


```python
my_list = [2, 7, 9, 10]
print(my_list[0])
```

    2


Index i Python starter altid med 0. Derfor gives i ovenstående det første element af listen `my_list` ved at refere til index 0.

Et element i en liste kan overskrives ved at refere til dets index:


```python
print(my_list)

my_list[2] = 28
print(my_list)
```

    [2, 7, 9, 10]
    [2, 7, 28, 10]


**Slicing**

Elementer i et vis interval kan kaldes frem ved brug af `:` (også omtalt "slicing"). Slicing tager elementer fra det første index givet (inklusiv) til det sidste index givet (eksklusiv).


```python
print(my_list[1:3])
```

    [7, 28]


Ovenstående tages fra index 1 og op til index 3 eklskusivt index 3; altså index 1 (listens andet element: 7) og index 2 (listens tredje element: 9).

Listens længde (antallet af elementer) returneres med funktionen `len()`:


```python
len(my_list)
```




    4



---
## VIDENSCHECK

Tag et kig på nedenstående liste:


```python
a_list = [45, 67, 3, 36, 87]
```

*Hvilket element (tal i listen) har index 3?*

{{%expand "Løsning" %}} Index 3 af `a_list` (`a_list[3]`) indeholder tallet 36; altså det fjerde element, da index tælles fra 0.  


```python
print(a_list[3])
```

    36


{{%/expand%}}

---

## Tuples

Tuples fungerer på mange måder ligesom lister med den undtagelse, at værdier i en tuple ikke kan ændres.

Tuples laves med `()`:


```python
my_tuple = ("Katarn", "Kenobi", "Windu")

print(my_tuple)
```

    ('Katarn', 'Kenobi', 'Windu')


Elementer i en tuple har indexes ligesom ved lister:


```python
my_tuple[0]
```




    'Katarn'



Forsøger man at ændre et element af en tuple, får man dog fejl:


```python
my_tuple[0] = "Palpatine"
```


    ---------------------------------------------------------------------------
    
    TypeError                                 Traceback (most recent call last)
    
    <ipython-input-76-b2ea6727d80b> in <module>
    ----> 1 my_tuple[0] = "Palpatine"


    TypeError: 'tuple' object does not support item assignment


---
## VIDENSCHECK

Tag et kig på de to nedenstående datastrukturer (`a` og `b`):


```python
a = [2, 90, 10, 17]
b = (56, 78, 3, -9)
```

*Kan tredje element af `b` (index 2: `3`) ændres til `49` ved at skrive `b[2] = 49`?* 

{{%expand "Løsning" %}} Nej. `b` er en tuple, og værdierne kan derfor ikke ændres. Værdierne i `a` kan dog ændres, da det er en liste. {{%/expand%}}

---
