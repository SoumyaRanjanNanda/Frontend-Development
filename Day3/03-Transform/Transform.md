# CSS Transform

## Definition

The **`transform` property** in CSS is used to **change the position, size, rotation, or shape of an element** without affecting the normal layout.

It is widely used for **animations, hover effects, and modern UI design**.

---

# 1. Translate (Move Element)

## Definition

`translate()` moves an element **from its original position**.

![Image](https://www.freecodecamp.org/news/content/images/2023/06/cartesian-coordinate-system-perspective-method-illustration-codesweetly.png)

![Image](https://i.sstatic.net/5d7n2.png)

![Image](https://codescracker.com/css/images/css-translatey-function.jpg)

![Image](https://static.d-libro.com/01-course-content-images/1011-11-HTML-CSS-Coding-with-AI/030-topic-og-images/translate-function-in-css-repositioning-html-elements-id101111040910.png)

### Example

```css
div{
  transform: translate(50px, 30px);
}
```

Meaning:

* Move **50px right**
* Move **30px down**

---

# 2. Rotate

## Definition

`rotate()` rotates an element **clockwise or anticlockwise**.

![Image](https://i.sstatic.net/QACww.png)

![Image](https://static.d-libro.com/01-course-content-images/1011-11-HTML-CSS-Coding-with-AI/010-main-figures/rotate-function-in-css-rotating-html-elements-id101111041010.webp)

![Image](https://i.sstatic.net/eBgcJ.png)

![Image](https://www.scaler.com/topics/images/css-rotate-thumbnail.webp)

### Example

```css
div{
  transform: rotate(45deg);
}
```

The element rotates **45 degrees**.

---

# 3. Scale

## Definition

`scale()` changes the **size of an element**.

![Image](https://i.sstatic.net/M7VbU.png)

![Image](https://www.w3.org/TR/css-transforms-1/examples/svg-translate1.svg)

![Image](https://miro.medium.com/v2/resize%3Afit%3A1400/1%2AKpR9CEx-bm_sMmUgQ2kjAQ.png)

![Image](https://scaler.com/topics/images/what-is-css-2d-transform.webp)

### Example

```css
div{
  transform: scale(1.5);
}
```

Meaning
Element becomes **1.5 times bigger**.

---

# 4. Skew

## Definition

`skew()` tilts the element **along the X or Y axis**.

![Image](https://i.sstatic.net/KNLE4.jpg)

![Image](https://scaler.com/topics/images/what-is-css-2d-transform.webp)

![Image](https://codesweetly.com/_astro/cartesian-coordinate-system-two-dimensional-diagram-codesweetly.C5cuHhSB_Z1tYNn.webp)

![Image](https://i.sstatic.net/paFvg.png)

### Example

```css
div{
  transform: skew(20deg);
}
```

The element becomes **slanted/tilted**.

---

# Combined Transform Example

```css
div{
  transform: translate(50px,20px) rotate(20deg) scale(1.2);
}
```

This will:

* Move the element
* Rotate it
* Increase its size

---

# Quick Summary

| Transform   | Purpose         |
| ----------- | --------------- |
| translate() | moves element   |
| rotate()    | rotates element |
| scale()     | resizes element |
| skew()      | tilts element   |

---

# One Powerful Line

**CSS transform allows developers to move, rotate, scale, and skew elements to create dynamic UI effects.**

---




