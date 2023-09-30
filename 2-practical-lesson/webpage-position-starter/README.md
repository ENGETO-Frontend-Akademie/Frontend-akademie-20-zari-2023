# Position příklady použití z praxe

1. nastavení loga v navigaci

```css
.navigation-wrapper {
  position: relative;
}

.logo {
  position: absolute;
  top: 18px;
}
```

2. nastavení navigace která se zafixuje na stránce a ostáva na sve pozici při skrolování

- pridani do třídy `.navigation` nasledujíci kód

```css
.navigation {
  position: fixed;
  width: 100%;
  top: 0;
  z-index: 1;
}
```

3. nastavení oteviraceho modálu a overlay

```css
.modal {
  position: fixed;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.8);
  top: 0;
  left: 0;
  z-index: 1;
  display: none;
}

.modal-content {
  background-color: #f0f0f0;
  width: 40%;
  padding: 32px;
  margin: 15% auto;
  position: relative;
}
```

4. nastavení zavíracího tlačitka na modaly

```css
.modal-content {
  position: relative;
}

.close-button {
  position: absolute;
  top: 8px;
  right: 16px;
}
```

4. nastavení tooltipu pri najetí kurzore nad určitý text

```css
.tooltip-text {
  position: absolute;
  visibility: hidden;
  bottom: 20px;
  left: 50%;
  background-color: var(--text-color);
  color: var(--footer-text);
  width: 200px;
  padding: 8px;
  border-radius: 4px;
  font-size: 12px;
}

.tooltip:hover .tooltip-text {
  visibility: visible;
}
```
