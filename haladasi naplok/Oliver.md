Csapat: Banálna \
Tag: Tepliczky Olivér

# 5. hét
Néztem android app dizájnokat, hogy a miénkhez mi lenne a megfelelő. Majd elkészítettem az applikáció UI tervét, még nem végleges, van alternatíva egy-két részhez.
# 6. hét
Létrehoztem az Android részhez egy repot. Mjd feltöltöttem abba a kiindulási android projekt kódot. És terveztem hogyan kéne megvalósítani az előző heti UI-t jetpack composeban.
# 7. hét
A múlt héten megkezdett demo bővítése és feltöltése [demo version 1](https://github.com/BME-banalna-temalab/banalna-app/commit/ac6a79112a7ce815b1b409792d3406163852b4a3), itt a generált json fájlból tölti be a membereket ([itt látható hogyan](https://github.com/BME-banalna-temalab/banalna-app/blob/main/README.md#members-preview)) amikre rányomva kiírja [Rolejukat](https://github.com/BME-banalna-temalab/banalna-app/blob/main/demo1_toast.png).
[(Current README.md part)](https://github.com/BME-banalna-temalab/banalna-app/blob/main/README.md#members-preview)
# 8. hét
A Member adatstruktúra hozzáigazítva a legújabb struktúrához, ezzel együtt új teszt adatok beolvasása megvalósítva, a membercardokat frissítettem, már [lenyithatóak](https://github.com/BME-banalna-temalab/banalna-app/raw/main/demo2.png). Ott látszik milyen projektekben és taskokban van illetve mely projekteket viszik az adott emberek.
Még egy új lenyitható résszel bővült a [membercard](https://github.com/BME-banalna-temalab/banalna-app/raw/main/demo2_2.png), amit lenyitva láthatóak leszneka  projektek melyek hozzá vannak rendelve. A projektek szintén lenyithatóak, hogy több adtaot tudjunk meg róluk valamint [kattintható is, hogy lássuk a státuszát](https://github.com/BME-banalna-temalab/banalna-app/raw/main/demo2_toast.png).
[(Current README.md part)](https://github.com/BME-banalna-temalab/banalna-app/blob/main/README.md#updatedweek8-members-preview) 
# 9. hét
A megjelnítés változtatva lett, már külön nézetben vannak a [tagok](https://github.com/BME-banalna-temalab/banalna-app/tree/main#members-preview-1) és [projektek](https://github.com/BME-banalna-temalab/banalna-app/tree/main#projects-preview). A nézetekbe felvettem topappbarokat, ahol a nézetek közötti váltásra van lehetőség a jobb felső sarokban lévő ikonos gommbal, ami a navigációs gráfnak jelez.
Már nem fájlból olvassa be az adatokat hanem a backenddel kommunikál, míg olvas [töltő ikon](https://github.com/BME-banalna-temalab/banalna-app/blob/main/demo3l.png) jelenik meg. Plusz átálltam modelview architektúrára.
# 10. hét
A különböző nézetek közötti váltás átszervezve [oldalsó navigációs menübe](https://github.com/BME-banalna-temalab/banalna-app/blob/main/demo4n.jpg), amit bal felső ikonra vagy csak simán balra húzással előhozható és új nézet felvéve amin a [Taskok](https://github.com/BME-banalna-temalab/banalna-app#tasks-preview) láthatóak. A Screen osztályok közös részének nagyobbik része egy ősbe kiszervezve. Már van [bejelentkezési képernyő](https://github.com/BME-banalna-temalab/banalna-app#login-screen), a beírt adatokat még nem veszi figyelembe, de beégetett adatokkal belehet jelentkezni, mivel csak a backendtől kapott tokennel lehet megnézni a membereket. Retrofit könyvtárt használok a token szerzéséhez és a memberek lekérdezéséhez.
