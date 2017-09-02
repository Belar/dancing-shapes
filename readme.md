<div align="center">
  <img width="100" height="100" src="./dancing_shapes_icon.png">
</div>

# Dancing Shapes

CSS-only, minimalist loading animations

[Demo](https://jsfiddle.net/Belar/syukjf0c/show/)

### CSS/Sass

Dancing Shapes can be used as a traditional CSS, with files available in `/dist` (after running build command) or through [CDN](#cdn). With Sass compiler, import necessary files from `/sass`: 

```scss
// Import within /sass directory
@import './loaders/<loader_type>';

// Import from npm package in /sass directory
@import '../node_modules/dancing-shapes/sass/loaders/<loader_type>';

// Import from npm package with Webpack
@import '~dancing-shapes/sass/loaders/<loader_type>'
```
where `<loader_type>` is one of loaders e.g. `bubble` or `fade-up`

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

### Browser support

Depends on required browser support, you may need to use `autoprefixer`, which is available for [all major build tools](https://github.com/postcss/autoprefixer#usage).

### CDN
Thanks to [unpkg.com](https://unpkg.com/) you can include Dancing Shapes on a website directly from the npm package:

```html
<!--Specific loader-->
<link href="https://unpkg.com/dancing-shapes@latest/dist/css/<loader_type>.css" rel="stylesheet">

<!--All loaders-->
<link href="https://unpkg.com/dancing-shapes@latest/dist/css/dancing-shapes.min.css" rel="stylesheet">
```

where `<loader_type>` is one of loaders e.g. `bubble` or `fade-up`
