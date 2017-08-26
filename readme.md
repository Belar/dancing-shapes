<div align="center">
  <img width="100" heigth="100" src="./dancing_shapes_icon.png">
</div>

# Dancing Shapes

CSS-only, minimalist loading animations

### CSS/Sass

Dancing Shapes can be used as a traditional CSS, available in `/dist` (after running build command) or with Sass compilers, by importing nessesary files from `/sass` e.g.

```css
@import 'loaders/jump';
```

Styling settings can be overwritten, full list can be found in `/sass/_settings`

### HTML

All loaders share the same markup structure:

```html
  <div class="loader <loader_type>">
    <div class="partial"></div>
    <div class="partial"></div>
    <div class="partial"></div>
    <div class="partial"></div>
  </div>
```

where `<loader_type>` is one of loaders e.g. `bubble` or `fade-up`
