# 1️⃣ `px` (Pixel)

**Definition:**
`px` is a **fixed unit** in CSS.

It does **not depend on screen size or parent element**.

### Example

```css
.box{
width: 200px;
height: 100px;
}
```

Meaning:

```
width = 200 pixels
height = 100 pixels
```

### Characteristics

* Fixed size
* Does not change with screen size
* Easy to control layout

### Example

```css
h1{
font-size: 24px;
}
```

---

# 2️⃣ `%` (Percentage)

**Definition:**
Percentage is **relative to the parent element**.

### Example

```css
.parent{
width: 500px;
}

.child{
width: 50%;
}
```

Result:

```
child width = 250px
```

Because:

```
50% of 500px = 250px
```

### Characteristics

* Depends on **parent size**
* Good for **responsive layout**

Example:

```css
img{
width: 100%;
}
```

Meaning image fills **entire parent width**.

---

# 3️⃣ `vh` (Viewport Height)

**Definition:**
`vh` is based on **browser screen height**.

```
1vh = 1% of viewport height
```

### Example

```css
.hero{
height: 100vh;
}
```

Meaning:

```
Hero section = full screen height
```

### Example Screen

If screen height = **900px**

```
100vh = 900px
50vh = 450px
```

### Usage

Used in:

* hero sections
* landing pages
* full screen layouts

---

# 4️⃣ `vw` (Viewport Width)

**Definition:**

```
1vw = 1% of viewport width
```

### Example

```css
.box{
width: 50vw;
}
```

If screen width = **1200px**

```
50vw = 600px
```

### Usage

Used for:

* responsive layouts
* full width sections

---

# 5️⃣ `rem` (Root EM)

**Definition:**
`rem` is relative to the **root element (`html`) font size**.

Default browser font size:

```
html = 16px
```

### Example

```css
h1{
font-size: 2rem;
}
```

Calculation:

```
2 × 16px = 32px
```

### Example

```css
html{
font-size: 20px;
}

p{
font-size: 2rem;
}
```

Result:

```
2 × 20px = 40px
```

### Advantages

* Consistent sizing
* Easy scaling
* Good for accessibility

---

# 6️⃣ `em`

**Definition:**
`em` is relative to the **parent element's font size**.

### Example

```css
.parent{
font-size: 20px;
}

.child{
font-size: 2em;
}
```

Result:

```
2 × 20px = 40px
```

### Nested Example

```css
.parent{
font-size:20px;
}

.child{
font-size:2em;
}

.grandchild{
font-size:2em;
}
```

Calculation:

```
child = 40px
grandchild = 80px
```

Because `em` multiplies again.

### Problem

`em` can become **too large in nested elements**.

---

# 📊 Quick Comparison

| Unit | Based On         | Example        |
| ---- | ---------------- | -------------- |
| px   | Fixed size       | width:200px    |
| %    | Parent element   | width:50%      |
| vh   | Viewport height  | height:100vh   |
| vw   | Viewport width   | width:50vw     |
| rem  | Root font size   | font-size:2rem |
| em   | Parent font size | font-size:2em  |

---

# 🎯 When To Use What

### Use `px`

* borders
* small spacing
* icons

### Use `%`

* flexible layouts

### Use `vh / vw`

* full screen sections

### Use `rem`

* font sizes
* scalable design

### Use `em`

* component based scaling

---
