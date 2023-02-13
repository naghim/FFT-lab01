# Labor 01

A tantárgy keretén belül, objektum orientált módon felépített grafikus felületű, egy-, illetve többablakos, több rétegű, eseményvezérelt alkalmazások készítésével fogunk foglalkozni. Azzal is megismerkedünk, hogy milyen elvek szerint tervezzük és vitelezzük ki ezeket a felületeket. 

Az [eseményvezérelt programozásban](https://wiki.prog.hu/wiki/Eseményvezérelt_programozás)  a program egyes részei, ágai nem szekvenciális és előre meghatározható sorrendben futnak le, hanem a vezérlés lefutását bizonyos külső, illetve belső események határozzák meg. A program egésze nem más, mint események bekövetkezésére válaszul végrehajtott szubrutinok (ún. eseménykezelők) laza halmaza, amelyek nagyrészt egymástól függetlenül dolgoznak és működtetik a program egészét. 

Az eseményvezérelt modellben külső események alatt tipikusan a felhasználói bevitelt (billentyű lenyomása, egérművelet), valamint a hardvertől származó eseményeket (pl. az időzítőáramkor vagy periférfia által kiváltott megszakítás, visszahívás) szokás érteni, míg a belső eseményeket a program más részeitől - vagy akár más programoktól - származó üzenetek képezik. 

Az eseményvezérelt programok egyetlen szekvenciális részeit a program az események begyűjtését és szétosztását (dispatch) végző főciklusa, valamint az egyes eseményeket kezelő szubrutinok képezik, amelyek azonban maguk is válhatnak további események kiváltójává és forrásává.

Eseményvezérelt program szinte bármilyen programozási nyelvben készíthető, mi C++-t és Qt-t fogunk tanulni és használni. A Qt egy többplatformos (nemcsak asztali, de akár mobil vagy beágyazott alkalmazások is fejleszthetők) alkalmazás-fejlesztési keretrendszer, amely egy komplett osztálykönyvtárat biztosít számos platformon történő alkalmazás-fejlesztésre elsősorban C++-ban. Jelmondatai: "One framework. One codebase. Any platform." és "Code less. Create more. Deploy everywhere.".

Az első laboron, az ingyenes Qt Creator - Open Source Qt Use ([letöltés](https://www.qt.io/download-open-source)) Integrált fejlesztői környezettel fogunk megismerkedni. Ennek a kézikönyve [itt](https://doc.qt.io/qtcreator/index.html) böngészhető.


# Feladatok

1. Milyen [típusú projekteket](https://doc.qt.io/qtcreator/creator-project-creating.html) lehet létrehozni?

2. Hozzunk létre egy egyszerű C++ projektet és implementáljuk egy `Mátrix` osztályt mely támogatja a mátrixszorzás műveletet. A projekt adatai hol és milyen formában vannak tárolva? Mi a projekt adatokat tartalmazó fájl neve, kiterjesztése, formátuma? Hogyan [kompilálható és futtatható]((https://doc.qt.io/qtcreator/creator-building-targets.html)) a projekt? 

3. Hozzunk létre egy [Qt Console Application](http://www.science.smith.edu/dftwiki/index.php/Qt5/Qt-Creator_%22Hello_World%22_Console_Application) típusú projektet, mely futtatáskor kiírja az aktuális dátumot és pontos időt. Használjuk a [`QDate`](https://doc.qt.io/qt-5/qdatetime.html) osztályt. Miben különbözik ez a projekt a sima C++ projektől?

4. A prímszámok megtalálására egy adott határértékig, implementáljuk [Eratoszthenész szitáját](https://hu.wikipedia.org/wiki/Eratoszthenész_szitája). Futtassuk a projektet lépésről lépésre, [hibakereső módban](https://doc.qt.io/qtcreator/creator-debugging.html). Hogyan tudunk tőréspontokat (breakpoint) definiálni?  Hogyan tudjuk az [egyes változók értékét megfigyelni](https://doc.qt.io/qtcreator/creator-debug-mode.html)?

![](https://doc.qt.io/qtcreator/images/qtcreator-debugger-views.png)

Ábra 1. Hibakeresés ([debugging](https://en.wikipedia.org/wiki/Debugging)) Qt-ben, illusztráció.

