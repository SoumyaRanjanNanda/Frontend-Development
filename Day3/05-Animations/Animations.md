**CSS Animation** lets you animate HTML elements without JavaScript by changing CSS properties over time. It works mainly with **`@keyframes`** and **animation properties**.

---

# 1. Basic CSS Animation Structure

```css
@keyframes example {
  from {
    background-color: red;
  }
  to {
    background-color: yellow;
  }
}

.box {
  width: 100px;
  height: 100px;
  background: red;
  animation: example 2s infinite;
}
```

**Explanation**

* `@keyframes example` → defines animation
* `from` → starting state
* `to` → ending state
* `animation` → applies animation to the element
* `2s` → duration
* `infinite` → repeats forever

---

# 2. HTML Example

```html
<!DOCTYPE html>
<html>
<head>
<style>

@keyframes moveBox {
  from { left: 0px; }
  to { left: 300px; }
}

.box {
  width: 100px;
  height: 100px;
  background: blue;
  position: relative;
  animation: moveBox 3s infinite;
}

</style>
</head>

<body>

<div class="box"></div>

</body>
</html>
```

This moves the box **from left to right continuously**.

---

# 3. Animation Properties

| Property                    | Description                  |
| --------------------------- | ---------------------------- |
| `animation-name`            | Name of keyframes            |
| `animation-duration`        | How long animation runs      |
| `animation-delay`           | Delay before animation       |
| `animation-iteration-count` | Number of repeats            |
| `animation-direction`       | Normal / reverse             |
| `animation-timing-function` | Speed curve                  |
| `animation-fill-mode`       | Style before/after animation |

Example:

```css
animation: moveBox 3s ease-in-out 1s infinite alternate;
```

---

# 4. Keyframes with Multiple Steps

```css
@keyframes colorChange {
  0%   { background: red; }
  50%  { background: blue; }
  100% { background: green; }
}
```

Apply:

```css
.box {
  animation: colorChange 4s infinite;
}
```

---

# 5. Hover Animation Example

```css
button {
  padding: 10px 20px;
  background: blue;
  color: white;
  transition: transform 0.3s;
}

button:hover {
  transform: scale(1.2);
}
```

When hovering, the button **zooms smoothly**.

---

# 6. Simple Loading Animation

```css
.loader {
  width: 40px;
  height: 40px;
  border: 5px solid lightgray;
  border-top: 5px solid blue;
  border-radius: 50%;
  animation: spin 1s linear infinite;
}

@keyframes spin {
  100% { transform: rotate(360deg); }
}
```

---

✅ **In short**

CSS Animation =
`@keyframes` + `animation properties`

Used for:

* loaders
* hover effects
* page transitions
* UI interactions
* website animations

---
