---
title: Pakker
weight: 6
---
Pakker i Python er samlinger af funktioner, metoder, værdier osv. Selvom man kan meget i Python, så når man ikke særlig langt uden at importere pakker.

Funktioner, metoder, værdier osv. fra pakker kan nemt indlæses ved at importere dem. Så snart pakken er importeret, er pakkens indhold tilgængeligt.

Fx kender Python ikke værdien pi med det samme:

- Check: Forstår python et stykke kode? (brug af funktion før og efter import)
- Øvelse: Importer pakke og brug funktion derfra
- Check: Hvilken type er variablen efter funktion er blevet brugt til at ændre den?


```python
print(pi)
```


    ---------------------------------------------------------------------------
    
    NameError                                 Traceback (most recent call last)
    
    <ipython-input-48-9e2d2bd32686> in <module>
    ----> 1 print(pi)


    NameError: name 'pi' is not defined


Værdien pi er en del af `math` pakken, så ved at importere pakken, kan man arbejde med værdien:


```python
import math

print(math.pi)
```

    3.141592653589793


Bemærk at man kalder noget frem, som er en del af en pakke, ved at skrive pakkens navn, punktum og det, som man skal bruge fra pakken.

Det er også muligt kun at importere enkelte dele af en pakke. I sådanne tilfælde er det ikke nødvendigt at skrive pakkens navn først:


```python
from math import pi

print(pi)
```

    3.141592653589793


Pakker kan have lange navne, så det er muligt at forkorte navnet, når de importeres:


```python
import math as m

print(m.pi)
```

    3.141592653589793


{{% notice warning %}} Vær varsom med blot at importere dele af pakker ind enkeltvis. En af grundene til, at man kalder dele af pakker ved at skrive pakken først er for at holde styr på, hvor funktionen, metoden eller værdien kommer fra. Man kan nemt miste overblikket eller, endnu værre, kalde den forkerte funktion, hvis man ikke har styr på, hvordan man har importeret.

Derudover bør man også altid overveje læsbarheden af ens kode, hvis andre skal kunne inspicere det, eller der skal samarbejdes om det. Derfor bør man også overveje, hvordan man forkorter pakkenavne ved import, da det også kan gøre koden svære at gennemskue. Mange pakker har dog gængse standardforkortelser, som man hurtigt lærer.
{{% /notice%}}

Python kommer med et standardbibliotek af pakker. Selvom funktionerne altså er installeret sammen med Python i pakker, så skal de stadig importeres, før de kan bruges. Python er opbygget sådan både for at gøre det hurtigere at arbejde med (jo mindre der skal indlæses ved opstart, jo hurtigere kan man komme i gang), og for at gøre det nemmere at håndtere funktioner, metoder og værdier fra forskellige pakker. 

Der et utal af pakker, som Python kan udvides med. I materiale fra CALDISS anvendes primært pakker inden for dataanalyse, web scraping, tekstanalyse og maskinlæring. Hvis du har installeret Python med Anaconda, så er mange af disse pakker allerede installert og klar til import.
