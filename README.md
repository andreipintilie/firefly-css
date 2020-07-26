# Why FireflyCSS
The best CSS library for small projects/apps. FireflyCSS comes with a very small filesize!

- main.css (42.1 kbps)
- main.min.css (34.8 kbps)

# Things that we haven't added yet

- Navbars
- Footers
- Grid System
- More button styles

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
    values: (
      25: 25%,
      50: 50%,
      75: 75%,
      100: 100%,
    ),
  ),
  'font-size': (
    property: font-size,
    class: fsize,
    values: (
      1: 42px,
      2: 32px,
      3: 24px,
      4: 20px,
      5: 18px,
      6: 16px,
   ),
);
```

# About
Firefly is a CSS library which contains modern components and modern UI elements, inspired by high-level CSS Frameworks.

# License
Released under the [MIT](https://mit-license.org/) License.
