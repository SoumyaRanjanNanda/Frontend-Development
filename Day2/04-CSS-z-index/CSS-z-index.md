# CSS z-index

## Definition

`z-index` controls the **vertical stacking order of elements** when they overlap.

It decides **which element appears in front and which appears behind**.

---

## How It Works

* Elements with **higher z-index appear on top**.
* Elements with **lower z-index appear behind**.

Example:

```
z-index: 5  → front
z-index: 1  → back
```

---

## Important Rule

`z-index` **only works on positioned elements**, meaning the element must have:

```
position: relative
position: absolute
position: fixed
position: sticky
```

It **does not work with `position: static`**.

---

# Example

### HTML

```html
<div class="box1"></div>
<div class="box2"></div>
```

### CSS

```css
.box1{
  width: 200px;
  height: 200px;
  background: red;
  position: absolute;
  z-index: 1;
}

.box2{
  width: 200px;
  height: 200px;
  background: blue;
  position: absolute;
  top: 50px;
  left: 50px;
  z-index: 2;
}
```

### Result

* **Blue box appears on top**
* **Red box appears behind**

because **z-index of blue = 2 > red = 1**

---

# Visual Idea

```
z-index:3   🔵 (Top Layer)

z-index:2   🟢

z-index:1   🔴 (Bottom Layer)
```

---

# Key Points

* Controls **stacking order of elements**
* Higher value = **closer to the viewer**
* Works only with **positioned elements**

---

# One Powerful Line

**`z-index` controls the stacking order of overlapping elements in CSS.**

---

