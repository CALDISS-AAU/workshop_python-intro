---
title: Hyppige fejltyper
weight: 5
---
Man vil uundgåeligt få fejl, når man arbejder med Python. Som nævnt er Python et meget bogstaveligt sprog, så der skal ikke meget til for, at Python giver en fejlbesked.

Pythons fejlbeskeder er meget detaljerede, men kan være svære at gennemskue - særligt hvis man er ny til Python. Dog kan selve fejl*typen* hjælpe os til at finde ud af, hvad der er galt med vores kode.

Herunder gennemgås de hyppigste fejltyper, og hvad de dækker over.

## SyntaxError

En `SyntaxError` gives, hvis ens kode ikke er et gyldigt Python udtryk. En `SyntaxError` kan også kaldes for en "sprogfejl". Disse opstår når vi skriver kommandoer, som er volapyk for Python:


```python
giv mig resultatet!
```


      File "C:\Users\kgk\AppData\Local\Temp\ipykernel_3800\4153195480.py", line 1
        giv mig resultatet!
              ^
    SyntaxError: invalid syntax
    


I ovenstående er der brugt mellemrum mellem flere (ikke eksisterende) variable. Dette er ugyldigt for Python. En `SyntaxError` opstår derfor typisk pga. slåfejl eller manglende tegn (kommaer, parenteser o.l.).

## NameError

En `NameError` gives, hvis man refererer til et objekt, som ikke eksisterer i Python-miljøet. Denne fejl opstår typisk, hvis man har glemt at definere en variabel eller mangler at importere en pakke.

Fordi Python er et meget bostaveligt sprog, får man også denne fejl, hvis man glemmer et tegn i sin variabel, når man refererer til den:


```python
addresser = ["Blomstervang 12", "Fuglevej 7", "Malergade 32"]

print(adresser)
```


    ---------------------------------------------------------------------------

    NameError                                 Traceback (most recent call last)

    ~\AppData\Local\Temp\ipykernel_3800\2535432249.py in <module>
          1 addresser = ["Blomstervang 12", "Fuglevej 7", "Malergade 32"]
          2 
    ----> 3 print(adresser)
    

    NameError: name 'adresser' is not defined


Ovenstående giver `NameError`, da det er `adresser`, der bliver kaldt, men listen hedder `addresser`. 

## TypeError

En `TypeError` gives, hvis man forsøger at gøre noget med en variabel, som ikke kan lade sig gøre med den type/class, som variablen er:


```python
"hej" + 2
```


    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    ~\AppData\Local\Temp\ipykernel_3800\1089118982.py in <module>
    ----> 1 "hej" + 2
    

    TypeError: can only concatenate str (not "int") to str


Ovenstående giver en `TypeError`, da det er ikke er muligt at lægge teksttyper og taltyper sammen.

## AttributeError

En `AttributeError` gives, hvis man forsøger at referere til et attribut eller en metode, som ikke findes for den pågældende variabel:


```python
tekst = 42

tekst.upper()
```


    ---------------------------------------------------------------------------

    AttributeError                            Traceback (most recent call last)

    ~\AppData\Local\Temp\ipykernel_3800\2065210826.py in <module>
          1 tekst = 42
          2 
    ----> 3 tekst.upper()
    

    AttributeError: 'int' object has no attribute 'upper'


Ovenstående giver en `AttributeError`, da metoden `.upper()` ikke findes for taltyper.

Denne fejl kan opstå enten pga. stavefejl i metoden eller fordi variablen er en anden class, end man regner med den er.

## IndexError/KeyError

En `IndexError` eller `KeyError` gives, hvis man refererer til et element i en datastruktur (fx liste eller dictionary), som ikke findes. 

For fx lister gives en `IndexError`, hvis man refererer til et indeks, som overstiger antallet af elementer i listen:


```python
adresser = ["Blomstervang 12", "Fuglevej 7", "Malergade 32"]

print(adresser[3]) # Indeks 3 findes ikke - husk at Python starter ved 0
```


    ---------------------------------------------------------------------------

    IndexError                                Traceback (most recent call last)

    ~\AppData\Local\Temp\ipykernel_3800\2954300856.py in <module>
          1 adresser = ["Blomstervang 12", "Fuglevej 7", "Malergade 32"]
          2 
    ----> 3 print(adresser[3])
    

    IndexError: list index out of range


For dictionaries gives en `KeyError`, hvis man refererer til en nøgle, som ikke findes i den dictionary:


```python
adresse = {"vej": "Blomstervang", "nummer": 12}

print(adresse["kommune"])
```


    ---------------------------------------------------------------------------

    KeyError                                  Traceback (most recent call last)

    ~\AppData\Local\Temp\ipykernel_3800\2520700864.py in <module>
          1 adresse = {"vej": "Blomstervang", "nummer": 12}
          2 
    ----> 3 print(adresse["kommune"])
    

    KeyError: 'kommune'