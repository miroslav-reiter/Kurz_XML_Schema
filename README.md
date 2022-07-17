# Kurz XML II. XML Schema
:briefcase: Materiály z [kurzu XML Schema](https://www.it-academy.sk/kurz/xml-ii-xml-scheme/)

## 📑 Anotácia a Osnova kurzu 
Kurz je určený všetkým, ktorý sa chcú zoznámiť s **použitím** a **vytváraním schém XSD pre XML dokumenty**. Význam a využitie schém vzhľadom k rozvoju **webových služieb** neustále rastie. Na kurze sa naučíš **využívať hotové schémy** a **vytvárať vlastné**, vrátane zložitých podmienok pre **overenie správnosti obsahu XML** dokumentov.

1. História formátu popisu XML dát
2. Základy XSD
3. XML a namespace
4. Komplexné typy v XSD
5. Využitie schém

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
```xml
<?xml version="1.0" encoding="utf-8"?>
<?xml version="1.0" encoding="windows-1250"?>
```
### :speech_balloon: Komentáre XML
```xml
<!-- Ja som komentár -->
```
### :safety_pin: Tagy - značky (Tags)
Otváracia značka (Opening tag): <>	
Uzatv8racia značka (Closing tag): </>

Rozdelenie značiek:
- **Párové (pair)**: \<dokument> \<dokument/>
- **Nepárové (Unpair)**: \<dokument />

### :blue_book: Elementy (tvorí otváracia + uzatváracia značka a obsah, dajú sa vnárať do seba)
```xml
<sprava>Ahoj občan</sprava>
```
### :label: Atribúty (súčasťou otváracej značky, môže ich byť viac, nedajú sa vnárať do seba)
```xml
<bond kategoria="tajne" popis="agent">007</bond>
```
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

## :bangbang: Základné pravidlá pre správne formátovanie/štruktúrovanie/správna syntax XML (well-formed)
1. Deklarácia/prolog na prvom riadku (žiadne prázdne riadky či komentáre) - odporúčanie
2. **Každý** **element** XML musí mať **začiatočnú** aj **koncovú značku** (tag)
3. Dokument XML musí obsahovať jediný pár značiek (skladajúci sa zo začiatočnej a koncovej značky), tzv. **koreňový element dokumentu **(root)
4. Počiatočné a koncové značky každého elementu musia byť riadne vnorené, elementy sa môžu vnárať, nie prekrývať
5. Mená elementov musia začínať písmenom alebo podčiarkovník (Môžu obsahovať číslice, pomlčky, bodky)
6. Zohľadňujú sa veľkosť písmen (XML a XML Scheme je case sensitive - záleží na velkosti písmen)
7. Žiadne slovo XML alebo jeho kombinácie v názvoch elementov
8. Atribúty nemôžu obsahovať viaceré hodnoty (elementy môžu)
9. **Atribúty** **musia** byť **uzavreté** v **úvodzovkách** resp. apostrofoch
10. Viaceré atribúty v jednom elemente oddelené medzerou

## :hammer_and_wrench: Nástroje na XML a XSD
1. [**Notepad++**](https://notepad-plus-plus.org/downloads/)
2. [**Netbeans**](https://netbeans.apache.org/download/index.html)
3. [**Visual Studio Code**](https://code.visualstudio.com/)
4. Microsoft Visual Studio
5. [**Altova XMLSpy**](https://www.altova.com/xmlspy-xml-editor/download#)
6. [**Online XSD to XML generator**](http://xsd2xml.com/)
7. [**Visual XSD**](http://visualxsd.com/)
8. [**Free Online XML to XSD Converter**](https://www.liquid-technologies.com/online-xml-to-xsd-converter)
9. XML Notepad
10. XBase
11. XMetal
12. CAMed
13. Xerlin

:memo: Odporúčané doplnky do [**Notepad++**](https://notepad-plus-plus.org/downloads):
1. **XML tools**
2. **Npp XML treview**
3. Python Script 	(kvoli emmet)
4. [**Emmet/Zen coding**](https://emmet.io/)

**Cesta štandardná** pluginy Notepad++:
C:\Program Files\Notepad++\plugins
 
**Cesta** pluginy Notepad++ z **Microsoft Store**:
C:\Users\Administrator\AppData\Roaming\Notepad++\plugins

:repeat: Odporúčané doplnky do [**Visual Studio Code**](https://code.visualstudio.com/)
1. [**XML Complete Rogalmic**](https://marketplace.visualstudio.com/items?itemName=rogalmic.vscode-xml-complete)
2. [**XML Red Hat**](https://marketplace.visualstudio.com/items?itemName=redhat.vscode-xml)
3. [**Emmet/Zen coding Mithril**](https://emmet.io/)

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

### Vzorové XML elementy
```xml
<sprava></sprava>
<karol></karol>
<laco></laco>
<dokument></dokument>
<pravidlo></pravidlo>
```
### Vnorenie (childing) XML elementov
```xml
<sprava>
   <odosielatel>Adam Sangala</odosielatel>
   <prijemca>Martin Marcin</prijemca>
   <predmet>Nauč sa XML a XML Scheme!</predmet>
   <text>Choď na tento skvelý kurz XML Schema(https://www.it-academy.sk/kurz/xml-ii-xml-scheme/). 
      Naučís s v pohodičke XMLko a schémy 👍. </text>
</sprava>
```
### Vzorové použitie Emmet/Zen coding
```xml
<!-- Multiplikácia elementu sprava (Multiply element)  -->
<!-- sprava*5 -->
<sprava></sprava>
<sprava></sprava>
<sprava></sprava>
<sprava></sprava>
<sprava></sprava>
```

