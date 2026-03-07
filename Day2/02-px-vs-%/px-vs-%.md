# px vs % in CSS

## 1. px (Pixels)

### Definition

`px` is a **fixed unit** used to define **exact size** in CSS.

It does **not change based on screen size**.

### Example

```css
div{
  width: 300px;
  height: 200px;
}
```

### Meaning

* Width = **300 pixels**
* Height = **200 pixels**

### Key Points

* Fixed size
* Does **not depend on parent element**
* Used for **precise design**

---

# 2. % (Percentage)

### Definition

`%` is a **relative unit** that defines size **relative to the parent element**.

### Example

```css
div{
  width: 50%;
}
```

### Meaning

The element takes **50% of the parent element's width**.

---

# Example

```html
<div class="parent">
   <div class="child"></div>
</div>
```

```css
.parent{
  width: 400px;
  height: 200px;
  background: lightgray;
}

.child{
  width: 50%;
  height: 100px;
  background: blue;
}
```

### Result

Child width = **200px**
because **50% of 400px = 200px**

---

# Difference Between px and %

| Feature           | px             | %               |
| ----------------- | -------------- | --------------- |
| Type              | Fixed unit     | Relative unit   |
| Depends on parent | No             | Yes             |
| Responsive        | No             | Yes             |
| Usage             | precise layout | flexible layout |

---

# When to Use

### Use **px**

* Borders
* Small elements
* Exact spacing

### Use **%**

* Layout
* Responsive design
* Flexible width

---

# One Powerful Line

**px gives fixed size, while % creates flexible and responsive layouts.**

