# CSS Box Properties

The **CSS Box Model** describes how every HTML element is displayed as a **rectangular box**.
It consists of **content → padding → border → margin**.

![Image](https://projects.accesscomputing.uw.edu/webd2/student/unit3/images/boxmodel.gif)

![Image](https://media2.dev.to/dynamic/image/width%3D1000%2Cheight%3D420%2Cfit%3Dcover%2Cgravity%3Dauto%2Cformat%3Dauto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Farticles%2F3yl6akpiqfzblci0egcn.png)

![Image](https://study.com/cimages/multimages/16/boxmodel.jpg)

---

# 1. Margin

## Definition

**Margin** is the **outer space outside the border** of an element.
It creates **distance between elements**.

## Example

```css
div{
  margin: 20px;
}
```

This creates **20px space outside the element**.

### Individual Margin

```css
div{
  margin-top: 10px;
  margin-bottom: 10px;
  margin-left: 20px;
  margin-right: 20px;
}
```

---

# 2. Padding

## Definition

**Padding** is the **space inside the element**, between the **content and the border**.

![Image](https://fedmentor.dev/posts/padding-margin/box-model-800w.jpeg)

![Image](https://www.tutorialspoint.com/css/images/css-box-model.jpg)

![Image](https://www.tutorialspoint.com/css/images/css-padding.jpg)

![Image](https://www.openbookproject.net/tutorials/getdown/css/images/lesson6/CSSBoxModel.png)

## Example

```css
div{
  padding: 15px;
}
```

This creates **15px space inside the element**.

### Individual Padding

```css
div{
  padding-top: 10px;
  padding-left: 20px;
}
```

---

# 3. Width

## Definition

`width` defines the **horizontal size of an element**.

## Example

```css
div{
  width: 200px;
}
```

This makes the element **200 pixels wide**.

---

# 4. Height

## Definition

`height` defines the **vertical size of an element**.

## Example

```css
div{
  height: 100px;
}
```

This makes the element **100 pixels tall**.

---

# 5. Box Sizing

## Definition

`box-sizing` controls **how width and height are calculated**.

### Types

1. **content-box (default)**
2. **border-box**

### Example

```css
div{
  width: 200px;
  padding: 20px;
  box-sizing: border-box;
}
```

Now the **padding will be included inside the width**.

---

# Full Example

```html
<!DOCTYPE html>
<html>
<head>
<style>

.box{
  width: 200px;
  height: 100px;
  padding: 20px;
  margin: 30px;
  background-color: lightblue;
}

</style>
</head>

<body>

<div class="box">
Hello CSS Box Model
</div>

</body>
</html>
```

---

# Quick Summary

| Property   | Meaning                   |
| ---------- | ------------------------- |
| Margin     | Space outside the element |
| Padding    | Space inside the element  |
| Width      | Horizontal size           |
| Height     | Vertical size             |
| Box-sizing | Controls box calculation  |

---