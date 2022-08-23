---
title: Loops
weight: 3
---
youtube mH_EWKqdo88 >}}

I arbejdet med dataanalyse udfører man ofte de samme kommandoer, kontroller, kørsler osv. igen og igen:

- En række oplysninger kan kontrolleres, om de er korrekte. Har de den rigtige type? Er værdierne gyldige? (fx at aldersværdier ikke har skøre værdier som 987 år).
- Den samme beregning skal foretages for en række oplysninger - fx udregning af gennemsnit for indkomst, alder, år i arbejde osv.
- De samme oplysninger skal hentes fra en række forskellige kilder (filer, hjemmesider eller andet).

I Python (og mange andre programmeringssprog) kan man anvende "loops" til at gentage kommandoer. De mest gængse loop typer er "for loops" og "while loops". "for loops" gentager en eller flere kommandoer over en afgrænset mængde værdier. "while loops" gentager en kommando, så længe en vis betingelse er opfyldt.

Loops kaldes også for kontrolstrukturer i programmeringssprog, da de er med til at sætte rammer og betingelser for, hvad visse kommandoer skal køre på.

## For loops

I nedenstående dannes tre variable. Det antages, at der er tale om tre forskellige aldersværdier. De tre værdier lagres i listen `ages`.


```python
age1 = 29
age2 = "41"
age3 = 87

ages = [age1, age2, age3]
```

Som tidligere gennemgået i materialet, adskiller Python mellem forskellige variabeltyper. For at Python kan arbejde med tal, skal Python fortælles, at variablen er et tal, hvis ikke Python har gættet det i forvejen. En typisk del af forarbejdet til dataanalyse er, at validere oplysninger på en eller anden måde for at sikre, at data er i gyldige formater og typer.

Hver variabel skal altså kontrolleres for, at det er en numerisk type, hvilket kan gøres med `type()`:


```python
print(type(age1))
```

    <class 'int'>
    

Skal det gøres for alle variable, skal kommandoen gentages for hver variabel:


```python
print(type(age1))
print(type(age2))
print(type(age3))
```

    <class 'int'>
    <class 'str'>
    <class 'int'>
    

Af ovenstående erfares, at `age2` er en string, og derfor skal konverteres, før der kan arbejdes videre med den.

At skulle gentage kommandoer ved at skrive dem ud hver gang, bliver dog hurtigt en tidsslugende og meget kedsommelig affære. Alternativt kan et loop bruges til at gøre det samme. 

Ovenstående kan gøres med et loop på følgende måde (husk at listen `ages` består af værdierne fra variablerne `age1`, `age2` og `age3`):


```python
for age in ages:
    print(type(age))
```

    <class 'int'>
    <class 'str'>
    <class 'int'>
    

**Opbygning af et for loop**

Et for loop består overordnet af to dele:
- En række værdier, som loopet skal køre over
- En eller flere kommandoer, som skal gentages for hver værdi

I ovenstående kommando bruges listen `ages` som den række værdier, som loopet skal køre over. `age` er en pladsholder for de enkelte værdier, som er i `ages`. Hver gang loopet gentages, ændrer `age` sig til den næste værdi i `ages`. 

