# CSS Borders

## Definition

A **border** is the **line surrounding an HTML element**.
It is placed **between padding and margin** in the CSS box model.

---

# 1. Border Width

## Definition

`border-width` controls the **thickness of the border**.

### Example

```css
div{
  border-width: 4px;
}
```

### Values

* `thin`
* `medium`
* `thick`
* `px` values (e.g., `2px`, `5px`)

---

# 2. Border Style

## Definition

`border-style` defines the **appearance of the border line**.

### Common Values

* `solid`
* `dashed`
* `dotted`
* `double`
* `groove`
* `ridge`
* `none`

### Example

```css
div{
  border-style: solid;
}
```

---

# 3. Border Color

## Definition

`border-color` sets the **color of the border**.

### Example

```css
div{
  border-color: red;
}
```

You can use:

* color name → `red`
* HEX → `#ff0000`
* RGB → `rgb(255,0,0)`

---

# 4. Border Radius

## Definition

`border-radius` is used to **create rounded corners**.

### Example

```css
div{
  border-radius: 10px;
}
```

### Result

Corners become **rounded instead of sharp**.

---

# Combined Border Example

```css
div{
  border-width: 3px;
  border-style: solid;
  border-color: blue;
}
```

---

# Short Border Property (Shorthand)

Instead of writing 3 lines, we can write **one line**.

```css
div{
  border: 3px solid blue;
}
```

---

# Rounded Button Example

```css
button{
  border: 2px solid black;
  border-radius: 20px;
}
```

This creates a **rounded button border**.

---

# Quick Summary

| Property      | Meaning              |
| ------------- | -------------------- |
| border-width  | thickness of border  |
| border-style  | appearance of border |
| border-color  | color of border      |
| border-radius | rounded corners      |

---

# One Powerful Line

**Borders define the visible boundary of an HTML element and help structure webpage layout.**

---
