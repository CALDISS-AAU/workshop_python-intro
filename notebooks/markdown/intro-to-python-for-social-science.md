# Introduktion til Python for Samfundsvidenskab

Denne lektion introducerer Python med særligt fokus på de dele af Python programmering, der er relevante for samfundsvidenskaberne. 

# {#Kapitel}Hvad er Python?

Python er et programmeringssprog, der anvendes inden for mange områder: hjemmesideopbygning, appudvikling, databaseopbygning og -vedligehold, dataanalyse mm.

I den seneste tid er Python blevet meget populært inden for dataanalyse og maskinlæring.

I denne første sektion introduceres til, hvordan man arbejder med Python som et programmeringssprog.

# {#Afsnit}At arbejde med et programmeringssprog

Python er et programmeringssprog. At arbejde med Python kræver derfor, at man "taler" det rette sprog, når man gerne vil have Python til at gøre noget.

I bruger uden tvivl forskellige programmer, apps og softwareløsninger i jeres hverdag til forskellige ting. Disse er alle opbygget af kode skrevet i et programmeringssprog, men de leveres altid med en eller anden form for "brugerflade"; altså en måde vi kan bruge programmet ved at trykke på knapper og lignende, uden at skulle kende til den måde, som programmet er programmeret på.

Python er et programmeringssprog og har derfor ikke en brugerflade, så for at få Python til at gøre noget, skal vi "fortælle" Python, hvad vi gerne vil ved at skrive kommandoer i Python sproget.

## Hvorfor arbejde med et programmeringssprog?

At skulle arbejde på denne måde kan virke lidt gammeldags. Når nu programmer til dataanalyse laves med brugerflader og brugervenlige måder at bruge dem på, hvorfor så arbejde med dataanalyse i et program, hvor vi selv skal programmere og skrive kommandoer for at opnå det, vi gerne vil?

Programmer med brugerflader som Excel, Stata, SPSS osv. har selvfølgelig deres styrke i, at de er nemmere at gå til. Dog er sådanne programmer begrænset i deres funktionalitet, da de er udviklet til at arbejde med data på bestemte måder i bestemte formater. Med Python kan vi opnå meget af det samme og meget mere, da man i et programmeringssprog ikke er tvunget til at arbejde med bestemte dataformater, filtyper osv. Samtidig giver det at arbejde med et programmeringssprog os også den mulighed, at vi selv skriver vores egne "mini-programmer", der løser den specifikke udfordring, som vi lige står over for.

## Python som programmeringssprog

Der findes et væld af programmeringssprog. I dette materiale arbejdes med sproget Python. Mange logikker i programmering går på tværs af sprog, men de har hver deres styrker, svagheder og kendetegn. 

**Python er "general purpose"**

Python er et "general purpose" programmeringssprog. Det vil sige, at det er udviklet til at blive brugt inden for så mange områder som muligt.

**Python er "objekt-orienteret"**

Python er et "objekt-orienteret" programmeringssprog. Det vil sige, at sproget er baseret på at arbejde med "objekter". Et objekt inden for programmering kan være nærmest hvad som helst. Meget kort sagt er et objekt en beholder for en eller anden form for information. At Python er "objekt-orienteret" betyder derfor, at vi arbejder med sproget ved kontinuerligt at definere objekter (lagre information i beholdere) og interagere med disse.

**Python er "cross-platform"**

Python er et "cross-platform" programmeringssprog. Det vil sige, at man kan arbejde med Python på tværs af styresystemer (Windows, macOS, Linux).

# Om dette materiale

Der fokuseres i dette materiale på Pythons brugbarhed og anvendelse inden for samfundsvidenskabelig analyse. Materialet vil derfor ikke give indføring i, hvordan programmeringssprog fungerer generelt og logikkerne bag. Der fokuseres i stedet på at give en tilstrækkelig forståelse for, hvordan man arbejder med programmeringssproget Python, sådan at man kan anvende det i samfundsvidenskabelig analyse.

Materialet er bygget op ved at give forståelse for relevante programmerings- som datatekniske termer gennem praktiske eksempler med Python.

# {#Afsnit}Interager med Python

