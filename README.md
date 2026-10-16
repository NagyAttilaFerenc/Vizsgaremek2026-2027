# Vizsgaremek 2026-2027
Készítők:
Apró Abigél, Nagy Attila Ferenc 

# 1. Projekt Áttekintés és Célkitűzés
A projekt célja egy modern, skálázható backend API kifejlesztése, amely hatékonyan kezeli és automatizáltan elosztja a közös utazások során felmerülő kiadásokat a résztvevők között. A rendszer kulcsfontosságú tulajdonsága a napi szintű bontás és a valós idejű (real-time) adatszinkronizáció, aminek köszönhetően a csoport tagjai azonnal láthatják a módosításokat, az aktuális egyenlegeket és a pontos tartozásokat anélkül, hogy manuális számításokat kellene végezniük.

# 2. Főbb Funkciók és Üzleti Logika
Utazás és Csoportkezelés:

Felhasználók regisztrációja, bejelentkezése (JWT alapú autentikáció).

Utazások (Trips) létrehozása egyedi időtartammal és résztvevői körrel.

Napi Kiadáskezelés (Daily Expenses):

Kiadások rögzítése adott naphoz, kategóriához és fizető személyhez kötve.

Rugalmas elosztási mechanizmusok: egyenlő arányú megosztás vagy egyedi összegek / százalékok megadása.

Kiadások valós idejű módosítása és törlése.

Valós Idejű Frissítések (WebSockets / Socket.io):

Ha valaki felvesz egy új tételt vagy módosít egy meglévő kiadást, a háttérrendszer azonnal értesíti az adott utazási szobában tartózkodó többi résztvevőt, frissítve a felületüket.

Intelligens Egyenleg-számítás és Optimalizálás:

A rendszer folyamatosan számolja a nettó egyenlegeket (ki mennyit fizetett és mennyit fogyasztott).

Az utazás végén egy optimalizáló algoritmus kiszámolja a minimális tranzakciószámot (aki tartozik, közvetlenül annak utaljon, aki pénzt követel).
