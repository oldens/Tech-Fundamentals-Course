# Lesson 15: Modern Layouts: CSS Grid (Overview) and Responsiveness

## Topics
- Basics of display: grid
- Viewport
- Media queries

## Notes
CSS Grid is a powerful layout system in CSS that allows for the creation of complex and responsive grid-based layouts. It provides a two-dimensional grid-based layout system, which means it can handle both columns and rows.

### Basics of display: grid
To use CSS Grid, you need to set the `display` property of a container element to `grid`. This makes the container a grid container and its children grid items.
```css
.container {
  display: grid;
}
```

### Defining Grid Structure
1. **grid-template-columns**: Defines the number and size of columns in the grid.
```css
.container {
  grid-template-columns: repeat(3, 1fr);
}
```
2. **grid-template-rows**: Defines the number and size of rows in the grid.
```css
.container {
  grid-template-rows: 100px 200px;
}
```
3. **grid-gap**: Defines the gap between grid items.
```css
.container {
  grid-gap: 10px;
}
```

### Placing Grid Items
1. **grid-column**: Specifies the column(s) a grid item should occupy.
```css
.item {
  grid-column: 1 / 3;
}
```
2. **grid-row**: Specifies the row(s) a grid item should occupy.
```css
.item {
  grid-row: 1 / 2;
}
```

### Viewport
The viewport is the visible area of a web page. It is important to design responsive layouts that adapt to different viewport sizes. You can use the `@viewport` rule to control the viewport settings.
```css
@viewport {
  width: device-width;
  zoom: 1.0;
}
```

### Media Queries
Media queries are used to apply different styles based on the characteristics of the device, such as its width, height, or orientation. They are essential for creating responsive designs.
```css
@media (max-width: 600px) {
  .container {
    grid-template-columns: 1fr;
  }
}
```

By understanding and using CSS Grid, viewport settings, and media queries, you can create more flexible and responsive layouts for your web pages.
