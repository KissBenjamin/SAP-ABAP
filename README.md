# SAP ABAP Gyakorlati Példák

Ez a projekt 9 különálló ABAP osztályt tartalmaz, amelyek célja **egyszerű algoritmusok, rendszeradatok és véletlenszám-generálás bemutatása** az SAP környezetben. A példák jól használhatók **ABAP nyelv tanulására, gyakorlására** vagy a **CL_ABAP_RANDOM_INT** és **SY rendszermezők** működésének megértésére.

## Tartalom

| Program neve                  | Rövid leírás                                                                                         |
|-------------------------------|------------------------------------------------------------------------------------------------------|
| **Z_RENDSZERDATUM_VEGLEGES**  | Kiírja a rendszer dátumát különböző formátumokban (YYYYMMDD, DDMMYYYY stb.).                       |
| **Z_BEJELENTKEZESI_ADATOK**   | Megjeleníti a felhasználó belépési adatait: név, dátum, idő, kliens és nyelv.                        |
| **Z_MEDIAN_VEGLEGES**         | 10 véletlenszámot generál és meghatározza a mediánt.                                                |
| **Z_MINMAX_VEGLEGES**         | 100 véletlenszámot generál, majd meghatározza a legkisebb és legnagyobb számot, valamint előfordulásukat. |
| **Z_PRIMOSZTO**               | Megkeresi egy adott szám legnagyobb prímosztóját.                                                   |
| **Z_ATLAGSZAMITAS**           | 100 véletlenszámot generál, kiszámolja és megjeleníti azok átlagát.                                 |
| **Z_SZAMSORREND**             | Számokat ír ki -5-től 5-ig és visszafelé.                                                           |
| **Z_OSZTALYOZAS**             | 5 véletlenszámot generál és osztályzatokat rendel hozzá (1=Elégtelen…5=Jeles).                      |

## Futtatás

A példák mindegyike egy ABAP osztály az `IF_OO_ADT_CLASSRUN` interfésszel, így futtatható:

1. **SAP GUI**: SE24 vagy SE80 tranzakcióval megnyitva, majd a "Teszt" opcióval.  
2. **ADT (ABAP Development Tools)**: Jobb gomb → *Run As → ABAP Application (Console)*.

Nem szükséges külön beállítás, a programok **a SAP rendszerből veszik az időt, dátumot stb.**

## Cél

A projekt célja:
- **ABAP szintaxis** és **OO koncepciók** gyakorlása (osztályok, metódusok, táblák).
- A **rendszerváltozók (SY- mezők)** használatának bemutatása.
- Véletlenszámok generálása és alapvető matematikai/statikai számítások SAP környezetben.

## Fejlesztői megjegyzések

- A véletlenszám-generálás a **CL_ABAP_RANDOM_INT** osztályra épül.  
- A programok nincsenek kötve konkrét üzleti logikához, **oktatási célra készültek**.  
- Könnyen bővíthetők további számításokkal vagy felhasználói bemenettel (*PARAMETERS*).
