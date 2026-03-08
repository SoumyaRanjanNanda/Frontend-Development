# CSS Transitions

## Definition

A **CSS Transition** allows an element to **change from one style to another smoothly over time**.

Instead of changing **instantly**, the change happens **gradually with animation**.

---

# Basic Idea

Without transition → change happens **immediately**
With transition → change happens **smoothly**

![Image](https://cdn.outrank.so/9baff5d7-bb14-4bc7-8399-349ad7704876/5fd73d23-66c1-4ebd-8d6a-aff2893936e4/css-buttons-hover-button-states.jpg)

![Image](https://joshcollinsworth.com/images/post_images/great-transitions.png)


---

# Syntax

```css
transition: property duration timing-function delay;
```

Example:

```css
transition: background 0.5s;
```

Meaning
Background color will change **in 0.5 seconds smoothly**.

---

# Example

### HTML

```html
<button>Hover Me</button>
```

### CSS

```css
button{
  background: red;
  transition: background 0.5s;
}

button:hover{
  background: blue;
}
```

### Result

When you hover on the button:

Red → Blue **smoothly in 0.5 seconds**.

---

# Important Transition Properties

| Property                     | Purpose                       |
| ---------------------------- | ----------------------------- |
| `transition-property`        | which property will animate   |
| `transition-duration`        | animation time                |
| `transition-timing-function` | animation speed style         |
| `transition-delay`           | delay before animation starts |

---

# Example with All Properties

```css
div{
  width: 100px;
  height: 100px;
  background: red;

  transition-property: width;
  transition-duration: 1s;
  transition-timing-function: ease;
}
```

When width changes → it **animates smoothly in 1 second**.

---

# Timing Functions

| Value         | Effect             |
| ------------- | ------------------ |
| `linear`      | same speed         |
| `ease`        | slow start and end |
| `ease-in`     | slow start         |
| `ease-out`    | slow end           |
| `ease-in-out` | slow start and end |

---

# Hover Animation Example

```css
.box{
  width: 100px;
  height: 100px;
  background: blue;
  transition: transform 0.5s;
}

.box:hover{
  transform: scale(1.2);
}
```

When hovering → **box grows smoothly**.

---

# One Powerful Line

**CSS transitions create smooth animations when a property changes.**

---





