Pro řešení a navrhování elektrických obvodů lze použít následující 3 zákony protože všude platí.
1. [[IEL#Ohmův zákon|Ohmův zákon]]
2. [[IEL#I. Kirchhoffův zákon|I. Kirchhoffův zákon]]
3. [[IEL#II. Kirchhoffův zákon|II. Kirchhoffův zákon]]

Popisují fungování obvodů a co v nich energie provede.

----
### Topologie obvodů

![[Uzel.png|200]]
>- **Uzel** - místo kde se stýká více vodičů

![[Větev.png|400]]
> - **Větev** - cesta mezi uzly

![[Smyčka.png|400]]
> - **Smyčka** - uzavřená dráha v obvodu tvořená větvemi

---
### Zdroje

##### Ideální zdroj napětí
>Zdroj jehož svorkové napětí nezávisí na zatížení, neboli je stále stejné.

![[Ideální zdroj napětí.png]]

##### Skutečný zdroj
>U tohoto zdroje svorkové napětí **klesá, pokud ho zatížíme**. **Čím více** odebíráme **proudu**, **tím víc** je svorkové **napětí nižší**. Skutečný zdroj má totiž vnitřní odpor ,na němž vzniká při odběru proudu úbytek.

![[Graf zdroje.png]]


##### Ideální zdroj proudu
> Zdroj, který dodává pořád stejný proud, bez ohledu na velikost zátěže. Neboli se mění svorkové napětí dle zátěže ale proud je stále stejný (Tak aby platil Ohmův zákon).

![[Ideální zdroj proudu.png]]

##### Zapojení skutečného zdroje
> Skutečný zdroj jde znázornit pomocí ideálních zdrojů následovně

![[Skutečný - Ideální zdroj proudu.png|400]]

![[Skutečný - Ideální zdroj napětí.png|400]]

##### Vnitřní odpor
> - Proměnlivý - závisí na energii, teplotě, atd.
> - Málo kdo poskytuje u výrobků přesné údaje
> - Lze ho potlačit regulací svorkového napětí (díky rezervě -> jen určitý rozsah)

##### Dělič napětí
>Obvod kde jsou dva rezistory připojeny ke stejnému zdroji. Lze ho považovat za dvojbran (Dvě vstupní a dvě výstupní svorky). 

![[Dělič napětí.png]]

 > ## $U_2 = \frac{R_2}{R_1 + R_2}U$
 
 