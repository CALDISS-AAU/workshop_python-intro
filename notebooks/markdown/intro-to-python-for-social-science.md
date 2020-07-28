# Introduktion til Python for Samfundsvidenskab

Denne lektion introducerer Python med særligt fokus på de dele af Python programmering, der er relevante for samfundsvidenskaberne. 

# {#Kapitel}Hvad er Python?

Python er et programmeringssprog, der anvendes inden for mange områder: hjemmesideopbygning, appudvikling, databaseopbygning og -vedligehold, dataanalyse mm.

I den seneste tid er Python blevet meget populært inden for dataanalyse og maskinlæring.

I denne første sektion introduceres til, hvordan man arbejder med et programmeringssprog.

# {#Afsnit}At arbejde med et programmeringssprog

Python er et programmeringssprog. At arbejde med Python kræver derfor, at man "taler" det rette sprog, når man gerne vil have Python til at gøre noget.

I bruger uden tvivl forskellige programmer, apps og softwareløsninger i jeres hverdag til forskellige ting. Disse er alle opbygget af kode skrevet i et programmeringssprog, men de leveres altid med en eller anden form for "brugerflade"; altså en måde vi kan bruge programmet ved at trykke på knapper og lignende, uden at skulle kende til den måde, som programmet er programmeret på.

Python har ikke en brugerflade, så for at få Python til at gøre noget, skal vi "fortælle" Python, hvad vi gerne vil, ved at skrive kommandoer i Python sproget.

# Hvorfor arbejde med et programmeringssprog?

At skulle arbejde på denne måde kan virke lidt gammeldags. Når nu programmer til dataanalyse laves med brugerflader og brugervenlige måder og bruge dem på, hvorfor så arbejde med dataanalyse i et program, hvor vi selv skal programmere og skrive kommandoer for at opnå det, vi gerne vil?

Programmer med brugerflader som Excel, Stata, SPSS osv. har selvfølgelig deres styrke i, at de er langt nemmere at bruge. Dog er sådanne programmer begrænset i deres funktionalitet, da de er udviklet til at arbejde med data på bestemte måder i bestemte formater. Med Python kan vi opnå meget af det samme og meget mere, da man i et programmeringssprog ikke er tvunget til at arbejde med bestemte dataformater, filtyper osv. Samtidig giver det at arbejde med et programmeringssprog os også den mulighed, at vi selv skriver vores egne "mini-programmer", der løser den specifikke udfordring, som vi lige står over for.

# Python som programmeringssprog

Der findes et væld af programmeringssprog. I dette materiale arbejdes med sproget Python. Mange logikker i programmering går på tværs af sprog, men de har hver deres styrker, svagheder og kendetegn. 

## Python er "general purpose"

Python er et "general purpose" programmeringssprog. Det vil sige, at det er udviklet til at blive brugt inden for så mange områder som muligt.

## Python er "objekt-orienteret"

Python er et "objekt-orienteret" programmeringssprog. Det vil sige, at sproget er baseret på at arbejde med "objekter". Et objekt inden for programmering kan være nærmest hvad som helst. Meget kort sagt er et objekt en beholder for en eller anden form for information. At Python er "objekt-orienteret" betyder derfor, at vi arbejder med sproget ved kontinuerligt at definere objekter (lagre information i beholdere) og interagere med disse.

## Python er "cross-platform"

Python er et "cross-platform" programmeringssprog. Det vil sige, at man kan arbejde med Python på tværs af styresystemer (Windows, macOS, Linux).

# Om dette materiale

Der fokuseres i dette materiale på Pythons brugbarhed og anvendelse inden for socialvidenskabelige analyse. Materialet vil derfor ikke give indføring i, hvordan programmeringssprog. Der fokuseres i stedet på at give en tilstrækkelig forståelse for, hvordan man arbejder med programmeringssproget Python, sådan at man kan anvende det i socialvidenskabelige analyse.

Materialet er bygget op ved at give forståelse for relevante programmerings- som datatekniske termer gennem praktiske eksempler med Python.

# {#Afsnit}Interager med Python

For at bruge Python skal vi "tale" Python. Man arbejde med Python ved at skrive kommandoer i Python-sproget. Hvis Python forstår din kommando udføres den. Hvis ikke, får du en eller anden form for fejl. Man kan se Python som et meget bogstaveligt og pernitten sprog: Kommandoer skal skrives på helt bestemte måder for at Python kan forstå, hvad du beder om.

Barberes Python ned til sine grundsten består det ikke af mere end en "interpreter" (fortolker). Alle programmeringssprog er bygget op om en fortolker, der "evaluerer" kommandoer. Inden for programmering vil evaluering sige, at sproget forsøger at forstå, hvad der står i en kommando.

## Python uden dikkedarer

Den "rene" installation af Python tilføjer fortolkeren til styresystemet, så man kan arbejde med Python gennem en terminal: 
![python_terminal.png](../img/python_terminal.png)

