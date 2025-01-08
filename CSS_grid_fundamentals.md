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
