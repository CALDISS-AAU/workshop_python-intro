---
title: Funktioner
weight: 4
---
{{< youtube pKID5oLWy5k >}}

En central del af det at arbejde med et programmeringssprog er at bruge funktioner. Funktioner tager et eller flere input (kaldet "argumenter"), foretager et eller andet med disse og returnerer (for det meste) et output.

Funktioner i Python har følgende format:

- `function(argument1, argument2, ...)`

Funktioner bruges ved at skrive funktionens navn efterfulgt af argumenterne i parentes. Hvert argument adskilles med et komma (`,`). En funktion kan have et utal af argumenter, men oftest skal de som minimum have en eller flere variable som input.

Udover argumenter tager funktioner også ofte en del "keyword arguments" som input. Disse kan betragte som indstillinger, som man slår til og fra i funktionen. "keyword arguments" indgår i funktionen med navnet på indstillingen, et `=` og hvad indstillingen skal sættes til; lig nedenstående:

- `function(argument1, argument2, keywordargument1 = "something")`

Ligesom med argumenter kan en funktion have rigtig mange "keyword arguments"/indstillinger. Det er dog sjældent, at man behøver at forholde sig til alle indstillingerne, da de fleste funktioner har en eller anden form for standardindstilling.

## Sådan bruges funktioner

Tidligere i dette materiale har funktionerne `print()` og `type()` været brugt. Ved `print()` har denne kun været brugt med et enkelt argument; altså den variabel, som skal printes, men faktisk accepterer print flere argumenter:


```python
a = "Hello"
b = "there"
print(a, b)
```

    Hello there


Derudover har `print()` også en række "keyword arguments"/indstillinger, som det ses af dokumentationen herunder:

```
Docstring:
print(value, ..., sep=' ', end='\n', file=sys.stdout, flush=False)

Prints the values to a stream, or to sys.stdout by default.
Optional keyword arguments:
file:  a file-like object (stream); defaults to the current sys.stdout.
sep:   string inserted between values, default a space.
end:   string appended after the last value, default a newline.
flush: whether to forcibly flush the stream.
Type:      builtin_function_or_method
```

Her ses det, at `print()` har adskilige indstillinger. `sep` bestemmer fx, hvad der skal adskille de forskellige værdier, som tages ind. Bemærk, at alle indstillinger er sat til en eller anden indstillling som standard. `sep=' '` betyder, at de forskellige værdier adskilles med et mellemrum som standard. Hvis denne ændres til noget andet, vil outputtet se anderledes ud:


```python
print(a, b)              # printer a og b med standardindstilling (adskiller med mellemrum)
print(a, b, sep = ", ")  # sep ændres til komma
```

    Hello there
    Hello, there


En funktion kan have rigtig mange indstillinger, og i praksis forholder man sig kun til få af disse, da man for det meste kan lade standardinstillingerne være, som de er. 

{{% notice info %}}
Man kan altid få hjælpefilen/dokumentationen frem til en funktion ved at skrive `?[function]` (fx `?print` for dokumentationen for `print()`). Mange IDE'er understøtter også, at man trykker `Shift + Tab` inde i parentesen af en funktion for at få vist dele af hjælpefilen.
{{% /notice%}}

{{% notice note %}}
Det, som der står i de forskellige "keyword arguments" i dokumentationen for en funktion, er funktionens standardindstillinger. 
{{% /notice%}}

---
## VIDENSCHECK

Hvordan får man `print()` til at adskille input værdierne med en `-`?

{{%expand "Løsning" %}}
Indstillingen `sep` sættes til `sep = '-'`.


```python
print(a, b, sep = '-')
```

    Hello-there


{{%/expand%}}

---

## Hvor kommer funktioner fra?

Python har en række funktioner indbygget, men faktisk kommer størstedelen af funktionerne i Python fra alle mulige andre, som har udviklet funktioner til forskellige formål, som andre derefter kan gøre brug af. Andre funktioner hentes ind i form af "pakker", som gennemgås senere i dette materiale.