For at bruge Python skal vi "tale" Python. Man arbejde med Python ved at skrive kommandoer i Python-sproget. Hvis Python forstår din kommando udføres den. Hvis ikke, får du en eller anden form for fejl. Man kan se Python som et meget bogstaveligt og pernitten sprog: Kommandoer skal skrives på helt bestemte måder for at Python kan forstå, hvad du beder om.

Barberes Python ned til sine grundsten består det ikke af mere end en "interpreter" (fortolker). Alle programmeringssprog er bygget op om en fortolker, der "evaluerer" kommandoer. Inden for programmering vil evaluering sige, at sproget forsøger at forstå, hvad der står i en kommando.

## Python uden dikkedarer

Den "rene" installation af Python tilføjer fortolkeren til styresystemet, så man kan arbejde med Python gennem en terminal: 
![python_terminal.png](/python_terminal.png)

I terminalen kan vi skrive en kommando og trykke "Enter" for at få fortolkeren til at evaluere. I nedenstående skrives kommandoen `2+42` hvilket Python evaluerer og giver outputtet `42`:
![python_interpret1.png](/python_interpret1.png)

Python forstår matematiske operationer og vil returnere resultatet af en udregning, når man skriver den ind. 

I nedenstående forsøges at bede om en opskrift på pandekager. Det går knap så godt: 
![python_interpret1.png](/python_interpret2.png)

Når Python ikke kan forstå kommandoen, returneres en fejl. Der findes et væld af fejltyper. I ovenstående gives en `SyntaxError`, fordi kommandoen er skrevet helt forkert (dette er dog ikke det eneste problem med denne kommando, men det er den første fejl, som fortolkeren støder på).

## Brug af Python IDE'er ("Integrated Development Environment")

Selvom man kan arbejde med Python direkte i terminalen frarådes det meget kraftigt, da det er meget vanskeligt at gemme sit arbejde undervejs og svært at bevare overblik over sin kode og arbejde. Derfor arbejder man for det meste gennem et IDE (Integrated Development Environment). Et IDE er et program, som man kan arbejde med Python igennem, som ofte har forskellige funktioner og egenskaber til at hjælpe en bevare overblikket. 

Her nævnes blot et mindre udvalg af IDE'er.

### Spyder

Spyder er bygget op omkring en "script-editor". Et script er et dokument bestående af en række af Python kommandoer, som man kan sende til fortolkeren på én gang. I et script kan fx samles al det databehandlings- og analysearbejde, som man skal lave. Ved at køre scriptet udføres så al arbejdet.
Script-editoren er indbygget med farvekoder, så man nemt kan adskille dele af koden. Spyder giver også automatisk forslag til kommandoer (Spyder 4 og frem).

Derudover giver Spyder en objekt-/variabeloversigt, så man kan se, hvad man har defineret og arbejder med; fx datasæt, resultater, osv.

Spyder er godt til de fleste ting og særligt, hvis man skal arbejde med længere scripts.

Spyder kan installeres sammen med Anaconda: https://www.anaconda.com/products/individual#Downloads

### Jupyter Notebook

Jupyter Notebook er opbygget omkring en såkaldt "notebook". En notebook i Jupyter Notebook kombinerer Python kode med almindelig tekst (skrevet i "Markdown"). Jupyter Notebook egner sig særdeles godt, hvis man skal dokumentere sit kodearbejde undervejs, da man har mulighed for at skrive almindelig tekst, sætte billeder ind, lave tabeller osv. omkring sin kode.

Dette materiale er udarbejdet i Jupyter Notebook.

Jupyter Notebook kan installeres sammen med Anaconda: https://www.anaconda.com/products/individual#Downloads

# {#Kapitel}Fundamentale koncepter i Python

I denne sektion gennemgås de grundlæggende koncepter i Python programmering. Disse kan siges at være byggestenene for næsten alt, som man foretager sig med Python programmering.

Det følgende materiale består af en del kodeeksempler, som er udarbejdet i Jupyter Notebook, men de vil kunne køres i hvilken som helst Python IDE.

# {#Afsnit}Python sproget

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


At arbejde med Python er at arbejde med funktioner. En funktion tager et eller flere input (kaldet "argumenter") og gør et eller andet ved dem. Funktionen `print()` tager enten et stykke tekst eller tal som input, og viser det som et stykke tekst:


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


      File "<ipython-input-28-727c4d594de0>", line 7
        2 * a % b) # modulus - returnerer rest efter "floor division"
                 ^
    SyntaxError: invalid syntax



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

