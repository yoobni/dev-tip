# Sass

Sass == SCSS

1. Incoding
```Sass
    @charset 'utf-8';
```

2. String
```Sass
    $temp: 'like this';
```

3. Sass 초기화

```
@mixin respond-to($breakpoint) {
  $raw-query: map-get($breakpoints, $breakpoint);

  @if $raw-query {
    $query: if(
      type-of($raw-query) == 'string',
      unquote($raw-query),
      inspect($raw-query)
    );

    @media #{$query} {
      @content;
    }
  } @else {
    @error 'No value found for `#{$breakpoint}`. '
         + 'Please make sure it is defined in `$breakpoints` map.';
  }
}


@mixin clearfix {
  &::after {
    content: '';
    display: table;
    clear: both;
  }
}

.button {
    // Styles for buttons
    background: red;
    a & {
        background: blue;
    }
}

```
