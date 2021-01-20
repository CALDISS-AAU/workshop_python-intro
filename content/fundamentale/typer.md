---
title: Typer
weight: 3
---

{{< youtube ranfUBt6538 >}}

En variabel er ikke bare en variabel i Python. Fordi en variabel kan være så mange ting, så er Python nødt til at adskille variable fra hinanden. Dette gøres ved at variable lagres som en bestemt *type*. 

Typen af variabel fortæller Python, hvad det er for en slags information, som variablen indeholder, og sætter betingelserne for, hvad der kan lade sig gøre med variablen.

Som man arbejder med Python, vil man støde på mange forskellige typer. I første omgang fokuseres på to af de mere gængse typer:

- Numeriske typer (fx integers og floats)
- Tekst typer (fx strings)

## Numeriske typer

Python gætter altid typen, når en variabel lagres. Når en variabel består af en talværdi, vil denne fx lagres som en numerisk type. Talværdien kan enten lagres som en *integer* (heltal) eller et *float point* (decimaltal). 

Python kan fortælle typen med funktionen `type()`:


```python
a = 42
print(type(a))
```

    <class 'int'>


Variablen `a` er typen `int`, som står for *integer* - et heltal. Som set i sidste afsnit, kan der foretages forskellige matematiske operationer med heltal.

Tildeles en variabel et tal med decimaler, lagres det som et *float point*.:


```python
b = 42.2
print(type(b))
```

    <class 'float'>


Bemærk, at når man dividerer, så vil typen altid blive et *float point* - også selvom resultatet er et heltal:


```python
print(a)
print(type(a))   # a er lige nu integer
b = a / 2        # b defineres som a / 2
print(b)
print(type(b))   # b er et float point
```

    42
    <class 'int'>
    21.0
    <class 'float'>


At Python gerne vil adskille mellem typer har noget at gøre med, hvordan én type information kræver mere computerhukommelse at lagre end en anden. Dette kan have betydning, når man arbejder med enorme datamængder, hvilket sjældent er tilfældet i samfundsvidenskabelige analysearbejder.

---
## VIDENSCHECK

I ovenstående bliver variablen `a` brugt til at definere variabel `b`. 

*Hvilken type er variablen `a` efter at variabel `b` defineres?*

{{%expand "Løsning" %}}
`a` er stadig en *integer*. `a` ændres ikke i koden, men bliver blot brugt til at lave variabel `b`.
{{% /expand%}}

---

## Tekst typer

Python lagrer variable som en tekst type, hvis det indeholder tekst. Python fortælles, at noget skal behandles som tekst, ved at indkapsle det med `'` eller `"`:


```python
a = "Hello"
print(type(a))
```

    <class 'str'>


En variabel med et stykke tekst kaldes en `string` (forkortet i Python som `str`). 

I modsætning til numeriske typer, giver matematiske operationer ikke meget mening på et stykke tekst. Dog tillader Python at bruge visse matematiske operatorer på tekst:


```python
b = " there"   # bemærk mellemrum i string
print(a * 2)   # gentager string
print(a + b)   # sætter de to strings sammen (kaldes også for "paste")
```

    HelloHello
    Hello there


{{% notice note %}}

Bemærk at Python *altid* vil lagre variablen som string, hvis teksten er indkapslet med `'` eller `"`. Dette gælder også, hvis tal lagres på denne måde:


```python
a = 42    # integer
b = '42'  # string

print(a * 2) # 42 * 2 = 84 - kan lade sig gøre, da a er integer.
print(b * 2) # b er ikke et tal. "Pastes" sammen, da det er en string.
```

    84
    4242


Python gætter altid typen. Derfor gættes typen også, når man indlæser data i Python. Her kan problemet opstå, at Python læser information ind forkert - fx at tal læses ind som tekst.

{{% /notice%}}

## Ændring af typer (casting)

I visse tilfælde kan variable tvinges til at være en anden type (casting) med bestemte funktioner:

- Returnerer tekst type: `str(variabel)`.
- Returnerer numerisk type: `int(variabel` (integer) eller `float(variabel)` (float point).

Python vil altid gætte typen. Hvis Python gætter forkert, kan Python fortælles eksplicit, hvad typen skal være (hvis muligt).

Fx kan det hænde, at tal ved en fejl indlæses som tekst. Disse kan tvinges om ved at *caste* til en anden type:


```python
print(type(b))  # typen for b er her string
b = int(b)      # b dannes på ny som integer af b
print(type(b))  # b er nu integer
```

    <class 'str'>
    <class 'int'>


Alle typer kan selvfølgelig ikke castes om. Fx kan man ikke meningsfuldt konvertere tekst i form af ord til tal:


```python
a = "Hello"     # a dannes som string
print(type(a))  # typen er string
a = int(a)      # forsøger at konvertere a til integer - ikke muligt
```

    <class 'str'>



    ---------------------------------------------------------------------------
    
    ValueError                                Traceback (most recent call last)
    
    <ipython-input-36-cc7b3220923a> in <module>
          1 a = "Hello"     # a dannes som string
          2 print(type(a))  # typen er string
    ----> 3 a = int(a)      # forsøger at konvertere a til integer - ikke muligt


    ValueError: invalid literal for int() with base 10: 'Hello'


---
## ØVELSE: Typer

Lav variablene variablene `my_number3` og `my_number4`.

* `my_number3` skal indeholde `21`
* `my_number4` skal indeholde `"12"` (med anførselstegn!)

Forsøg at divider de to tal med hinanden (`my_number3 / my_number4`). Det giver fejl, men hvorfor?

Undersøg hvilken type `my_number3` og `my_number4` er med `type()`. Begge skal gerne være numeriske typer, før de kan divideres.

Ændr typen til numerisk for den variabel, som ikke er numerisk. 

Forsøg at divider de to tal med hinanden igen. Hvis du har rettet typen korrekt, bør det kunne lade sig gøre og give tallet `1.75`.

{{%expand "Løsning" %}}
`my_number4` er lagret som tekst. Denne skal derfor konverteres til et tal, fx ved at definere variablen om som `my_number4 = int(my_number4)`. Derefter bør det kunne lade sig gøre at dividere de to tal med hinanden (`my_number3 / my_number4`).


```python
my_number3 = 21
my_number4 = "12"

print(type(my_number3))
print(type(my_number4))

my_number4 = int(my_number4)
print(type(my_number4))

my_number3 / my_number4
```

    <class 'int'>
    <class 'str'>
    <class 'int'>





    1.75



{{% /expand%}}

---
