# Haladási napló minta
 
 
## 4. hét
Csapat: Banálna
Tag: Gipsz Jakab

Beszéltünk arról, hogy válasszam ki, hogy milyen design patternt szeretnék használni. A legtöbb helyen az MVVM-et ajánlották SwiftUI-hoz. Már ebben el is kezdtem írni az app-ot. Szerintem ide tényleg jobban illik, mint a VIPER.

 Dependency managernek a CocoaPods-ot választottam a Swift Package Manager helyett. Megnéztem a héten a CocoaPods használatát, ezután behúztam a Firebase függőségeket.

Volt egy kis (nagy) problémám azzal, hogy az iOS most kapott új verziót, illetve az Xcode is. A Firebase függőség még egy kicsit le van maradva, nem frissítették, emiatt nem akart fordulni a kód. A header fájlok importálásával volt a baj, mert átálltak egy másik formátumra, szerencsére sikerült végül kikapcsolni ennek a vizsgálatát és már csak egy warningot kapok buildelésnél, azt olvastam, hogy egy következő verzióban majd a Google ezt javítja.

 Létrehoztam a projektet Firebase-en, sikerült összekapcsolni az applikációval. Olvasgattam a Firebase-es autentikáció dokumentációját. Eljutottam addig, hogy lett egy View, ahol a felhasználó létre tud hozni egy fiókot és ez a fiók már Firebase-en is megjelenik. Kezeltem az előforduló hibákat regisztráció és bejelentkezés esetén.

 A SwiftUI app életciklusa más, ezért kivették az AppDelegate-et, viszont ezt muszáj volt visszahoznom a Firebase-es config miatt. Így ezzel is foglalkoztam, hogy erre milyen módszerek vannak, az Apple készített rá egy Adaptort.

 Utánanéztem annak, hogy hogyan lehet a stringeket kiszervezni, illetve több nyelven is megjeleníteni. Lefordítottam a Firebase-től visszakapott üzeneteket és az applikációnak a felületetét is.

 Készítettem egy github repositoryt is, ahol láthatod majd a kódomat: https://github.com/.……

Jelenleg 3 branch is van (master, develop, authentication_view). Úgy gondoltam, hogy a masterbe mennének a "release"-ek. Tehát minden félév végen a develop mergelve lenne bele és meg is lenne tagelve, ezzel lehetne követni, hogy az adott félévben végül mennyire jutottam. A develop-ból ágaznának ki mindig a feature branchek és amikor készen vagyok eggyel, akkor mergelném vissza a developba.

Megismertem a LinearGradient-et SwiftUI-ban, ami meg is tetszett és végül regisztrációnál ezt használtam a képernyőtervnél mutatott háttér helyett. Csatoltam egy a képet az elkészített képernyőről.
 
Beszéltünk róla, hogy 1-2 képernyőterv hiányzik. Csatoltam a kiegészítést. Mindegyik terv mellé írtam 1-2 mondatot, hogy mire használható az adott képernyő.
 
Ezen a héten már próbáltam inkább magával az alkalmazással haladni, ami szerintem így kezdetnek jól is sikerült. Sajnos az adatmodellekre nem jutott így időm, ezzel még foglalkozni fogok. Annyi jutott eszembe ezzel kapcsolatban csak, hogy kliens oldalon CoreData-ban nem hiszem, hogy bármit is tárolni kellene. Még a beállításokat is Firebase-en terveztem eltárolni, hogy másik eszköz használatánál is megmaradjanak az adatok.