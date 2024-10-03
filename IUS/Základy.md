## Use case diagram

> - cílem je najít **aktéry** a jejich **případy užití**
> - obsahuje hranice systému, aktéra, případ užití a interakce

![[Use case diagram.png|300]]

#### Specifikace

> - konkretizuje případ užití
> - většinou se píše do tabulky
> - případ užití obsahuje název, identifikátor a specifikaci
> - specifikace potom vstupní podmínky, události a podmínky

![[Specifikace Use case diagram.png|350]]

#### Vazba \<\<include\>\> a \<\<extend\>\>

> Relace \<\<include\>\> - use case obsahuje připojený use case (pevně spojené)
> Relace \<\<extend\>\> - use case může obsahovat připojený use case
> Zobecnění účastníka - podobné OOP (aktér dědí od jiného aktéra)

![[iclude a exclude.png|600]]


## Diagram aktivit

>Reprezentují objektově orientované vývojové diagramy. Modelují procesy, většinou s více účastníky. Modelují se pomocí nich scénáře případů užití nebo detaily operaci či algoritmů.
>Skládá se z
>- uzlů - objektové modelují objekty podílející se na aktivitách, akční modelují aktivitu a řídící modelují rozhodování
>- hrany - řídící modelují přechody mezi uzly a objektové modelují cesty mezi objekty a uzly

![[Diagram aktivit.png|400]]


## Stavové diagramy

> Modeluje životní cyklus reaktivního objektu. Reaguje na vnější události. Cyklus je modelován pomocí stavů přechodů a událostí. Chování je důsledkem předchozího stavu (chování). 
> U přechodů se značí událost jako 
	event smazat(m)
> podmínku jako
	[cislo > 5]
> a akci jako
	entry / nastavit

![[Stavový diagram.png|400]]

