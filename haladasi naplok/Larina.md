Csapat: Banálna \
Tag: Sőregi Larina

# 5. hét
Webalkalmazás design minta készítése. Login oldal megtervezése. Menü bar, különböző nézetek és a azokon lévő tartalom elrendezése, layoutok, gombok, textfield-ek pozíciói. A bejelentkezésnél a jelszó-hashez használandó bcrypt utánaolvasása.

# 6. hét
Adatgenerálás JSON generatorral a következő scripttel: 

[
    '{{repeat(3000)}}',
    {
        name: '{{firstName()}}, {{surname()}}',
        email: '{{email()}}',
        role: function (tags) {
            var roles = ['ADMIN', 'LEADER', 'MEMBER'];
            return roles[tags.integer(0, roles.length - 1)];
        };
        taskId: '{{objectId()}}',
        projectId: '{{objectId()}}'
    }
]

# 7. hét
Demo frontend elkészítése a tagok kilistázásához. 
ListGroup.txt fájlban
Header a webapp nevével, 4 gombbal és a csapat képével, mint logo. 
A gombok még nem reagálnak a kattintásra, csak a színe változik meg a kattintott gombnak. 
A főrészben a tagok vannak kilistázva egy ListGroup-ban: név, email és szerep.

# 8. hét
Login screen frontend elkészítése
Login.tsx fájlban
Az oldal kettő flexbox-ból áll 3:4 arányban. 
A baloldali tartalmazza az alkalmazás nevét a balfelső sarokban, valamint egy üdvözlést középen.
Ennek háttere egy kép. Minden kép az images mappában található.
A jobboldali a login rész. 
Kettő textbox, egy az email címnek, egy a jelszónak, valamint egy gomb a bejelentkezéshez. 
Alapértelmezett szöveg bennük (placeholder) az "Email address" és a "Password".
Az emailnél text az input, a jelszónál password. 
A "Sign in" gombon az kurzor pointer típusú lesz. 
Ha hibás adatokat ad meg a felhasználó akkor az "Invalid username or password. Please try again." üzenet jelenik meg. 

# 9. hét
A fájlokat szétszedtem egy tsx és egy css fájlra. 
A projekt hozzáadása oldal váza készen van, már csak szebben el kell rendezni a textfield-eket.
A prioritás és a státusz legördülő menüből választható. A member hozzáadás is lehet így egyszerűbb lesz majd, egyelőre annál textfield van.
A routing is kész a meglévő oldalak között (list members-ig).
Van egy root, ami a kezdőoldal. Itt található két opció a Login és a Create Account.
A Login az előző héten elkészített login oldalra navigál. 
A Create Account oldal jelenleg hasonlóan néz ki, más szöveggel. 
A login oldalon az admin név és admin jelszóval tovább lehet lépni a list members oldalra. 

# 10. hét
Add Project oldalt elkészítettem
Az összes css fájlt átírtam .module-ra, ezért a className-et a tsx fájlokban is át kellett írni
Megvan a navigáció minden oldal között
Két oldalhoz megcsináltam a headert és a hozzájuk tartozó css-t

# 11. hét
profile.module.css elkészítése
projekt members hozzáadása multiple selectorral
kisebb szépséghibák javítása, mint:
navbar-ban a logó alá került egy felirat
add project oldalon a gomb hover megadása
a create account oldalon egy "Username" textbox is van már

# 12. hét
navigation kijavítása, login után profile
edit gomb hozzáadása a projekt listához
edit project oldal 

# 13. hét
leader selector az add project oldalrra
edit project page létrehozása, layout, textboxok, selectorok
add task gomb a navbarra
add task oldal elkészítése
a tasknál egy projekt hozzárendeléséhez selector
list projectnél details funkció, új oldalon a projekt részletei 

# 14. hét
details oldalra a tasok listája
edit task oldal elkészítése
a taskok listájához az eltérítés hozzáadása
törlés funkció a projekthez és a taskhoz
edit task oldalra az eltérítés: declined by tagok listája 