# {#Afsnit}Typer

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

# {#Afsnit}Funktioner

En central del af det at arbejde med et programmeringssprog er at bruge funktioner. Funktioner tager et eller flere input (kaldet "argumenter"), foretager et eller andet med disse og returnerer (for det meste) et output.

Funktioner i Python har følgende format:

- `function(argument1, argument2, ...)`

Funktioner bruges ved at skrive funktionens navn efterfulgt af argumenterne i parentes. En funktion kan have et utal af argumenter, men oftest skal de som minimum have en eller flere variable som input.

Udover argumenter tager funktioner også ofte en del "keyword arguments" som input. Disse kan betragte som en form for indstillinger, som man slår til og fra i funktionen. "keyword arguments" indgår i funktionen med navnet på indstillingen, et `=` og hvad indstillingen skal sættes til, lig nedenstående:

- `function(argument1, argument2, keywordargument1 = "something")`

Ligesom med argumenter, kan en funktion have rigtig mange "keyword arguments"/indstillinger. Det er dog sjældent, at man behøver forholde sig til alle indstillingerne, da de fleste funktioner har en eller anden form for standardindstilling.

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


En funktion kan have rigtig mange indstillinger, og i praksis forholder man sig kun til få af disse, da man oftest kan lade standardinstillingerne være, som de er. 

{{% notice info %}}
Man kan altid få hjælpefilen/dokumentationen frem til en funktion ved at skrive `?[function]` (fx `?print` for dokumentationen for `print()`). Mange IDE'er understøtter også, at man trykker `Shift + Tab` inde i parentesen af en funktion for at få vist en bid af hjælpefilen.
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

Man kan fristes til at lære Python ved at forsøge at lære så mange funktioner som muligt. Dette er en håbløs og nærmest umulig opgave givet omfanget af, hvad der findes af funktioner, der kan hentes til Python. I praksis opbygger man sig arbejdsgange eller workflows, hvori man har tendens til at bruge de samme funktioner igen og igen. Derfor er en god tilgang til Python at spørge: *"Kan jeg bruge Python til X?"* eller *"Hvordan løser jeg problem Y i Python?"*, og så forsøge at finde de rette funktioner til det, frem for at spørge: *"Hvad kan jeg bruge Python til?"*, da man med dette spørgsmål ikke får nogen retning på det, man gerne vil lære om Python.

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


Funktioner defineres med `def` efterfulgt af navnet på den funktion, man gerne vil lave. I parenteserne skrives de input, som funktionen skal have. I ovenstående dannes funktionen `add10`, der tager et enkelt input og lægger ti til. `x` i ovenstående er blot en "pladsholder", da `x` erstattes med hvadend, der sættes i funktionen, når den bruges.

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


En funktion afslutter altid, når den når til en `return` linje. Det vil sige, at ting i funktionen, som skrives ind efter `return`, ignoreres:


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

# {#Afsnit}Metoder

Udover funktioner i Python findes der også "metoder". Lig funktioner tager metoder også en form for input og returnerer et output. 

I modsætning til funktioner er metoder bundet op på bestemte variabeltyper. Det vil sige at variablen skal være en bestemt type for, at metoden kan bruges. Metoder kaldes med `variabel.method(option1 = something)`. Tekstværdier (strings) har fx en række metoder tilknyttet til at ændre teksten:


```python
word = "Hello"

print(word.upper())  # Konverterer til store bogstaver
print(word.lower())  # Konverterer til små bogstaver
```

    HELLO
    hello


Bemærk at metoder som hovedregel ikke ændrer på variablen. Variablen skal derfor defineres om eller på ny, hvis output af en metode skal lagres:


```python
print(word)         # Stadig som det oprindeligt blev lavet

word = word.upper() 
print(word)         # Er nu overskrevet til at være med store bogstaver
```

    Hello
    HELLO


Forsøger man at bruge metoder på variabel af en forkert type, gives der fejl:


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


Metoder tager ofte yderligere argumenter og indstillinger. I nedenstående bruges metoden `.replace()` til at erstatte et hvis ord i tekstvariablen med et andet.


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

# {#Afsnit}Pakker

Pakker i Python er samlinger af funktioner, metoder, værdier osv. Selvom man kan meget i Python, så når man ikke særlig langt uden at importere pakker.

