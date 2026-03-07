# CSS `transform: translate(x, y)`

## Definition

`transform: translate(x, y)` is used to **move an element horizontally (X-axis) and vertically (Y-axis)** from its original position.

* **X value → horizontal movement**
* **Y value → vertical movement**

It **does not affect the document flow** (other elements stay in the same place).

---

# Visual Idea

![Image](https://getflywheel-images.s3.us-east-2.amazonaws.com/uploads/2017/03/css3-transitions-transforms-coordinate-basics.png)

![Image](https://www.w3.org/TR/css-transforms-1/examples/svg-translate1.svg)

![Image](https://user.oc-static.com/upload/2019/01/24/15483267462887_pt02ch02_08_dualRot_v001.gif)

![Image](https://static.d-libro.com/01-course-content-images/1011-11-HTML-CSS-Coding-with-AI/030-topic-og-images/translate-function-in-css-repositioning-html-elements-id101111040910.png)

---

# Syntax

```css
transform: translate(x, y);
```

Example values:

* `px`
* `%`
* `rem`

---

# Example 1

```css
div{
  transform: translate(50px, 30px);
}
```

### Meaning

* Move **50px right**
* Move **30px down**

---

# Example 2 (Negative Value)

```css
div{
  transform: translate(-40px, -20px);
}
```

### Meaning

* Move **40px left**
* Move **20px up**

---

# Example 3 (Percentage)

```css
div{
  transform: translate(50%, 50%);
}
```

### Meaning

Moves element **relative to its own size**.

---

# Complete Example

### HTML

```html
<div class="box"></div>
```

### CSS

```css
.box{
  width: 150px;
  height: 150px;
  background: blue;
  transform: translate(80px, 40px);
}
```

The box moves **80px right and 40px down**.

---

# X and Y Direction

```
       ↑
       Y-
       |
X- ----+---- X+
       |
       Y+
       ↓
```

* `translateX()` → horizontal move
* `translateY()` → vertical move

Example:

```css
transform: translateX(100px);
transform: translateY(50px);
```

---

# Key Points

* Moves element **without affecting layout**
* Can move **left, right, up, down**
* Used in **animations and UI effects**

---

# One Powerful Line

**`transform: translate()` moves elements smoothly without changing the layout structure.**



