# Semantic List CSS
> CSS for putting semantic numbers into nested list.

## Usage

### Install
Download `semantic-list.css` and include it to your HTML.
Also available on [npm](https://www.npmjs.com/).

- Download: [**semantic-list.css**](./semantic-list.css)
- `$ npm install semantic-list --save`

### Example
Create `<ol>` element with `"semantic-list"` class.

```html
<ol class="semanic-list">
  <li>List item
    <ol>
      <li>List item
        <ol>
          <li>List item</li>
          <li>List item</li>
        </ol>
      </li>
      <li>List item</li>
    </ol>
  </li>
  <li>List item</li>
</ol>
```

List item will have `1`, `1.1`, `1.1.1`, ... marker according to the depth.

```
1 List item
  1.1 List item
    1.1.1 List item
    1.1.2 List item
  1.2 List item
2 List item
```

## Marker types
Add optional class to change the marker type.

### dot (default)
`<ol class="semantic-list">` or `<ol class="semantic-list dot">`

```
1 List item
  1.1 List item
    1.1.1 List item
    1.1.2 List item
  1.2 List item
2 List item
```

### hyphen
`<ol class="semantic-list hyphen">`

```
1 List item
  1-1 List item
    1-1-1 List item
    1-1-2 List item
  1-2 List item
2 List item
```

### ja-formal
`<ol class="semantic-list ja-formal">`

Follows [公用文作成の要領](https://ja.wikipedia.org/wiki/%E5%85%AC%E7%94%A8%E6%96%87%E4%BD%9C%E6%88%90%E3%81%AE%E8%A6%81%E9%A0%98#.E7.AC.AC3_.E6.9B.B8.E5.BC.8F.E3.82.84.E6.96.87.E6.9B.B8.E3.81.AE.E6.A7.98.E5.BC.8F.E3.81.AB.E9.96.A2.E3.81.99.E3.82.8B.E9.80.9A.E5.89.87).
第1 → 1 → (1) → ア → (ア)

```
第1 List item
  1 List item
    (1) List item
    (2) List item
  2 List item
第2 List item
```

### ja-semi-formal
`<ol class="semantic-list ja-semi-formal">`

1 → (1) → (ア)

```
1. List item
  (1) List item
    (ア) List item
    (イ) List item
  (2) List item
2. List item
```

## License
Copyright (c) 2016 Hiroyuki Tanjo.
Licensed under the MIT License.