Funktioner, metoder, værdier osv. fra pakker kan nemt indlæses ved at importere dem. Så snart pakken er importeret, er pakkens indhold tilgængeligt.

Fx kender Python ikke værdien pi med det samme:


```python
print(pi)
```


    ---------------------------------------------------------------------------
    
    NameError                                 Traceback (most recent call last)
    
    <ipython-input-53-9e2d2bd32686> in <module>
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

Der et utal af pakker, som Python kan udvides med. I materiale fra CALDISS anvendes primært pakker inden for dataanalyse, web scraping, tekstanalyse og maskinlæring. Hvis du har installeret Python med Anaconda, så er mange af disse pakker allerede installeret og klar til import.

# {#Afsnit}Logiske værdier (booleans)

En stor del af programmeringsarbejde involverer at arbejde med logiske værdier; også kaldt booleanske værdier. Disse lagres som typen `bool`.

Variable af typen `bool` kan *kun* antage værdien sandt (`True`) eller falsk (`False`). Python har en række operatorer, som altid returnerer en booleansk værdi:


```python
a = 10
b = 12

a == b
```




    False



I ovenstående bruges `==` til at spørge: "Er a lig med b?" (`=` bruges selvfølgelig ikke, da denne bruges til at danne variable).

En booleansk værdi kan tilskrives en variabel ligesom alle mulige andre værdier. Sådanne variable bliver typen boolean, som altså kun kan være sand (`True`) eller falsk (`False`).


```python
check = a == b

print(check, 
      type(check))
```

    False <class 'bool'>


Her er en række operatorer, som altid returnerer en booleansk værdi:


```python
a == b  # Lig med
a != b  # Ikke lig med
a > b   # Større end
a >= b  # Større end eller lig med
a < b   # Mindre end
a <= b  # Mindre end eller lig med
```




    True



Mange funktioner og metoder returnerer også booleanske værdier. Fx returnerer metoden `.startswith()` en booleansk værdi afhængig af, om en tekststreng starter med et vis stykke tekst eller ej:


```python
words = "Hello there!"

print(words.startswith("Hello"))
```

    True


Booleanske værdier har mange formål:

- Check af resultat: Værdier checkes op imod et sæt af gyldige værdier
- Filtrering: Værdier udvælges efter bestemte betingelser
- Betinget udførelse: Dele af kode udføres kun, hvis en bestemt betingelse er mødt (noget er "sandt" eller "falsk")
- Fejlhåndtering: Visse fejl kan forventes ved at sætte betingelser op, for derefter at håndtere dem

---
## VIDENSCHECK

Tag et kig på nedenstående kode:


```python
a = 7
b = 17
c = a < b
```

*Hvilken variabel indeholder en booleansk værdi?*

{{%expand "Løsning" %}} `c` indeholder en booleansk værdi (`True`), da det er resultatet af testen af, hvorvidt `a` er mindre end `b`.
{{%/expand%}} 

---

# {#Kapitel}Arbejd med flere værdier

Indtil videre har materialet fokuseret på at arbejde med enkelte værdier i Python. I denne sektion gennemgås de forskellige indbyggede datastrukturer til at håndtere flere værdier.

Derudover introduceres såkaldte kontrolstrukturer, der er måder at udføre funktioner (på en eller flere værdier) baseret på givne betingelser.

# {#Afsnit}Lister, dictionaries og tuples

## Lister

Den mest basale datastruktur er en liste. En liste defineres med `[]`:


```python
my_list = [2, 7, 9, 10]
```

I ovenstående defineres listen `my_list` til at indeholde værdierne 2, 7, 9 og 10. En liste kan fremkaldes ligesom hvilken som helst anden variabel:


```python
print(my_list)
```

    [2, 7, 9, 10]


En liste er blot en beholder af forskellige variable. Lister kan derfor indeholde variable af forskellig typer:


```python
my_list2 = [2, "hello", 10, True]

print(my_list2)
```

    [2, 'hello', 10, True]


Lister kan også indeholde andre lister:


```python
my_list3 = [9, 17, [2, 91], 16]

print(my_list3)
```

    [9, 17, [2, 91], 16]


**Variable i lister**

En liste kan bestå af en række variable:


