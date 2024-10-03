
> Pro práci s haldou v c je funkce malloc(size_t size). Při chybě vrací NULL

``` c
int *p = malloc(sizeof(int));

if(p=malloc(sizeof(int)) == NULL)
	return ERR_MALLOC;
``` 
>Při práci s malloc je potřeba dávat pozor na přepsání adresy. Pokud se tak stane nemám jak alokované místo uvolnit.

``` c
int *p = malloc(sizeof(int));

p = &x; // Chyba !!!
``` 
> Pro uvolnění se používá funkce free(void \*ptr). Tato funkce se smí použít pouze jednou pro danou adresu!!! Dále je důležité tuto funkci použít (například ve funkci při předčasném returnu).

``` c
int *p = malloc(sizeof(int));

// Kód

free(p);
```

``` c
int x(){
	int *p = malloc(sizeof(int));

	// Kód

	if(podmínka)
		return 0; // NEZAPOMENOUT na free(p)!!!

	// Kód

	free(p);
	return 0;
}
```

### Pole na haldě

>Pokud chci dynamicky alokovat pole musím to udělat na haldě opět pomocí malloc. 

``` c
int delka = 5;
int *pole = malloc(delka * sizeof(int));

pole[delka-1] = 0;

// Kód

free(pole);
```
``` c
int x = 5;
int y = 6;
int **pole = malloc(x * sizeof(int *));

for(int i = 0; i < x; i++){
pole[i] = malloc(y * sizeof(int));
}

pole[x-1][x-2] = 0;
// Kód

free(pole);
```