#  Témalabor Frontend Dokumentáció

Az index.tsx fáj a router, az útvonalak vannak deklarálva itt. 
Minden routes mappában található tsx fájlhoz tartozik egy styles mappában lévő .module.css fájl.
A components mappában lévő navbar a bejelentkezés után minden oldalon szerepel. 
Ez a felcél ami tertalmazza a menüpontokat.

A root.tsx a főoldal, két opcióval: Creat Account és Login. 
A navigáláshoz a react-router-dom package-et használja.
A Create Account oldalon van 3 textbox, az email-nél figyelmezteti a felhasználót a helyes formátumra. 
A Login 2 textboxot tartalmaz, ha hibásan adnak meg valamit, figyelmeztet, hogy helytelen a megadott adat.

Bejelentkezés után a profile oldal jelenik meg a felhasználó információival, és egy Log out gombbal.
Erre visszanavigálni a fejécben található Main Menu feletti képre kattintva lehet. 
A fejlécen lehet navigálni az oldalak között. 
Az Add Project-nél új projektet vehetünk fel. A leader és members kiválasztása egy selector segítségével történik. 
A members-nél több is kiválasztható. 
A határidő datetime-local típusként adható meg. A státusz és prioritás szintén select-tel.
Az Add Task-nál taskok vehetők fel, itt meg kell adni, hogy melyik projekthez vesszük fel. 

A felvett projektek a List Project oldalon találhatók. Egy gridben, két gombbal. 
A Detalis a projekt adatait mutatja, valamint a hozzátartozó taskokat, szintén egy gridben listázva. 
A másik gomb az edit, amivel a megadott adatok szerkeszthetők, valamint törölhető is a projekt. 
Az eredeti adatok be vannak töltve és módosítani lehet őket. 
A task lista szerkesztése is hasonlóképpen történik. 

A List Members oldalon a tagok vannak kilistázva email címmel és szerepkörrele együtt. 

Eltérítés: 
A taskoknak van egy Accepted státusza, ami Declined-ra változik, ha elutasították.
A task listánál látható ez a státusz. Ha el lett utasítva a szerkesztésnél hozzáadható új taghoz. 
Ilyenkor a szerkesztés oldalon megjelenik annak a neve, aki elutasította, így neki nem lehet kiadni mégegyszer.
