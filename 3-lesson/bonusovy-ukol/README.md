# 1. Vytvoření souboru index.html a základni struktúry HTML

- vytvořte soubor **index.html**
- základní struktúru HTML vytvoříme napsánim znaku ! a následním stisknutím ENTER na klávesnici

# 2. Přidáni obsahu

- odkaz na obrazek v hero sekci: https://shorturl.at/jmX23
- odkaz na druhy obrazek: https://shorturl.at/esENQ
- text v hero sekci:
  "Exploring Icelandic Villages"
  "Where Nature and Culture Converge"
- menu sekce: Home, About Us, Explore, Contact Us

# 3. Vytvoření souboru styles.css

- vytvořite soubor s názvem **styles.css**
- přelinkujte soubor index.html se souborem styles.css vložením nasledujíciho kusu kódu do hlavičky html souboru

# 4. Přidani třid

- přidejte do kódu sémantický element `nav`, který bude představovat navigaci.
- položky navigace obalte elementem `a` s prázdnim atribútem `href`.
- současti navigace bude ikonka menu pro mobilni verzi. Pro ikonku vytvořte blokový element `<div></div>` s třídou `icon`. Elementu přidáte `img` tag s atribútem `src`, který bude obsahovat odkaz na obrázek.
- vytvořte blokový element `<div></div>` s třídou `hero-section`, kterému nastavíte obrázek na pozadi. Tento element bude obsahovat element s třídou `hero-text`.
- Element `hero-text` bude obsahovat dve elementy. Jeden bude obalovat text "Exploring Icelandic Villages". Tomuto elementu nastavte třídu `hero-subtitle`. Druhý text "Where Nature and Culture Converge" bude nádpis první úrovně s třídou `hero-title`.
- vytvořte další blokový element `<div></div>` s třídou `image-container`. Elementu přidáte `img` tag s atribútem `src`, který bude obsahovat odkaz na obrázek.

# 5. Přidejte selektory tříd

- přidejte selektory tříd do css souboru

# 6. Nastavení navigace

- nastavte tagu `nav` barvu pozadí pomocí vlastnosti `background-color` na `#F08D8F`.
- nastavte velikost ikonky menu na `width: 30px` a `height: 25px`. Pozor ikonku vkládate jako obrázek, proto musíte nastavit obrázku responzívni chováni pomoci `width: 100%` a `height: 100%`.
- pro umístnění položek menu vedle sebe nastavte vlastnosti `display: flex` a `justify-content: space-evenly` na tag `nav`.
- položkam vypnete podtržení pomocí vlasntosti `text-decoration: none`.
- skryjte iconu menu pro viewport větší než `768px` a naopak zobrazte položky menu. Skrývani a zobrazení dosáhnete pomocí vlastnosti `dislay: none`, `display: block` a použití media query.

```css
/* pseudo kód */
.icon {
  display: none;
}

@media (max-width: 768px) {
  .icon {
    display: block;
  }
  .nav a {
    display: none;
  }
}
```

- nastavte pro položky menu `padding-top` a `padding-bottom` hodnotu `16px`, barvu písma na `#fff`, velikost na `20px` a `font-weight: bold`.
- pro ikonu nastavte `padding: 8px`.
- jednou z možnosti jak napozicovat ikonku na levu stranu je nastavením `margin-left: auto`.
- tagu `nav` nastavte `border-radius: 8px`.
- tagu `nav` nastavte `margin-bottom: 10px` aby se vytvořil prostor mezi navigaci a obrázkem pod ní.

# 7. Nastavení hero sekce

- elementu s třídou `hero-section` nastavte vlastnosti:
  - `background-image: url('link obrazku')`
  - `background-size`
  - `background-position`
  - `background-repeat`
  - `border-radius: 12px`
- elementu s třídou `hero-section` nastavte `margin-bottom: 24px` aby se vytvořil prostor mezi hero sekci a nasledujícim obrázkem.
- napozicujte element s třídou `hero-text` do levého dolního rohu `hero-section`. V prvním kroku je potřebné nastavit `position: relative` pro element `hero-section`. V druhém kroku je potřebné nastavit `position: absolute` pro element `hero-text`. Element napozicujte z levého kraje 32px a dolního 16px.
- elementu `hero-text` nastavte bílu barvu písma.
- elementu s třídou `hero-subtitle` nastavte velkost písma na 20px.
- elementu s třídou `hero-title` nastavte `margin-top: 8px`.

# 8. Nastavení obrázku

- obálke obrázku s třídou `image-container` nastavte šířku 50% z celkové šířky viewportu.
- nastavte tagu `img` aby se přispůsobil velikosti sve obálky pomoci vlastnosti `width: 100%` a `height: 100%`.
- obrázku nastavte `border-radius` na 12px.

# 9. Prostor kolem stránky

- nastavte na tagu `body` vnější okraj `margin: 16px 32px`.

# 10. Mobilní nastavení

- pro viewport menší než 768px upravte:
  - velkost písma pro nádpis na 24px a subtitle na 18px.
  - šířku obrázku na 100% viewportu
  - vnejší okraj na tagu `body` na 8px.

```css
@media (max-width: 768px) {
}
```

# 11. Rodina písma

- Nastavte rodinu písma `Roboto` pomoci vlastnosti `font-family` na selektoru `body`.
- Nejdříve musite písmo `Roboto` naimportovat.
