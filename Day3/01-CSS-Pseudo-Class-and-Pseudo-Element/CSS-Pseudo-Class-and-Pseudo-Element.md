# CSS Pseudo-Class and Pseudo-Element

These are special CSS selectors used to **style elements in a specific state or specific part of an element**.

---

# 1. Pseudo-Class

## Definition

A **Pseudo-class** is used to **define a special state of an HTML element**.

It is written using **`:` (single colon)**.

Examples of states:

* hover
* active
* visited
* focus

![Image](https://tutorial.techaltum.com/images/css-before-after.jpg)

![Image](https://iq.opengenus.org/content/images/2020/11/Image_1.png)

![Image](https://19898180.fs1.hubspotusercontent-na1.net/hubfs/19898180/2024/blog%20image/css/How%20to%20Style%20Links/How%20to%20Style%20Links_%20Hover%2C%20Focus%2C%20and%20Active%20States.jpg)

![Image](https://s1.o7planning.com/web-rs/web-image/en/arf-1155628-vi.gif)

---

## Common Pseudo-Classes

| Pseudo-Class | Meaning                      |
| ------------ | ---------------------------- |
| `:hover`     | when mouse is over element   |
| `:active`    | when element is clicked      |
| `:focus`     | when input field is selected |
| `:visited`   | visited link                 |

---

## Example

```css
button:hover{
  background-color: blue;
}
```

### Meaning

When the mouse **hovers over the button**, the background becomes **blue**.

---

# 2. Pseudo-Element

## Definition

A **Pseudo-element** is used to **style a specific part of an element**.

It is written using **`::` (double colon)**.

![Image](https://cdn.hashnode.com/res/hashnode/image/upload/v1605187166481/YcU2uf4SA.png)

![Image](https://ayc0.github.io/_astro/css-before-after-hover.D0PxOjqI_V89Py.webp)

![Image](https://static.d-libro.com/01-course-content-images/1011-11-HTML-CSS-Coding-with-AI/030-topic-og-images/pseudo-elements-in-css-id101111040310.png)

![Image](https://www.w3docs.com/uploads/media/default/0001/03/2c23d36c4972e7b5b815229efea812d5b9f18ab4.png)

---

## Common Pseudo-Elements

| Pseudo-Element   | Purpose                       |
| ---------------- | ----------------------------- |
| `::before`       | insert content before element |
| `::after`        | insert content after element  |
| `::first-letter` | style first letter            |
| `::first-line`   | style first line              |

---

## Example

```css
p::first-letter{
  font-size: 40px;
  color: red;
}
```

### Result

The **first letter of the paragraph becomes large and red**.

---

# Example: Before and After

```css
h1::before{
  content: "★ ";
}

h1::after{
  content: " ★";
}
```

Result:

```
★ Hello World ★
```

---

# Difference Between Pseudo-Class and Pseudo-Element

| Feature | Pseudo-Class         | Pseudo-Element         |
| ------- | -------------------- | ---------------------- |
| Symbol  | `:`                  | `::`                   |
| Purpose | styles element state | styles part of element |
| Example | `:hover`             | `::before`             |

---

# One Powerful Line

**Pseudo-classes style element states, while pseudo-elements style specific parts of elements.**

---
