# Python
> *Kódy, které tu jsou napsané můžeš spouštět buď někde v online kompilátoru, nebo je možné si stáhnout Python do Visual Studia. Jestli budete s Pythonem pracovat víc, tak se vyplatí si nastavit Python ve Visual Studiu. Když si klikneš na Visual Studio Installer, tak ti nabídne stáhnout balíček pro podporu Pythonu*

Pythonu je narozdíl od C# docela jedno, jak se chováš ke svým proměnným. Uvidíš dál, že můžeš mít list, ve kterém jsou proměnné typu int, string, float, bool... . Má to své výhody, že u každého listu nemusíš specifikovat, co v něm má být. Problémy jsou ale s rychlostí a složitější kontrolou, co v tom listu vlastně všechno je. To samé platí i o jiných strukturách, jako například funkce, kde nemusíš zadávat typy vstupních proměnných a vlastně ani výstupních.

## If-else konstrukce

Konstrukci if-else už znáš. Jde jen o to, jak se to píše v Pythonu. Druhý případ má těch podmínek pouze trochu více.

```python
a = 3

if a > 5:
    print("Velke cislo")
else:
    print("Male cislo")
```

```python
a = 3

if a > 30:
    print("Hodne velke cislo")
elif a>20:
    print("Velke cislo")
elif a>2:
    print("Male cislo")
else:
    print("To je skoro nula, ne?")
```

Co se ale vypíše zde jinak a proč?

```python
a = 22

if a>20:
    print("Velke cislo")
if a>10:
    print("Stredne velke cislo cislo")
else:
    print("Male cislo")
```

## Funkce range

Zkusíš na několika příkladech přijít na to, co dělá funkce range a jak to souvisí s for cykly a while cykly.

```python
for i in range(7):
    print(i, end = ' ')
```
V čem je jiný následující kód?

```python
a = 3
b = 9

for i in range(a,b):
    print(i, end = ' ')
```

Toto je sice while cyklus, ale vypíše stejná čísla, jako jeden z předešlých for cyklů. Který for cyklus z těch dvou to je?

```python
k = 0
while k<7:
    print(k, end = ' ')
    k+=1
```

Dokážeš napsat while cyklus, který vypíše stejné věci jako ten zbývající for cyklus :pencil: ? Funkce range je v Pythonu důležitá, protože jinak se meze cyklů nedají stanovit, to znamená, že **nelze** psát něco podobného, jako v C#

```csharp
for (int i=1; i<=5; i++) {
    Console.WriteLine("cislo {0}", i);
}
```
Zde taky vidíš, že Python má funkci prostě funkci print, kdežto C# má metodu WriteLine, která patří do třídy Console. Proto ten rozdíl mezi funkce(parametry) a třída.metoda(parametry).

Jak by jsi vyrobil následující list pomocí while cyklu :pencil: ? Určitě budeš také potřebovat if-else konstrukci.

```python
list_nasobku = []
for i in range(0,10,3):
    list_nasobku.append(i)

print(list_nasobku)
```
Všechny dosavadní příklady byly pouze s celými čísly, ale to neznamená, že listy nefungují pro obecný typ. Copak dělá následující kód?

```python
list_psu = ["Kolie", "Dalmatin", "Kokrspanel", "Retrivr", "Vlcak"]
list_znacek = []

for i in list_psu:
    if len(i)>5:
        list_znacek.append(True)
    else:
        list_znacek.append(False)

print(list_znacek)
```
## Přepisování proměnných
Proměnné se mohou přepisovat velmi snadno. Proto mají název **proměnné**. Nebudeme se ale pouštět do toho, co všechno je proměnná, to zjistíš časem. Navíc to závisí na jazyku. (Jsou jazyky, kde se vytvoří nějaký datový typ a ten už nemůžeš v průběhu programu přepsat.)

```python
cislo = 3
listik = [2,7]

cislo = 5
listik[0]=1
```
Kdyby se proměnné *číslo* a *listík* vypsaly na terminál, co by se na terminálu objevilo za hodnoty? Také není problém testovat jednotlivé prvky listu v if-else konstrukci.

```python
listik = [2,7]
if listik[1]==6:
    print("Je to sestka")
else:
    print("Ne není")
```
