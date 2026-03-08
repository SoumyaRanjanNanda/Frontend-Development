# CSS Transform

## Definition

The **`transform` property** in CSS is used to **change the position, size, rotation, or shape of an element** without affecting the normal layout.

It is widely used for **animations, hover effects, and modern UI design**.

---

# 1. Translate (Move Element)

## Definition

`translate()` moves an element **from its original position**.



![Image](https://i.sstatic.net/5d7n2.png)



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



![Image](https://static.d-libro.com/01-course-content-images/1011-11-HTML-CSS-Coding-with-AI/010-main-figures/rotate-function-in-css-rotating-html-elements-id101111041010.webp)



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



![Image](https://scaler.com/topics/images/what-is-css-2d-transform.webp)


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





