# CSS Background Properties

## Definition

**Background properties** are used to **control the background appearance of an HTML element**.

---

## 1. Background Color

### Definition

`background-color` sets the **background color of an element**.

### Example

```css
div{
  background-color: lightblue;
}
```

---

## 2. Background Image

### Definition

`background-image` sets an **image as the background**.

### Example

```css
div{
  background-image: url("image.jpg");
}
```

---

## 3. Background Size

### Definition

`background-size` controls the **size of the background image**.

### Values

* `cover`
* `contain`
* `px` values

### Example

```css
div{
  background-size: cover;
}
```

---

## 4. Background Position

### Definition

`background-position` controls **where the background image appears**.

### Example

```css
div{
  background-position: center;
}
```

### Common Values

* `top`
* `bottom`
* `left`
* `right`
* `center`

---

## 5. Background Repeat

### Definition

`background-repeat` controls **whether the background image repeats**.

### Values

* `repeat`
* `no-repeat`
* `repeat-x`
* `repeat-y`

### Example

```css
div{
  background-repeat: no-repeat;
}
```

---

## 6. Linear Gradient

### Definition

A **linear gradient** creates a **smooth color transition** between two or more colors.

### Example

```css
div{
  background: linear-gradient(red, blue);
}
```

This creates a **red → blue gradient background**.

---

# Quick Example

```css
div{
  background-color: lightblue;
  background-image: url("bg.jpg");
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  
}
```

---

# Quick Summary

| Property            | Purpose                  |
| ------------------- | ------------------------ |
| background-color    | sets background color    |
| background-image    | sets image background    |
| background-size     | controls image size      |
| background-position | controls image position  |
| background-repeat   | controls image repeating |
| linear-gradient     | gradient background      |