Man kan fristes til at lære Python ved at forsøge at lære så mange funktioner som muligt. Dette er en håbløs og nærmest umulig opgave givet omfanget af, hvad der findes af funktioner, der kan hentes til Python. I praksis opbygger man arbejdsgange eller workflows, hvori man har tendens til at bruge de samme funktioner igen og igen. Derfor er en god tilgang til Python at spørge: *"Kan jeg bruge Python til X?"* eller *"Hvordan løser jeg problem Y i Python?"*, og så forsøge at finde de rette funktioner til det, frem for at spørge: *"Hvad kan jeg bruge Python til?"*, da man med dette spørgsmål ikke får nogen retning på det, man gerne vil lære om Python.

At Python kan så mange ting i dag skyldes netop, at folk rundt omkring i verden har stået over for forskellige udfordringer, som de har løst ved at udvikle funktioner til Python, som de derefter stiller til rådighed. 

Python fortæller med det samme, hvis funktionen, som man forsøger at bruge, ikke kendes af Python:


```python
add10(5)
```


    ---------------------------------------------------------------------------
    
    NameError                                 Traceback (most recent call last)
    
    <ipython-input-41-7452fc393844> in <module>
    ----> 1 add10(5)


    NameError: name 'add10' is not defined


Man kan dog til enhver tid definere sine egne funktioner:


```python
def add10(x):
    result = x + 10
    return result

print(add10(5))
```

    15


Funktioner defineres med `def` efterfulgt af navnet på den funktion, man gerne vil lave. I parenteserne skrives de input, som funktionen skal have. I ovenstående dannes funktionen `add10`, der tager et enkelt input og lægger 10 til. `x` i ovenstående er blot en "pladsholder", da `x` erstattes med hvadend, der sættes i funktionen, når den bruges.

Efter `:` skrives det, som skal ske i funktionen. Alle variable, som defineres inde i funktionen, eksisterer *kun* i selve funktionen. Sagt på en anden måde, så kan variable, der defineres i funktionen, ikke kaldes frem. I funktionen `add10()` defineres `result` undervejs, men den eksisterer ikke uden for funktionen:


```python
print(result)
```


    ---------------------------------------------------------------------------
    
    NameError                                 Traceback (most recent call last)
    
    <ipython-input-43-6459d04d738f> in <module>
    ----> 1 print(result)


    NameError: name 'result' is not defined


`result` er en variabel, der dannes inde i funktionen til at lave den nødvendige beregning. 

Hvis man vil lagre outputtet af en funktion til en variabel, kan man blot tilskrive variablen funktionen med det input, som funktionen skal have, for at få det ønskede output:


```python
a = add10(5)

print(a)
```

    15


En funktion skal gerne slutte med en `return` linje. Denne bestemmer, hvad funktionen skal sende tilbage. Udelades denne, returnerer funktionen `None`; altså intet:


```python
def add10(x):
    result = x + 10
    
print(add10(10))
```

    None


En funktion afsluttes altid, når den når til en `return` linje. Det vil sige, at ting i funktionen, som skrives ind efter `return`, ignoreres:


```python
def add10(x):
    print("Adding 10...")          # Denne linje printes, da den ligger før return-linjen
    result = x + 10
    return result
    print("And then more stuff!")  # Denne linje printes ikke, da den ligger efter return-linjen
    
print(add10(10))
```

    Adding 10...
    20


Indrykningen er ikke kun for syns skyld, men er her med til at afgrænse, hvor meget funktionen indeholder. Funktionens indhold (linjer skrevet efter `def`-linjen) skal rykkes ind med et enkelt tab eller fire mellemrum.

---
##  VIDENSCHECK

*Hvad returnerer nedenstående funktion, hvis `x = 122`?*


```python
def tenth(x):
    result = x / 10
    return result
    result = x * 10
    return result
```

{{%expand "Løsning" %}}
Funktionen returnerer `12.2`, hvis input er `122`, da input divideres med 10 og returneres. Alt efter den første return-linje ignoreres.
{{%/expand%}}

---

---
## ØVELSE

*Lav en funktion, der udregner arealet af en trekant (A), ved at tage højde (h) og grundlinje (g) som input.*

\[A = {{1 \over 2} * h * g}\]

{{%expand "Løsning" %}} 


```python
def triarea(h, g):
    area = 0.5 * h * g
    return area

print(triarea(5, 9))
```

    22.5


{{%/expand%}}

---
