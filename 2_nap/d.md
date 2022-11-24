# Feladat a "D" jelű csapattag részére

**Figyelem!** A feladatok elvégzése során megeshet, hogy valaki kiadta a push parancsot, így a helyi repóban nem a legfrissebb a tartalom. A távoli repóban történt változások "letöltéséhez" a `git pull` parancsot kell kiadni. Érdemes odafigyelni, hogy előtte az elvégzett  módosítások legyenek commitolva.

1. Az egyik csapattársad éppen most hozza létre a feladathoz tartozó repository-t (repót, tárolót). Segítsd a munkáját és add meg neki a felhasználóneved a githubon.

1. Fogadd el a meghívást, majd klónozd le a repo-t.

1. A te feladatod a **Előételek oldal** elkészítése lesz. Hozz létre ehhez egy új branchet `eloetelek` néven.

1. Hozz létre egy oldalt `eloetelek.html` néven. A fájl egy HTML5 kódolású, oldal legyen `utf-8` karakterkódolással, továbbá állítsd be a nyelvet magyarra.


    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Előételek</title>
        <link rel="stylesheet" href="./css/fini.css">
    </head>
    <body>

    </body>
    </html>
    ```

1. Az oldal címe legyen *"Előételek"*, és a böngészőfülön is ugyanez jelenjen meg!

1. Készíts commit-ot *" Előételek oldal létrehozva"* megjegyzéssel.

1. Hozz létre a tartalomnak egy `main` elemet, majd illeszd be a `forras/eloetelek.txt` fájl tartalmát az oldalba, és tördeld a minta alapján. Az oldal címe legyen *"Előételek"*, és a böngészőfülön is ugyanez jelenjen meg!

1. A címsor alá szúrd be az oldalhoz tartozó képet. A kép kapja meg a `kiemelt-kep` osztályt.

    ```html
    <img src="./img/eloetelek.jpg" alt="" class="kiemelt-kep">
    ```

1. Készíts commit-ot *"Előételek tartalommal feltöltve"* megjegyzéssel.

1. Próbáld meg a `git push` parancs kiadásával feltölteni a távoli repóba a helyi változásokat. Ha nem megy, próbáld ki a `git push --set-upstream origin eloetelek` parancsot.

    Mivel az `eloetelek` branch lokálisan lett létrehozva, ezért nem tudja, hogy a távoli repón belül ezt hova kell feltöltenie.

1. Nyisd meg a github oldalán a repót, majd keresd ki az `eloetelek` branchet, azon belül nyisd meg az `eloetelek.html` oldalt szerkesztésre az online felületen.

1. A *"Rántott sajtok"* felsoroláshoz add hozzá a *"Rántott Trappista sajt rizzsel"*  ételt.

1. Hozz létre egy commitot *"Rántott Trappista hozzáadva"* üzenettel és "A Rántott sajtok felsorolás bővítve, egy rántott Trappista sajt rizzsel" részletes leírással.

1. Folytasd az oldal módosítását a VS Code-ban. Szintén a *Rántott sajtok* felsorolásához add hozzá az *"Rántott Trappista sajt hasábburgonyával"* opciót.

1. A `git fetch` paranccsal frissítsd le a helyi repót, majd vizsgáld meg a `git status` által, hogy mi is az aktuális állapota.

1. Mivel a távoli repóban volt egy olyan commit, ami ugyanazt a sort szerkesztette, ezért az auto merge nem tudja megoldani a problémát -> conflict (kód ütközés) keletkezett, amit manuálisan kell feloldani.

1. Jelenleg a fájlokban az ütközést okozó sorok megtalálhatóak, a `git merge --abort` parancs futtatásával lehet visszaállítani a helyi repót a korábbi, helyesen működő állapotára. Utána újra ki kell adni a `git pull` parancsot, amennyiben fel szeretnénk oldani az ütközést.

1. Módosítsd úgy a fájlokat, hogy mind a két módosítást tartalmazza!

1. Add hozzá a staging area-hoz az elvégzett módosításokat, majd a `git push` parancs kiadásával töltsd fel a távoli repóba a helyi változásokat.

1. Az így elkészült `eloetelek.html` oldalt integráld a `main` branch-be a `git merge` megfelelő alkalmazásával.

1. A `git push` parancs kiadásával töltsd fel a távoli repóba a helyi változásokat. Amennyiben valaki közben push-olt, úgy neked a `git pull` paranccsal kell kezdened.

1. Nyisd meg a `main` branch-en az `index.html` oldalt és a `<nav></nav>` elemen belül helyezz el egy újabb felsorolás elemet, ami a nemrég elkészített oldalra mutat.

1. Készíts commitot *"eloetelek menüpont létrehozva"* üzenettel, majd a `git push` parancs kiadásával töltsd fel a távoli repóba a helyi változásokat.

1. Hozd létre a "Rántott finomságok" részt a főoldal tartalmi részének a végén. Szúrd be a `rantott-finomsagok.jpg` képet. A kép kapja meg a `kiemelt` class-t, végül a leírás helyén egy lorem ipsum szöveget tartalmazó bekezdést helyezz el.

    ```html
    <h2>Nap levese</h2>

    <img src="img/rantott-finomsagok.jpg" alt="" class="kiemelt">


    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quo cumque neque illo nam voluptatem quis, aperiam, alias saepe fugiat debitis, quod molestias at vero consequatur. Voluptatum, corporis porro. Facere, animi?</p>
    ```

1. Készíts commitot *"nap levese"* üzenettel, majd a `git push` parancs kiadásával töltsd fel a távoli repóba a helyi változásokat.

1. A `TODO.md` fájlban jelezd, hogy kész az oldalad, majd `add`,`commit` és `push`.

1. Nyisd meg a `main` branch-en az `italok.html` oldalt. A "Gyümölcsleves" kategóriában nem található meg a *"Eper"* leves. Bővítsd ki a listát!

1. Készíts commitot *"gyömbér hozzáadva"* üzenettel, majd a `git push` parancs kiadásával töltsd fel a távoli repóba a helyi változásokat.

1. A megrendelő új kinézetet szeretne az oldalnak. Cseréld le a CSS fájlban az alábbi színkódokat, akár a keresés-csere funkciót alkalmazva.

    |   Régi    |    Új     |
    |-----------|-----------|
    | `#386B62` | `#488DAB` |
    | `#FFFFFF` | `#68CCF7` |
    | `#6DD1BF` | `#FFFFFF` |
    | `#AB4B44` | `#2D6B86` |
    | `#EB4130` | `#004CFF` |

1. Készíts commitot *"kinézet frissítve"* üzenettel, majd a `git push` parancs kiadásával töltsd fel a távoli repóba a helyi változásokat.
