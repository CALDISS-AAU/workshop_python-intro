# Manus til videoer - Introduktion til Python



## Landingsside

**Velkomstvideo**

- Hvad indeholder kurset?
- Hvem er det lavet til?
- Hvordan bruger man kurset?



## 1. Hvad er Python

**At arbejde med et programmeringssprog**

- Hvad er Python?
- Hvad er et programmeringssprog?
- Eksempelkode - kort analyseeksempel
- Hvorfor bruge Python?
- Hvad kendetegner Python?
- OBS: Dette kursus har fokus på Python til dataanalyse



**Interager med Python**

- Hvordan virker Python? - En fortolker
- Hvad er en fortolker?
- Kommandoer og evaluering
- Ting Python forstår
- Ting Python ikke forstår
- Brug af IDE'er (i dette kursus bruges Jupyter)



## 2. Fundamentale koncepter i Python

**Python sproget**

- Hurtig introduktion til Jupyter
- Evaluering af matematiske operationer i Jupyter Notebook
- Jupyter: Tillader at skrive flere linjer og køre dem alle (printer automatisk output af sidste linje)
- Kort omkring funktioner (`print`)



**Variable**

- Hvad er en variabel i Python?
- Forveksl ikke variabel med variabel i statistisk forstand
  - Evt. kald det "objekter"
- Definition af variable
- Kald af variable
  - Bemærk forskel mellem lille og stort bogstav
- Variable med tekst
- Ændring af variable 
  - Bemærk hvornår der overskrives og ikke overskrives!
- Gode variabelnavne



**Typer**

- Hvad er 'typer'? (Pythons måde at adskille mellem variable)
- Her gennemgås først numeriske typer og tekst typer
- Numeriske typer: integer og float
- Tekst typer - kaldes strings
- Ændring af typer: casting
- Typer kan for det meste laves om
  - Obs: Funktioner til casting variere



**Funktioner**

- Funktioner: En central del af Python programmering
- Opbygning: function(argument1, argument2, ...)
  - function(argument1, argument2, keywordargument1 = "something")
- Brug af print (med flere argumenter)
  - `print` og `typer` er eksempler på funktioner!
- Se hjælpefunktioner/dokumentation (i jupyter)
- Brug af keyword arguement "sep" i `print`
- Hvordan laver man egne funktioner?
  - Bemærk: Netop derfor man kan så meget i Python
- Lav `add10()` funktion
- Hvordan fungerer variable inden i en funktion?
- Obs: Output af funktion skal gemmes i variabel, hvis det skal kaldes frem igen
- Hvad laver `return`?
  - Obs: Ting efter return ignoreres



**Metoder**

- Hvad er metoder?
- Metoder kan betragtes som funktioner, som er tilknyttet bestemte typer (eller rettere, klasser)
- Format: `variabel.method(option1 = something)`
- Eksempler med `.upper()` og `.lower()`
- Eksempler med `replace` - bemærk argumenters rækkefølge



**Pakker**

- Hvad er pakker?: Samling af funktioner
- Man når ikke langt uden pakker
- Hvordan importeres pakker? (eksempel med `math.pi`)
  - `import`
  - `from X import Y`
  - `import X as Y`
- Pas på med at importere dele af pakker - kan være svært at overskue, hvor noget kommer fra
  - Overvej læsbarhed af kode



**Logiske værdier (booleans)**

- Hvad er logiske værdier?: Kan kun være sandt eller falsk
- Bruges til kontroller, betingelser, filtreringer
- Logiske operatorer
  - Særlig obs på `=` og `==`
- Eksempel med metode, der returnerer boolean





## Arbejd med flere værdier

**Lister**

- Hvordan laver man en liste?
- Lister er ligeglad med typer
  - Obs: lister i lister derfor mulig
- Variable i lister mulig
- Index
  - Obs: Python tæller fra 0
- Slicing 
  - Obs: første inklusiv, sidste eksklusiv
- Indexes og slicing ses også i andre datastrukturer
- Tuples: Lister som ikke kan ændres



**Dictionaries**

- Anden måde at lagre på
- key-value pairs
- Hvordan laver man dictionary?
- Hvordan kaldes værdi fra dictionary frem?
- Obs: Dictionary har ikke rækkefølge (intet index)
- Key skal være unik
- Hvordan tilføjes til dictionaries?
- Dictionaries kan laves hierarkisk



**Loops**

- Man er ofte ude for at skulle gentage kommandoer: det kan loops hjælpe med
- Mest gængse loops: `for loops` og `while loops`
- For loops: gentager kommando for hvert element i en afgrænset mængde af elementer/variable
- Eksempel med at printe type for liste af variable
- Opbygning af loop: Værdier, som loop skal køre over samt kommandoer, som skal køre for hver værdi
- Obs på placeholder-værdien i `for`-sætningen: bruges og findes kun i for loopet
- <u>While loops</u>
  - Loop der gentager sig, så længe en betingelse er sand
  - Obs på uendelige loops!
  - Hvornår bruges de? Fx web scraping



**If-betingelser**

- Bruges til at sætte betingelser: kode der kun skal køre, hvis en hvis betingelse er sand
- `if` og `else` blok
- Flere betingelser kan sættes med `elif`
- Kombination af if-betingelser og for loops
- if betingelser og funktioner

