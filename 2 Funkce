## Listy
Copak znamenají čísla v tomto listě? Zkus se zamyslet, jak by jsi to řekl přesně.

```python
list_modulo = []
for i in range(10):
    list_modulo.append(i % 5)

print(list_modulo)
```

# Funkce
## Příklady s inty

Funkce mohou mít v Pythonu několik podob. Nejčastější je ale tato

```python
def suma(a, b):
    return a+b

prvni = int(input('prvni cislo: '))
druhe = int(input('druhe cislo: '))
vysledek = suma(prvni,druhe)
print(f'Suma cisel {prvni} a {druhe} je {vysledek}')
```

Asi je jasné, co daná funkce dělá. Funkce by mohla být napsána také takto

```python
def suma(a, b):
    c = a+b
    return c
```
Možná to vypadá trochu lépe a je to názornější. Proměnná c je výsledek nějaké operace a funkce vrací proměnnou c. V prvním případě funkce nevrací nějakou operaci "sečti dvě čísla", ale nejdřív se čísla sečtou a následně funkce vrátí výsledek. Jak by se naprogramovala funkce, která vrací zbytek po celočíselném dělení číslem 5 :pencil: ? Funkce můžeš "skládat" do sebe. Možná ti bude připadat následující kód zvláštní, ale zkus si ho spustit a uvidíš, že funguje

```python
def suma(a,b):
    return a+b

vysledek = suma(2,suma(3,5))
print(vysledek)
```
## Příklady s listy

Ne vždy musí funkce vracet nějakou hodnotu. Následující funkce přičte jedničku ke každému prvku zadaného listu.

```python
listik = [1,2,3,4]

def sum(list):
    delka_listu = len(list)
    for i in range(delka_listu):
        list[i]=list[i]+1

sum(listik,3)
print(listik)
```
Jak by vypadala funkce, která přičte ke všem sudým číslům v listu trojku a vynásobí všechna lichá čísla dvěmi :pencil: ?

## Proč chceme funkce
Spoustu věcí by se zvládlo bez nějakých složitějších funkcí. Například tyto tři funkce vypadají jednoduše a určitě fungují. Nešlo by z nich ale udělat jednu, která umožní přičíst libovolně zvolené číslo :pencil: ?

```python
def pricti_dva(a):
    return a+2

def pricti_tri(a):
    return a+3

def pricti_sedm(a):
    return a+7
```
*Bonus* - už máš všechny nástroje k tomu, aby jsi sečetl dva listy. Zkus napsat funkci, která sečte listy A a B a vrátí list C :pencil: . Pro takto krátké listy to můžeš jednoduše obejít. Dokážeš to ale napsat pro listy, které mají délku třeba 1000?

list A | list B | list C
--- | --- | ---
[2,3,5] | [3,1,7] | [5,4,12]

Copak dělá následující funkce? Bylo by možné ji nějak zobecnit?

```python
def cisilko(a):
    s = 0
    while a>1:
        s=s+a%10
        a = a // 10
    print(s)
```
