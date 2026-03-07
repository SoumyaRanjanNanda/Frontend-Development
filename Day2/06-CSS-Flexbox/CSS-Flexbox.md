# CSS Flexbox

## Definition

**Flexbox (Flexible Box Layout)** is a CSS layout system used to **align and arrange elements easily in rows or columns**.

It helps developers **create responsive layouts** and **control spacing, alignment, and direction of elements**.

To use Flexbox, we apply:

```css
display: flex;
```

to the **parent container**.

---

# Flex Container and Flex Items

* **Flex Container** → Parent element (`display: flex`)
* **Flex Items** → Child elements inside the container

![Image](https://web.dev/static/learn/css/flexbox/image/a-labelled-diagram-the-a-a9bf061b5d5b2.svg)

![Image](https://wizardzines.com/comics/flexbox-basics/flexbox-basics.png)

![Image](https://www.tutorialspoint.com/css/images/flexbox.png)



---

# Basic Example

### HTML

```html
<div class="container">
  <div class="box">1</div>
  <div class="box">2</div>
  <div class="box">3</div>
</div>
```

### CSS

```css
.container{
  display: flex;
}

.box{
  width: 100px;
  height: 100px;
  background: lightblue;
  margin: 10px;
}
```

### Result

All boxes appear **in one horizontal row**.

---

# Important Flexbox Properties

## 1. Flex Direction

Controls the **direction of flex items**.

![Image](https://scaler.com/topics/images/flex-direction-all-properties.webp)

![Image](https://images.prismic.io/prismic-main/aFs1f3fc4bHWisHd_align-items.png?auto=format%2Ccompress)

![Image](https://htmlandcssguidebook.com/images/flex-direction.png)

![Image](https://i.sstatic.net/U4iwQ.jpg)

### Values

* `row` (default)
* `column`
* `row-reverse`
* `column-reverse`

### Example

```css
.container{
  display: flex;
  flex-direction: column;
}
```

Items appear **vertically**.

---

# 2. Justify Content

Controls **horizontal alignment** of items.

![Image](https://samanthaming.gumlet.io/flexbox30/12-justify-content-row.jpg.gz?format=auto)

![Image](https://marina-ferreira.github.io/img/tutorials/css/flexbox/digest.png)

![Image](https://developer.mozilla.org/en-US/docs/Web/CSS/Guides/Flexible_box_layout/Aligning_items/align11.png)

![Image](https://developer.mozilla.org/en-US/docs/Web/CSS/Guides/Flexible_box_layout/Aligning_items/align4.png)

### Values

* `flex-start`
* `center`
* `flex-end`
* `space-between`
* `space-around`
* `space-evenly`

### Example

```css
.container{
  display: flex;
  justify-content: center;
}
```

Items move to the **center horizontally**.

---

# 3. Align Items

Controls **vertical alignment** of items.

![Image](https://developer.mozilla.org/en-US/docs/Web/CSS/Guides/Flexible_box_layout/Aligning_items/align4.png)

![Image](https://developer.mozilla.org/en-US/docs/Web/CSS/Guides/Flexible_box_layout/Aligning_items/align5.png)

![Image](https://developer.mozilla.org/en-US/docs/Web/CSS/Guides/Flexible_box_layout/Aligning_items/align11.png)

![Image](https://www.tutorialspoint.com/css/images/flexbox.png)

### Values

* `flex-start`
* `center`
* `flex-end`
* `stretch`

### Example

```css
.container{
  display: flex;
  align-items: center;
}
```

Items align **vertically in the center**.

---

# Example: Perfect Centering

```css
.container{
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}
```

This will **perfectly center an element horizontally and vertically**.

---

# Quick Summary

| Property        | Purpose              |
| --------------- | -------------------- |
| display:flex    | activates flexbox    |
| flex-direction  | controls row/column  |
| justify-content | horizontal alignment |
| align-items     | vertical alignment   |

---

# One Powerful Line

**Flexbox is a modern CSS layout system that makes alignment and responsive design easy.**

