# Flexbox Properties (Wrap, Gap, Shrink)

These properties help **control spacing, wrapping, and resizing of flex items** inside a flex container.

---

# 1. Flex Wrap

## Definition

`flex-wrap` controls **whether flex items stay in one line or move to the next line when space is not enough**.

![Image](https://miro.medium.com/v2/resize%3Afit%3A1400/1%2AM2m88Z_hvK9-VuBGjgIZng.png)


### Values

* `nowrap` (default)
* `wrap`
* `wrap-reverse`

### Example

```css
.container{
  display: flex;
  flex-wrap: wrap;
}
```

### Result

Items **move to the next line when space is full**.

---

# 2. Gap

## Definition

`gap` creates **space between flex items**.



![Image](https://www.scaler.com/topics/images/css-gap-property.webp)


### Example

```css
.container{
  display: flex;
  gap: 20px;
}
```

### Result

Each item will have **20px space between them**.

---

# 3. Flex Shrink

## Definition

`flex-shrink` controls **how much an item shrinks when there is not enough space**.

![Image](https://miro.medium.com/v2/resize%3Afit%3A1400/1%2Av4U8j4DFlaziMqgfHvc3rg.png)

![Image](https://ishadeed.com/assets/flex-css/flex-shrink-1-2.png)

![Image](https://i.sstatic.net/UmcguNXE.png)

![Image](https://bs-uploads.toptal.io/blackfish-uploads/components/open_graph_image/8959861/og_image/optimized/Flexbox-Luke_Social-d032d7504957097a13f96272a38a3c78.png)

### Example

```css
.box{
  flex-shrink: 1;
}
```

### Meaning

* `1` → item can shrink
* `0` → item will **not shrink**

Example:

```css
.box{
  flex-shrink: 0;
}
```

The box **keeps its original size**.

---

# Full Example

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
  flex-wrap: wrap;
  gap: 20px;
}

.box{
  width: 150px;
  height: 100px;
  background: lightblue;
  flex-shrink: 1;
}
```

---

# Quick Summary

| Property    | Purpose                           |
| ----------- | --------------------------------- |
| flex-wrap   | allows items to move to next line |
| gap         | space between items               |
| flex-shrink | controls shrinking of items       |

---

# One Powerful Line

**Flexbox properties like wrap, gap, and shrink help create flexible and responsive layouts.**


