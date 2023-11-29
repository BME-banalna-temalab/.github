Csapat: Banálna \
Tag: Dancs Krisztián

# 5. hét
Prisma sémát definiáltam, és Benivel generáltuk a fontosabb resourceokat mint például member, task, project.

# 6. hét
Elkezdtem az alapvető crud műveleteket implementálni, DTO-kat hoztam létre ahol szükséges volt és próbálkoztam a swagger kisebb nagyobb sikeres bekötésével.

# 7. hét
Generáltam a többi entityhez is adatokat. Megcsináltam a tasknak is a crud műveleteit, nem nagyon működik most a backend, mivel refactoráltam a múlt heti kódot, hogy many to many relationship legyen. Ennek hatására a members findMany metódus most nem nagyon megy.

# 8. hét
Főleg bug fixeket csináltam a héten, egy két adatmódosítás is volt mivel nem volt teljesen helyes a séma. Befejeztem a basic CRUD endpointokat az entityknek (member, task, project), jelenleg Date validáció problémákba ütköztem. Ezen felül, a member update endpointját átalakítottam, mostmár Query-vel lehet assignolni az adott membert taskhoz vagy projekthez.

# 9. hét
Implementáltam authentikációt illetve authorizációt a backendre. A Memberhez hozzáadtam egy password mezőt, ahol hashelve tároljuk a jelszavakat (a generált adatokban még nem ez van, de ha létrehozunk egyet vagy updatelünk egyet akkor hashelve lesz).

# 10. hét
Ezen a héten is főleg fixelgettem a dolgokat, mostmár a legtöbb endpointon ahol szükséges van authorizáció illetve authentikáció. Hozzáadtam a DTO validációhoz egy ValidationPipe-ot, mostmár csak a DTO-nak megfelelő adatokat engedi át, ez eddig egy hiba volt.

# 11. hét
Az eltérítéssel foglalkoztam és csináltam neki új endpointot, sémaváltoztatás stb.

# 12. hét
Főleg az eltérítésen elmélkedtem és próbáltam jó megoldást találni, hibát dob ha már foglalt stb.

# 13. hét
Bugfixek, végső simítások, még hátravan pár apró dolog, hogy tökéletes legyen.
