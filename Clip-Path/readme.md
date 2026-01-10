
clip-path lets you cut or shape an element visually (circle, polygon, custom shapes) by hiding the outside area.

## 1️⃣ What is clip-path? (Simple explanation)

Think of clip-path like cutting paper with scissors ✂️.

The element still exists fully

But only the clipped area is visible

Rest is hidden (not removed from DOM)

## 🧠 Real-world analogy:
Imagine putting a stencil over a photo — only the stencil shape shows.


## 2️⃣ Most important clip-path shapes (You MUST know)
### 🔹 1. circle()

```css
.box {
  clip-path: circle(50%);
}
```

✔ Creates a circular cut
✔ Perfect for avatars, profile images

### 🔹 2. ellipse()
```css
.box {
  clip-path: ellipse(50% 30%);
}
```


✔ Oval shape
✔ Useful for soft UI highlights

### 🔹 3. inset() (Rectangle cut)

```css
.box {
  clip-path: inset(20px 40px);
}
```

✔ Cuts from edges (top right bottom left)
✔ Like padding, but for clipping

### 🔹 4. polygon() 🔥 MOST POWERFUL
```css
.box {
  clip-path: polygon(
    50% 0%,
    100% 50%,
    50% 100%,
    0% 50%
  );
}
```


✔ Create:

Diamonds

Stars

Waves

Custom cards

💡 Percentages are relative to element size
