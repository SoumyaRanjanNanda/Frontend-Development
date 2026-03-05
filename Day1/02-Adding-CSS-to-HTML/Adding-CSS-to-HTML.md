# Adding CSS to HTML

CSS can be added to an HTML document in **three different ways**.

---

# 1. Inline CSS

## Definition

**Inline CSS** is written **directly inside an HTML tag** using the `style` attribute.

## Example

```html
<h1 style="color: red;">Hello World</h1>
```

### Explanation

* `style` → attribute
* `color` → CSS property
* `red` → value

### Key Points

* Applied to **one element only**
* **Highest priority**
* Not recommended for large websites

---

# 2. Internal CSS

## Definition

**Internal CSS** is written inside the **`<style>` tag** in the `<head>` section of an HTML document.

## Example

```html
<!DOCTYPE html>
<html>
<head>

<style>
h1{
  color: blue;
}

p{
  font-size: 20px;
}

</style>

</head>

<body>

<h1>Hello</h1>
<p>This is a paragraph</p>

</body>
</html>
```

### Key Points

* Used for **styling a single webpage**
* Written inside the **`<style>` tag**
* Placed in the **head section**

---

# 3. External CSS (Best Method)

## Definition

**External CSS** is written in a **separate `.css` file** and linked to the HTML file.

## Example

### HTML File

```html
<link rel="stylesheet" href="style.css">
```

### CSS File (style.css)

```css
h1{
  color: green;
}
```

### Key Points

* **Best practice for real websites**
* One CSS file can style **many HTML pages**
* Code becomes **clean and reusable**

---