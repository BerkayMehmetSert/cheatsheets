<h1 style="font-family: Roboto" align="center"> 
SCSS Cheat Sheets 
</h1>

<h3 style="font-family: Roboto">
Sass Basics 
</h3>

<h4 style="font-family: Roboto">
<code>variables</code>
</h4>

```scss
$defaultLinkColor: #46EAC2;

a {
  color: $defaultLinkColor;
}
```

<h4 style="font-family: Roboto">
<code>comments</code>
</h4>

```scss
/*
 Block comments
 Block comments
 Block comments
*/

// Line comments
```

<h4 style="font-family: Roboto">
<code>string interpolation</code>
</h4>

```scss
$wk: -webkit-;

.rounded-box {
  #{$wk}border-radius: 4px;
}
```

<h4 style="font-family: Roboto">
<code>mixins</code>
</h4>

```scss
@mixin heading-font {
    font-family: sans-serif;
    font-weight: bold;
}
h1 {
    @include heading-font;
}
```

<h4 style="font-family: Roboto">
<code>nestings</code>
</h4>

```scss
.markdown-body {
    a {
      color: blue;
      &:hover {
        color: red;
      }
    }
}
```

<h4 style="font-family: Roboto">
<code>extend</code>
</h4>

```scss
.button {
    ···
}
.push-button {
    @extend .button;
}
```

<h4 style="font-family: Roboto">
<code>@import</code>
</h4>

```scss
@import './other_sass_file';
@import '/code', 'lists';

// Plain CSS @imports
@import "theme.css";
@import url(theme);
```

<h4 style="font-family: Roboto">
<code>properties</code>
</h4>

```scss
@import './other_sass_file';
@import '/code', 'lists';

// Plain CSS @imports
@import "theme.css";
@import url(theme);
```

<h3 style="font-family: Roboto">
Sass Mixins 
</h3>

<h4 style="font-family: Roboto">
<code>parameters</code>
</h4>

```scss
@mixin font-size($n) {
    font-size: $n * 1.2em;
}
body {
    @include font-size(2);
}
```

<h4 style="font-family: Roboto">
<code>default values</code>
</h4>

```scss
@mixin pad($n: 10px) {
    padding: $n;
}
body {
    @include pad(15px);
}
```

<h4 style="font-family: Roboto">
<code>default variable</code>
</h4>

```scss
$default-padding: 10px;

@mixin pad($n: $default-padding) {
    padding: $n;
}

body {
    @include pad(15px);
}
```

<h3 style="font-family: Roboto">
Sass Color Functions 
</h3>

<h4 style="font-family: Roboto">
<code>rgba</code>
</h4>

```scss
rgb(100, 120, 140)
rgba(100, 120, 140, .5)
rgba($color, .5)
```

<h4 style="font-family: Roboto">
<code>mixing</code>
</h4>

```scss
mix($a, $b, 10%)   // 10% a, 90% b 
```

<h4 style="font-family: Roboto">
<code>hsl</code>
</h4>

```scss
darken($color, 5%)
lighten($color, 5%)
saturate($color, 5%)
desaturate($color, 5%)
grayscale($color)
adjust-hue($color, 15deg)
complement($color)    // like adjust-hue(_, 180deg)
invert($color)
fade-in($color, .5)   // aka opacify()
fade-out($color, .5)  // aka transparentize()
rgba($color, .5)      // sets alpha to .5
```

<h4 style="font-family: Roboto">
<code>rgb</code>
</h4>

```scss
red($color)         // 0..255
green($color)
blue($color)
```

<h4 style="font-family: Roboto">
<code>adjustments</code>
</h4>

```scss
// Changes by fixed amounts
adjust-color($color, $blue: 5)
adjust-color($color, $lightness: -30%) // darken(_, 30%)
adjust-color($color, $alpha: -0.4)     // fade-out(_, .4)
adjust-color($color, $hue: 30deg)      // adjust-hue(_, 15deg)
// Changes via percentage
scale-color($color, $lightness: 50%)
// Changes one property completely
change-color($color, $hue: 180deg)
change-color($color, $blue: 250) 
```

<h3 style="font-family: Roboto">
Sass Other Functions 
</h3>

<h4 style="font-family: Roboto">
<code>strings</code>
</h4>

```scss
unquote('hello')
quote(hello)
to-upper-case(hello)
to-lower-case(hello)
str-length(hello world)
str-slice(hello, 2, 5)     // "ello" - it's 1-based, not 0-based
str-insert("abcd", "X", 1) // "Xabcd" 
```

<h4 style="font-family: Roboto">
<code>units</code>
</h4>

```scss
unit(3em)        // 'em'
unitless(100px)  // false
```

<h4 style="font-family: Roboto">
<code>numbers</code>
</h4>

```scss
floor(3.5)
ceil(3.5)
round(3.5)
abs(3.5)
min(1, 2, 3)
max(1, 2, 3)
percentage(.5)   // 50%
random(3)        // 0..3
```

<h4 style="font-family: Roboto">
<code>misc</code>
</h4>

```scss
variable-exists(red)    // checks for $red
mixin-exists(red-text)  // checks for @mixin red-text
function-exists(redify)
global-variable-exists(red)
selector-append('.menu', 'li', 'a')   // .menu li a
selector-nest('.menu', '&:hover li')  // .menu:hover li
selector-extend(...)
selector-parse(...)
selector-replace(...)
selector-unify(...)
```

<h3 style="font-family: Roboto">
Sass Feature Checks 
</h3>

<h4 style="font-family: Roboto">
<code>feature check</code>
</h4>

```scss
feature-exists(global-variable-shadowing)
```

<h3 style="font-family: Roboto">
Sass Loops 
</h3>

<h4 style="font-family: Roboto">
<code>for</code>
</h4>

```scss
@for $i from 1 through 4 {
    .item-#{$i} { left: 20px * $i; }
}
```

<h4 style="font-family: Roboto">
<code>each</code>
</h4>

```scss
$menu-items: home about contact;

@each $item in $menu-items {
    .photo-#{$item} {
      background: url('#{$item}.jpg');
    }
}
```

<h4 style="font-family: Roboto">
<code>while</code>
</h4>

```scss
$i: 6;
@while $i > 0 {
    .item-#{$i} { width: 2em * $i; }
    $i: $i - 2;
}
```

<h3 style="font-family: Roboto">
Sass Other Features 
</h3>

<h4 style="font-family: Roboto">
<code>conditionals</code>
</h4>

```scss
@if $position == 'left' {
     position: absolute;
     left: 0;
}
@else if $position == 'right' {
     position: absolute;
     right: 0;
}
@else {
     position: static;
}
```

<h4 style="font-family: Roboto">
<code>interpolation</code>
</h4>

```scss
.#{$klass} { ... }      // Class
call($function-name)    // Functions

@media #{$tablet}
font: #{$size}/#{$line-height}
url("#{$background}.jpg")
```

<h4 style="font-family: Roboto">
<code>lists</code>
</h4>

```scss
$list: (a b c);

nth($list, 1)  // starts with 1
length($list)

@each $item in $list { ... }
```

<h4 style="font-family: Roboto">
<code>maps</code>
</h4>

```scss
$map: (key1: value1, key2: value2, key3: value3);

map-get($map, key1)
```