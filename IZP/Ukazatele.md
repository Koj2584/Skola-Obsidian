
>Existují dva ukazatele referenční(\&) a dereferenční(\*).
>Dereferenční se používá pro nastavení proměnné jako nosič adresy na paměť. Jde použít buď jako inicializace.

``` c
int *px;
```
>Nebo jako samotná paměť na kterou ukazuje.

``` c
*p = 10;
```

>Referenční se používá pro zjištění adresy paměti nějaké proměnné.

``` c
int x = 10;
int *px = &x;
```

> V knihovně je definice NULL která se doporučuje nahrávat na místo nepotřebovaných ukazatelů. Poté pokaždé zjistit zda je NULL.

``` c
int x = 10;
int *px = NULL;
if(px==NULL)
	px = &x;
else
	*px = 15; //x = 15;
``` 

>Pozor na chyby jako vytvoření ukazatele s větším datovým typem. Editor neupozorní na špatný datový typ pokud by ukazoval na menší datový typ a my jsme pomocí pointeru zapisovali větší datový typ (přepis vedlejší paměti).

``` c
int x = 10;
double *px = &x; // Nedoporučuje se

*px = 1.5; // Chyba která přepíše paměť vedle
``` 
> Při tvoření konstantního ukazatele se zapisuje takto.

``` c
int * const p; // Lze měnit, paměť na kterou ukazuje ne
const int *p; // Nelze měnit, paměť na kterou ukazuje ano
const int * const p; // Nelze měnit nic
``` 
>Existuje obecný ukazatel void \* který je třeba přetypovat pro zapisování do odkazované paměti.

``` c
int x =2;
float y = 3.1;
void *p = &x;
*(int *)p = 5;

p = &y;
*(float *)p = 2.3;
``` 
