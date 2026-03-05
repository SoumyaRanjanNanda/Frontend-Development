# CSS Selector

## Definition

A **CSS Selector** is used to **select HTML elements** so that CSS styles can be applied to them.

It tells the browser **which HTML element should be styled**.

---

# CSS Basic Syntax

```css
selector{
   property: value;
}
```

Example:

```css
h1{
   color: red;
}
```

* **h1 → Selector**
* **color → Property**
* **red → Value**

This means: **All `<h1>` elements will become red.**

---

# Example with HTML

```html
<!DOCTYPE html>
<html>
<head>
<style>

p{
   color: blue;
}

</style>
</head>

<body>

<p>Hello World</p>

</body>
</html>
```

### Output

The paragraph text becomes **blue**.

---

# Key Points

* Selector **targets HTML elements**.
* It tells CSS **where the style should apply**.
* Without selectors, CSS **cannot style elements**.

---


# Types of CSS Selectors

## 1. Element Selector

### Definition

The **Element Selector** selects HTML elements **by their tag name**.

### Example

```css
p{
   color: blue;
}
```

This means **all `<p>` elements will be blue**.

### HTML Example

```html
<p>Hello</p>
<p>Welcome</p>
```

Both paragraphs will become **blue**.

---

# 2. Class Selector

### Definition

The **Class Selector** selects elements using the **class attribute**.

Class selectors start with **`.` (dot)**.

### Example

```css
.title{
   color: red;
}
```

### HTML

```html
<h1 class="title">Hello</h1>
```

The heading becomes **red**.

### Key Point

A **class can be used multiple times**.

---

# 3. ID Selector

### Definition

The **ID Selector** selects an element using the **id attribute**.

It starts with **`#` (hash)**.

### Example

```css
#header{
   color: green;
}
```

### HTML

```html
<h1 id="header">Welcome</h1>
```

### Key Point

An **ID should be unique** (used only once in a page).

---

# 4. Universal Selector

### Definition

The **Universal Selector** selects **all elements** in the webpage.

It is written using `*`.

### Example

```css
*{
   margin: 0;
   padding: 0;
}
```

This applies style to **every element**.

---

# 5. Attribute Selector

### Definition

The **Attribute Selector** selects elements based on their **HTML attributes**.

### Example

```css
input[type="text"]{
   background-color: yellow;
}
```

### HTML

```html
<input type="text">
```

The input box will have **yellow background**.

---

# Quick Summary

| Selector  | Symbol   | Example         |
| --------- | -------- | --------------- |
| Element   | tag name | `p`             |
| Class     | `.`      | `.title`        |
| ID        | `#`      | `#header`       |
| Universal | `*`      | `*`             |
| Attribute | `[ ]`    | `[type="text"]` |

---


