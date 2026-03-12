Soumya, since you are learning **CSS deeply for building stylish responsive websites**, the **next topic after Flexbox** should be **CSS Grid**.
Flexbox is for **1-dimensional layouts**, while Grid is for **2-dimensional layouts** (rows + columns). Modern websites use **Flexbox + Grid together**.

---

# Next Topic: CSS Grid

![Image](https://www.w3.org/TR/2017/CR-css-grid-1-20170209/images/auto-flow.svg)

![Image](https://www.programiz.com/sites/tutorial2program/files/css-grid-container.png)

![Image](https://miro.medium.com/0%2Aog90_m1gsg9iOY7i.png)

![Image](https://paper-attachments.dropbox.com/s_CF11FE1AEA43B692C216C3C654FC1C4F2481FE1BD5D05FA13CF8348052371C18_1642184415008_template-columns-rows-01.svg)

## 1. Grid Container

To create a grid layout:

```css
.container{
display: grid;
}
```

Example:

```html
<div class="container">
<div class="box">1</div>
<div class="box">2</div>
<div class="box">3</div>
<div class="box">4</div>
</div>
```

---

# 2. grid-template-columns

Defines **number of columns**

```css
grid-template-columns: 200px 200px 200px;
```

Example:

```css
.container{
display:grid;
grid-template-columns:200px 200px 200px;
}
```

OR responsive way:

```css
grid-template-columns: repeat(3,1fr);
```

Meaning:

```
3 equal columns
```

---

# 3. grid-template-rows

Defines **rows**

```css
grid-template-rows: 100px 200px;
```

---

# 4. gap

Space between grid items

```css
gap:20px;
```

Example

```css
.container{
display:grid;
grid-template-columns:repeat(3,1fr);
gap:20px;
}
```

---

# 5. grid-column

Item spans multiple columns

```css
.box1{
grid-column:1 / 3;
}
```

Meaning

```
start column 1 → end column 3
```

---

# 6. grid-row

Span multiple rows

```css
.box1{
grid-row:1 / 3;
}
```

---

# 7. place-items (center easily)

```css
place-items:center;
```

Equivalent to:

```
align-items:center
justify-items:center
```

---

# Complete Example

```css
.container{
display:grid;
grid-template-columns:repeat(3,1fr);
gap:20px;
}

.box{
height:100px;
background:tomato;
}
```

---

# Flexbox vs Grid (Important)

| Flexbox       | Grid             |
| ------------- | ---------------- |
| 1D layout     | 2D layout        |
| Row OR column | Rows AND columns |
| Navbar        | Full page layout |
| Cards         | Dashboard        |

Example:

```
Navbar → Flexbox
Page layout → Grid
```

---
