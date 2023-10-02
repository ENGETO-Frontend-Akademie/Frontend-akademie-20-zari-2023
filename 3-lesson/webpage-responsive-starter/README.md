1. změnit šířku contentu pro mobil na 90%

```css
@media (max-width: 576px) {
  .content {
    max-width: 90%;
  }
}
```

2. změnit velikost h1 pro mobil na 28px

```css
@media (max-width: 576px) {
  h1 {
    font-size: 28px;
  }
}
```

3. změnit navigaci pro mobil - nastavit šířku `navigation-wrapper` na 90%

- zobrazit menu icon pro mobil
- skryt element s třídou `.navigation-list`

```css
@media (max-width: 576px) {
  .navigation-wrapper {
    max-width: 90%;
  }
  .navigation-list {
    display: none;
  }
  .icon {
    display: block;
  }
}
```

4. odstránit obrázek pro mobil

```css
@media (max-width: 576px) {
  .image-container {
    display: none;
  }
}
```

5. změnit button na celou šířku pro mobil

```css
@media (max-width: 576px) {
  .button {
    width: 100%;
  }
}
```

6. nastavit modal na 90% šířku viewportu pro mobil

```css
@media (max-width: 576px) {
  .modal-content {
    width: 90%;
  }
}
```
