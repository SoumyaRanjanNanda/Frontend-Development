# CSS Font Properties

## 1. Font Family

### Definition

`font-family` specifies the **typeface (style of text)** used in the webpage.

### Example

```css
p{
  font-family: Arial, sans-serif;
}
```

### Key Point

* Multiple fonts can be provided as **fallback options**.

---

## 2. Font Style

### Definition

`font-style` specifies the **style of the text**.

### Values

* `normal`
* `italic`
* `oblique`

### Example

```css
p{
  font-style: italic;
}
```

---

## 3. Font Weight

### Definition

`font-weight` controls the **thickness (boldness) of the text**.

### Values

* `normal`
* `bold`
* `100 – 900`

### Example

```css
p{
  font-weight: bold;
}
```

---

## 4. Font Size (Height)

### Definition

`font-size` controls the **size or height of the text**.

### Example

```css
p{
  font-size: 20px;
}
```

### Units

* `px`
* `em`
* `rem`
* `%`

---

## 5. Letter Spacing

### Definition

`letter-spacing` controls the **space between letters**.

### Example

```css
p{
  letter-spacing: 2px;
}
```

---

## 6. Word Spacing

### Definition

`word-spacing` controls the **space between words**.

### Example

```css
p{
  word-spacing: 5px;
}
```

---

# CSS Text Properties

## 1. Text Align

### Definition

`text-align` controls the **horizontal alignment of text**.

### Values

* `left`
* `right`
* `center`
* `justify`

### Example

```css
p{
  text-align: center;
}
```

---

## 2. Text Transform

### Definition

`text-transform` changes the **case of text**.

### Values

* `uppercase`
* `lowercase`
* `capitalize`

### Example

```css
p{
  text-transform: uppercase;
}
```

---

## 3. Text Decoration

### Definition

`text-decoration` adds **decorative lines to text**.

### Values

* `underline`
* `overline`
* `line-through`
* `none`

### Example

```css
p{
  text-decoration: underline;
}
```

---

## 4. Text Shadow

### Definition

`text-shadow` adds **shadow effect to text**.

### Syntax

```css
text-shadow: horizontal vertical blur color;
```

### Example

```css
h1{
  text-shadow: 2px 2px 5px gray;
}
```

---

# Quick Example

```css
p{
  font-family: Arial;
  font-size: 18px;
  font-weight: bold;
  letter-spacing: 1px;
  word-spacing: 3px;
  text-align: center;
  text-transform: capitalize;
}
```

---

# One Powerful Line

**Font properties control the appearance of text, while text properties control the formatting and alignment of text.**

---
