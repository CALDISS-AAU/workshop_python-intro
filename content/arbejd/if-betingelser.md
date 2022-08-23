---
title: If-betingelser
weight: 4
---
youtube zaJBdItYYPs >}}

Når man arbejder med Python, kan det ofte være brugbart at sætte if-betingelser i sin kode. If-betingelser er kodestumper, hvor visse kommandoer kun udføres, hvis en betingelse er opfyldt:



```python
x = 12

if x > 10:
    print("Tallet er større end 10!")
else:
    print("Tallet er ikke større end 10!")
```

    Tallet er større end 10!
    

Ovenstående kode består af to blokke: en if-blok og en else-blok. 

I koden evalueres først if-betingelsen: `x > 10`. Hvis denne evalueres til `True`, udføres kommandoen efter `:`. I ovenstående er `x = 12`, hvorfor kommandoen udføres. Her er kommandoen blot at printe teksten `Tallet er større end 10!`.

Herunder ses hvad der sker med samme kode, hvis x er mindre end 10:


```python
x = 8

if x > 10:
    print("Tallet er større end 10!")
else:
    print("Tallet er ikke større end 10!")
```

    Tallet er ikke større end 10!
    

I ovenstående er `x = 8`. Derfor evaluerer betingelsen denne gang til `False`, og kommandoen lige efter if-betingelsen udføres ikke. I stedet springes videre til else-blokken, hvor kommandoen er at printe teksten `Tallet er ikke større end 10!`.

Else-blokken udløses i alle tilfælde, hvor if-betingelsen ikke er opfyldt. En else-blok er ikke nødvendig. Udelades den, sker der blot ingenting, hvis if-betingelsen ikke er opfyldt:


```python
x = 8

if x > 10:
    print("Tallet er større end 10!")
```

**Flere if-betingelser**

Det er muligt at udvide med flere betingelser med `elif` ("else if"). `elif` fungerer ved, at hvis if-betingelsen ikke er opfyldt, så evalueres den første `elif`. Sådan kører Python videre indtil, at der findes en betingelse, der evaluerer til sand, eller der nås en else-blok. 


```python
x = 7

if x > 10:
    print("Tallet er større end 10!")
elif x > 5:
    print("Tallet er større end 5!")
else:
    print("Tallet er ikke større end 5!")
```

    Tallet er større end 5!
    

---
## ØVELSE

Tag et kig på nedenstående kode:


```python
master = "Obi-Wan Kenobi"

if master == "Luke Skywalker":
    apprentice = "Ben Solo"
elif master == "Qui-Gon Jinn":
    apprentice = "Obi-Wan Kenobi"
elif master == "Obi-Wan Kenobi":
    apprentice = "Anakin Skywalker"
elif master == "Yoda":
    apprentice = "Mace Windu"
else:
    apprentice = "Ingen"
```

*Hvad indeholder variablen `apprentice`, når koden er kørt? (se om du kan løse det uden at køre koden)*

{{%expand "Løsning" %}}Variablen indeholder "Anakin Skywalker", da det er sætningen `master = "Obi-Wan Kenobi"`, som er sand.{{%/expand%}}

---

## If-betingelser og for loops

If-betingelser er yderst nyttige i kombination med andre kontrolstrukturer. Fx kan man i kombinationen med for loops og if-betingelser skrive kode, hvor en kommando kun udføres på visse værdier i en liste:


```python
values = range(1, 10)

for value in values:
    if value % 3 == 0:
        print(str(value) + " kan divideres med 3!")
    else:
        print(str(value) + " kan ikke divideres med 3!")
```

    1 kan ikke divideres med 3!
    2 kan ikke divideres med 3!
    3 kan divideres med 3!
    4 kan ikke divideres med 3!
    5 kan ikke divideres med 3!
    6 kan divideres med 3!
    7 kan ikke divideres med 3!
    8 kan ikke divideres med 3!
    9 kan divideres med 3!
    

I ovenstående ses et for loop, der kører over værdierne 1 til 9 (`range(1, 10)`). Hver værdi tjekkes om det kan divideres med 3 (`value % 3 == 0`). Hvis den kan det, printes at det kan divideres med 3. Hvis ikke, printes teksten, at det ikke kan divideres med 3.

{{% notice note %}}Husk at `%` bruges til at returnere den rest, der er tilbage efter heltalsdivision. `7 % 3` giver fx 1, da 7 kan divideres med 3 to hele gange, hvorefter der er 1 tilbage.{{% /notice%}}

## If-betingelser og funktioner

Funktioner kan skrives med if-betingelser. På den måde kan man skrive funktioner sådan, at det, der returneres, varierer afhængigt af, hvad det er for et input:


```python
jedis = ["Kenobi", "Yoda", "Windu", "Ki-Adi-Mundi", "Koon", "Skywalker", "Katarn"]
siths = ["Sidious", "Desann", "Tyrannus", "Revan", "Maul", "Vader", "Plagueis"]

def jedi_checker(name):
    if name in jedis:
        return "jedi"
    elif name in siths:
        return "sith"
    else:
        return "neither jedi nor sith"
    
print(jedi_checker("Windu"))
print(jedi_checker("Revan"))
```

    jedi
    sith
    

{{% notice note %}}Bemærk at ovenstående funktion er meget begrænset, da den kun baserer sig på en begrænset mængde navne og kun accepterer, at navnet er stavet på en helt bestemt måde.{{% /notice%}}

---
## ØVELSE

*Skriv et stykke kode, der går igennem hvert ord i listen `words` og printer ordet i blokbogstaver, hvis ordet er mere end 6 bogstaver langt. Ellers skal der ikke ske noget.*


```python
words = ["potato", "cat", "scrumptious", "monitor", "carpenter"]
```

{{%expand "Løsning" %}}


```python
for word in words:
    if len(word) > 6:
        print(word.upper())
```

    SCRUMPTIOUS
    MONITOR
    CARPENTER
    

{{%/expand%}}

---
