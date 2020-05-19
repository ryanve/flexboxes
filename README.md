# flexboxes
[flexboxes](https://ryanve.github.io/flexboxes) is a functional flexbox library and pure flexbox grid system designed for prototyping and production.

## setup

Download [flexboxes.css](flexboxes.css) and load [stylesheet](https://dev.opera.com/articles/css-basics/#external)

```html
<link rel="stylesheet" href="flexboxes.css">
```

- Browse [releases](../../releases) or the [latest release](../../releases/latest)
- [Codepens](https://codepen.io) can link [unpkg](https://unpkg.com/flexboxes)
- Dependers can [npm install flexboxes](https://www.npmjs.com/package/flexboxes) and `@import` via `node_modules`
- Deprecated classes are in [deprecated.css](deprecated.css)

## classes

### [`display`](https://www.w3.org/TR/css-flexbox-1/#flex-containers)
- `.inline-flex` for `inline-flex`
- `.block-flex` for `flex`

### [`flex-flow`](https://www.w3.org/TR/css-flexbox-1/#flex-flow-property)

- Compose [`flex-direction`](#flex-direction) [`flex-wrap`](#flex-wrap)
- Default is `row nowrap`

### [`flex-direction`](https://www.w3.org/TR/css-flexbox-1/#flex-direction-property)

- `.flow-east` for `row`
- `.flow-west` for `row-reverse`
- `.flow-south` for `column`
- `.flow-north` for `column-reverse`

### [`flex-wrap`](https://www.w3.org/TR/css-flexbox-1/#flex-wrap-property)

- `.flow-over` for `nowrap`
- `.flow-wrap` for `wrap`
- `.flow-warp` for `wrap-reverse`

### [`margin`](https://www.w3.org/TR/css-flexbox-1/#auto-margins)

<a name="distribute-free-space" href="https://ryanve.github.io/flexboxes#freeing">Distribute free space</a> via `auto` margins

- `.free-all` frees all
- `.free-top` frees top
- `.free-bottom` frees bottom
- `.free-left` frees left
- `.free-right` frees right
- `.free-north` frees block-start
- `.free-south` frees block-end
- `.free-west` frees inline-start
- `.free-east` frees inline-end

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
- `.just-start`
- `.just-end`
- `.just-center`
- `.just-between`
- `.just-around`

### [`align-content`](https://www.w3.org/TR/css-flexbox-1/#align-content-property)
- `.pack-start`
- `.pack-end`
- `.pack-center`
- `.pack-between`
- `.pack-around`
- `.pack-stretch`

### [`flex`](https://www.w3.org/TR/css-flexbox-1/#flex-property)

<a name="flex-presets"></a>
<a name="flex-shorthand"></a>

Shorthand classes supply [common presets](https://www.w3.org/TR/css-flexbox-1/#flex-common)

- `.flex-fade` for `0 1 auto` aka shrinkable
- `.flex-fame` for `1 0 auto` aka growable
- `.flex-auto` for `1 1 auto` aka flexible
- `.flex-none` for `none` aka inflexible

Compose with [`grow`](#flex-grow) [`shrink`](#flex-shrink) [`basis`](#flex-basis)

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

### area
<a name="size-control"></a>

Some [flexbugs](https://github.com/philipwalton/flexbugs) are solvable via min or max width or height

- `.area-min` sets both mins to `0` [re: nesting](https://goo.gl/3IZRMt)
- `.area-max` sets both maxes to `100%`

Consider [area.css](https://github.com/ryanve/area.css) for more

### `@media`

Responsive [`orientation`](https://drafts.csswg.org/mediaqueries-4/#orientation) classes are available for [`flex-flow`](#flex-flow) and [`display`](#display) classes. Append [`@portrait`](#portrait) or [`@landscape`](#landscape) to these classes to limit them to that orientation. This affords layouts that flow or wrap differently based on viewport orientation or layouts that only flex in one orientation. Try the [#fitting](https://ryanve.github.io/flexboxes/#fitting) example in both portrait and landscape to see how it adapts. You can do this on a phone by rotating the phone or on a computer by resizing the browser window.

```html
class="block-flex flow-west@portrait flow-north@landscape"
```

#### `portrait`

- `flow-east@portrait`
- `flow-west@portrait`
- `flow-south@portrait`
- `flow-north@portrait`
- `flow-over@portrait`
- `flow-wrap@portrait`
- `flow-warp@portrait`
- `inline-flex@portrait`
- `block-flex@portrait`

#### `landscape`

- `flow-east@landscape`
- `flow-west@landscape`
- `flow-south@landscape`
- `flow-north@landscape`
- `flow-over@landscape`
- `flow-wrap@landscape`
- `flow-warp@landscape`
- `inline-flex@landscape`
- `block-flex@landscape`

## examples

[ryanve.github.io/flexboxes](https://ryanve.github.io/flexboxes)
