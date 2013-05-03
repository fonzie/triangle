# Triangle

Create triangles with pure CSS. Useful for creating carets on pseudo elements.

## Installation

```
bower install fonzie-triangle
```

## Usage

You can turn any box into a triangle:

```scss
.triangle {
  @include fz-triangle('north', $width: 20px, $height: 10px, $color: red);
}
```

But they're useful for creating carets on pseudo elements:

```scss
.tab {
  &:after {
    @include fz-triangle('south', $width: 16px, $height: 8px, $color: #555);
    display: block;
    content: '';
    position: absolute;
    bottom: 0;
    left: 50%;
    margin-left: -8px;
  }
}
```