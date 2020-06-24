# Firefly CSS Library
Firefly is a CSS Library based on the latest high-level frameworks, made for responsivity and easy-importable components, Firefly was inspired by Bootstrap and Tailwind.

# Grid System & Layout

### Container

```html
<div class = 'container'>
  <!-- your code here -->
</div>
```

1. Note that the `.container`'s functionality is like the Bootstrap's one, responsive for each viewport.
2. The default width is set to 80% and centered (`margin: 0 auto;`). Its width will be changed according to the viewport.

### Container-Fluid

```html
<div class = 'container-fluid'>
  <!-- your code here -->
</div>
```

1. `.container-fluid`'s has a fixed-width (`width: 100%;`) and it will NOT change according to the viewport.
2. The margins for this container are always set to zero.

### Columns

```html
<div class = 'row'>
  <div class = 'col-6'>
    <!-- your code here -->
  </div>
  <div class = 'col-6'>
    <!-- your code here -->
  </div>
</div>
```

1. The `.col` classes have to be direct children to the `.row` class, otherwise the cols won't be on the same line.
2. Every col has a different width:

```sass
$columnSizes: (
    1: 8.33%,
    2: 16.66%,
    3: 25%,
    4: 33.33%,
    5: 41.66%,
    6: 50%,
    7: 58.33%,
    8: 66.66%,
    9: 75%,
    10: 83.33%,
    11: 91.66%,
    12: 100%,
);
```

### Borders

1. If you want to set an element's border to none, you can use:

```html
<button class = 'border-none'>Click here</button>
```

2. If you want to set a border's radius, use:

```html
<button class = 'radius-5'>Click here</button>
```

- The "5" in the `radius-5` means 5px.
- Syntax: radius-{1-10}

# Typography

### Align.

```html
<p class = 'text-center'>This text is centered.</p>
```

Supported:
- text-left
- text-center
- text-right

### Weight.

```html
<p class = 'font-bold'>This text is bold.</p>
```

1. If you're using a heading and want to get rid of the default boldness, you can use:

```html
<h1 class = 'font-normal'>This text will not be bold</h1>
```

2. However, if you want to have more control over a text's weight, you can use:

```html
<p class = 'font-weight-700'>This text is bold.</p>
```

Usage: 
- font-size-{100-900}

### Size.

```html
<p class = 'font-size-5'>My size is 1.83em</p>
```

- Usage: font-size-{1/2/3/4/5}

### Set the color of a text.

```html
<p class = 'color-dark'>I'm dark!</p>

<p class = 'color-default'>The default color class stands for #F0F0F0</p>
```

- Usage: color-{color name}

Colors:
- ![hex-color](https://via.placeholder.com/15x15/f0f0f0/f0f0f0?Text=) default #f0f0f0
- ![hex-color](https://via.placeholder.com/15x15/007bff/007bff?Text=) primary #007bff
- ![hex-color](https://via.placeholder.com/15x15/17a2b8/17a2b8?Text=) info #17a2b8
- ![hex-color](https://via.placeholder.com/15x15/6c757d/6c757d?Text=) secondary #6c757d
- ![hex-color](https://via.placeholder.com/15x15/dc3545/dc3545?Text=) danger #dc3545
- ![hex-color](https://via.placeholder.com/15x15/ffc107/ffc107?Text=) warning #ffc107
- ![hex-color](https://via.placeholder.com/15x15/28a745/28a745?Text=) success #28a745
- ![hex-color](https://via.placeholder.com/15x15/6c757d/6c757d?Text=) disabled #6c757d
- ![hex-color](https://via.placeholder.com/15x15/343a40/343a40?Text=) dark #343a40

# Padding & Margin

### Padding (First Method)

1. Padding Top

```html
<p class = 'py-2'>Padding Top</p>
```

2. Padding Bottom

```html
<p class = 'py-n2'>The Opposite for padding top.</p>
```

- The "n" in `py-n2` stands for negative, it's the opposite for padding-top.

3. Padding Left

```html
<p class = 'px-2'>This is padding left.</p>
```

4. Padding Right

```html
<p class = 'px-n2'>This is padding right.</p>
```

- Just like padding-bottom, the "n" in `px-n2` stands for negative, it's the opposite for padding-left.

### Padding (Second Method)

Of course the first method is not as popular as Bootstrap's one, so we've included that as well.

1. Padding Top

```html
<p class = 'pt-5'> Your text here </p>
```

2. Padding Bottom

```html
<p class = 'pb-5'> Your text here </p>
```

3. Padding Left

```html
<p class = 'pl-5'> Your text here </p>
```

4. Padding Right

```html
<p class = 'pr-5'> Your text here </p>
```

### Margin (First Method)

Of course, the padding classes and margin classes share the same techniques.

1. Margin Top

```html
<div class = 'my-2'>
  <!-- your code here -->
</div>
```

2. Margin Bottom

```html
<div class = 'my-n2'>
  <!-- n stands for negative, so it's the opposite -->
  <!-- your code here -->
</div>
```

3. Margin Left

```html
<div class = 'mx-2'>
  <!-- your code here -->
</div>
```

4. Margin Right

```html
<div class = 'mx-n2'>
  <!-- n stands for negative, so it's the opposite -->
  <!-- your code here -->
</div>
```

### Margin (Second Method)

1. Margin Top

```html
<div class = 'mt-2'>
  <!-- your code here -->
</div>
```

2. Margin Bottom

```html
<div class = 'mb-2'>
  <!-- your code here -->
</div>
```

3. Margin Left

```html
<div class = 'ml-2'>
  <!-- your code here -->
</div>
```

4. Margin Right

```html
<div class = 'mr-2'>
  <!-- your code here -->
</div>
```

# Cards

### Basic Card

```html
<div class="card">
  <div class="card-header">
    <p class="card-text">Welcome to our website.</p>
  </div>
  <div class="card-body">
    <p class="card-title">Lorem ipsum.</p>
    <p class="card-text">
      Lorem ipsum dolor sit, amet consectetur
      adipisicing elit. Nulla, suscipit.
    </p>
  </div>
  <div class="card-footer">
    <p class="card-text">3 hours ago</p>
  </div>
</div>
```

However, if you want a custom card, you can use `.card-{card-style}`.

### Dark Card

```html
<div class="card-dark">
  <div class="card-header">
    <!-- your code here -->
  </div>
  <div class="card-body">
    <!-- your code here -->
  </div>
  <div class="card-footer">
    <!-- your code here -->
  </div>
</div>
```

Card Classes:
- card
- card-dark
- card-primary
- card-info
- card-danger
- card-warning
- card-success

`.card-title` will be bold by default.

# Backgrounds

### Solid backgrounds.

```html
<div class = 'bg-danger'>
  <!-- your code here -->
</div>
```

Available classes:
- bg-default (#F0F0F0)
- bg-primary (#007BFF)
- bg-info (#17A2B8)
- bg-secondary (#6C757D)
- bg-danger (#DC3545)
- bg-warning (#FFC107)
- bg-success (#28A745)
- bg-disabled (#6C757D)
- bg-dark (#343A40)

### Transparent Backgrounds

```html
<div class = 'bg-transparent-danger'>
  <!-- your code here -->
</div>
```

- The `.bg-transparent-danger` class it's the same background as `.bg-danger`, but with the opacity set to 50%.

# License

Released under the [MIT](https://mit-license.org/) License.
