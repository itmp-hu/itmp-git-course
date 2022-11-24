# Feladat az "C" jelű csapattag részére

**Figyelem!** A feladatok elvégzése során megeshet, hogy valaki kiadta a push parancsot, így a helyi repóban nem a legfrissebb a tartalom. A távoli repóban történt változások "letöltéséhez" a `git pull` parancsot kell kiadni. Érdemes odafigyelni, hogy előtte az elvégzett  módosítások legyenek commitolva.

A forrás fájlokat a `forras_2_resz` mappában találod.

1. Az egyik csapattársad éppen most hozta létre a feladathoz tartozó repository-t (repót, tárolót). Segítsd a munkáját és add meg neki a felhasználóneved a githubon.

1. Ha megkaptad a meghívót, fogadd el a meghívást, majd klónozd le a repo-t.

1. A te feladatod a **Levesek oldal** elkészítése lesz. Hozz létre ehhez egy új branchet `levesek` néven.

1. Hozz létre egy oldalt `levesek.html` néven. A fájl egy HTML5 kódolású, oldal legyen `utf-8` karakterkódolással, továbbá állítsd be a nyelvet magyarra.  Az oldal címe legyen *"Levesek"*, ahogy a böngészőfülön is ugyanez jelenjen meg!

    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Levesek</title>
        <link rel="stylesheet" href="./css/fini.css">
    </head>
    <body>

    </body>
    </html>
    ```

1. Készíts commit-ot *" Italok oldal létrehozva"* megjegyzéssel.

1. Hozz létre a tartalomnak egy `main` elemet, majd illeszd be a [levesek.txt](forras_2_resz/levesek.txt) fájl tartalmát az oldalba, és tördeld a [minta](kiegeszitok/levesek_html_minta.png) alapján. ([Lustábbak számára előkészített forrás :)](forras_2_resz/levesek_html_forras.txt).)

1. A címsor alá szúrd be az oldalhoz tartozó képet. A kép kapja meg a `kiemelt-kep` osztályt.

    ```html
    <img src="./img/levesek.jpg" alt="" class="kiemelt-kep">
    ```

1. Készíts commit-ot *"Italok tartalommal feltöltve"* megjegyzéssel.

1. Próbáld meg a `git push` parancs kiadásával feltölteni a távoli repóba a helyi változásokat. 

    A sikertelen próbálkozásnak az az oka, hogy a `levesek` branch lokálisan lett létrehozva, a git így nem tujda a távoli repón belül ezt hova kell feltöltenie.

    Próbáld ki a `git push --set-upstream origin levesek` parancsot.

1. Nyissa meg a github oldalán a repót, majd keresse ki a `levesek` branchet, azon belül nyissa meg a `levesek.html` oldalt szerkesztésre az online felületen.

1. A *"Kiemelt leveseink"* felsoroláshoz add hozzá az *"Húsleves májgombóccal"* levest.

1. Hozzon létre egy commitot *"Húsleves hozzáadva"* üzenettel és "A kiemelt levesek felsorolása bővítve egy Húsleves májgombóccal opcióval" részletes leírással.

1. Folytasd az oldal módosítását a VS Code-ban. Szintén a *"Kiemelt leveseink"* felsorolásához add hozzá az *"Jókai bableves"* opciót.

1. A `git fetch` paranccsal frissítsd le a helyi repót, majd vizsgált meg a `git status` által mi is az aktuális állapota.

1. Mivel a távoli repóban volt egy olyan commit, ami ugyanazt a sort szerkesztette, így az auto merge nem tudja megoldani a problémát, conflict (kód ütközés) keletkezett, amit manuálisan kell feloldani.

1. Jelenleg a fájlokban az ütközést okozó sorok megtalálhatóak, a `git merge --abort` parancs futtatásával lehet visszaállni a helyi repót a korábbi, helyesen működő állapotára. Utána újra ki kell adni a `git pull` parancsot, ha szeretnénk feloldani az ütközést.

1. Módosítsd úgy a fájlokat, hogy mind a két módosítást tartalmazza.

1. Add hozzá a staging area-hoz az elvégzett módosításokat, majd a `git push` parancs kiadásával töltsd fel a távoli repóba a helyi változásokat.

1. Az így elkészült `levesek.html` oldalt integráltd a `main` branch-be a `git merge` megfelelő alkalmazásával.

1. A `git push` parancs kiadásával töltsd fel a távoli repóba a helyi változásokat. Amennyiben valaki közben push-olt, úgy neked a `git pull` paranccsal kell kezdened.

1. Nyisd meg a `main` branch-en az `index.html` oldalt és a `<nav></nav>` elemen belül helyezz el egy újabb felsorolás elemet, ami a nemrég elkészített oldalra mutat.

1. Készíts commitot *"levesek menüpont létrehozva"* üzenettel, majd a `git push` parancs kiadásával töltsd fel a távoli repóba a helyi változásokat.

1. Hozz létre a "Nap itala" részt a főoldal tartalmi részének a végén. Szúrd be a `nap-levese.jpg` képet. A kép kapja meg a `kiemelt` class-t, végül a leírás helyén egy lorem ipsum szöveget tartalmazó bekezdés helyezzen el.

    ```html
    <h2>Nap levese</h2>

    <img src="img/nap-levese.jpg" alt="" class="kiemelt">


    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quo cumque neque illo nam voluptatem quis, aperiam, alias saepe fugiat debitis, quod molestias at vero consequatur. Voluptatum, corporis porro. Facere, animi?</p>
    ```

1. Készíts commitot *"nap levese"* üzenettel, majd a `git push` parancs kiadásával töltsd fel a távoli repóba a helyi változásokat.

1. A `TODO.md` fájlban jelezd, hogy kész az oldalad, majd `add`,`commit` és `push`.

1. Nyisd meg a `main` branch-en az `italok.html` oldalt. A "Szénsavas" kategóriában nem található meg a *"Gyömbér"* ital. Bővítsd ki a listát!

1. Készíts commitot *"gyömbér hozzáadva"* üzenettel, majd a `git push` parancs kiadásával töltsd fel a távoli repóba a helyi változásokat.

1. A megrendelő új kinézetet szeretne az oldalnak. Cserélje le a CSS fájlban az alábbi színkódokat, akár a keresés-csere funkciót alklamazva.

    |   Régi    |    Új     |
    |-----------|-----------|
    | `#386B62` | `#488DAB` |
    | `#FFFFFF` | `#68CCF7` |
    | `#6DD1BF` | `#FFFFFF` |
    | `#AB4B44` | `#2D6B86` |
    | `#EB4130` | `#004CFF` |

1. Készíts commitot *"kinézet frissítve"* üzenettel, majd a `git push` parancs kiadásával töltsd fel a távoli repóba a helyi változásokat.