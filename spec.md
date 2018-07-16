# Fejlesztői leírás

## Technológia
* JAVASCRIPT
* HTML
* CSS

## Játéktér
* Egy div, ami magába foglalja a többi divet amelyek display: inline beállításúak.
* Méretezést egy függvénnyel oldjuk meg, majd akkor is, ha átméretezik az oldalt.
* A négyzeteket szélességét százalékosan adjuk meg.
* Egy legördülő menüből lehet kiválasztani a jatekter szelesseget.
* A "tile" osztályhoz rendeljük az egyes csempéket.
* Az eledel csempe osztálya "food", a kigyo csempe osztalya "snake" legyen, az üres csepme osztálya pedig "empty".

## Kígyó mozgása
* A "new game" gomb megnyomására a kígyó középen megjelenik.
* Azonnal indul a kígyó jobbra.
* Lépésenkénti ellenőrzés: a csempe osztályát vizsgáljuk. Ha snake az osztály, legyen vége a játéknak. Ha food, akkor nő egyet a kígyó. Ha nincs olyan csempe, ahova lepni akar a fej, akkor vége a jateknak.
* Irányítás: keydown eseményre változtatjuk az irányt. 
* Óraütésre mindig elvégezzük az ellenőrzést egy metódusban.
* A kigyo testét egy tömbben taroljuk es lepes eseten minden tömb elem az előző helyébe lép.

## Pontok és eledel
* A points változóban tároljuk az aktuális pontokat.
* Egy eledel egy pontot ér.
* Random jelenik meg egyszerre egy eledel.
* Ellenőrizni kell, hogy ne a kígyó testére essen az eledel pozíciója.
* Ha a kígyó feje rálép az eledelre, akkor növeljük a pontokat és átállítjuk az osztályokat.
* Az eledel elfogyasztása után újat generálunk.