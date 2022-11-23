# ITMP Git tanfolyam

## 2. nap

### Feladatok

#### SSH kapcsolat a GitHub-hoz

1.	Hozz létre ssh kulcspárt és alakíts ki kapcsolatot a GitHub-hoz SSH segítségével a [tutorial](kiegeszitok/ssh_tutoria.pdf) alapján.

#### Petőfi

1.	Hozz létre egy repository-t (repót, tárolót) `irodalom` néven. A létrehozáskor add meg, hogy tartalmazzon `README.md` fájlt!

2.	Klónozd le a `git clone` parancs alkalmazásával ssh használatával a repót a `koltok-1` mappába.

3.	Nyisd meg a helyi gépen lévő repót.

4.	Hozz létre egy `TODO.md` fájl, benne az alábbi tartalommal. (A megfelelő markdown kód előállításhoz használhatod [az előkészített forrást](forras/todo_md_forras.txt).)

> - [x] A távoli repo klónozása.
> - [ ] Petőfi oldalának létrehozása.
> - [ ] A helyi repo felküldése a távoli repóba.
> - [ ] A távoli repo klónozása külön mappába.
> - [ ] A README.md fájlban link létrehozása a petofi.md fájlra.

5.	Hozz létre egy mappát koltok néven, benne egy petofi.md fájlt.

6.	A [minta](kiegeszitok/minta_petofi.pdf) alapján alakítsd ki a [petofi.txt](forras/petofi_md_forras.txt) felhasználásával a fájl tartalmát markdown formázások alkalmazásával. Ne felejtsd el a repóhoz adni a [képfájlt](forras/Petofi_haza_Kiskunfelegyhazan.jpg)! (Ha most nem szeretnél a markdown kóddal bajlódni, akkor használhatod [az előkészített forrást](forras/petofi_md_forras.txt))

7.	A `TODO.md` módosításával jelöld meg, hogy elvégezted a "Petőfi oldalának létrehozása" feladatot:

> - [x] Petőfi oldalának létrehozása.

8.	Add hozzá a staging area-hoz az összes módosított fájlt.

9.	Készíts commit-ot `Petőfi oldala létrehozva` megjegyzéssel.

10.	A `push` parancs kiadásával szinkronizáld a helyi változásokat a távoli repóval.

11.	Klónozd le a git clone parancs alkalmazásával repót, most a `koltok-2` mappába. A következő feladatokat ebben a mappában végezd egyéb utasításig.

12.	A `README.md` fájlban hozz létre hivatkozást a petofi.md fájlra ([lustábbak számára előkészített forrás :)](forras/link_md_forras.txt))).

13.	A `TODO.md` fájlban állíts mindent készre:

> - [x] A távoli repo klónozása.
> - [x] Petőfi oldalának létrehozása.
> - [x] A helyi repo felküldése a távoli repóba.
> - [x] A távoli repo klónozása külön mappába.
> - [x] A `README.md` fájlban link létrehozása a `petofi.md` fájlra.

14.	Készíts commit-ot `kész` megjegyzéssel.

15.	Válts vissza a `koltok-1` mappába.

16.	A `git fetch` paranccsal töltsd le a az 1-es számú helyi repóba a központi repóban található összes változást.

17.	A `git status` segítségével ellenőrizd hol is tart az 1-es számú helyi repo.

18.	A `git pull` kiadásával frissítsd az 1-es számú repot, így ha minden rendben zajlott, úgy a mind a két mappában ugyanaz lesz megtalálható.

#### Cheat Sheet

1.	Hozz létre egy új branchet `segitseg` néven, majd válaszd ki aktuális branch-nek.

2.	Hozz létre egy fájlt cheatsheet.md néven.

3.	A fájlban hozz létre leírást, hogy hogyan lehet létrehozni címsor 1-es és címsor 2-es kiemeléseket. ([lustábbak számára előkészített forrás :)](forras/cheatsheet_md_forras.txt)))

4.	Készíts commit-ot `Cheat Sheet` megjegyzéssel.

5.	A push parancs kiadásával töltsd fel a távoli repóba a helyi változásokat.

6.	Válts át a `koltok-2` mappába. a A `git pull` kiadásával frissítsd a 2-es számú repót.

#### Extra

1. Válassz egy másik költőt és készítsd el az oldalát.