```python
a = 4
b = 9
c = 11

my_list4 = [a, b, c]

print(my_list4)
```

    [4, 9, 11]


Bemærk dog, at når en liste dannes med variable, så er det variablenes værdi(er), der lagres i listen og ikke selve variablen. 

Det kan ses, hvis man ændrer en af variablerne i listen. Herunder ændres variabel `a` fra `4` til `21`. Selvom variablen ændres, så er indholdet af listen (`my_list4`) ikke ændret. 


```python
print(my_list4)   # listen består af værdierne 4, 9 og 11 tilsvarende variable a, b og c

a = 21            # værdien af variabel af ændres

print(my_list4)   # listens indhold er uændret (stadig 4, 9 og 11)
```

    [4, 9, 11]
    [4, 9, 11]


Når listen genereres, lagres den værdi, som `a` har på det tidspunkt, listen generes. Værdiens tilknytning til variabel `a` lagres altså ikke i listen.

**Index**

Hvert element i en liste tildeles et *index*. Et bestemt element kan altid kaldes frem ved at refere til elementets index med `[]`:


```python
my_list = [2, 7, 9, 10]
print(my_list[0])
```

    2


Index i Python starter altid med 0. Derfor gives i ovenstående det første element af listen `my_list` ved at refere til index 0.

Et element i en liste kan overskrives ved at refere til dets index:


```python
print(my_list)

my_list[2] = 28
print(my_list)
```

    [2, 7, 9, 10]
    [2, 7, 28, 10]


**Slicing**

Elementer i et vis interval kan kaldes frem ved brug af `:` (også omtalt "slicing"). Slicing tager elementer fra det første index givet (inklusiv) til det sidste index givet (eksklusiv).


```python
print(my_list[1:3])
```

    [7, 28]


Ovenstående tages fra index 1 og op til index 3 eklskusivt index 3; altså index 1 (listens andet element: 7) og index 2 (listens tredje element: 9).

Listens længde (antallet af elementer) returneres med funktionen `len()`:


```python
len(my_list)
```




    4



---
## VIDENSCHECK

Tag et kig på nedenstående liste:


```python
a_list = [45, 67, 3, 36, 87]
```

*Hvilket element (tal i listen) har index 3?*

{{%expand "Løsning" %}} Index 3 af `a_list` (`a_list[3]`) indeholder tallet 36; altså det fjerde element, da index tælles fra 0.  


```python
print(a_list[3])
```

    36


{{%/expand%}}

---

## Tuples

Tuples fungerer på mange måder ligesom lister med den undtagelse, at værdier i en tuple ikke kan ændres.

Tuples laves med `()`:


```python
my_tuple = ("Katarn", "Kenobi", "Windu")

print(my_tuple)
```

    ('Katarn', 'Kenobi', 'Windu')


Elementer i en tuple har indexes ligesom ved lister:


```python
my_tuple[0]
```




    'Katarn'



Forsøger man at ændre et element af en tuple, får man dog fejl:


```python
my_tuple[0] = "Palpatine"
```


    ---------------------------------------------------------------------------
    
    TypeError                                 Traceback (most recent call last)
    
    <ipython-input-76-b2ea6727d80b> in <module>
    ----> 1 my_tuple[0] = "Palpatine"


    TypeError: 'tuple' object does not support item assignment


---
## VIDENSCHECK

Tag et kig på de to nedenstående datastrukturer (`a` og `b`):


```python
a = [2, 90, 10, 17]
b = (56, 78, 3, -9)
```

*Kan tredje element af `b` (index 2: `3`) ændres til `49` ved at skrive `b[2] = 49`?* 

{{%expand "Løsning" %}} Nej. `b` er en tuple, og værdierne kan derfor ikke ændres. Værdierne i `a` kan dog ændres, da det er en liste. {{%/expand%}}

---

## Dictionaries

En tredje måde at lagre flere værdier i Python er med *dictionaries*. Dictionaries består af en række sæt af nøgler og værdier. 

Dictionaries defineres med `{}`:


```python
my_dict = {"jedi": "Katarn", "sith": "Desann"}
```

Hvert nøgle- og værdisæt defineres med en nøgle i form af en string efterfulgt af værdien efter `:`. Værdien kan være tal, tekst, liste, en anden dictionary osv.

De forskellige nøgle- og værdisæt adskilles med `,`.

