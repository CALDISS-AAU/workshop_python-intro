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

## Hvorfor arbejde med et programmeringssprog?

At skulle arbejde på denne måde kan virke lidt gammeldags. Når nu programmer til dataanalyse laves med brugerflader og brugervenlige måder og bruge dem på, hvorfor så arbejde med dataanalyse i et program, hvor vi selv skal programmere og skrive kommandoer for at opnå det, vi gerne vil?

Programmer med brugerflader som Excel, Stata, SPSS osv. har selvfølgelig deres styrke i, at de er langt nemmere at bruge. Dog er sådanne programmer begrænset i deres funktionalitet, da de er udviklet til at arbejde med data på bestemte måder i bestemte formater. Med Python kan vi opnå meget af det samme og meget mere, da man i et programmeringssprog ikke er tvunget til at arbejde med bestemte dataformater, filtyper osv. Samtidig giver det at arbejde med et programmeringssprog os også den mulighed, at vi selv skriver vores egne "mini-programmer", der løser den specifikke udfordring, som vi lige står over for.

## Python som programmeringssprog

Der findes et væld af programmeringssprog. I dette materiale arbejdes med sproget Python. Mange logikker i programmering går på tværs af sprog, men de har hver deres styrker, svagheder og kendetegn. 

**Python er "general purpose"**

Python er et "general purpose" programmeringssprog. Det vil sige, at det er udviklet til at blive brugt inden for så mange områder som muligt.

**Python er "objekt-orienteret"**

Python er et "objekt-orienteret" programmeringssprog. Det vil sige, at sproget er baseret på at arbejde med "objekter". Et objekt inden for programmering kan være nærmest hvad som helst. Meget kort sagt er et objekt en beholder for en eller anden form for information. At Python er "objekt-orienteret" betyder derfor, at vi arbejder med sproget ved kontinuerligt at definere objekter (lagre information i beholdere) og interagere med disse.

**Python er "cross-platform"**

Python er et "cross-platform" programmeringssprog. Det vil sige, at man kan arbejde med Python på tværs af styresystemer (Windows, macOS, Linux).

# Om dette materiale

Der fokuseres i dette materiale på Pythons brugbarhed og anvendelse inden for socialvidenskabelige analyse. Materialet vil derfor ikke give indføring i, hvordan programmeringssprog. Der fokuseres i stedet på at give en tilstrækkelig forståelse for, hvordan man arbejder med programmeringssproget Python, sådan at man kan anvende det i socialvidenskabelige analyse.

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

Derfor er det en god ide at indarbejde en god navngivningsskik. Kunsten er at balancere mellem korte navne og navne, som er sigende for det, som variablen indeholder.


```python
a = 10              # kort, men ikke sigende for indholdet
the_number_ten = 10 # sigende, men ret langt, hvis man skal bruge variablen igen og igen
```

{{% notice tip %}}

**Tips til variabelnavne**

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

---
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

---

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

---
## VIDENSCHECK

I ovenstående bliver variablen `a` brugt til at definere variabel `b`. 

*Hvilken type er variablen `a` efter at variabel `b` defineres?*

{{%expand "Løsning" %}}
`a` er stadig en *integer*. `a` ikke ændres i koden, men bliver blot brugt til at lave variabel `b`.
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


---
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

---

# {#Afsnit}Funktioner

En central del af det at arbejde med et programmeringssprog er at bruge funktioner. Funktioner tager et eller flere input (kaldet "argumenter"), foretager et eller andet med disse og returnerer (for det meste) et output.

Funktioner i Python har følgende format:

- `function(argument1, argument2, ...)`

Funktioner bruges ved at skrive funktionens navn og skrive de argumenterne i parentes. En funktion kan have et utal af argumenter, men oftest skal de som minimum have et eller flere variable som input.

Udover argumenter tager funktioner også ofte en del "keyword arguments" som input. Disse kan betragte som en form for indstillinger, som man slår til og fra i funktionen. "keyword arguments" indgår i funktionen med navnet på indstillingen, et `=` og hvad indstillingen skal sættes til, lig nedenstående:

- `function(argument1, argument2, keywordargument1 = "something")`

Ligesom med argumenter, kan en funktion have rigtig mange "keyword arguments"/indstillinger. Det er dog sjældent, at man behøver forholde sig til alle indstillingerne, da de fleste funktioner har en eller anden form for standardindstilling.

## Sådan bruges funktioner

