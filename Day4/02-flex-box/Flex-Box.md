## CSS Flexbox Notes (Beginner → Practical)

![Image](https://web.dev/static/learn/css/flexbox/image/a-labelled-diagram-the-a-a9bf061b5d5b2.svg)

![Image](https://samanthaming.gumlet.io/flexbox30/4-flexbox-axes.jpg.gz)

![Image](https://marina-ferreira.github.io/img/tutorials/css/flexbox/digest.png)

![Image](https://media.licdn.com/dms/image/v2/D4D12AQGNVLU6cbfwNA/article-cover_image-shrink_720_1280/article-cover_image-shrink_720_1280/0/1728904809763?e=2147483647\&t=sVSZOTgUbgeaBzSSspQUbpcvxLbXHcddnDDt9WEzNs4\&v=beta)

Flexbox (**Flexible Box Layout**) is a **CSS layout system** used to align and distribute items inside a container.

It makes **responsive layouts** easier compared to float or positioning.

---

# 1. Flex Container

The parent element becomes a **flex container** when you apply:

```css
display: flex;
```

Example:

```html
<div class="container">
  <div class="box">1</div>
  <div class="box">2</div>
  <div class="box">3</div>
</div>
```

```css
.container{
display:flex;
}
```

Now all children become **flex items**.

---

# 2. Main Axis and Cross Axis

Flexbox works on two directions.

**Main Axis**

* Direction where items move

**Cross Axis**

* Perpendicular direction

Example:

```
Row direction

Main Axis → (horizontal)

Cross Axis ↓ (vertical)
```

---

# 3. flex-direction

Controls **direction of items**

```css
flex-direction: row;
```

Types:

| Value          | Meaning                |
| -------------- | ---------------------- |
| row            | left → right (default) |
| row-reverse    | right → left           |
| column         | top → bottom           |
| column-reverse | bottom → top           |

Example:

```css
.container{
display:flex;
flex-direction: column;
}
```

---

# 4. justify-content

Align items **horizontally (main axis)**.

```css
justify-content: center;
```

Values:

| Value         | Meaning             |
| ------------- | ------------------- |
| flex-start    | start               |
| flex-end      | end                 |
| center        | center              |
| space-between | equal space between |
| space-around  | space around items  |
| space-evenly  | equal spacing       |

Example:

```css
.container{
display:flex;
justify-content:center;
}
```

---

# 5. align-items

Align items **vertically (cross axis)**.

```css
align-items: center;
```

Values:

| Value      | Meaning             |
| ---------- | ------------------- |
| stretch    | default             |
| flex-start | top                 |
| flex-end   | bottom              |
| center     | middle              |
| baseline   | align text baseline |

Example:

```css
.container{
display:flex;
align-items:center;
}
```

---

# 6. flex-wrap

Controls **wrapping of items**.

```css
flex-wrap: wrap;
```

Values:

| Value        | Meaning           |
| ------------ | ----------------- |
| nowrap       | default           |
| wrap         | move to next line |
| wrap-reverse | reverse wrap      |

Example:

```css
.container{
display:flex;
flex-wrap:wrap;
}
```

---

# 7. gap

Adds **space between flex items**.

```css
gap:20px;
```

Example:

```css
.container{
display:flex;
gap:20px;
}
```

---

# 8. align-content

Works when **multiple rows exist**.

```css
align-content:center;
```

Values:

* center
* flex-start
* flex-end
* space-between
* space-around
* space-evenly

---

# 9. flex property (for items)

Controls **size of flex items**.

```css
flex:1;
```

It is shorthand for:

```
flex-grow
flex-shrink
flex-basis
```

Example:

```css
.box{
flex:1;
}
```

Meaning → all items take **equal width**.

---

# 10. flex-grow

Controls how items **grow**.

```css
flex-grow:1;
```

Example:

```css
.box1{
flex-grow:2;
}

.box2{
flex-grow:1;
}
```

Box1 becomes **twice bigger**.

---

# 11. flex-shrink

Controls how items **shrink**.

```css
flex-shrink:1;
```

---

# 12. flex-basis

Initial size of item.

```css
flex-basis:200px;
```

Example:

```css
.box{
flex-basis:200px;
}
```

---

# 13. align-self

Overrides **align-items for a single item**.

```css
align-self:center;
```

Example:

```css
.box1{
align-self:flex-end;
}
```

---

# Complete Example

```html
<div class="container">
<div class="box">1</div>
<div class="box">2</div>
<div class="box">3</div>
</div>
```

```css
.container{
display:flex;
justify-content:center;
align-items:center;
gap:20px;
height:300px;
background:#eee;
}

.box{
width:80px;
height:80px;
background:red;
color:white;
display:flex;
justify-content:center;
align-items:center;
}
```

---

# Real Websites Use Flexbox For

* Navbar
* Cards layout
* Centering elements
* Responsive design
* Dashboard UI

---

✅ **Most Important Flexbox Properties**

```
display:flex
flex-direction
justify-content
align-items
flex-wrap
gap
flex
align-self
```

---