Dictionaries har ikke et index, da Python ikke betragter dem som værende i en bestemt rækkefølge. Værdierne kaldes derfor frem ved at referere til deres nøgle:


```python
print(my_dict["jedi"])
```

    Katarn


Nøgler *skal* være unikke. Det er ikke muligt at lave en dictionary med to identiske nøgler. Hvis man forsøger at gøre det, vil den senest skrevne værdi til nøglen blive lagret:


```python
my_dict = {"jedi": "Katarn", "sith": "Desann", "jedi": "Kenobi"}

print(my_dict)
```

    {'jedi': 'Kenobi', 'sith': 'Desann'}


Ligeledes kan værdier til en bestemt nøgle overskrives:


```python
my_dict["jedi"] = "Katarn"

print(my_dict)
```

    {'jedi': 'Katarn', 'sith': 'Desann'}


Elementer kan tilføjes til en dictionary ved blot at tilknytte det til en nøgle, som endnu ikke er brugt i dictionarien:


```python
my_dict["dealer"] = "Watto"

print(my_dict)
```

    {'jedi': 'Katarn', 'sith': 'Desann', 'dealer': 'Watto'}


---
## VIDENSCHECK

*Kan en dictionary indeholde forskellige typer af værdier?*

{{%expand "Løsning" %}} Ja. Værdier i en dictionary kan være af alle mulige typer, men nøglen skal altid være en string. {{%/expand%}}

---

---
## VIDENSCHECK

Tag et kig på nedenstående dictionary:


```python
famous_animals = {"Pluto": "dog", "Oggy": "cat", "Pinky": "mouse", "Pumba": "warthog"}
```

*Hvordan fremkaldes den 3. værdi ("mouse")?*

{{%expand "Løsning" %}} Den 3. værdi fremkaldes ved at refere til den rigtige nøgle: `famous_animals["Pinky"]`. Python betragter ikke værdien som den 3. værdi, da værdien knyttes op på nøglen og ikke på rækkefølgen, som den står i dictionary. {{%/expand%}}

---

# {#Afsnit}Loops

I arbejdet med dataanalyse udfører man ofte de samme kommandoer, kontroller, kørsler osv. igen og igen:

- En række oplysninger kan kontrolleres, om de er korrekte. Har de den rigtige type? Er værdierne gyldige? (fx at aldersværdier ikke har skøre værdier som 987 år).
- Den samme beregning skal foretages for en række oplysninger - fx udregning af gennemsnit for indkomst, alder, år i arbejde osv.
- De samme oplysninger skal hentes fra en række forskellige hjemmesider.

I Python (og mange andre programmeringssprog) kan man anvende "loops" til at gentage kommandoer. De mest gængse loop typer er "for loops" og "while loops". "for loops" gentager en eller flere kommandoer over en række værdier. "while loops" gentager en kommando, så længe en hvis betingelse er opfyldt.

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

