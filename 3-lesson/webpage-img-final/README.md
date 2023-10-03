1. Přidejte do sekce `about-section` obrázek, který bude obaleny obálkou s třídou `image-container`. Cestu k obrázku použijte link https://shorturl.at/qQRWZ

- obrázek by měl mít výšku 400px a šířku 100% rodiče

```html
<div class="image-container">
  <img src="https://shorturl.at/qQRWZ" alt="about us image" />
</div>
```

```css
.image-container {
  width: 100%;
  height: 400px;
  margin-top: 20px;
}

.image-container img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  border-radius: 4px;
}
```

2. Přidejte background image do header sekce. Pracujte s nasledujíci kodem:

```html
<header class="hero-section">
  <div class="hero-section-wrapper">
    <h1 class="hero-text">
      Welcome to <br />WebSolutions Pro <i class="fas fa-globe"></i>
    </h1>
  </div>
</header>
```

- nastavte pro `hero-section-wrapper` šířku 70% a `margin: 0 auto`
- nastavte pro `hero-section` background image, který nájdete na linku https://shorturl.at/CV458
- nastavte velkost obrázku
- vycentrujte obrázek
- zabrántě opakováni obrázku
- výšku nastavte na 70 procent výšky viewportu
- napozicujte text `hero-text` na `bottom: 30px`
- podle potřeby upravte styl textu

```css
.hero-section {
  background-image: url("https://shorturl.at/CV458");
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  height: 70vh;
  position: relative;
  background-color: rgba(0, 0, 0, 0.4);
  background-blend-mode: overlay;
}

.hero-section-wrapper {
  max-width: 70%;
  margin: 0 auto;
}

.hero-text {
  color: #fff;
  position: absolute;
  bottom: 30px;
  font-size: 48px;
  text-align: left;
}
```
