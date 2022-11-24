# Feladat az "A" jelű csapattag részére

**Figyelem!** A feladatok elvégzése során megeshet, hogy valaki kiadta a push parancsot, így a helyi repóban nem a legfrissebb a tartalom. A távoli repóban történt változások "letöltéséhez" a `git pull` parancsot kell kiadni. Érdemes odafigyelni, hogy előtte az elvégzett  módosítások legyenek commitolva.

A forrás fájlokat a `forras_2_resz` mappában találod.

1. Gratulálok! Te nyerted el a repository (repó, tároló) létrehozását a GitHub-on. Hozz létre egyet `fini-etterem` néven. A létrehozásánál állítsd be, hogy legyen privát és tartalmazzon egy `README.md` fájlt.

1. Oszd meg a csapattársaiddal! A repo oldalán kattints a **Settings** (beállítások) gombra, majd a bal oldali menüben keresd meg a **Collaborators** (együttműködők) menüpontot. Itt kérheti a fiókod jelszavát. A megadása után az **Add people** (Személyek hozzáadása) gombra kattintva keress rá a csapatod tagjainak a nevére, vagy e-mail címére. A felajánlott nevek közül válaszd ki a megfelelő felhasználót. A tényleges hozzáadás az "Add XXXX to this repository" (XXXX hozzáadása ehhez a tárolóhoz) gombra kattinta történik meg.

1. Klónozd le a repo-t a saját gépedre és a továbbiakban a helyi repóban dolgozz.

1. Hozz létre egy oldalt `index.html` néven. A fájl egy HTML5 kódolású, oldal legyen `utf-8` karakterkódolással, továbbá állítsd be a nyelvet magyarra.

    ```html
    <!DOCTYPE html>
    <html lang="hu">
    <head>
        <meta charset="UTF-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Document</title>
    </head>
    <body>
        
    </body>
    </html>
    ```

1. Készíts commit-ot *"Főoldal létrehozva"* megjegyzéssel.

1. Hozz létre a menünek egy `nav` elemet, míg a tartalomnak egy `main` elemet. Az oldal címe legyen *"Fini étterem"*, ahogy a böngészőfülön is ugyanez jelenjen meg!
    
1. A `nav` elemen belül hozz létre egy felsorolást, aminek egyetlen eleme van: Egy link, ami az `index.html`-re mutat, felirata: *"Főoldal"*.

    ```html
    <nav>
        <ul>
            <li><a href="./index.html">Főoldal</a></li>
        </ul>
    </nav>
    <main>
        <h1>Fini étterem</h1>

        <p>Üdvözöljük az étterem oldalán</p>
    </main>
    ```

1. Készíts commit-ot *"Főoldal tartalommal feltöltve"* megjegyzéssel.

1. A projekt gyökerében hozz létre egy `css` mappát, majd másold bele a [fini.css](forras_2_resz/fini.css) fájlt. Kösd is össze a HTML és CSS fájlt.

    ```html
    <link rel="stylesheet" href="./css/fini.css">
    ```

1. Készíts commit-ot *"CSS hozzáadva"* megjegyzéssel.

1. Próbáld meg a `git push` parancs kiadásával feltölteni a távoli repóba a helyi változásokat.

1. Hozz létre egy új branchet `todo` néven. Ezen az ágon hozz létre egy fájlt `TODO.md` néven, töltsd fel az alábbi feladatokkal:

    ```md
    - [x] Repository létrehozása a GitHubon.
    - [x] Főoldal létrehozása
    - [x] CSS hozzáadása
    ```

1. Próbáld meg a `git push` parancs kiadásával feltölteni a távoli repóba a helyi változásokat. 

A sikertelen próbálkozásnak az az oka, hogy a `todo` branch lokálisan lett létrehozva, a git így nem tujda a távoli repón belül ezt hova kell feltöltenie.

Próbáld ki a `git push --set-upstream origin todo` parancsot.

1. Nyisd meg a github oldalán a repót, majd keresd ki a `todo` branchet, azon belül nyisd meg a `TODO.md` fájlt szerkesztésre az online felületen. Bővítsd ki a feladatlistát az italok oldal elkészítésének feladatával.

    ```
    - [ ] Italok oldal elkészítése
    ```

1. Hozz létre egy commitot "todo italok" hozzáadva üzenettel és "A TODO listához az italok oldal elkészítése hozzáadva" részletes leírással.

1. Folytasd az oldal módosítását a VS Code-ban. Adj hozzá további feladatokat.

    ```
    - [ ] Italok oldal elkészítése
    - [ ] Előételek oldal elkészítése
    - [ ] Levesek oldal elkészítése
    ```

1. A `git fetch` paranccsal frissítsd le a helyi repót, majd vizsgált meg a `git status` által mi is az aktuális állapota.

1. Mivel a távoli repóban volt egy olyan commit, ami ugyanazt a sort szerkesztette, így az auto merge nem tudja megoldani a problémát, conflict (kód ütközés) keletkezett, amit manuálisan kell feloldani.

1. Jelenleg a fájlokban az ütközést okozó sorok megtalálhatóak, a `git merge --abort` parancs futtatásával lehet visszaállni a helyi repót a korábbi, helyesen működő állapotára. Utána újra ki kell adni a `git pull` parancsot, ha szeretnénk feloldani az ütközést.

1. Módosítsd úgy a fájlokat, hogy mind a két módosítást tartalmazza.

1. Az így elkészült `README.md` oldalt integráltd a `main` branch-be a `git merge` megfelelő alkalmazásával.

1. A `git push` parancs kiadásával töltsd fel a távoli repóba a helyi változásokat. Amennyiben valaki közben push-olt, úgy neked a `git pull` paranccsal kell kezdened.

1. Nyisd meg a `main` branch-en az `italok.html` oldalt. A "szénsavas" kategóriában nem található meg' a *"Narancs (cukormentes)"* ital. Bővítsd ki a listát!

1. Készíts commitot *"cukormentes narancs hozzáadva"* üzenettel, majd a `git push` parancs kiadásával töltsd fel a távoli repóba a helyi változásokat.

1. Remélhetőleg a töbieknek már sikerült a többi menüpontot is hozzáadni a navigációs sávhoz.
Hozz létre egy új branchet `menu` néven. Másold át a főoldalról a menü teljes tartalmát úgy ahogy van az összes oldalra.

1. Készíts commitot *"menü hozzáadva az ololdalakhoz"* üzenettel, majd pushold fel a távoli repóba a változásokat.
