# CSS 3D Transforms

## Definition

**CSS 3D Transforms** allow elements to **move, rotate, or scale in three-dimensional space (X, Y, Z axis)**.

It creates **depth and realistic animation effects** on web pages.

---

# 3D Axes in CSS



![Image](https://cdn-images-1.medium.com/max/1600/0%2AbxMneFPF6loTMIlI.png)



### Axes Explanation

| Axis   | Direction          |
| ------ | ------------------ |
| X-axis | left ↔ right       |
| Y-axis | up ↕ down          |
| Z-axis | forward ↔ backward |

---

# 1. rotateX()

## Definition

Rotates the element **along the X-axis** (tilting forward/backward).



![Image](https://www.frontend.fyi/article-images/perspective.webp)

![Image](https://miro.medium.com/1%2ApQePBD-OmFlkywwcssy6FA.gif)

![Image](https://www.html-code-generator.com/images/css/flip-animation.webp)

### Example

```css
div{
  transform: rotateX(45deg);
}
```

The element **tilts forward**.

---

# 2. rotateY()

## Definition

Rotates the element **along the Y-axis** (left/right rotation).

![Image](https://media.24ways.org/2010/desandro/card-flip01.png)

![Image](https://assets.htmlgoodies.com/uploads/2021/04/ss_transform.png)


![Image](https://codescracker.com/css/images/css-rotatey-example.jpg)

### Example

```css
div{
  transform: rotateY(45deg);
}
```

The element **rotates sideways**.

---

# 3. rotateZ()

## Definition

Rotates the element **around the Z-axis** (normal 2D rotation).

![Image](https://codesweetly.com/_astro/cartesian-coordinate-system-three-dimensional-diagram-codesweetly.D2iq30Vn_1syqpQ.webp)

![Image](https://codesweetly.com/_astro/cartesian-coordinate-system-three-dimensional-diagram-codesweetly.D2iq30Vn_ZLrLlL.webp)

![Image](https://raw.githubusercontent.com/Codecademy/docs/main/media/css-rotateZ.png)

![Image](https://codesweetly.com/og/css-rotatez-function.png)

### Example

```css
div{
  transform: rotateZ(45deg);
}
```

The element **spins like a wheel**.

---

# 4. translateZ()

## Definition

Moves the element **towards or away from the viewer**.



![Image](https://assets.digitalocean.com/articles/alligator/css/translatez-and-perspective/user-and-laptop-translatez.png)

![Image](https://raw.githubusercontent.com/Codecademy/docs/main/media/css-translateZ-pos.png)

![Image](https://codesweetly.com/_astro/cartesian-coordinate-system-three-dimensional-diagram-codesweetly.D2iq30Vn_1syqpQ.webp)

### Example

```css
div{
  transform: translateZ(50px);
}
```

The element moves **forward in 3D space**.

---

# Perspective (Important)

To see 3D effects clearly we use **perspective**.

```css
.container{
  perspective: 800px;
}
```

This adds **depth to the scene**.

---

# Example

```css
.container{
  perspective: 800px;
}

.box{
  width: 150px;
  height: 150px;
  background: blue;
  transform: rotateY(45deg);
}
```

This creates a **3D rotating box effect**.

---

# Quick Summary

| Property     | Effect            |
| ------------ | ----------------- |
| rotateX()    | tilt forward/back |
| rotateY()    | rotate sideways   |
| rotateZ()    | spin element      |
| translateZ() | move in depth     |
| perspective  | adds 3D depth     |

---

# One Powerful Line

**CSS 3D transforms allow elements to move and rotate in three-dimensional space for advanced visual effects.**

---

