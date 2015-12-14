# CSS Counter Styles for Telugu

The [CSS Counter Styles Level 3](http://www.w3.org/TR/css-counter-styles-3/) module defines only [numeric style for Telugu](http://dev.w3.org/csswg/css-counter-styles/#valdef-counter-style-name-telugu). This project aims to collect all counter styles needed for Telugu.

**NOTE**: As of December 2015, only Firefox supports user-defined `@counter-style` rules. So, these rules do not (yet) work on other browsers.

## Base counter styles

### Numeric (`telugu`)

```css
@counter-style telugu {
  system: numeric;
  symbols: '౦' '౧' '౨' '౩' '౪' '౫' '౬' '౭' '౮' '౯';
}
```
*NOTE*: This rule is specified in the specification. So, major browsers may include it as built-in.


### Alphabetic (`telugu-alphabetic`)

```css
@counter-style telugu-alphabetic {
  system: alphabetic;
  symbols: 'అ' 'ఆ' 'ఇ' 'ఈ' 'ఉ' 'ఊ' 'ఎ' 'ఏ' 'ఐ' 'ఒ' 'ఓ' 'ఔ' 'అం' 'అః' 'క' 'ఖ' 'గ' 'ఘ' 'ఙ' 'చ' 'ఛ' 'జ' 'ఝ' 'ఞ' 'ట' 'ఠ' 'డ' 'ఢ' 'ణ' 'త' 'థ' 'ద' 'ధ' 'న' 'ప' 'ఫ' 'బ' 'భ' 'మ' 'య' 'ర' 'ల' 'వ' 'శ' 'ష' 'స' 'హ' 'ళ' 'క్ష' 'ఱ';
}
```

## Extended counter styles

The base counter styles can be [exteded](http://www.w3.org/TR/css-counter-styles-3/#extends-system) to style with right parenthis `అ)` or surrounded parentheses `(అ)`.

### Numeric with right paren (`telugu-right-paren`)

```css
@counter-style telugu-right-paren {
  system: extends telugu;
  suffix: ") ";
}
```

### Numeric with surrounded parens (`telugu-parens-around`)

```css
@counter-style telugu-parens-around {
  system: extends telugu;
  prefix: "(";
  suffix: ") ";
}
```

### Alphabetic with right paren (`telugu-alphabetic-right-paren`)

```css
@counter-style telugu-alphabetic-right-paren {
  system: extends telugu-alphabetic;
  suffix: ") ";
}
```

### Alphabetic with surrounded parens (`telugu-alphabetic-parens-around`)

```css
@counter-style telugu-alphabetic-parens-around {
  system: extends telugu-alphabetic;
  prefix: "(";
  suffix: ") ";
}
```
