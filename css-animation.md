# Web Animation Techniques for 582 Multimedia

Here are some notes developed with the help of ChatGPT.
Some are good. Some not so good. Some are outdated.
We will be fixing them up as we go.

---

## **1. CSS 2D Transforms**

2D Transforms allow you to manipulate elements in two-dimensional space, including translation, rotation, scaling, and skewing.

### Key Transform Properties

- **`transform`**: The main property to apply 2D transforms.
- **`transform-origin`**: Specifies the point of origin for the transformation.
- **`transform-style`**: Determines how nested elements are displayed.

### Transform Functions

- **`translate(x, y)`**: Moves an element along the x- and y-axes.

  ```css
  .translate-example {
    transform: translate(50px, 100px);
  }
  ```

- **`rotate(deg)`**: Rotates an element by a specified degree.

  ```css
  .rotate-example {
    transform: rotate(45deg);
  }
  ```

- **`scale(x, y)`**: Scales an element by the given factor. Use a single value for uniform scaling.

  ```css
  .scale-example {
    transform: scale(1.5); /* Increases size by 50% */
  }
  ```

- **`skew(x, y)`**: Tilts an element along the x- or y-axis.

  ```css
  .skew-example {
    transform: skew(20deg, 10deg);
  }
  ```

- **`matrix(a, b, c, d, e, f)`**: Combines multiple transforms into a single matrix.

  ```css
  .matrix-example {
    transform: matrix(1, 0, 0, 1, 50, 100);
  }
  ```

### Combining Transforms

You can combine multiple transform functions in a single declaration.

```css
.combined-example {
  transform: translate(50px, 100px) rotate(45deg) scale(1.2);
}
```

The values represent the following functions:
matrix(scaleX(), skewY(), skewX(), scaleY(), translateX(), translateY()).

### Hover Example

Use transforms to create interactive hover effects.

```css
.button {
  transition: transform 0.3s ease;
}
.button:hover {
  transform: scale(1.1) rotate(5deg);
}
```

## **2. CSS Animations**

CSS animations allow you to define transitions between states with keyframes and timing.

### Transitions

Smoothly change property values over time.

```css
.button {
  background-color: #3498db;
  transition: background-color 0.3s ease;
}
.button:hover {
  background-color: #2980b9;
}
```

### Keyframes

Define multiple states for an element during an animation.

```css
@keyframes slideIn {
  from {
    transform: translateX(-100%);
  }
  to {
    transform: translateX(0);
  }
}
.element {
  animation: slideIn 1s ease-out;
}
```

## **3. JavaScript for Animations**

JavaScript provides dynamic control over animations for interactivity.

### DOM Manipulation

Use JavaScript to trigger animations.

```javascript
const box = document.querySelector(".box");
box.addEventListener("click", () => {
  box.style.transform = "rotate(45deg)";
  box.style.transition = "transform 0.5s";
});
```

### requestAnimationFrame

Create smooth, high-performance animations.

```javascript
let position = 0;
function move() {
  position += 1;
  document.querySelector(".box").style.transform = `translateX(${position}px)`;
  if (position < 200) {
    requestAnimationFrame(move);
  }
}
move();
```

## **4. Scroll-Based Animations**

Scroll-based animations trigger effects as users scroll through a webpage, enhancing interactivity and visual appeal.

### Intersection Observer API

Efficiently animate elements when they enter the viewport.

```javascript
const observer = new IntersectionObserver((entries) => {
  entries.forEach((entry) => {
    if (entry.isIntersecting) {
      entry.target.classList.add("visible");
    }
  });
});

document.querySelectorAll(".fade-in").forEach((el) => observer.observe(el));
```

### CSS

```css
.fade-in {
  opacity: 0;
  transform: translateY(20px);
  transition: opacity 0.5s ease, transform 0.5s ease;
}

.fade-in.visible {
  opacity: 1;
  transform: translateY(0);
}
```