Tidligere i dette materiale har funktionerne `print()` og `type()` været brugt. Ved `print()` har denne kun været brugt med et enkelt argument; altså det, som skal vises, men faktisk accepterer print flere argumenter:


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
Man kan altid få hjælpefilen/dokumentationen frem til en funktion ved at skrive `?[function]` (fx `?print` for dokumentationen for `print()`. Mange IDE'er understøtter også, at man trykker `Shift + Tab` inde i parentesen af en funktion for at få vist en bid af hjælpefilen.
{{% /notice%}}

{{% notice note %}}
Det, som der står i de forskellige "keyword arguments" i dokumentationen for en funktion, er funktionens standardindstillinger. 
{{% /notice%}}

---
## VIDENSCHECK

Hvordan får man `print()` til at adskille input værdierne med en `-`?

{{%expand "Løsning" %}}
Indstillingen `sep` sættes til `sep = '-'.


```python
print(a, b, sep = '-')
```

    Hello-there


{{%/expand%}}

---

## Hvor kommer funktioner fra?

Python har en række funktioner indbygget, men faktisk kommer størstedelen af funktionerne i Python fra alle mulige andre, som har udviklede funktioner til forskellige formål, som andre derefter kan gøre brug af. Andre funktioner hentes ind i form af "pakker", som gennemgås senere i dette materiale.

Man kan fristes til at lære Python ved at forsøge at lære så mange funktioner som muligt. Dette er en håbløs og nærmest umulig opgave givet omfanget af, hvad der findes af funktioner, der kan hentes til Python. I praksis opbygger man sig arbejdsgange eller workflows, hvori man har tendens til at bruge de samme funktioner igen og igen. Derfor er en god tilgang til Python at spørge: *"Kan jeg bruge Python til X?"* eller *"Hvordan løser jeg problem Y i Python?"*, og så forsøge at finde de rette funktioner til det, frem for at spørge: *"Hvad kan jeg bruge Python til?"*, da man med dette spørgsmål ikke får nogen retning på det, man gerne vil lære om Python.

At Python kan så mange ting i dag skyldes netop, at folk rundt omkring i verden har stået over for forskellige udfordringer, som de har løst ved at udvikle funktioner til Python, som de derefter stiller til rådighed. 

Python fortæller med det samme, hvis funktionen, som man forsøger at bruge, ikke kendes af Python:


```python
add10(5)
```


    ---------------------------------------------------------------------------
    
    NameError                                 Traceback (most recent call last)
    
    <ipython-input-13-7452fc393844> in <module>
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


Funktioner defineres med `def` efterfulgt af navnet på den funktion, man gerne vil lave. I parenteserne skrives de input, som funktionen skal have. I ovenstående dannes funktionen `add10`, der tager et enkelt input og lægger ti til. `x` i ovenstående er blot en pladsholder, da `x` erstattes med hvadend, der sættes i funktionen, når den bruges.

Efter `:` skrives det, som skal ske i funktionen. Alle variable, som defineres inde i funktionen, eksisterer *kun* i selve funktionen. Sagt på en anden måde, så kan variable, der defineres i funktionen, ikke kaldes frem. I funktionen `add10()` defineres `result` undervejs, men den eksisterer ikke uden for funktionen:


```python
print(result)
```


    ---------------------------------------------------------------------------
    
    NameError                                 Traceback (most recent call last)
    
    <ipython-input-30-6459d04d738f> in <module>
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

$A = \frac{1}{2} * h * g$

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


Bemærk at metoder som hovedregel ikke ændrer på variablen. Variablen skal derfor defineres om eller på ny, hvis output af brug af en metode skal lagres:


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
    
    <ipython-input-38-d30eebf09ae0> in <module>
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

# {#Afsnit} Logiske værdier (boolean)

En stor del af programmeringsarbejde involverer at arbejde med logiske værdier; også kaldt booleanske værdier.

Booleanske værdier kan *kun* antage værdien sandt eller falsk. Python har en række operatorer, som altid returnerer en booleansk værdi:


```python
a = 10
b = 12

a == b
```




    False



I ovenstående bruges `==` til at spørge: "Er a lig med b?" (`=` bruges selvfølgelig ikke, da denne bruges til at lave variable).

En booleansk værdi kan tilskrives en variabel ligesom alle mulige andre værdier. Sådanne variable bliver typen boolean, som altså kun kan være sand (`True`) eller falsk (`False`).


```python
check = a == b

print(check, type(check))
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

Mange funktioner og metoder returnerer også booleanske værdier. Fx returnerer metoden `.startswith()` en booleansk værdi afhængig af, om en tekststreng starter med et hvis stykke tekst eller ej:


```python
words = "Hello there!"

print(words.startswith("Hello"))
```

    True


Booleanske værdier har mange formål:

- Check af resultat: Værdier checkes op imod et sæt af gyldige værdier
- Filtrering: Værdier udvælges efter bestemte betingelser
- Betinget udførelse: Dele af kode udføres kun, hvis en bestemt betingelse er mødt
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

{{%expand "Løsning" %}} `c` indeholder den booleanske værdi (`True`), da det er resultatet af testen af, hvorvidt `a` er mindre end `b`.
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


En liste er blot en beholder af forskellige variable. Lister kan derfor indeholde variable af forskellig type:


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


**Index**

Hvert element i en liste tildeles et *index*. Et bestemt element kan altid kaldes frem ved at refere til elementets index med `[]`:


```python
my_list = [2, 7, 9, 10]
print(my_list[0])
```

    2


Index i Python starter altid med 0. Derfor gives i ovenstående det første element af listen `my_list3` ved at refere til index 0.

Et element i en liste kan overskrives ved at refere til dets index:


```python
print(my_list)

my_list[2] = 28
print(my_list)
```

    [2, 7, 9, 10]
    [2, 7, 28, 10]


**Slicing**

Elementer i et hvis interval kan kaldes frem ved brug af `:` (også omtalt "slicing"). Slicing tager elementer fra det første index givet (inklusiv) til det sidste index givet (eksklusiv).


```python
print(my_list[1:3])
```

    [7, 9]


Ovenstående tager fra index 1 og op til index 3 eklskusivt index 3; altså index 1 (listens andet element: 7) og index 2 (listens tredje element: 9).

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
    
    <ipython-input-100-b2ea6727d80b> in <module>
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

En anden måde at lagre flere værdier i Python er med *dictionaries*. Dictionaries består af en række sæt af nøgler og værdier. 

Dictionaries defineres med `{}`:

- Nøgler og værdier
- Check: Hvad er en dictionary?
- Check: Kan de indeholde forskellige typer?
- Check: Har dictionary et index?
- Øvelse: Definer dictionary


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

# {#END}