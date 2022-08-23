---
title: Metoder
weight: 5
---
youtube xOz52Dmn-GY >}}

Udover funktioner i Python findes der også "metoder". Lig funktioner tager metoder også en form for input og returnerer et output. 

I modsætning til funktioner er metoder bundet op på bestemte variabeltyper (eller rettere en bestemt "class"). Det vil sige at variablen skal være en bestemt type for, at metoden kan bruges. Metoder kaldes med `variabel.method(option1 = something)`. Tekstværdier (strings) har fx en række metoder tilknyttet til at ændre teksten:


```python
word = "Hello"

print(word.upper())  # Konverterer til store bogstaver
print(word.lower())  # Konverterer til små bogstaver
```

    HELLO
    hello
    

Bemærk at metoder ikke altid ændrer på variablen. For ovenstående metoder skal variablen derfor defineres om eller på ny, hvis output af en metode skal lagres:


```python
print(word)         # Stadig som det oprindeligt blev lavet

word = word.upper() 
print(word)         # Er nu overskrevet til at være med store bogstaver
```

    Hello
    HELLO
    

Forsøger man at bruge metoder på en variabel af en forkert type, gives der fejl:


```python
number = 627

number.upper()
```


    ---------------------------------------------------------------------------

    AttributeError                            Traceback (most recent call last)

    <ipython-input-51-d30eebf09ae0> in <module>
          1 number = 627
          2 
    ----> 3 number.upper()
    

    AttributeError: 'int' object has no attribute 'upper'


Metoder tager ofte yderligere argumenter og indstillinger. I nedenstående bruges metoden `.replace()` til at erstatte et ord i tekstvariablen med et andet.


```python
words = "Hello there!"

words.replace("there", "world")
```




    'Hello world!'



{{% notice note %}} Bemærk i hjælpefilen for `.replace()` at de to argumenter, som der tages kaldes `old` og `new` og står i den rækkefølge. Det er derfor også den rækkefølge, som de skal skrives ind, når man bruger metoden.
{{% /notice%}}

---
## VIDENSCHECK

I ovenstående er metoden `.replace()` brugt til at erstatte ordet "there" med "world" i variablen `words`.

*Hvad indeholder `words` efter `.replace()` er brugt?*

{{%expand "Løsning" %}} 
`words` indeholder stadig `"Hello there!"`, da variablen ikke er defineret om.
{{%/expand%}}

---
