# Responzivní menu
Menu je vytvořeno ve 3 variantách:
- menu, kde se jednotlivé itemy na desktopu poskládají vedle sebe a na mobilu se poskládají pod sebe
- menu, kde se jednotlivé itemy na desktopu poskládají vedle sebe a na mobilu zmizí a místo nich se obejví jen lišta s ikonkou
- menu, které funguje jako předchozí, ale na při kliknutí na hamburger ikonku se otevře a zavře (spíš ro zajímavost)

použité technologie: media query

### cíle
- zopakovat základní html syntaxi
- zopakovat odkazy
- ukázat využití media query
- umístit menu do exitující stránky (tzn. procvičit odkazy s id)
- pro zájemce ukázat javascript

### Postup

#### Menu, které se mění z vedle sebe na pod sebou (a naopak)
1. začít nejdřív samotnou kostrou html souboru (tzn. vytvořit strukturu nav a pod tím odkazy (obalené odkazy))
2. trochu to nastylovat - žákům nutno ukázat display: flex a display: block
3. dodat media query

#### Menu, které na mobilu zmizí a poté se mu ukáže ikonka
1. zkopírovat si strukturu z prvního menu
2. přidat tam ikonku + nastylovat ikonku
3. změnit media query pro jednotlivé odkazy (dát tam display: none)
4. přidat mizení a objevování ikonky podle media query


#### Menu, které se umí zavírat a otvírat
- je myšleno pouze jako zajímovast pro ty, kteří už toho umí víc (není myšleno na rozebírání na hodině)

### Na závěr
- implementace menu do dlouhé stránky
- zkopírovat vybrané menu do stránky a změnit jeho popisky a odkazy podle toho, kam má který odkazovat (s využitím id)