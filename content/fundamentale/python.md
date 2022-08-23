---
title: Python sproget
weight: 1
---
youtube 1iD74PlcMUw >}}

Som nævnt arbejder man med Python ved at skrive kommandoer i Python sproget. Kommandoer bliver "evalueret" af fortolkeren. Hvis koden forstås, bliver den kørt, og der gives et output, en ændring eller andet afhængigt af, hvad man beder om.

Hvis man fx skriver en kommando besteånde af matematiske operationer i Python, vil man få resultatet tilbage som output:


```python
2 + 5
```




    7




```python
7 * 6
```




    42




```python
923 / 45
```




    20.511111111111113



Her køres Python kode i Jupyter Notebook. Som vist i sidste sektion, kan man køre Python kode direkte fra en terminal, hvor man sender en kommando afsted ved at trykke "Enter". Med Jupyter Notebook (eller anden IDE) har vi mulighed for at skrive flere kommandoer efter hinanden adskilt af linjeskift. Når koden køres, evalueres linjerne enkeltvis i rækkefølge.

Bemærk, at når flere linjer køres, vises kun output fra den sidste linje kørt (i Jupyter Notebook):


```python
90 - 65
0.7 * 23
45 + 12
```




    57



Hvis output for alle linjer skal vises, kan man bede om det eksplicit med funktionen `print()`. 


```python
print(90 - 65)
print(0.7 * 23)
print(45 + 12)
```

    25
    16.099999999999998
    57
    

At arbejde med Python er at arbejde med funktioner. En funktion tager et eller flere input (kaldet "argumenter") og gør et eller andet ved dem. Funktionen `print()` tager enten et stykke tekst eller tal som input, og viser det som et stykke tekst:


```python
print("Hello there!")
print(921 - 20)
```

    Hello there!
    901
    

{{% notice note %}}
Bemærk at mellemrum ikke er nødvendige for at koden virker. Faktisk ignorerer Python mellemrum, når de er en del af en kommando. Dog kan brug af mellemrum være med til at gøre kode mere overskuelig og læsbar.
{{% /notice%}}
