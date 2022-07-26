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
<!-- Ja som jednoriadkový komentár -->
```

```xml
<!-- 
   Ja som  
   viacriadkový komentár
-->
```
### :safety_pin: Tagy - značky (Tags)
Otváracia značka (Opening tag): <>	
Uzatv8racia značka (Closing tag): </>

Rozdelenie značiek:
- **Párové (pair)**: \<dokument> \<dokument/> v html napr. \<div> \</div>, \<h1> \</h1>, \<a> \</a>, \<p> \</p>, \<video> \</video>
- **Nepárové (Unpair)**: \<dokument /> v html napr. \<br />, \<hr />, \<img />

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
3. Dokument XML musí obsahovať jediný pár značiek (skladajúci sa zo začiatočnej a koncovej značky), tzv. **koreňový element dokumentu** (root)
4. Počiatočné a koncové značky každého elementu musia byť riadne vnorené, elementy sa môžu vnárať, nie prekrývať
5. Mená elementov musia začínať písmenom alebo podčiarkovník (Môžu obsahovať číslice, pomlčky, bodky). Nesmie začínať číslom (<101-dalmantincov>) alebo neštandarnými znakmi (<*dalmantincov>)
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
9. [**Free Online XSD to XML Converter**](https://www.liquid-technologies.com/online-xsd-to-xml-converter)
10. [**Freeformatter XML Validator**](https://www.freeformatter.com/xml-validator-xsd.html)
11. [**Freeformatter XSD Generator**](https://www.freeformatter.com/xsd-generator.html)
12. [**Codebeautify XML Tree Viewe**](https://codebeautify.org/xmlviewer)
13. XML Notepad
14. XBase
15. XMetal
16. CAMed
17. Xerlin

:memo: Odporúčané doplnky do [**Notepad++**](https://notepad-plus-plus.org/downloads):
1. [**XML tools**](https://github.com/morbac/xmltools )
2. **Npp XML treview**
3. Python Script 	(kvôli emmet)
4. [**Emmet/Zen coding**](https://emmet.io/)
5. Random Values
6. Converter
7. Regex Trainer

**Cesta štandardná** pluginy Notepad++:
C:\Program Files\Notepad++\plugins
 
**Cesta** pluginy Notepad++ z **Microsoft Store**:
C:\Users\Administrator\AppData\Roaming\Notepad++\plugins

:repeat: Odporúčané doplnky do [**Visual Studio Code**](https://code.visualstudio.com/)
1. [**XML Complete Rogalmic**](https://marketplace.visualstudio.com/items?itemName=rogalmic.vscode-xml-complete)
2. [**XML Red Hat**](https://marketplace.visualstudio.com/items?itemName=redhat.vscode-xml)
3. [**Emmet/Zen coding Mithril**](https://emmet.io/)

### 📄 Dokumentácia
1. [W3C Dokumentácia XML](https://www.w3.org/TR/xml/)
2. [W3C – Špecifikácia XML](http://www.w3.org/XML/)
3. [W3C Dokumentácia XML Schema](https://www.w3.org/TR/xmlschema11-1/)
4. [XML Schema Part 1: Structures Second Edition](https://www.w3.org/TR/xml/](https://www.w3.org/TR/xmlschema-1/))
5. [XML Schema Part 2: Datatypes Second Edition](https://www.w3.org/TR/xmlschema-2/)
6. [W3C XML Schema Definition Language (XSD) 1.1 Part 1: Structures](https://www.w3.org/TR/xmlschema11-1/)
5. [W3C XML Schema Definition Language (XSD) 1.1 Part 2: Datatypes](https://www.w3.org/TR/xmlschema-2/)

### :books: Odporúčané zdroje
1. [ZVON – Všetko o XML a ako vytvoriť XML](http://www.zvon.org/) 
2. [Interval – Všetko o odkazoch](http://interval.cz/clanky/slabikar-xml-odkazy/)
3. [Kosek – Seriál o XML](http://www.kosek.cz/clanky/swn-xml/index.html)
4. [W3Schools – Tutorial XML](http://www.w3schools.com/xml/default.asp)
5. [W3Schools – Tutorial XML Schema](https://www.w3schools.com/xml/schema_intro.asp)
6. [Derek Banas – Video tutorial XML](https://www.youtube.com/watch?v=tAN-1xUsftg&list=PLBB413675AFBDC1F4)
7. [Emmet toolkit](https://emmet.io/)
8. [Tutorialspoint XML Schemas](https://www.tutorialspoint.com/xml/xml_schemas.htm#)
9. [Edutechwiki](https://edutechwiki.unige.ch/en/XML_Schema_tutorial_-_Basics)
10. [Microsoft podpora typu údajov xsd xml schema](https://support.microsoft.com/sk-sk/office/podpora-typu-údajov-xsd-xml-schema-definition-7cd3c906-9b9e-4a64-ba77-1b23dc5c771c)
11. [Google XML Document Format Style Guide](https://google.github.io/styleguide/xmlstyle.html)
12. [Global versus Local](http://www.xfront.com/GlobalVersusLocal.html#SecondDesign)
13. [Introducing Design Patterns in XML Schemas](https://www.oracle.com/technical-resources/articles/java/design-patterns.html)
14. [Balisage Paper: Four Basic Building Principles (Patterns) for XML Schemas](https://www.balisage.net/Proceedings/vol25/print/Bruggemann-Klein01/BalisageVol25-Bruggemann-Klein01.html)

### Vzorové XML elementy
```xml
<sprava></sprava>
<predmet></predmet>
<zamestnanec></zamestnanec>
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
## XML Schema desings 
🎎 Russian doll (Ruská bábika) - **Napodobňuje štruktúru XML dokumentu**, t. j. prvky v rámci iných prvkov sú **deklarované** **lokálne**.  
🍕 Salami slice (Salámový plátok) - R**ozloží dokument na jednotlivé prvky** a **poskladá** ich do **komponentov** tak, že **na ich odkazuje** (cez **ref**).  
🦯 Venetian Blind (Benátsky slepec) - Rozloží dokument na **jednotlivé** **komponenty**, ale namiesto deklarácie prvkov **vytvorí definície typu**.  

```xml
<Kniha>
        <Nazov>Harry Potter</Nazov>
        <Autor>J. K. Rowlingová</Autor>
</Kniha>
```
### 🎎 Russian doll



|      Princíp      | Russian Doll | Venetian Blind |
|:-------------------:|:-----------------------:|:-------------------------:|
| Cohesion (Súdržnosť)            | High                    | High                      |
| Coupling (Spojenie)            | Low                     | High                      |
| Reusable Components (Znovupoužitelnosť komponentov) | Low                     | High                      |
