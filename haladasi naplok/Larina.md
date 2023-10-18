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
Header a webapp nevével, 4 gombbal és a csapat képével, mint logo. 
A gombok még nem reagálnak a kattintásra, csak a színe változik meg a kattintott gombnak. 
A főrészben a tagok vannak kilistázva egy ListGroup-ban: név, email és szerep.
