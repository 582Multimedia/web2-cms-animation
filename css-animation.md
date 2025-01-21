# Web Animation Techniques for Students

This guide covers essential web animation techniques to help students build engaging and interactive web experiences.

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
