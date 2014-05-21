#Entity

A Sass function that will output properly encoded entities.

##Usage
The `entity` function accepts the actual character, the HTML name without the ampersand and semi-colon or the decimal number.

```
body {
  &:after {
    content: entity('€');
  }
}
```
will output

```
body:after {
  content: "\20AC";
}
```

## Requirements

* Sass ~> 3.3.0
