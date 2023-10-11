Csapat: Banálna \
Tag: Sőregi Larina

# 5. hét
Webalkalmazás design minta készítése. Login oldal megtervezése. Menü bar, különböző nézetek és a azokon lévő tartalom elrendezése, layoutok, gombok, textfield-ek pozíciói. A bejelentkezésnél a jelszó-hashez használandó bcrypt utánaolvasása.

# 6. hét
Adatgenerálás JASON generatorral a következő scripttel: 

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
