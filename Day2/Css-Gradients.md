# CSS Gradients

Gradients are used to **create smooth transitions between two or more colors** without using images.
CSS mainly provides **two types of gradients**:

1. **Linear Gradient**
2. **Radial Gradient**

---

# 1. Linear Gradient

## Definition

A **linear gradient** creates a **color transition in a straight line** (top → bottom, left → right, or any angle).



![Image](https://media.licdn.com/dms/image/v2/D5612AQH3rS8Zeqy29w/article-cover_image-shrink_720_1280/article-cover_image-shrink_720_1280/0/1677765229622?e=2147483647\&t=jk-vrYE1ykpP4k5a4KwLM24BkYWhCZErAh-gT7MOAXo\&v=beta)


## Syntax

```css
background: linear-gradient(direction, color1, color2);
```

---

## Example

```css
div{
  height: 200px;
  width: 300px;
  background: linear-gradient(red, blue);
}
```

### Result

Color changes smoothly from **red → blue**.

---

## Direction Example

```css
background: linear-gradient(to right, red, yellow);
```

Possible directions:

* `to right`
* `to left`
* `to top`
* `to bottom`
* `45deg` (angle)

---

# 2. Radial Gradient

## Definition

A **radial gradient** creates a **color transition from the center outward in a circular or elliptical shape**.

![Image](https://happycoding.io/tutorials/processing/for-loops/images/radial-gradient-2.png)


---

## Syntax

```css
background: radial-gradient(color1, color2);
```

---

## Example

```css
div{
  height: 200px;
  width: 300px;
  background: radial-gradient(red, yellow);
}
```

### Result

Color spreads **from center red → outer yellow**.

---

# Linear vs Radial Gradient

| Feature   | Linear Gradient          | Radial Gradient   |
| --------- | ------------------------ | ----------------- |
| Shape     | Straight line            | Circle / ellipse  |
| Direction | top, bottom, left, right | center outward    |
| Use       | backgrounds, buttons     | spotlight effects |

---

# Example Code (Both)

```css
.box1{
  background: linear-gradient(to right, red, blue);
}

.box2{
  background: radial-gradient(red, yellow);
}
```

---

# One Powerful Line

**Gradients allow developers to create beautiful color transitions without using image files.**

---
