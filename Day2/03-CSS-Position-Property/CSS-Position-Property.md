# CSS Position Property

## Definition

The **`position` property** in CSS is used to **control how an element is placed on a webpage**.

It works with properties like:

* `top`
* `bottom`
* `left`
* `right`

---

# Types of Position

1. **Static**
2. **Relative**
3. **Absolute**
4. **Fixed**
5. **Sticky**

---

# 1. Static Position

## Definition

`static` is the **default position** of all HTML elements.

The element follows the **normal document flow**.

![Image](https://media.licdn.com/dms/image/v2/D5612AQGPLy7W7RHp9w/article-cover_image-shrink_600_2000/article-cover_image-shrink_600_2000/0/1661311449135?e=2147483647\&t=bBaRKe7akklSAXJNfQ8-oj2t_3Z2QhDbxH1_TcKt4Y4\&v=beta)

![Image](https://pbs.twimg.com/media/GAQMKxvaAAAgQWr.jpg)

![Image](https://miro.medium.com/v2/resize%3Afit%3A2000/1%2A8OQ7qwYSCuVVwGFTC82KrQ.png)

![Image](https://cdn.hashnode.com/res/hashnode/image/upload/v1683410454812/5670f8fb-d7bc-496f-83f8-01f4fd6a573e.jpeg)

### Example

```css
div{
  position: static;
}
```

### Key Point

* `top`, `left`, `right`, `bottom` **do not work**.

---

# 2. Relative Position

## Definition

`relative` moves an element **relative to its original position**.

![Image](https://www.easeout.co/images/uploads/position-relative.png)

![Image](https://chenhuijing.com/images/posts/css-positioning/tb-ltr.png)

![Image](https://cdn.hashnode.com/res/hashnode/image/upload/v1683720992015/89cc23b8-a57d-4d89-ac96-72b267bb1f21.png)

![Image](https://miro.medium.com/v2/resize%3Afit%3A613/1%2Ape9E2kzrX48Wwn_0wKklmw.png)

### Example

```css
div{
  position: relative;
  top: 20px;
  left: 30px;
}
```

### Meaning

The element moves **20px down and 30px right** from its original position.

---

# 3. Absolute Position

## Definition

`absolute` positions an element **relative to the nearest positioned parent**.

![Image](https://miro.medium.com/1%2Apt8bgEQFBm0Eu1XXYgB_XQ.gif)

![Image](https://i.sstatic.net/h1EBq.jpg)

![Image](https://media.licdn.com/dms/image/v2/D5612AQGPLy7W7RHp9w/article-cover_image-shrink_600_2000/article-cover_image-shrink_600_2000/0/1661311449135?e=2147483647\&t=bBaRKe7akklSAXJNfQ8-oj2t_3Z2QhDbxH1_TcKt4Y4\&v=beta)

![Image](https://chenhuijing.com/images/posts/css-positioning.jpg)

### Example

```css
.parent{
  position: relative;
}

.child{
  position: absolute;
  top: 0;
  right: 0;
}
```

### Key Point

The element **ignores normal flow**.

---

# 4. Fixed Position

## Definition

`fixed` positions an element **relative to the browser window**.

![Image](https://i.sstatic.net/yZbBw.jpg)

![Image](https://i.sstatic.net/UTrdU.png)

![Image](https://i.sstatic.net/ZvH67.png)

![Image](https://i.sstatic.net/BfRBU.png)

### Example

```css
div{
  position: fixed;
  top: 0;
  right: 0;
}
```

### Use Case

* Navigation bars
* Chat buttons
* Floating icons

---

# 5. Sticky Position

## Definition

`sticky` behaves like **relative until scrolling**, then becomes **fixed**.


![Image](https://user-images.githubusercontent.com/181364/58353635-a0a3cf80-7e34-11e9-9901-da5ab3cfe1c0.gif)

### Example

```css
div{
  position: sticky;
  top: 0;
}
```

### Use Case

* Sticky headers
* Section titles

---

# Quick Summary

| Position | Meaning                             |
| -------- | ----------------------------------- |
| static   | default position                    |
| relative | moves relative to original position |
| absolute | positioned relative to parent       |
| fixed    | positioned relative to browser      |
| sticky   | switches between relative and fixed |

---

# One Powerful Line

**The `position` property controls how elements are placed and moved on a webpage layout.**

---