I terminalen kan vi skrive en kommando og trykke "Enter" for at få fortolkeren til at evaluere. I nedenstående skrives kommandoen `2+42` hvilket Python evaluerer og giver outputtet `42`:
![python_interpret1.png](../img/python_interpret1.png)

Python forstår matematiske operationer og vil returnere resultatet af en udregning, når man skriver den ind. 

I nedenstående forsøges at bede om en opskrift på pandekager. Det går knap så godt: 
![python_interpret1.png](../img/python_interpret2.png)

Når Python ikke kan forstå kommandoen, returneres en fejl. Der findes et væld af fejltyper. I ovenstående gives en `SyntaxError`, fordi kommandoen er skrevet helt forkert (dette er dog ikke det eneste problem med denne kommando, men det er den første fejl, som fortolkeren støder på).

## Brug af Python IDE'er ("Integrated Development Environment")

Selvom man kan arbejde med Python direkte i terminalen frarådes det meget kraftigt, da det er meget vanskeligt at gemme sit arbejde undervejs og svært at bevare overblik over sin kode og arbejde. Derfor arbejder man for det meste gennem et IDE (Integrated Development Environment). Et IDE er et program, som man kan arbejde med Python igennem, som ofte har forskellige funktioner og egenskaber til at hjælpe en bevare overblikket. 

Her nævnes blot et mindre udvalg af IDE'er.

### Spyder

Spyder er bygget op omkring en "script-editor". Et script er et dokument bestående af en række af Python kommandoer, som man kan sende til fortolkeren på én gang. I et script kan fx samles al det databehandlings- og analysearbejde, som man skal lave. Ved at køre scriptet udføres så al arbejdet.
Script-editoren er indbygget med farvekoder, så man nemt kan adskille dele af koden samt automatiske forslag til kommandoer (Spyder 4 og frem).

Derudover giver Spyder en objekt-/variabeloversigt, så man kan se, hvad man har defineret og arbejder med; fx datasæt, resultater, osv.

Spyder er godt til de fleste ting og særligt, hvis man skal arbejde med længere scripts.

Spyder installeres sammen med Anaconda: https://www.anaconda.com/products/individual#Downloads

### Jupyter Notebook

Jupyter Notebook er opbygget omkring en såkaldt "notebook". En notebook i Jupyter Notebook kombinerer Python kode med almindelig tekst (Markdown). Jupyter Notebook egner sig særdeles godt, hvis man skal dokumentere sit kodearbejde undervejs, da man har mulighed for at skrive almindelig tekst, sætte billeder ind, lave tabeller osv. omkring sin kode.

Dette materiale er udarbejdet i Jupyter Notebook.

Jupyter Notebook installeres sammen med Anaconda: https://www.anaconda.com/products/individual#Downloads

# {#Kapitel}Fundamentale koncepter i Python

I denne sektion gennemgås de grundlæggende koncepter i Python programmering. Disse kan sige at være byggestenene for næsten alt, som man foretager sig med Python programmering.

Det følgende materiale består af en del kodeeksempler, som er udarbejdet i Jupyter Notebook, men de vil kunne køres i hvilken som helst Python IDE.

# {#Afsnit}Python sproget

Som nævnt arbejder man med Python ved at skrive kommandoer i Python sproget. Kommandoer bliver "evalueret" af fortolkeren. Hvis koden forstås, bliver den kørt, og der gives et output, en ændring eller andet, afhængig af, hvad vi beder om.

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

Bemærk, at når flere linjer køres, vises kun output fra den sidste linje kørt:


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