Pladsholderen `age` bruges i kommandoerne, som skal gentages for hvert loop. Kommandoerne skrives på linjen efter `:`. Her er det vigtigt, at kommandoerne i loopet er rykket ind (enten med tab eller fire mellemrum, men de fleste IDE'er laver dette indryk automatisk).

Der kunne have været brugt hvilket som helst navn som pladsholder i stedet for `age`, så længe at pladsholder-navnet ændres i kommandoerne også.

Herunder ses et andet for loop, der går igennem hver værdi i `values` og printer værdien ganget med to:


```python
values = [9, 10, 4, 91, 27]

for value in values:
    print(value * 2)
```

    18
    20
    8
    182
    54
    

Når for loopet sættes i gang, ser Python på værdierne i `values` og tager den første værdi (`9`). `value` er altså lig med `9` i den første kørsel af loopet. Derefter udføres kommandoen, som i dette tilfælde er at printe værdien ganget med to: `print(value * 2)`. `value = 9` i den første kørsel af loopet, så derfor udføres: `print(9 * 2)`, som giver `18`.

Når enden af kommandoerne i loopet nås, går Python tilbage til værdierne i `values` og tager den næste værdi (`10`), så `value` er lig med `10` i den næste kørsel: `print(10 * 2)`, som giver `20`. Sådan fortsætter Python, indtil der ikke er flere værdier i listen (eller at der stødes på en eller anden fejl).

Bemærk, at en liste ikke behøver at være defineret som variabel, inden den bruges i et loop:


```python
for value in [9, 10, 4, 91, 27]:
    print(value * 2)
```

    18
    20
    8
    182
    54
    

---
## VIDENSCHECK

*Hvornår giver det mening at bruge et for loop?*

{{%expand "Løsning" %}} Når de samme kommandoer skal gentages for en række værdier.{{%/expand%}}

---

---
## ØVELSE

Tidligere i dette materiale er metoder blevet gennemgået. Blandt andet kan man bruge `.upper()` på en tekstværdi, for at få værdien tilbage i blokbogstaver. 

Tag et kig på denne liste af ord:


```python
words = ["potato", "cat", "scrumptious", "monitor", "carpenter"]
```

*Skriv et for loop, der printer hvert ord i `words` i blokbogstaver.*

{{%expand "Løsning" %}}


```python
for word in words:
    print(word.upper())
```

    POTATO
    CAT
    SCRUMPTIOUS
    MONITOR
    CARPENTER
    

{{%/expand%}}

---

**Loop over talrækker**

Et for loop kan køres på et interval med kommandoen `range()`:


```python
for x in range(10, 20):
    print(x+5)
```

    15
    16
    17
    18
    19
    20
    21
    22
    23
    24
    

`range()` danner en talrække fra det første tal angivet til tallet *før* det sidste tal angivet ([10:20[).

Angives et enkelt tal som argument, antages det, at intervallet skal dannes fra `0` og frem til tallet før tallet angivet:


```python
for x in range(5):
    print(x)
```

    0
    1
    2
    3
    4
    

Som standard dannes intervallet med skridt på `1`; altså hver enkelt heltal mellem det første tal og tallet før det sidste tal. Dette kan ændres ved at tilføje et tredje argument for, hvor store "skridt", der skal være i intervallet:


```python
for x in range(5, 10, 2):
    print(x)
```

    5
    7
    9
    

## While loops

While loops er en anden type loops i Python. Hvor for loops gentager en eller flere kommandoer for hver værdi i en række af værdier, så gentager while loops en eller flere kommandoer, så længe en given betingelse er opfyldt.

Herunder ses et eksempel på et simpel while loop:


```python
x = 1

while x < 5:
    print("loopet kører videre")
    x = x + 1
```

    loopet kører videre
    loopet kører videre
    loopet kører videre
    loopet kører videre
    

Et while loop består overordnet af to dele:
- En betingelse som skal være opfyldt for, at loopet gentages
- En eller flere kommandoer, som skal gentages for hvert loop

I ovenstående defineres først `x` til at være `1`. Derefter igangsættes et while loop, som skal køre, så længe at `x < 5`. Kommandoerne, som skal køre i loopet, skrives på linjen efter `:`. Her er det igen vigtigt, at kommandoerne i loopet er rykket ind (enten med tab eller fire mellemrum, men de fleste IDE'er laver dette indryk automatisk).

Derefter overskrives `x` til at være `x + 1`; altså at værdien af `x` øges med `1`. *Bemærk at hvis denne linje undlades, så bliver loopet ved med at gentage sig, da `x` ikke ændres og derfor bliver ved med at være `1`; altså mindre end `5`, som er betingelsen for, at loopet kører*.

{{% notice warning %}} Man skal være forsigtig, når man skriver while loops, da man meget nemt kan komme til at skabe uendelige loops! 

Uendelige loops sker, hvis ikke den betingelse, som while loopet baseres på, ændres. Uendelige loops skal afbrydes manuelt, men i tilfælde, hvor det, der sker i loopet, er krævende, kan Python ende med at gå helt i stå af at arbejde med loopet, da Python (og computeren) til sidst ikke kan følge med. {{% /notice%}}

Herunder ses et andet while loop, der bliver ved, så længe antallet af karakterer i variablen `fruit` ikke overstiger 22:


```python
fruit = "banana"

while len(fruit) <= 22:
    print("the word is " + fruit)
    fruit = fruit + "na"
```

    the word is banana
    the word is bananana
    the word is banananana
    the word is bananananana
    the word is banananananana
    the word is bananananananana
    the word is banananananananana
    the word is bananananananananana
    the word is banananananananananana
    

{{% notice info %}} Funktionen `len()` har tidligere været brugt til at give antallet af elementer i en liste. Bruges `len()` på en tekstværdi (en string), returneres antallet af karakterer i tekstværdien. {{% /notice%}}

Når Python læser linjen med while loopet, starter Python med at evaluere betingelsen: `len(fruit) <= 22`. Hvis denne er `True`, udføres kommandoerne. `fruit` indeholder til at starte med teksten `banana` og har en længde på 6 bogstaver; altså mindre end 22, så kommandoerne udføres. 

Første kommando er at printe teksten `"the word is " + fruit` (husk at tekststykker kan sættes sammen med `+`). Da `fruit` i den første kørsel indeholder `banana` bliver teksten `the word is banana`. 

Dernæst ændres `fruit` til at få tilføjet teksten `na`, så `fruit` nu indeholder `bananana`. 

Loopet starter herefter forfra, og betingelsen evalueres igen. Nu indeholder `fruit` teksten `bananana` med en længde på 8 bogstaver; altså stadig mindre end 22, hvorfor kommandoerne igen udføres. Da `fruit` nu indeholder `bananana` printes teksten `the word is bananana`. 

**Brug af while loops**

Det kan måske virke svært at se, hvad while loops kan bruges til. De bruges meget i programmering i det hele taget, men finder sjældent anvendelse i analysearbejde. 

Arbejder man med web scraping (indsamling af data fra nettet), kan while loops være brugbare. En teknik i web scraping er fx at sætte "crawlers" op. En crawler fungerer kort sagt ved at gå fra hjemmeside til hjemmeside ud fra de links, som der findes på siden. Her kan et while loop bruges til at begrænse, hvor langt crawleren skal gå; fx ved at sætte den til at stoppe efter et vis antal sider er indsamlet eller sætte den til at stoppe, hvis crawleren bevæger sig ud fra et eller andet hoveddomæne. 

Hvis man fx gerne vil indsamle tekster og artikler fra EU's hjemmeside (https://europa.eu/), kan man bruge et while loop til at fortsætte indsamlingen, så længe siden befinder sig under domænet https://europa.eu/. 

---
## ØVELSE

Bør nedenstående while loop køres?:

```python
y = 10

while y > 5:
    print("the value is " + str(y))
```

{{%expand "Løsning" %}}Nej. Det er et uendeligt loop. `y` ændres ikke og betingelsen for while loopet bliver derfor ved med at være sand. {{%/expand%}}

---
