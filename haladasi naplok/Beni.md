Csapat: Banálna \
Tag: Kis Benedek M.

# 5. hét
Megbeszéltük hogy milyen legyen nagyjából az API struktúrája. Ezt Krisztián definiálta is Prismában. Miután eldöntöttük Krisztánnal hogy Nest.js lesz a backend elkezdtem utána nézni hogyan is működik. Megnéztem azt is hogy hogyan tudnám felkonfigurálni az otthoni raspberry szervert hogy ki tudja majd szolgálni a klienseket.

# 6. hét
Megcsináltam a naplózási mintákat, és a README.md-t. Tanultam a typescriptet és átnéztem hogy érdemes e nem Node.js-t használni mert a Deno elég jó alternatívának tűnik és potenciálisan egyszerűbb és gyorsabb is lehet.

# 7. hét
A héten a CI/CD vel foglalkoztam a backendben és a mobil appban. A backendnek automatikusan elindul egy build és dockerizálja majd feltölti a repo packages tárolójába. Az android appnál egy telepíthető apk-t készít belőle ami a workflow artifacts menüben van. A CI/CD-t a github actions-al oldottam meg. Még fogok dolgozni a backend működésén illetve a frontend összekapcsolásán.

# 8. hét
Sajnos az eredeti módszer ahogy generáltuk az adatokan nem volt megfelelő ezért írtam egy saját scriptet amit tudunk majd használni erre a célra typescriptben, fakenator külső package-el. A taskok beállítható hogy alapból ne legyenek emberhez rendelve. Segítettem Krisztiánnak kijavítani egy hibát az adatszerkezettel  kapcsolatban mikor implementáltam az adat sémából az entityket.

# 9. hét
Ezen a héten sikerült megcsinálnom hogy az otthoni szerveremet összekötöttem a cloudflare tunnelel és így elérhető online már a friss backend. Egyben ezzel frissítettem a dockerizációt és bevezettem a dotenv-vault-ot ami lehetővé teszi hogy csak a production fázisban lehessen elérni a titkos adatokat. Ezután elkezdtem dolgozni a frontend routingon is illetve hogy az is online legyen a szerveren és a CI/CD-vel automatikusan containerizálódjon.

## Linkek:
- [Backend](https://banalna.afkfish.com/api)
- [Frontend](https://banalna.afkfish.com/)
- [Swagger](https://banalna.afkfish.com/swagger)

# 10. hét
Ezen a héten a bacend és a frontend szerver oldali futásával foglalkoztam illetve segítettem a frontend fejlesztésében is. A szerveren mostmár a legfrissebb docker image-k futnak mint a backend ami mostmár authentikációval rendelkezik. A frontenden a sample data renderelése sikerült és a public resource fájlokat állítottam be hogy egy statikus helyről szolgálja ki a szerver.

# 11. hét
A héten a frontenddel foglalkoztam végig, megcsináltam a projek listázó képernyőt és bekötöttem az adat lekérdezéseket a backendbe is. Mostmár ha be akarunk jelentkezni akkor egy létező felhaszálóval lehet csak akinek kezeli a backend a jogait, továbbá csináltam egy alap profile page-et is. Ha nincs authentikálva a felhasználó akkor automatikusan redirectel a bejelentkező képernyőre.

# 12. hét
Most a frontendel foglalkoztam mint a projektek felrakása az adatbázisba. Devops feladatokat is csináltam. A backenden volt egy kis hiba a notes-be.

# 13. hét - 14. hét
Most is a frontenddel foglakoztunk, megcsinaltam az api muveleteket a legtobb helyen es a hibakezelest is. Megcsinaltam az uj user regisztraciot is automatikus loginnel. Tovabbi simitasok.