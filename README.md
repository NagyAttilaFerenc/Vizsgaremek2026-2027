# Vizsgaremek 2026-2027
Készítők:
Apró Abigél, Nagy Attila Ferenc 

# 1. Projekt Áttekintése és Célkitűzése
A projekt célja egy modern, skálázható backend API kifejlesztése, amely hatékonyan kezeli és automatizáltan elosztja a közös utazások során felmerülő kiadásokat a résztvevők között.
A rendszer kulcsfontosságú tulajdonsága a napi szintű bontás és a valós idejű (real-time) adatszinkronizáció, aminek köszönhetően a csoport tagjai azonnal láthatják a módosításokat, az aktuális egyenlegeket és a pontos tartozásokat anélkül, hogy manuális számításokat kellene végezniük.

# 2. Főbb Funkciók és Üzleti Logika
Utazás és Csoportkezelés cá:

Felhasználók regisztrációja, bejelentkezése.

Utazások létrehozása egyedi időtartammal és résztvevői körrel.

Napi Kiadáskezelés:

Kiadások rögzítése adott naphoz, kategóriához és fizető személyhez kötve.

Rugalmas elosztási mechanizmusok: egyenlő arányú megosztás vagy egyedi összegek / százalékok megadása.

Kiadások valós idejű módosítása és törlése.

# 3. Valós Idejű Frissítések:

Ha valaki felvesz egy új tételt vagy módosít egy meglévő kiadást, a háttérrendszer azonnal értesíti az adott utazási szobában tartózkodó többi résztvevőt, frissítve a felületüket.

Intelligens Egyenleg-számítás és Optimalizálás:

A rendszer folyamatosan számolja a nettó egyenlegeket (ki mennyit fizetett és mennyit fogyasztott).

Az utazás végén egy optimalizáló algoritmus kiszámolja a minimális tranzakciószámot (aki tartozik, közvetlenül annak utaljon, aki pénzt követel).

# 4. A célunk
A célunk, hogy egyszerűben tudják a csoportban utazók elosztani a költségeket, mely ebben a formában felgyorsítja és leegyszerűsíti az alábbi folyamatot, melyett valós időben lehet modosítani.

# 5. Folyamatok:
Adatbázis: Relációs táblákban biztonságosan tárolja a felhasználókat, az utazásokat, a résztvevőket, a napokra bontott kiadásokat és a pontos megosztási arányokat.

Backend: REST API-kat biztosít az adatok kezeléséhez, valamint üzleti logikát futtat a kiadások elosztására és a tartozások kiszámítására.

Frontend: Egy átlátható felhasználói felületet biztosít, ahol napokra bontva láthatók a kiadások, rögzíthetők újak, és követhető az aktuális egyenleg.
