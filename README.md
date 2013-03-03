# Triangle

Create triangles with pure CSS. Useful for creating carets on pseudo elements.

## Installation

```
fonzie install triangle
```

## Usage

You can turn any box into a triangle:

```scss
.triangle {
  @include triangle('north', $width: 20px, $height: 10px, $color: red);
}
```

But they're useful for creating carets on pseudo elements:

```scss
.tab {
  &:after {
    @include triangle('south', $width: 16px, $height: 8px, $color: #555);
    display: block;
    content: '';
    position: absolute;
    bottom: 0;
    left: 50%;
    margin-left: -8px;
  }
}
```