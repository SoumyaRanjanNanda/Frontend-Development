# CSS Selector Precedence (Specificity)

## Definition

**Selector Precedence** means **which CSS selector has higher priority when multiple selectors apply styles to the same HTML element**.

The browser chooses the **most specific selector**.

---

# Priority Order (Highest → Lowest)

1. **Inline CSS**
2. **ID Selector (`#`)**
3. **Class Selector (`.`), Attribute Selector, Pseudo-class**
4. **Element Selector**
5. **Universal Selector (`*`)**

---

# Example

```html
<style>

p{
  color: blue;
}

.text{
  color: green;
}

#para{
  color: red;
}

</style>

<p id="para" class="text">Hello World</p>
```

### Result

The text becomes **red**.

### Why?

Because **ID selector has higher priority than class and element selectors**.

---

# Priority Table

| Selector Type | Example    | Priority |
| ------------- | ---------- | -------- |
| Inline        | `style=""` | Highest  |
| ID            | `#header`  | High     |
| Class         | `.box`     | Medium   |
| Element       | `p`, `h1`  | Low      |
| Universal     | `*`        | Lowest   |

---

# Important Rule

If selectors have **same priority**, the **last written CSS rule wins**.

Example:

```css
p{
 color: red;
}

p{
 color: blue;
}
```

Output → **Blue** (because it is written last).

---
