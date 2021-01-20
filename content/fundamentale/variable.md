---
title: Variable
weight: 2
---

{{< youtube tNmobEPK_uU>}}

Python er et objekt-orienteret programmeringssprog. Dette indebærer, at man kontinuerligt arbejder med forskellige objekter, som indeholder en eller anden for for information.

I Python kaldes objekter "variable". Dette er ikke at forveksle med en variabel, som forstået i statistik som en egenskab ved en observation, da en variabel i Python blot er en beholder for en eller anden form for information.

Alle disse kan være variable i Python:
- Et tal
- Et ord
- En tekst
- Et datasæt
- En mappesti
- En hjemmesideadresse
- Et billede

## Variable med tal

En variabel defineres med `=`. På venstre side gives variablen et navn, og på højre skrives det, som variablen skal indeholde: 


```python
a = 42
b = 7
c = 6
```

Når først en variabel er defineret (altså at koden hvor variablen defineres er kørt), kan variablen kaldes frem og bruges i andre kommandoer:


```python
print(a)
print(a / b)
```

    42
    6.0


Defineres en variabel som et matematisk udtryk, er det resultatet af dette udtryk, som bliver lagret i variablen:


```python
d = 13 + 25
print(d)
```

    38


Bemærk at Python læser kode meget bogstaveligt, og skelner derfor mellem store og små bogstaver. Kaldes en variabel, som ikke findes, returnerer Python en fejl:


```python
print(d)
print(D)
```

    38



    ---------------------------------------------------------------------------
    
    NameError                                 Traceback (most recent call last)
    
    <ipython-input-21-f03a0baf7732> in <module>
          1 print(d)
    ----> 2 print(D)


    NameError: name 'D' is not defined


## Variable med tekst

En variabel kan også indeholde tekst. Tekst markeres med enten `'` eller `"`:


```python
e = "Hello there!"
print(e)
```

    Hello there!


Hvis ikke Python fortælles, at noget er tekst, vil Python antage, at det er en eller anden form for variabel eller funktion, som der forsøges at blive kaldt frem:


```python
e = Hello there
```


      File "<ipython-input-23-d5c54fdddaa2>", line 1
        e = Hello there
                      ^
    SyntaxError: invalid syntax



## Ændring af variable

Som hovedregel ændres en variabel ikke blot ved at bruge den. 


```python
a = 42
print(a + 7) # returnerer a + 7
print(a)     # a er ikke ændret. Stadig 42
```

    49
    42


Variablen skal defineres om, hvis man gerne vil ændre indholdet af variablen:


```python
a = a + 7    # a overskrives med a +7
print(a)     # a er nu ændret
```

    49


{{% notice tip %}}
Brug `#` til at skrive kommentarer i din kode. Tekst der følger et `#` ignoreres af Python. Når man for alvor begynder at arbejde med kode, kan man nemt glemme, hvorfor man skrev bestemte kodestykker, eller hvad kodestykkerne gør. Kommentarer til ens kode hjælper både dig selv og evt. andre, som skal kigge på eller arbejde med din kode.
{{% /notice%}}

---
## VIDENSCHECK

Tag et kig på nedenstående kode:


```python
g = 90
g + 10
f = g - 10
g = g - f
```

*Hvad indeholder variablen `g` når ovenstående kode er kørt?*

{{%expand "Løsning" %}}
`g` indeholder tallet `10`. `g` bliver kun ændret ved den sidste linje (`g = g - f`), og `f` indeholder tallet `80`, da `g` på tidspunktet `f` defineres indeholder tallet `90`.
{{% /expand%}}

---

## At arbejde med variable

At arbejde med Python er at arbejde med variable. Man definerer hele tiden nye variable, som bruges senere hen. Selvom man kun er interesseret i ét endeligt produkt eller output, så bruges variable til at holde styr på information og mellemresultater undervejs.

Det er en god ide at indarbejde en god navngivningsskik. Kunsten er at balancere mellem korte navne og navne, som er sigende for det, som variablen indeholder.


```python
a = 10              # kort, men ikke sigende for indholdet
the_number_ten = 10 # sigende, men ret langt, hvis man skal bruge variablen igen og igen
```

{{% notice tip %}}

**Tips til variabelnavne**

Variable kan blive navngivet næsten alt, men der er visse restriktioner:

* Variabelnavne kan ikke indeholde mellemrum.
* De fleste specielle karakterer kan ikke bruges, som fx: `/`, `?`, `*`, `?`, `.` osv. Disse betyder noget i Python og vil blive forsøgt fortolket.

Derudover er det en god ide at undgå at bruge allerede eksisterende navne i Python, da man ellers overskriver en allerede eksisterende funktion. Dette kan man nemt komme til i starten, når man ikke har stort kendskab til Pythons funktioner.

{{% /notice%}}

{{% notice info %}}
Her ses en oversigt over de matematiske operationer, som kan bruges i Python:

```python
a + b      # addition
a * b      # multiplikation
a - b      # subtraktion
a / b      # division
b ** a     # exponentiering
a // b     # "floor division" - returner antal hele gange, at tal til venstre kan divideres med tal til højre
a % b      # modulus - returnerer rest efter "floor division"
```

{{% /notice%}} 

---
## ØVELSE: Definer variable

Lav variablene `my_number1`, `my_number2` og `my_word`. 

* `my_number1` skal indeholde tallet `42` 
* `my_number2` skal indeholde tallet `9` 
* `my_word` skal indeholde ordet `hello` (husk at brug `'` eller `"` til at fortælle Python, at det er tekst).

Når de er defineret, prøv da nogen af de forskellige matematiske operationer på jeres variable, fx: 

* `my_number1 + 10`
* `my_number2 / my_number1`
* `my_word` + `my_number1`
* `my_word` * `my_number2`

Læg mærke til hvilke operationer, der kan lade sig gøre og hvilke resultater, de producerer (nogle af disse operationer vil give fejl).

---
