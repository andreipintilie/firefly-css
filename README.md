# Why FireflyCSS
The best CSS library for small projects/apps. FireflyCSS comes with a very small filesize!

# CSS Import

- main.css(42.7 kbps)

```css
@import 'https://andreipintilie.github.io/firefly-css/main.css';
```

- main.min.css(35.3 kbps)

```css
@import 'https://andreipintilie.github.io/firefly-css/main.min.css';
```

[CodePen – See some examples](https://codepen.io/andreiliviuu/pen/RwabQma)

# Things that we haven't added yet

- Footers
- Grid System
- More button styles

# Things that we are currently working on

- Navbars
- Notifications

# FireflyCSS's includes

```scss
@import 'variables';
@import 'resets';
@import 'utilities';
@import 'typography';
@import 'grids';
@import 'align';
@import 'borders';
@import 'display';
@import 'flex';
@import 'buttons';
@import 'cards';
@import 'badges';
@import 'tips';
@import 'notifications';
@import 'navbar';
```

# API Designed for custom classes

```scss
$utilities: (
  'opacity': (
    property: opacity,
    class: o,
    important: yes,
    values: (
      25: 25%,
      50: 50%,
      75: 75%,
      100: 100%,
    ),
  ),
);
```

## What the API-generated classes will look like

```scss
.o-25 {
  opacity: 25% !important;
}

.o-50 {
  opacity: 50% !important;
}

.o-75 {
  opacity: 75% !important;
}

.o-100 {
  opacity: 100% !important;
}
```

# Create a custom function by using our API

If you're using Firefly with SCSS:

```scss
$utilities: () !default;
$utilities: map-merge(
  (
    // ...
    "width": (
      property: width,
      class: w,
      important: yes,
      values: (
        25: 25%,
        50: 50%,
        75: 75%,
        100: 100%,
        auto: auto
      )
    ),
    // ...
  ), $utilities);
```

# About
Firefly is a CSS library which contains modern components and modern UI elements, inspired by high-level CSS Frameworks.

# License
Released under the [MIT](https://mit-license.org/) License.
