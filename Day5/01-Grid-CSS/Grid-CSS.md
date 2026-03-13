## CSS Grid

![Image](https://miro.medium.com/0%2Aog90_m1gsg9iOY7i.png)

![Image](https://www.programiz.com/sites/tutorial2program/files/css-grid-container.png)

![Image](https://miro.medium.com/0%2A9Ncg_Yr5IiW5Z_E5.png)

![Image](https://www.tutorialspoint.com/css/images/css-grid.jpg)

**CSS Grid** is a **2-dimensional layout system** in CSS used to create layouts with **rows and columns**.

It helps you design **complex responsive layouts easily**, like dashboards, galleries, or full website layouts.

Unlike **Flexbox (1D → row OR column)**, **Grid works in 2D → row AND column together**.

---

# 1. Grid Container

To start using Grid, you apply `display: grid` to the **parent element**.

```css
.container{
  display: grid;
}
```

Example:

```html
<div class="container">
  <div>1</div>
  <div>2</div>
  <div>3</div>
</div>
```

Here:

* `.container` → **Grid container**
* inner `div`s → **Grid items**

---

# 2. grid-template-columns

Defines **number and size of columns**.

```css
.container{
  display: grid;
  grid-template-columns: 100px 100px 100px;
}
```

Result:

```
|100px|100px|100px|
```

Example responsive:

```css
grid-template-columns: 1fr 1fr 1fr;
```

`fr` = **fraction of available space**

Example:

```
| 1fr | 1fr | 1fr |
```

3 equal columns.

---

# 3. grid-template-rows

Defines **row size**.

```css
grid-template-rows: 100px 200px;
```

Result:

```
Row1 → 100px
Row2 → 200px
```

---

# 4. gap

Space between rows and columns.

```css
gap: 20px;
```

Example:

```css
.container{
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  gap: 20px;
}
```

---

# 5. grid-column

Make an item **span multiple columns**.

```css
.item1{
  grid-column: 1 / 3;
}
```

Meaning:

```
start column 1
end column 3
```

So it covers **2 columns**.

---

# 6. grid-row

Make an item span **multiple rows**.

```css
.item1{
  grid-row: 1 / 3;
}
```

---

# 7. repeat()

Instead of writing many columns manually.

```css
grid-template-columns: repeat(3, 1fr);
```

Same as:

```
1fr 1fr 1fr
```

---

# 8. minmax()

Set **minimum and maximum size**.

```css
grid-template-columns: repeat(3, minmax(200px, 1fr));
```

Meaning:

```
minimum = 200px
maximum = available space
```

Good for **responsive design**.

---

# 9. auto-fit / auto-fill (Responsive grids)

Example:

```css
grid-template-columns: repeat(auto-fit, minmax(200px,1fr));
```

Grid automatically adjusts columns based on screen size.

---

# 10. justify-items

Align items **horizontally**.

```css
justify-items: center;
```

Values:

```
start
center
end
stretch
```

---

# 11. align-items

Align items **vertically**.

```css
align-items: center;
```

---

# 12. place-items

Shortcut for both.

```css
place-items: center;
```

---

# Simple Example

```html
<div class="container">
  <div class="box">1</div>
  <div class="box">2</div>
  <div class="box">3</div>
  <div class="box">4</div>
</div>
```

```css
.container{
  display: grid;
  grid-template-columns: repeat(2,1fr);
  gap: 20px;
}

.box{
  background: pink;
  padding: 40px;
}
```

Result:

```
1   2
3   4
```

---

# Flexbox vs Grid

| Flexbox          | Grid              |
| ---------------- | ----------------- |
| 1D layout        | 2D layout         |
| Row OR Column    | Row AND Column    |
| Small UI layouts | Full page layouts |

Example:

```
Navbar → Flexbox
Full webpage layout → Grid
```

---

# For Stylish Websites (Important Grid Topics)

Soumya, since you want to build **stylish responsive websites**, focus on these:

1. `display: grid`
2. `grid-template-columns`
3. `grid-template-rows`
4. `gap`
5. `repeat()`
6. `minmax()`
7. `auto-fit / auto-fill`
8. `grid-column`
9. `grid-row`
10. `place-items`

*** Most Important ***
