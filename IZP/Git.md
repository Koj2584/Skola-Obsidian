Každý počítač uchovává celou [[Verzování|verzi projektu]] a nahrává jej na server odkud si ji mohou stáhnout ostatní počítače.

==Patch = rozdílné soubory==

Patch se používá pro záznam rozdílu u dvou verzí (například oprava chyb, záplaty atd.). Zároveň je to **úspornější uložení změn** dvou verzí. Může zaznamenat změny jednoho i více souborů (celé adresáře).


#### Souhrn Git příkazů

Inicializace adresáře .git:

	 git init 

Přidání souboru do commitu:

	git add [soubor]
	git add . - Všechny změny

Vytvoření commitu:

	git commit -m "[zpráva]"

Zobrazení statusu:

	git status

Zobrazit log:

	git log

Zobrazí/vytvoří větve:

	git branch 
	git breanch [jméno nevé větve]

Pohyb mezi verzemi:

	git checkout [commit hash nebo větev]

Spojení větví:

	git merge [větev]

Naclonování repozitáře:

	git clone [url]

Založení adresy vzdáleného repozitáře:

	git remote add [nazev] [url]

Nahrání mých verzí:

	git push -u [nazev] [větev]

Stažení poslední verze:

	git pull -u [nazev] [větev]
