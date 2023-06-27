---
title: "Instructor Notes"
---
FIXME



Why are we using the magrittr pipe ( %>% ) instead of the
base-R pipe (|>)?
As long as the default pipe-shortcut in RStudio (ctrl-alt-m) 
results int the magrittr pipe and not the base pipe, we are
using the magrittr pipe. The alternative would be to have 
all learners change the standard settings in RStudio.

SKAL vi have dette eksempel med???
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

## Medianen

Medianen er et hyppigt brug alternativ til gennemsnit. Vi finder den ved at 
sortere alle observationer af en bestemt variabel efter størrelse. Den miderste
værdi er medianen. Det er den værdi for hvilken det gælder, at halvdelen af
vores observationer er større. Og den anden halvdel er mindre. Det er ofte 
et bedre bud på den typiske værdi af variablen end gennemsnittet, der kan
skævvrides en del af enkelte meget store eller meget små værdier.

## Yderligere tips og tricks til organisering
Disse links kan være nyttige til inspiration:

https://ntguardian.wordpress.com/2018/08/02/how-should-i-organize-my-r-research-projects/

https://kkulma.github.io/2018-03-18-Prime-Hints-for-Running-a-data-project-in-R/

https://www.chrisvoncsefalvay.com/2018/08/09/structuring-r-projects/

{% include links.md %}
