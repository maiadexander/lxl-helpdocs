# Hjälpdokumentation

Filerna i mappen (``docs``) utgör hjälpdokumentationen för gränssnittet. Om det i denna mapp skapas, ändras eller redigeras så kommer de ändringarna att komma in i gränssnittet.

## Förstasidan

Förstasidan redigeras i filen `index.md`.

## Egenskaper på ett avsnitt

Överst i varje dokumentationsfil finns ett par rader som definierar ett par egenskaper på dokumentet, t ex vilken kategori den tillhör och vilken titel den ska få.

    ---
    section: Sök
    title: Träfflista
    order: 1
    date: 2018-01-01
    tags:
    - search
    ---

**Section:**  
Kategori på dokumentet. Används till exempel för att lägga dokumenten bredvid varandra i menyn.  

**Title:**  
Titel på dokumentet. Används till menyn. **Används inte till rubriker i dokumentet.**  

**Order:**  
Ordning inom kategorin i menyn. Högre siffra -> Längre ner inom kategorin. Avsnitt som saknar order-attributet hamnar alltid längre ner än de som har attributet.

**Date:**  
Datum i `YYYY-MM-DD` format. Ska ej ha citationstecken. Exempel: `2018-05-23`

**Tags:**  
Etiketter på dokumentet som eventuellt skulle kunna användas till sökning. Lägg till `under arbete` för att visa en notis högs upp i dokumentet.

## Innehåll

Under egenskaperna följer sedan själva innehållet i avsnittet. Man använder sig av [markdown](https://daringfireball.net/projects/markdown/) för att strukturera rubriker, länkar, bilder etc.

### Bilder

För att bilderna ska kunna paketeras och visas korrekt, lägg bilden i mappen `img` och lägg till bilden i dokumentet med följande kod. **Obs** måste vara av formatet `.png`.

    ![Förklaring av bilden](Bildnamn.png) 