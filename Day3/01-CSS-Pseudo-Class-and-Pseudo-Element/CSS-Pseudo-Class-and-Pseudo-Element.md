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


![Image](https://static.d-libro.com/01-course-content-images/1011-11-HTML-CSS-Coding-with-AI/030-topic-og-images/pseudo-elements-in-css-id101111040310.png)


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

