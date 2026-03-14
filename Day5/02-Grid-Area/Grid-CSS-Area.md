### CSS **`grid-area`** (CSS Grid)

In **CSS Grid Layout**, `grid-area` is used to **place a grid item in a specific position inside the grid**.

It can do two things:

1. **Assign a name to an area**
2. **Place an item using row/column lines**

---

# 1️⃣ Basic Meaning

`grid-area` tells **where the item should appear in the grid layout**.

Syntax:

```css
grid-area: row-start / column-start / row-end / column-end;
```

---

# 2️⃣ Example

### HTML

```html
<div class="container">
  <div class="box1">1</div>
  <div class="box2">2</div>
  <div class="box3">3</div>
</div>
```

### CSS

```css
.container{
  display: grid;
  grid-template-columns: 100px 100px 100px;
  grid-template-rows: 100px 100px;
  gap: 10px;
}

.box1{
  background: red;
  grid-area: 1 / 1 / 2 / 3;
}

.box2{
  background: blue;
}

.box3{
  background: green;
}
```

### Meaning of

```css
grid-area: 1 / 1 / 2 / 3;
```

| Value | Meaning      |
| ----- | ------------ |
| 1     | row start    |
| 1     | column start |
| 2     | row end      |
| 3     | column end   |

So **box1 spans across 2 columns**.

---

# 3️⃣ Visual Example

Grid:

```
| 1 | 2 | 3 |
| 4 | 5 | 6 |
```

If we write

```css
grid-area: 1 / 1 / 3 / 3;
```

It will cover:

```
| box | box | 3 |
| box | box | 6 |
```

---

# 4️⃣ Named Grid Area (Very Important)

You can create **named layout sections**.

### CSS

```css
.container{
  display: grid;

  grid-template-areas:
  "header header"
  "sidebar content"
  "footer footer";
}
```

### Items

```css
.header{
  grid-area: header;
}

.sidebar{
  grid-area: sidebar;
}

.content{
  grid-area: content;
}

.footer{
  grid-area: footer;
}
```

---

# 5️⃣ Real Website Layout Example

```
-------------------
|     HEADER      |
-------------------
| SIDEBAR | MAIN  |
-------------------
|     FOOTER      |
-------------------
```

This is **very common in website layouts**.

---

# 6️⃣ Shortcut

Instead of writing:

```css
grid-row-start:1;
grid-column-start:1;
grid-row-end:2;
grid-column-end:3;
```

You can write:

```css
grid-area: 1 / 1 / 2 / 3;
```

---
