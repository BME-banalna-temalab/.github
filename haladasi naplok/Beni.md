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