# Praktický úkol - Produktová karta

![images](https://imgtr.ee/images/2023/09/09/8ce2c9b5c0c9b4ba14b97ec7a4071cb6.png)

# 1. Vytvoření souboru index.html a základni struktúry HTML

- vytvořte soubor **index.html**
- základní struktúru HTML vytvoříme napsánim znaku ! a následním stisknutím ENTER na klávesnici
- základni struktúra HTML vypadá následovně:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>
  <body></body>
</html>
```

# 2. Přidáni obsahu

- skopírujte nasledující text a vložte ho do souboru index.html mezi html tag `<body></body>`

Bestseller
-50%
Kvalitní Pánská Sportovní Bota Nike METCON 2
Tato pánská sportovní bota je dokonalým spojením komfortu a stylu. Vyrobena z vysoce kvalitního materiálu, nabízí optimální oporu a pohodlí pro vaše nohy...
Více info
Doprava zdarma
Skladem 4 kusy
Cena produktu
2799 Kč
1100 Kč
Přidat do košíku

# 3. Vytvoření souboru styles.css

- vytvořite soubor s názvem **styles.css**
- přelinkujte soubor index.html se souborem styles.css vložením nasledujíciho kusu kódu do hlavičky html souboru

```html
<link rel="stylesheet" href="style.css" />
```

- výsledek vypadá následovně:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    Text s kterým budeme pracovat
  </body>
</html>
```

# 4. Přidani třid

- vytvořte blokový element `<div></div>` s třídou `product-card` do které vložíme text. Tento element bude sloužit jako obálka pro kartu.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <div class="product-card">
      Bestseller -50% Kvalitní Pánská Sportovní Bota Nike METCON 2 Tato pánská
      sportovní bota je dokonalým spojením komfortu a stylu. Vyrobena z vysoce
      kvalitního materiálu, nabízí optimální oporu a pohodlí pro vaše nohy...
      Více info Doprava zdarma Skladem 4 kusy Cena produktu 2799 Kč 1100 Kč
      Přidat do košíku
    </div>
  </body>
</html>
```

- Do souboru **styles.css** napíšeme selector `body`.

```css
body {
}
```

- V prvním kroku obalte elementy třídou a pridejte selektor třídy do css souboru. Postupujte podle příkladu níže.

> Bestseller

```html
<span class="bestseller-badge">Bestseller</span>
```

```css
.bestseller-badge {
}
```

> -50%

```html
<span class="discount-badge">-50%</span>
```

```css
.discount-badge {
}
```

> Kvalitní Pánská Sportovní Bota Nike METCON 2

```html
<h1 class="product-title">Kvalitní Pánská Sportovní Bota Nike METCON 2</h1>
```

```css
.product-title {
}
```

> Tato pánská sportovní bota je dokonalým spojením komfortu a stylu. Vyrobena z
> vysoce kvalitního materiálu, nabízí optimální oporu a pohodlí pro vaše nohy...

```html
<p class="product-description">
  Tato pánská sportovní bota je dokonalým spojením komfortu a stylu. Vyrobena z
  vysoce kvalitního materiálu, nabízí optimální oporu a pohodlí pro vaše nohy...
</p>
```

```css
.product-description {
}
```

> Více info

```html
<span class="product-more-info">Více info</span>
```

```css
.product-more-info {
}
```

> Doprava zdarma

```html
<span class="product-shipping-label">Doprava zdarma</span>
```

```css
.product-shipping-label {
}
```

> Skladem 4 kusy

```html
<span class="product-stock-label">Skladem 4 kusy</span>
```

```css
.product-stock-label {
}
```

> Cena produktu

```html
<span class="product-price-label">Cena produktu</span>
```

```css
.product-price-label {
}
```

> 2799 Kč

```html
<span class="product-price">2799 Kč</span>
```

```css
.product-price {
}
```

> 1100 Kč

```html
<span class="product-discount-price">1100 Kč</span>
```

```css
.product-discount-price {
}
```

> Přidat do košíku

```html
<span class="add-to-cart-button">Přidat do košíku</span>
```

```css
.add-to-cart-button {
}
```

# 5. Nastavení barev

V této sekci nastavíme barvu jednotlivým elementom podle obrázku karty.

Nastavte barvu pozadí celému dokumentu. Selektoru `body` přidáte vlastnost `background-color` s hodnotou `#ecebeb` nebo `rgb(236, 235, 235)`. Jedná se o stejnou barvu s rozdílnym zápisem.

```css
body {
  background-color: #ecebeb;
}
```

Nastavte barvu pro jednotlive sekce nasledovně:

```css
.bestseller-badge {
  background-color: #fffa87;
  color: #413e01;
}
```

```css
.discount-badge {
  background-color: #ee1212;
  color: #fff;
}
```

```css
.product-more-info {
  color: #808080;
}
```

```css
.product-shipping-label {
  color: #ee1212;
}
```

```css
.product-stock-label {
  color: #3b990f;
}
```

```css
.product-price {
  color: #808080;
}
```

```css
.add-to-cart-button {
  background-color: #ee1212;
  color: #fff;
}
```

# 6. Vytvoření proměnných

- Z použitých barev vytvořte proměnné.

```css
:root {
  --product-white: #fff;
  --product-red: #ee1212;
  --product-green: #3b990f;
  --product-gray: #808080;
  --product-brown: #413e01;
  --product-yellow: #fffa87;
  --background-gray: #ecebeb;
}
```

- Nahradte barvy proměnnými.

```css
.bestseller-badge {
  background-color: var(--product-yellow);
  color: var(--product-brown);
}
```

```css
.discount-badge {
  background-color: var(--product-red);
  color: var(--product-white);
}
```

```css
.product-more-info {
  color: var(--product-gray);
}
```

```css
.product-shipping-label {
  color: var(--product-red);
}
```

```css
.product-stock-label {
  color: var(--product-green);
}
```

```css
.product-price {
  color: var(--product-gray);
}
```

```css
.add-to-cart-button {
  background-color: var(--product-red);
  color: var(--product-white);
}
```

# 7. Zarovnání textu

Některé inline elementy obalte do blokových elementov aby zabírali cely řádek. Vytvořte třídu pro blokový element a doplntě třídu selektora do styles.css. Následne nastavte zarovnání textu pomocí vlasnosti `text-align` na novovzniknuté tříde.

> Více info

```html
<div class="product-info-container">
  <span class="product-more-info">Více info</span>
</div>
```

```css
.product-info-container {
  text-align: center;
}
```

- Defaultni zarovnani elementu je na levo, proto nemusíte nastavovat zarovnáni `text-align: left`. Pro učel procvičení je tato hodnota zapísana.
  > Cena produktu

```html
<div class="product-price-label-container">
  <span class="product-price-label">Cena produktu</span>
</div>
```

```css
.product-price-label-container {
  text-align: left;
}
```

> 2799 Kč

```html
<div class="product-price-container">
  <span class="product-price">2799 Kč</span>
</div>
```

```css
.product-price-container {
  text-align: left;
}
```

> 1100 Kč

```html
<div class="product-discount-price-container">
  <span class="product-discount-price">1100 Kč</span>
</div>
```

```css
.product-discount-price-container {
  text-align: left;
}
```

# 8. Styl písma

- Nastavte tříde `product-more-info` styl písma italic pomocí vlasnosti `font-style: italic`.

```css
.product-more-info {
  color: var(--product-gray);
  font-style: italic;
}
```

# 9. Tučnost písma

- Nastavte vybraným textom tučne písmo.

```css
.bestseller-badge {
  background-color: var(--product-yellow);
  color: var(--product-brown);
  font-weight: bold;
}

.discount-badge {
  background-color: var(--product-red);
  color: var(--product-white);
  font-weight: bold;
}

.product-shipping-label {
  color: var(--product-red);
  font-weight: bold;
}

.product-stock-label {
  color: var(--product-green);
  font-weight: bold;
}

.product-price-label {
  font-weight: bold;
}

.product-discount-price-container {
  text-align: left;
  font-weight: bold;
}

.add-to-cart-button {
  background-color: var(--product-red);
  color: var(--product-white);
  font-weight: bold;
}
```

# 10. Velikost textu

- Nastavte vybraným textem velkost písma.

```css
.bestseller-badge {
  background-color: var(--product-yellow);
  color: var(--product-brown);
  font-weight: bold;
  font-size: 14px;
}

.discount-badge {
  background-color: var(--product-red);
  color: var(--product-white);
  font-weight: bold;
  font-size: 20px;
}

.product-title {
  font-size: 32px;
}

.product-shipping-label {
  color: var(--product-red);
  font-weight: bold;
  font-size: 18px;
}

.product-stock-label {
  color: var(--product-green);
  font-weight: bold;
  font-size: 18px;
}

.product-discount-price {
  font-size: 28px;
}

.add-to-cart-button {
  background-color: var(--product-red);
  color: var(--product-white);
  font-weight: bold;
  font-size: 24px;
}
```

# 11. Výška řádku

- Nastavte výšku řádku pro nazev produktu pomoci vlastnosti `line-height`.

```css
.product-title {
  font-size: 32px;
  line-height: 1.5;
}
```

# 12. Podtržené písmo

- Nastavte podtržení písma pomocí vlastnosti `text-decoration: underline`.

```css
.product-more-info {
  color: var(--product-gray);
  font-style: italic;
  text-decoration: underline;
}

.product-stock-label {
  color: var(--product-green);
  font-weight: bold;
  font-size: 18px;
  text-decoration: underline;
}

.product-price {
  color: var(--product-gray);
  text-decoration: line-through;
}
```

# 13. Textové transformace

- Převedte text Doprava zdarma na velké písmena pomoci vlastnosti `text-transform`.

```css
.product-shipping-label {
  color: var(--product-red);
  font-weight: bold;
  font-size: 18px;
  text-transform: uppercase;
}
```

# 14. Rodina písma

- Nastavte rodinu písma `Inter` pomoci vlastnosti `font-family` na selektoru `body`. Nejdříve musite písmo `Inter` naimportovat a pak ho přidejte na začátek seznamu písem oddelene čárkou. Jako druhé písmo zvolte `Arial` a poslední písmo v seznamu použijte `sans-serif`.

- Import písma `Inter` vložte do hlavičky `<heade></head>` html struktúry:

```html
<link rel="preconnect" href="https://fonts.googleapis.com" />
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
<link
  href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;700&family=Roboto&display=swap"
  rel="stylesheet"
/>
```

- Přidejte rodinu písma selektoru `body`.

```css
body {
  background-color: #ecebeb;
  font-family: "Inter", Arial, sans-serif;
}
```

# 15. Výška a šířka

- Nastavte šířku produktové karty na `450px` pomocí vlastnosti `width` na tříde `product-card` a barvu pozadí na bílou.

```css
.product-card {
  width: 450px;
  background-color: var(--product-white);
}
```

# 16. Vnitřní okraje

- Pro lepší pochopení vnejších a vnitřních okraju nastavte dočasne rámeček pro vsechny elementy na stránce.

```css
div,
span,
h1,
p {
  border: 1px solid black;
}
```

- Nastavte vnitřní okraj (`padding`) `16px` na tříde `product-card`, který je blokový element.

```css
.product-card {
  width: 450px;
  background-color: var(--product-white);
  padding: 16px;
}
```

- Nastavte vnitřní okraj (`padding`) na inline elemente s třídou `bestseller-badge` s hodnotou `4px`. Pozor `span` je inline element, proto aby jsme mohli nastavit šířku, výšku, vnitřní a vnejší okraj, musíme nejdřív nastavit vlastnost `display` na hodnotu `inline-block`.

```css
.bestseller-badge {
  background-color: var(--product-yellow);
  color: var(--product-brown);
  font-weight: bold;
  font-size: 14px;
  padding: 4px;
}
```

- Nastavte vnitřní okraj pro horni a spodní stranu (`padding-top` a `padding-bottom`) na inline elemente s třídou `add-to-cart-button` s hodnotou `8px`. Pozor `span` je inline element, proto aby jsme mohli nastavit šířku, výšku, vnitřní a vnejší okraj, musíme nejdřív nastavit vlastnost `display` na hodnotu `inline-block`.

- Nastavte na stejnem elementů šířku tlačítka na 100% svého rodiče.

```css
.add-to-cart-button {
  background-color: var(--product-red);
  color: var(--product-white);
  font-weight: bold;
  font-size: 24px;
  display: inline-block;
  padding: 8px 0;
  width: 100%;
}
```

- Vycentrujte text v tlačítku pomoci vlastnost `text-align` s hodnotou `center`.

```css
.add-to-cart-button {
  background-color: var(--product-red);
  color: var(--product-white);
  font-weight: bold;
  font-size: 24px;
  display: inline-block;
  padding: 8px 0;
  width: 100%;
  text-align: center;
}
```

- Nastavte vnitřní okraj (`padding`) na inline elemente s třídou `product-shipping-label` s hodnotou `8px`. Pozor `span` je inline element, proto aby jsme mohli nastavit šířku, výšku, vnitřní a vnejší okraj, musíme nejdřív nastavit vlastnost `display` na hodnotu `inline-block`.

```css
.product-shipping-label {
  color: var(--product-red);
  font-weight: bold;
  font-size: 18px;
  text-transform: uppercase;
  display: inline-block;
  padding: 8px;
}
```

- Obalte elementy `product-shipping-label` a `product-stock-label` novým <div></div> blokovývm elementem, s třídou `product-details-container`.

```html
<div class="product-details-container">
  <span class="product-shipping-label">Doprava zdarma</span>
  <span class="product-stock-label">Skladem 4 kusy</span>
</div>
```

- Novému elementu nastavte vnitřní okraj `8px` a barvu pozadí na hodnotu `#e2dfdf`, kterou uložíte do proměnny s nazvem `--product-light-red`.

```css
.product-details-container {
  padding: 8px;
  background-color: var(--product-light-red);
}
```

# 17. Vnější okraje

- Nastavte spodní vnější okraj (`margin-bottom`) na elementu s třídou `product-info-container` na hodnotu `8px`.

```css
.product-info-container {
  text-align: center;
  margin-bottom: 8px;
}
```

- Nastavte spodní vnější okraj (`margin-bottom`) na elementu s třídou `product-details-container` na hodnotu `16px`.

```css
.product-details-container {
  padding: 8px;
  background-color: var(--product-light-red);
  margin-bottom: 16px;
}
```

- Nastavte spodní vnější okraj (`margin-bottom`) na elementu s třídou `product-price-label-container` na hodnotu `8px`.

```css
.product-price-label-container {
  text-align: left;
  margin-bottom: 8px;
}
```

- Nastavte spodní vnější okraj (`margin-bottom`) na elementu s třídou `product-price-container` na hodnotu `8px`.

```css
.product-price-container {
  text-align: left;
  margin-bottom: 8px;
}
```

- Nastavte spodní vnější okraj (`margin-bottom`) na elementu s třídou `product-discount-price-container` na hodnotu `8px`.

```css
.product-discount-price-container {
  text-align: left;
  font-weight: bold;
  margin-bottom: 8px;
}
```

- Nastavte spodní vnější okraj (`margin-bottom`) na elementu s třídou `product-description` na hodnotu `4px`.

```css
.product-description {
  margin-bottom: 4px;
}
```

- Vymažte dočasne nastavený rámeček na všech elementech.

```css
/* Odmazat */
div,
span,
h1,
p {
  border: 1px solid black;
}
```

# 18. Slučování vnějších okrajů

- elementy `h1` a `p` mají výchozí nastavení vlastnosti `margin-top` a `margin-bottom`.

```html
<h1 class="product-title">Kvalitní Pánská Sportovní Bota Nike METCON 2</h1>
<p class="product-description">
  Tato pánská sportovní bota je dokonalým spojením komfortu a stylu. Vyrobena z
  vysoce kvalitního materiálu, nabízí optimální oporu a pohodlí pro vaše nohy...
</p>
```

- V tomto případe dochází k slučování vnějších okrajů `margin-bottom` elementů `h1` a `margin-top` elementů `p`.

- Nastavte `margin-top` elementů `p` na hodnotu `0` čímž vyrešíte problém se slučováním.

```css
.product-description {
  margin-bottom: 4px;
  margin-top: 0;
}
```

- Upravte výchozí hodnotu `margin-bottom` elementů `h1` na hodnotu `4px`.

```css
.product-title {
  font-size: 32px;
  line-height: 1.5;
  margin-bottom: 4px;
}
```

# 19. Rámeček

- Nastavte rámeček pomoci vlastnosti `border`, elementu s třídou `product-shipping-label` o velkosti `1px` a barvy `--product-red`. Nastavte barvu pozadi na bílou.

```css
.product-shipping-label {
  color: var(--product-red);
  font-weight: bold;
  font-size: 18px;
  text-transform: uppercase;
  display: inline-block;
  padding: 8px;
  border: 1px solid var(--product-red);
  background-color: var(--product-white);
}
```

- Nastavte zakulacení rohu rámečku stejnému elementu pomoci vlastnosti `border-radius` na hodnotu `6px`.

```css
.product-shipping-label {
  color: var(--product-red);
  font-weight: bold;
  font-size: 18px;
  text-transform: uppercase;
  display: inline-block;
  padding: 8px;
  border: 1px solid var(--product-red);
  background-color: var(--product-white);
  border-radius: 6px;
}
```

- Nastavte zakulacení rohu rámečku elementu s třídou `add-to-cart-button` pomoci vlastnosti `border-radius` na hodnotu `30px`.

```css
.add-to-cart-button {
  background-color: var(--product-red);
  color: var(--product-white);
  font-weight: bold;
  font-size: 24px;
  display: inline-block;
  padding: 8px 0;
  width: 100%;
  text-align: center;
  border-radius: 30px;
}
```

# 20. Kruh

- Vytvořte kruh z elementu, s třídou `discount-badge`. Aby ste vytvořili kruh je potřebné nastavit elementu výšku a šířku. Pozor, element je inline element, a proto musíte nejdřív nastavit `display: inline-block` aby ste mohli upravovat výšku, šírku, vnější a vnitřní okraje. V dalším kroku nastavte `border-radius` na `50%`. Pro vertikálni zacentrovaní nastavte `line-height` na hodnotu výšky elementu a pro horiznotálni zacentrovaní nastavte `text-align` na hodnotu `center`.

```css
.discount-badge {
  background-color: var(--product-red);
  color: var(--product-white);
  font-weight: bold;
  font-size: 20px;
  display: inline-block;
  border-radius: 50%;
  height: 70px;
  width: 70px;
  line-height: 70px;
  text-align: center;
}
```

- Nastavte zakulacení na elementě `bestseller-badge` pro pravý horní a pravý dolní rohu.

```css
.product-image-container {
  .bestseller-badge {
    background-color: var(--product-yellow);
    color: var(--product-brown);
    font-weight: bold;
    font-size: 14px;
    padding: 4px;
    position: absolute;
    top: 30px;
    left: 0px;
    border-radius: 0 5px 5px 0;
  }
}
```

# 20. Přidani obrázku

- Práce s obrázkem je obsahem třetí lekce, z toho důvodu jenom skopírujte nasledujíci kus html kodu a přidejte ho do `index.html` mezi elementy`discount-badge` a `product-title`. Styly přidejte do `styles.css`.

```html
<div class="product-image-container">
  <img src="/images/bota-1.webp" />
</div>
```

```css
.product-image-container {
}

img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
```

# 21. Pozicování prvků na stránce

- Nastavte element s třídou `bestseller-badge` na levý horní okraj pomocí vlastnosti `position: absolute` s hodnotou `top: 30px` a `left: 0`. Pozor, element pozicujeme vůči elementů s třídou `product-card`, proto musíte nastavit na danom elementů `position: relative`.

```css
.product-card {
  width: 450px;
  background-color: var(--product-white);
  padding: 16px;
  position: relative;
}

.bestseller-badge {
  background-color: var(--product-yellow);
  color: var(--product-brown);
  font-weight: bold;
  font-size: 14px;
  padding: 4px;
  position: absolute;
  top: 30px;
  left: 0px;
}
```

- Nastavte element s třídou `discount-badge` na pravý horní okraj elementu s třídou `product-card`. Element napozicujte od horního okraje `16px` a `16px` z pravé strany.

```css
.discount-badge {
  background-color: var(--product-red);
  color: var(--product-white);
  font-weight: bold;
  font-size: 20px;
  display: inline-block;
  border-radius: 50%;
  height: 70px;
  width: 70px;
  line-height: 70px;
  text-align: center;
  position: absolute;
  top: 16px;
  right: 16px;
}
```

- Nastavte element s třídou `product-stock-label` na pravý okraj rodičovského elementu `product-details-container`. V prvním kroku, proto musíme nastavit `position: relative` elementu `product-details-container` vůči, kterému pozicujeme. V druhým kroku, nastavíme pomoci vlastnosti `position: absolute` element `product-stock-label` s hodntou `top: 16px` a `right: 16px`.

```css
.product-details-container {
  padding: 8px;
  background-color: var(--product-light-red);
  margin-bottom: 16px;
  position: relative;
}

.product-stock-label {
  color: var(--product-green);
  font-weight: bold;
  font-size: 18px;
  text-decoration: underline;
  position: absolute;
  top: 16px;
  right: 16px;
}
```
