# CSS Color Representation

## Definition

**Color representation** in CSS means the **different ways to define colors** for HTML elements.

CSS allows colors to be written in **multiple formats**.

---

# 1. Color Name

### Definition

Using **predefined color names** provided by CSS.

### Example

```css
p{
  color: red;
}
```

### Common Color Names

* red
* blue
* green
* black
* white
* yellow

---

# 2. HEX Color

### Definition

HEX represents color using **hexadecimal numbers**.

### Format

```
#RRGGBB
```

* RR → Red
* GG → Green
* BB → Blue

### Example

```css
p{
  color: #ff0000;
}
```

This represents **red**.

---

# 3. RGB Color

### Definition

RGB stands for **Red, Green, Blue**.

Each value ranges from **0 to 255**.

### Example

```css
p{
  color: rgb(255,0,0);
}
```

This also represents **red**.

---

# 4. RGBA Color

### Definition

RGBA is similar to RGB but includes **Alpha (opacity)**.

### Format

```
rgba(red, green, blue, alpha)
```

Alpha value ranges from **0 to 1**.

### Example

```css
p{
  color: rgba(255,0,0,0.5);
}
```

This creates **semi-transparent red**.

---

# 5. HSL Color

### Definition

HSL stands for:

* **H → Hue (color type)**
* **S → Saturation**
* **L → Lightness**

### Example

```css
p{
  color: hsl(0,100%,50%);
}
```

This also represents **red**.

---

# Quick Summary

| Method     | Example             |
| ---------- | ------------------- |
| Color Name | `red`               |
| HEX        | `#ff0000`           |
| RGB        | `rgb(255,0,0)`      |
| RGBA       | `rgba(255,0,0,0.5)` |
| HSL        | `hsl(0,100%,50%)`   |

---