At arbejde med Python er at arbejde med funktioner. En funktion tager et eller flere input (kaldet "argumenter) og gør et eller andet ved dem. Funktionen `print()` tager enten et stykke tekst eller tal som input, og viser det som et stykke tekst:


```python
print("Hello there!")
print(921 - 20)
```

    Hello there!
    901


{{% notice note %}}
Bemærk at mellemrum ikke er nødvendige for at koden virker. Faktisk ignorerer Python mellemrum, når de er en del af en kommando. Dog kan brug af mellemrum være med til at gøre kode mere overskuelig og læsbart.
{{% /notice%}}

# {#Afsnit}Variable

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


Defineres en variabel som et matematisk udtryk, er det resultatet af dette, som bliver lagret i variablen:


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
    
    <ipython-input-30-f03a0baf7732> in <module>
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


      File "<ipython-input-33-d5c54fdddaa2>", line 1
        e = Hello there
                      ^
    SyntaxError: invalid syntax



## Ændring af variable

Som hovedregel ændres en variabel ikke blot ved at bruge det. Variablen skal defineres om, hvis vi gerne vil ændre indholdet af variablen:


```python
a = 42
print(a + 7) # returnerer a + 7
print(a)     # a er ikke ændret. Stadig 42
a = a + 7    # a overskrives med a +7
print(a)     # a er nu ændret
```

    49
    42
    49


{{% notice tip %}}
Brug `#` til at skrive kommentarer i din kode. Tekst der følger et `#` ignoreres af Python. Når man for alvor begynder at arbejde med kode, kan man nemt glemme, hvorfor man skrev bestemte kodestykker, eller hvad kodestykkerne gør. Kommentarer til ens kode hjælper både dig selv og evt. andre, som skal kigge på eller arbejde med din kode.
{{% /notice%}}

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

## At arbejde med variable

At arbejde med Python er at arbejde med variable. Man definerer hele tiden nye variable, som bruges senere hen. Selvom man kun er interesseret i ét endeligt produkt eller output, så bruges variable til at holde styr på information og mellemresultater undervejs.

Derfor er det en god ide at indarbejde en god navngivningsskik. Kunsten er at balancere mellem korte navne og navne, som er sigende for det, som variablen indeholder.


```python
a = 10              # kort, men ikke sigende for indholdet
the_number_ten = 10 # sigende, men ret langt, hvis man skal bruge variablen igen og igen
```

{{% notice tip %}}

### Tips til variabelnavne

Variable kan blive navngivet næsten alt, men der er visse restriktioner:
- Variabelnavne kan ikke indeholde mellemrum.
- De fleste specielle karakterer kan ikke bruges, som fx: `/`, `?`, `*`, `?`, `.` osv. Disse betyder noget i Python og vil blive forsøgt fortolket.

Derudover er det en god ide at undgå at bruge allerede eksisterende navne i Python, da man ellers overskriver en allerede eksisterende funktion. Dette kan man nemt komme til i starten, når man ikke har stort kendskab til Pythons funktioner.

{{% /notice%}}

{{% notice info %}}
Her ses en oversigt over de matematiske operationer, som kan bruges i Python.


```python
a + b      # addition
a * b      # multiplikation
a - b      # subtraktion
a / b      # division
b ** a     # exponentiering
a // b     # "floor division" - returner antal hele gange, at tal til venstre kan divideres med tal til højre
2 * a % b) # modulus - returnerer rest efter "floor division"
```

{{% /notice%}} 

## ØVELSE: Definer variable

Lav variablene `my_number1`, `my_number2` og `my_word`. 
- `my_number1` skal indeholde tallet `42` 
- `my_number2` skal indeholde tallet `9` 
- `my_word` skal indeholde ordet `hello` (husk at brug `'` eller `"` til at fortælle Python, at det er tekst).

Når de er defineret, prøv da nogen af de forskellige matematiske operationer på jeres variable, fx: 

- `my_number1 + 10`
- `my_number2 / my_number1`
- `my_word` + `my_number1`
- `my_word` * `my_number2`

Læg mærke til hvilke operationer, der kan lade sig gøre og hvilke resultater, de producerer (nogle af disse operationer vil give fejl).

# {#Afsnit}Typer

En variabel er ikke bare en variabel i Python. Fordi en variabel kan være så mange ting, så er Python nødt til at adskille variable fra hinanden. Dette gøres ved at variable lagres som en bestemt *type*. 

Typen af variabel fortæller Python, hvad det er for en slags information, som variablen indeholder, og sætter betingelserne for, hvad der kan lade sig gøre med variablen.

Som man arbejder med Python, vil man støde på mange forskellige typer. I første omgang fokuseres på to af de mere gængse typer:

- Numeriske typer (fx integers og floats)
- Tekst typer (fx strings)

## Numeriske typer

Python gætter altid typen, når en variabel lagres. Når en variabel består af en talværdi, vil denne fx lagres som en numerisk type. Talværdien kan enten lagres som en *integer* (heltal) eller et *float point* (decimaltal). 

Python kan fortælle os typen med funktionen `type()`:


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


At Python gerne vil adskille mellem typer har noget at gøre med, hvordan en type information kræver mere at lagre end en anden. Dette kan have betydning, når man arbejder med enorme datamængder, hvilket sjældent er tilfældet i socialvidenskabelig analysearbejder.

## VIDENSCHECK

I ovenstående bliver variablen `a` brugt til at definere variabel `b`. 

*Hvilken type er variablen `a` efter at variabel `b` defineres?*

{{%expand "Løsning" %}}
`a` er stadig en *integer*. `a` ikke ændres i koden, men bliver blot brugt til at lave variabel `b`.
{{% /expand%}}

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
b = " there"
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
    
    <ipython-input-12-cc7b3220923a> in <module>
          1 a = "Hello"     # a dannes som string
          2 print(type(a))  # typen er string
    ----> 3 a = int(a)      # forsøger at konvertere a til integer - ikke muligt


    ValueError: invalid literal for int() with base 10: 'Hello'


## ØVELSE: Typer

Lav variablene variablene `my_number3` og `my_number4`.
- `my_number3` skal indeholde `21`
- `my_number4` skal indeholde `"12"` (med anførselstegn!)

Forsøg at divider de to tal med hinanden (`my_number3 / my_number4`). Det giver fejl, men hvorfor?

Undersøg hvilken type `my_number3` og `my_number4` er med `type()`. Begge skal gerne være numeriske typer, før der kan divideres.

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
