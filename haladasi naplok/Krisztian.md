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
