# flexboxes
<b>flexboxes</b> is a functional flexbox utility library and pure flexbox grid system. It offers a hybrid between other frameworks. It is designed for both prototyping and production.

## setup

```
npm install flexboxes
```

```css
@import 'node_modules/flexboxes/main';
```

## classes

### [`display`](https://www.w3.org/TR/css-flexbox-1/#flex-containers)
- `.flex`
- `.inline-flex`

### [`flex-direction`](https://www.w3.org/TR/css-flexbox-1/#flex-direction-property)
- `.flex-row`
- `.flex-row-reverse`
- `.flex-column`
- `.flex-column-reverse`

### [`flex-wrap`](https://www.w3.org/TR/css-flexbox-1/#flex-wrap-property)
- `.flex-wrap`
- `.flex-nowrap`
- `.flex-wrap-reverse`

### [distribute free space](https://www.w3.org/TR/css-flexbox-1/#auto-margins)
- `.free-top`
- `.free-left`
- `.free-right`
- `.free-bottom`

### [`order`](https://www.w3.org/TR/css-flexbox-1/#order-property)
- `.order-before`
- `.order-after`

### [`align-items`](https://www.w3.org/TR/css-flexbox-1/#align-items-property)
- `.items-start`
- `.items-end`
- `.items-center`
- `.items-baseline`
- `.items-stretch`

### [`align-self`](https://www.w3.org/TR/css-flexbox-1/#align-items-property)
- `.self-center`
- `.self-baseline`
- `.self-stretch`
- `.self-start`
- `.self-end`

### [`justify-content`](https://www.w3.org/TR/css-flexbox-1/#justify-content-property)
- `.justify-start`
- `.justify-end`
- `.justify-center`
- `.justify-between`
- `.justify-around`

### [`align-content`](https://www.w3.org/TR/css-flexbox-1/#align-content-property)
- `.content-start`
- `.content-end`
- `.content-center`
- `.content-between`
- `.content-around`
- `.content-stretch`

### size control
- `.flex-min` re: [nesting](https://goo.gl/3IZRMt)
- `.flex-max`

### [`flex`](https://www.w3.org/TR/css-flexbox-1/#flex-property) presets
- `.flex-golden`
- `.flex-initial`
- `.flex-auto`
- `.flex-none`

### [`flex`](https://www.w3.org/TR/css-flexbox-1/#flex-common) shorthand
- `.flex-0`
- `.flex-1`
- `.flex-2`
- `.flex-3`
- `.flex-4`
- `.flex-5`
- `.flex-6`
- `.flex-7`
- `.flex-8`
- `.flex-9`
- `.flex-10`
- `.flex-11`
- `.flex-12`

### [`flex-grow`](https://www.w3.org/TR/css-flexbox-1/#flex-grow-property)
- `.grow-0`
- `.grow-1`
- `.grow-2`
- `.grow-3`
- `.grow-4`
- `.grow-5`
- `.grow-6`
- `.grow-8`
- `.grow-7`
- `.grow-9`
- `.grow-10`
- `.grow-11`
- `.grow-12`

### [`flex-shrink`](https://www.w3.org/TR/css-flexbox-1/#flex-shrink-property)
- `.shrink-0`
- `.shrink-1`
- `.shrink-2`
- `.shrink-3`
- `.shrink-4`
- `.shrink-5`
- `.shrink-6`
- `.shrink-7`
- `.shrink-8`
- `.shrink-9`
- `.shrink-10`
- `.shrink-11`
- `.shrink-12`

### [`flex-basis`](https://www.w3.org/TR/css-flexbox-1/#flex-basis-property)
- `.basis-0` 0/12 grid
- `.basis-1` 1/12 grid
- `.basis-2` 2/12 grid
- `.basis-3` 3/12 grid
- `.basis-4` 4/12 grid
- `.basis-5` 5/12 grid
- `.basis-6` 6/12 grid
- `.basis-7` 7/12 grid
- `.basis-8` 8/12 grid
- `.basis-9` 9/12 grid
- `.basis-10` 10/12 grid
- `.basis-11` 11/12 grid
- `.basis-12` 12/12 grid
- `.basis-100vw`
- `.basis-100vh`
- `.basis-100vmax`
- `.basis-100vmin`
- `.basis-golden`
- `.basis-content`
- `.basis-auto`

### `@media`

#### portrait

- `.portrait-flex`
- `.portrait-inline-flex`
- `.portrait-flex-wrap`
- `.portrait-flex-nowrap`
- `.portrait-flex-wrap-reverse`

#### landscape

- `.landscape-flex`
- `.landscape-inline-flex`
- `.landscape-flex-wrap`
- `.landscape-flex-nowrap`
- `.landscape-flex-wrap-reverse`

## examples

### [balanced grid](https://codepen.io/ryanve/pen/mmgjXE)

```html
<div class="flex">
  <div class="flex-auto">item</div>
  <div class="flex-auto">item</div>
  <div class="flex-auto">item</div>
</div>
```

### [wrapping grid](https://codepen.io/ryanve/pen/JNzPMw)

```html
<div class="flex flex-wrap">
  <div class="basis-4">grid item</div>
  <div class="basis-4">grid item</div>
  <div class="basis-4">grid item</div>
  <div class="basis-4">grid item</div>
  <div class="basis-4">grid item</div>
</div>
```

## development

```
npm start
```

## inspirations

- [basscss-flexbox](https://www.npmjs.com/package/basscss-flexbox)
- [flexboxgrid](https://www.npmjs.com/package/flexboxgrid)

* * *

flexpress yo' self
