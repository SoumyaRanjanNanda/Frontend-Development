# CSS Media Query

**Media Query** is used to make a **responsive website**.
It allows CSS to apply **different styles for different screen sizes** like **mobile, tablet, and desktop**.

---

# 1️⃣ Basic Syntax

```css
@media (condition) {
  CSS code
}
```

Example:

```css
@media (max-width: 600px){
  body{
    background-color: lightblue;
  }
}
```

Meaning:

```
If screen width ≤ 600px
then background becomes lightblue
```

---

# 2️⃣ Example of Media Query

```css
.box{
width: 400px;
height: 200px;
background-color: red;
}

@media (max-width: 600px){
.box{
width: 200px;
background-color: green;
}
}
```

Result:

* **Desktop** → Red box (400px)
* **Mobile** → Green box (200px)

---

# 3️⃣ Types of Media Queries

## 1. max-width

Used when screen size is **less than or equal to a value**.

```css
@media (max-width:768px){
body{
background-color: yellow;
}
}
```

Meaning:

```
Apply CSS when screen width ≤ 768px
```

Used for **mobile design**.

---

## 2. min-width

Used when screen size is **greater than or equal to a value**.

```css
@media (min-width:768px){
body{
background-color: pink;
}
}
```

Meaning:

```
Apply CSS when screen width ≥ 768px
```

Used for **tablet and desktop**.

---

# 4️⃣ Common Breakpoints (Important)

These are commonly used screen sizes.

| Device       | Width         |
| ------------ | ------------- |
| Mobile       | 0 – 480px     |
| Large Mobile | 481 – 768px   |
| Tablet       | 769 – 1024px  |
| Laptop       | 1025 – 1280px |
| Desktop      | 1281px +      |

Example:

```css
/* Mobile */
@media (max-width:480px){}

/* Tablet */
@media (max-width:768px){}

/* Laptop */
@media (max-width:1024px){}
```

---

# 5️⃣ Real Website Example

```css
.container{
width:1200px;
margin:auto;
}

@media (max-width:768px){

.container{
width:90%;
}

}
```

Meaning:

Desktop → `1200px`
Mobile → `90% width`

---

# 6️⃣ Multiple Conditions

You can combine conditions.

Example:

```css
@media (min-width:600px) and (max-width:900px){
body{
background-color: orange;
}
}
```

Meaning:

```
Apply CSS only between 600px and 900px
```

---

# 7️⃣ Orientation Media Query

Detects **portrait or landscape**.

```css
@media (orientation: landscape){
body{
background-color: lightgreen;
}
}
```

---

# 8️⃣ Where to Write Media Query

Usually written **at the bottom of CSS file**.

Example structure:

```css
/* Normal CSS */

body{
font-size:18px;
}

/* Media Query */

@media (max-width:768px){
body{
font-size:14px;
}
}
```

---

# 🎯 Why Media Query is Important

Media Queries help to make websites:

* Mobile friendly
* Tablet friendly
* Responsive
* Professional

Without Media Query → website **breaks on small screens**.

---

# 💡 Example Used in Real Websites

```css
@media (max-width:768px){

.navbar{
flex-direction: column;
}

}
```

Navbar becomes **vertical on mobile**.

---

