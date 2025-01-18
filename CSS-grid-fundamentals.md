# Fundamentals of CSS Grid Layout

CSS Grid is a powerful layout system for creating responsive, two-dimensional layouts with rows and columns.

---

## What is CSS Grid?

CSS Grid Layout is a two-dimensional layout system in CSS. It allows you to define both rows and columns, making it ideal for complex layouts.

### Key Features
- Two-dimensional layout: Works with rows and columns simultaneously.
- Explicit and implicit grid creation.
- Flexible alignment and spacing options.

---

## Basic Terminology

- **Grid Container**: The parent element where grid properties are applied.
- **Grid Items**: The children of the grid container.
- **Grid Lines**: The horizontal and vertical lines that divide the grid.
- **Grid Tracks**: The rows or columns between grid lines.
- **Grid Cells**: The smallest unit in a grid (intersection of a row and column).

---

## Setting Up a Grid

### 1. Define the Grid Container
Use `display: grid;` to create a grid container.

```css
.container {
  display: grid;
}
```
---

## Use fractional units

### 2. define grid columns using <fr>
```css
main {
  grid-template-columns: 1fr 2fr; /* First column gets 1 part, second gets 2 parts */
}
```
---

## Min/Max Constraints

### 3. Use minmax() to define flexible track sizes.

```css
section {
  grid-template-columns: repeat(3, minmax(100px, 1fr)); /* Three columns */
}
```
---

## Media Queries

### 4. Combine Grid with media queries for responsive designs.

```css
@media (min-width: 900px) {
  section {
    grid-template-columns: 1fr 1fr 1fr; /* 3-column layout */
  }
}
```
---

Alignment in CSS Grid
1. Align Items and Content
align-items: Align items along the block (vertical) axis.
justify-items: Align items along the inline (horizontal) axis.

```css
section {
  align-items: center;
  justify-items: start;
}
/* common centering technique */
.container {
  display: grid;
  place-items: center;
}
```


2. Align Entire Grid
align-content: Align the grid as a whole vertically.
justify-content: Align the grid as a whole horizontally.

```css
section {
  align-content: center;
  justify-content: space-between;
}

```
3. Align Individual Items
Use align-self and justify-self for specific items.

```css
.item {
  align-self: end;
  justify-self: center;
}

```
---

## Responsive Layout
### using some of the techniques above

```css
section {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 16px;
}
```