Pladsholderen `age` bruges i kommandoerne, som skal gentages for hvert loop. Kommandoerne skrives på linjen efter `:`. Her er det vigtigt, at kommandoerne i loopet er rykket ind (enten med tab eller fire mellemrum, men de fleste IDE'er laver dette mellemrum automatisk).

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

While loops er en anden type loops i Python. Hvor for loops gentager en eller flere kommandoer for hver værdi i en række af værdier, så gentager while loops en eller flere kommandoer, så længe en hvis betingelse er opfyldt.

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

I ovenstående defineres først `x` til at være `1`. Derefter igangsættes et while loop, som skal køre, så længe at `x < 5`. Kommandoerne, som skal køre i loopet, skrives på linjen efter `:`. Her er det igen vigtigt, at kommandoerne i loopet er rykket ind (enten med tab eller fire mellemrum, men de fleste IDE'er laver dette mellemrum automatisk).

Derefter overskrives `x` til at være `x + 1`; altså at værdien af `x` øges med `1`. Bemærk at hvis denne linje undlades, så bliver loopet ved med at gentage sig, da `x` ikke ændres og derfor bliver ved med at være `1`; altså mindre end `5`, som er betingelsen for, at loopet kører.

{{% notice warning %}} Man skal være forsigtig, når man skriver while loops, da man meget nemt kan komme til at skabe uendeligt loops! 

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

Første kommando at printe teksten `"the word is " + fruit` (husk at tekststykker kan sættes sammen med `+`). Da `fruit` i den første kørsel indeholder `banana` bliver teksten `the word is banana`. 

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

# {#Afsnit}If-betingelser

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

I koden evalueres først if-betingelse: `x > 10`. Hvis denne evalueres til `True`, udføres kommandoen efter `:`. I ovenstående er `x = 12`, hvorfor kommandoen udføres. Her er kommandoen blot at printe teksten `Tallet er større end 10!`.

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

If-betingelser er yderst nyttige i kombination med andre kontrolstrukturer. Fx kan man i kombinationen med for loops og if-betingelser skrive kode, hvor en vis kommando kun udføres på visse værdier i en liste:


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

# {#Kapitel}Supplerende materiale

De følgende sider indeholder diverse materiale til at hjælpe videre med Python.

# {#Afsnit}Python IDE'er

Der findes mange måder at arbejde med Python. Her er blot tre forslag til IDE'er ("Integrated development environment").

---


**Jupyter Notebook**
Med Jupyter Notebook arbejder man med Python i celler. Det egner sig især til kortere kodestykker, hvor der skal kommenteres undervejs. Det er muligt at kombinere Python kode med normale tekstceller. 

Jupyter Notebook tillader både en meget interaktiv måde at arbejde med Python samt nemme løsninger til at lave samlede rapporter og dokumenter, hvor kode, beskrivelse og output kombineres.

Læs mere om Jupyter Notebook her: https://jupyter.org/

Jupyter Notebook kan installeres sammen med Anaconda: https://www.anaconda.com/products/individual#Downloads

---

**Jupyter Lab**
Jupyter Lab er en videreudvikling af Jupyter Notebook. Jupyter Lab er en samlet platform, der giver bedre overblik over forskellige filer og dokumenter, som man har liggende i sin arbejdssti. 

Læs mere om Jupyter Lab her: https://jupyter.org/

---

**Spyder**
Spyder er baseret på en script-editor, hvor ens kode skrives i et langt stykke tekst. Det kan være lidt mere avanceret at arbejde med, men til gengæld har Spyder en del funktionalitet, der hjælper med at holde styr på ens data, variable, funktioner osv.

Læs mere om Spyder her: https://www.spyder-ide.org/

Spyder kan installeres sammen med Anaconda: https://www.anaconda.com/products/individual#Downloads

---

# {#Afsnit}Serverløsninger til Python

Der findes adskillige online løsninger til at arbejde med Python. På den måde slipper man for selv at skulle sætte det op, og man vil ofte have mere computerkraft til rådighed, end man har på sin egen computer.

---

**CALDISS serverløsning**

CALDISS har en server til Jupyter Notebook. På den måde kan man komme i gang med Python uden at skulle installere det på egen computer. Serveren ligger på AAU's netværk og kan tilgås på AAU's netværk eller via VPN.

Serveren har adressen: https://samf-jupyter.aau.dk/hub/login

Bliv bruger af serveren ved at udfylde [denne formular](https://forms.office.com/Pages/ResponsePage.aspx?id=Sbrb9QbOb0msPgzxQ2HZNGg7-JICeN1Kopl4dsYkgftUQTE3UDRMWUtFQzBKT0dLVTNROVdBUk05MCQlQCN0PWcu).

---

**Google Colab**

Google Colab fungerer ligesom en online version af Jupyter Notebook. Her kan man skrive notebooks, som man gør i Jupyter Notebook, men køre dem over Google's servere. Det kræver en Google konto for at bruge.

Læs mere her: https://colab.research.google.com/notebooks/intro.ipynb (i øvrigt en fin introduktion til at arbejde med notebooks også).

---


# {#Afsnit}Litteratur og yderligere materiale

Her ses forslag til steder, hvor du kan lære mere om basalt brug af Python.


## Online kurser

- "Data Analysis and Visualization with Python for Social Scientists *alpha*" af DataCarpentry: https://datacarpentry.org/python-socialsci/
- "Python Tutorial" af Tutorialspoint: https://www.tutorialspoint.com/python/index.htm
- "Introduction to Python" af DataCamp: https://www.datacamp.com/courses/intro-to-python-for-data-science (betalingsside, men første del er gratis)

# {#END}
