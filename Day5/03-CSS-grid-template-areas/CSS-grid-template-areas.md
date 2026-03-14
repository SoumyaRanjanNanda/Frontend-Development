## CSS **`grid-template-areas`**

In **CSS Grid Layout**, `grid-template-areas` is used to **define a layout structure using names** instead of numbers.
It makes complex layouts **very easy and readable**.

---

# 1️⃣ Basic Idea

Instead of using row/column numbers, you **name the areas** of the grid.

Example layout:

```
HEADER
SIDEBAR | CONTENT
FOOTER
```

---

# 2️⃣ Syntax

```css
grid-template-areas:
"area-name area-name"
"area-name area-name";
```

Each **word represents a grid area**.

---

# 3️⃣ Simple Example

### HTML

```html
<div class="container">
  <div class="header">Header</div>
  <div class="sidebar">Sidebar</div>
  <div class="content">Content</div>
  <div class="footer">Footer</div>
</div>
```

---

### CSS

```css
.container{
  display: grid;

  grid-template-columns: 200px 1fr;
  grid-template-rows: 80px 300px 80px;

  grid-template-areas:
  "header header"
  "sidebar content"
  "footer footer";
}

.header{
  grid-area: header;
  background: red;
}

.sidebar{
  grid-area: sidebar;
  background: blue;
}

.content{
  grid-area: content;
  background: green;
}

.footer{
  grid-area: footer;
  background: orange;
}
```

---

# 4️⃣ How it Works

```
grid-template-areas:

"header header"
"sidebar content"
"footer footer"
```

Grid becomes:

```
-------------------
|     header      |
-------------------
| sidebar |content|
-------------------
|     footer      |
-------------------
```

---

# 5️⃣ Important Rules

### 1️⃣ Same name merges columns

```
"header header"
```

Header **spans across 2 columns**

---

### 2️⃣ Dot (`.`) means empty space

Example:

```css
grid-template-areas:
"header header"
"sidebar ."
"footer footer";
```

Layout:

```
HEADER
SIDEBAR | empty
FOOTER
```

---

### 3️⃣ Every grid item must have `grid-area`

Example

```css
.header{
grid-area: header;
}
```

---

# 6️⃣ Why Developers Love It

Without `grid-template-areas`

```css
grid-area: 1 / 1 / 2 / 3;
```

Hard to remember.

With `grid-template-areas`

```css
grid-area: header;
```

Much **cleaner and readable**.

---

# 7️⃣ Real Website Layout Example

Common website layout:

```
NAVBAR
SIDEBAR | MAIN CONTENT
FOOTER
```

```css
grid-template-areas:
"nav nav"
"sidebar main"
"footer footer";
```

---

