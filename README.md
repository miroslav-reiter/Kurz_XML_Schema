# Kurz XML II. XML Schema
:briefcase: Materiály z [kurzu XML Schema](https://www.it-academy.sk/kurz/xml-ii-xml-scheme/)

## :heavy_check_mark: Využitie XML a XML Schema
1. **Protokoly a webové služby (SOAP)**
2. SVG
3. RSS
4. Google služby
5. Microsoft Office a ich súbory s rozšíreniami (**x** na konci - xml):
   - doc**x**
   - ppt**x**
   - xls**x**
   - vsd**x**

## :evergreen_tree: Štruktúra XML

### :closed_book: Deklarácia/prolog XML
\<?xml version="1.0" encoding="utf-8"?>
\<?xml version="1.0" encoding="windows-1250"?>

### :speech_balloon: Komentáre XML
\<!-- Ja som komentár -->

### :safety_pin: Tagy - značky (Tags)
Otváracia značka (Opening tag): <>	
Uzatvaracia značka (Closing tag): </>

Rozdelenie značiek:
- **Párové (pair)**: \<dokument> \<dokument/>
- **Nepárové (Unpair)**: \<dokument />

### :blue_book: Elementy (tvorí otváracia + uzatváracia značka a obsah, dajú sa vnárať do seba)
\<sprava>Ahoj občan \</sprava>

### :label: Atribúty (súčasťou otváracej značky, môže ich byť viac, nedajú sa vnárať do seba)
\<bond kategoria="tajne" popis="agent">007</bond>

### :earth_africa: Znakové entity
- &lt;   \&lt;
- &gt;   \&gt;
- &amp;  \&amp;
- &quot; \&quot;
- &apos; \&apos;

**Ďalšie entity (HTML)**
- &euro; \&euro;
- &#NNN; \&NNN;
- &#064; \&064;
Ďalšie znaky z [ASCII tabuľka](https://sk.wikipedia.org/wiki/ASCII)

## :bangbang: Základné právidla pre správne formátovanie/štruktúrovanie/správna syntax XML (well-formed)
1. Deklária/prolog na prvom riadku (žiadne prázdne riadky či komentáre)
2. Každý element XML musí mať začiatočnú aj koncovú značku
3. Dokument XML musí obsahovať jediný pár značiek (skladajúci sa zo začiatočnej a koncovej značky), tzv. koreňový element dokumentu
4. Počiatočné a koncové značky každého elementu musia byť riadne vnorené, elementy sa môžu vnárať nie prekrývať
5. Mená elementov musia začínať písmenom alebo podčiarkovník (Môžu obsahovať číslice, pomlčky, bodky)
6. Zohľadňujú sa veľkosť písmen (XML je case sensitive)
7. Žiadne slovo XML, alebo jeho kombinácie v názvoch elementov
8. Atribúty nemôžu obsahovať viaceré hodnoty (elementy môžu)
9. Atribúty Musia byť uzavreté v úvodzovkách resp. apostrofoch
10. Viaceré atribúty v jednom elemente oddelené medzerou


## :hammer_and_wrench: Nástroje na XML
1. **Notepad++**
2. **Netbeans**
3. Microsoft Visual Studio
4. **Altova XMLSpy**
5. XML Notepad
6. XBase
7. XMetal
8. CAMed
9. Xerlin

:memo: Odporúčané doplnky do [**Notepad++**](https://notepad-plus-plus.org/downloads):
1. **XML tools**
2. **Npp XML treview**
3. Python Script 	(kvoli emmet)
4. [**Emmet/Zen coding**](https://emmet.io/)
 
**Cesta štandardná** pluginy Notepad++:
C:\Program Files\Notepad++\plugins
 
**Cesta** pluginy Notepad++ z **Microsoft Store**:
C:\Users\Administrator\AppData\Roaming\Notepad++\plugins

### :books: Odporúčané zdroje
1. [W3C Dokumentácia XML](https://www.w3.org/TR/xml/)
2. [W3C – Špecifikácia XML](http://www.w3.org/XML/)
3. [W3C Dokumentácia XML Schema](https://www.w3.org/TR/xmlschema11-1/)
4. [ZVON – Všetko o XML a ako vytvoriť XML](http://www.zvon.org/) 
5. [Interval – Všetko o odkazoch](http://interval.cz/clanky/slabikar-xml-odkazy/)
6. [Kosek – Seriál o XML](http://www.kosek.cz/clanky/swn-xml/index.html)
7. [W3Schools – Tutorial XML](http://www.w3schools.com/xml/default.asp)
8. [Derek Banas – Video tutorial XML](https://www.youtube.com/watch?v=tAN-1xUsftg&list=PLBB413675AFBDC1F4)
9. [Emmet toolkit](https://emmet.io/)

**Vzorové XML elementy**:
\<sprava></sprava>
\<karol></karol>
\<laco></laco>
\<dokument></dokument>
\<pravidlo></pravidlo>

\<sprava>
\<odosielatel>Adam Sangala</odosielatel>
\<prijemca>Martin Marcin</prijemca>
\<predmet>Nauč sa XML a XML Scheme!</predmet>
\<text>Choď na tento skvelý [kurz XML Schema](https://www.it-academy.sk/kurz/xml-ii-xml-scheme/). Naučís s v pohodičke XMLko a schémy :thumbsup:. </text>
\</sprava>

**Vzorové použitie Emmet/Zen coding**
\<!-- Multiplikácia elementu sprava (Multiply element)  -->
\<!-- sprava*5 -->
\<sprava></sprava>
\<sprava></sprava>
\<sprava></sprava>
\<sprava></sprava>
\<sprava></sprava>


