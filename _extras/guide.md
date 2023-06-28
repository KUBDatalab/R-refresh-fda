---
title: "Instructor Notes"
---

## Generelt om kurset
Kurset er en genopfriskning af hvad der bør være
kendt stof for de studerende, med henblik på at de
skal have fundamentet på plads til kurset Fødevaredataanalyse.

Der er derfor ikke tale om en introduktion, og de fleste emner kan derfor gennemgås noget hurtigere end ellers.

Vær dog opmærksom på om de studerende rent faktisk har forstået de centrale pointer!

## Piper

Fødevaredataanalyses undervisningsmateriale bruger i ret høj grade base-R i stedet for Tidyverse. 

Vi introducerer dog piper når vi viser alternativer
til datamanipulation og aggregate() funktionen.

Her bruger vi magrittr pipen ( %>% ) i stedet for 
den relativt nye base-R pipe (|>).
Det bliver vi ved med indtil RStudio ændrer default tastaturgenvejen (ctrl-alt-m) til at 
levere en base-R pipe. Og det gør vi, fordi vi tager udgangspunkt i default opsætninger - vi skal ikke bruge tid på at ændre Rstudio fra det de studerende har når de har en frisk installation.


## Maskerede funktioner
Her er et konkret eksempel.
```{r eval = F}
library(dplyr)
library(MASS)

mtcars %>% select(cyl)
```

## Kvartiler

Har vi en variabel der indeholder tal, kan vi sortere den variabel, så 
de mindste tal står først, og de største til sidst. 

Deler vi dernæst alle disse tal op i fire lige store portioner, har vi såkaldte
kvartiler. Den første kvartil, der indeholder 25% af observationer, kaldes også 
25% kvartilen. Vi interesserer os ofte for den "interkvartile afstand",
på engelsk Inter Quartile Range, der er afstanden fra den mindste værdi i 
anden kvartil, til den største værdi i tredie kvartil. Det er det interval
hvor halvdelen af af observationerne ligger, vel at mærke den halvdel der ligger
omkring medianen.

Der tales ofte om deciler. Det er hvad vi får når vi deler de sorterede
observationer op i 10 portioner. 

Vi kan forestille os mange andre opdelinger. De kaldes under et stadig for kvartiler - også selvom de egentlig hedder kvintiler hvis opdelingen er fem.

## Medianen

Medianen er et hyppigt brug alternativ til gennemsnit. Vi finder den ved at 
sortere alle observationer af en bestemt variabel efter størrelse. Den miderste
værdi er medianen. Det er den værdi for hvilken det gælder, at halvdelen af
vores observationer er større. Og den anden halvdel er mindre. Det er ofte 
et bedre bud på den typiske værdi af variablen end gennemsnittet, der kan
skævvrides en del af enkelte meget store eller meget små værdier.

Lidt mere om hvad der sker hvis der er et lige antal observationer. Og mindre knudret formulering.

## Yderligere tips og tricks til organisering
Disse links kan være nyttige til inspiration:

https://ntguardian.wordpress.com/2018/08/02/how-should-i-organize-my-r-research-projects/

https://kkulma.github.io/2018-03-18-Prime-Hints-for-Running-a-data-project-in-R/

https://www.chrisvoncsefalvay.com/2018/08/09/structuring-r-projects/

{% include links.md %}
