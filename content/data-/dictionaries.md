---
title: Dictionaries
weight: 2
---
youtube ZW_chK-cDlM >}}

Man kan også lagre flere værdier i Python med *dictionaries*. Dictionaries består af en række sæt af nøgler og værdier. 

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

{{%expand "Løsning" %}} Den 3. værdi fremkaldes ved at refere til den rigtige nøgle: `famous_animals["Pinky"]`. Python betragter ikke værdien som den 3. værdi, da værdien knyttes op på nøglen og ikke på rækkefølgen, som den er skrevet ind i en dictionary. {{%/expand%}}

---
