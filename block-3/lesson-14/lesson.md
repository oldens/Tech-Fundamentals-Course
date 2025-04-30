# Lesson 14: Modern Layouts: Flexbox

## Topics
- display: flex
- main properties of the container and items for flexible layout

## Notes
Flexbox is a modern layout model in CSS that allows for the creation of flexible and responsive layouts. It is designed to distribute space along a single axis, either horizontally or vertically, and to align items within a container.

### display: flex
To use Flexbox, you need to set the `display` property of a container element to `flex`. This makes the container a flex container and its children flex items.
```css
.container {
  display: flex;
}
```

### Main Properties of the Container
1. **flex-direction**: Defines the direction of the main axis (row, row-reverse, column, column-reverse).
```css
.container {
  flex-direction: row;
}
```
2. **justify-content**: Aligns flex items along the main axis (flex-start, flex-end, center, space-between, space-around, space-evenly).
```css
.container {
  justify-content: center;
}
```
3. **align-items**: Aligns flex items along the cross axis (flex-start, flex-end, center, baseline, stretch).
```css
.container {
  align-items: stretch;
}
```
4. **flex-wrap**: Controls whether flex items should wrap onto multiple lines (nowrap, wrap, wrap-reverse).
```css
.container {
  flex-wrap: wrap;
}
```

### Main Properties of the Items
1. **flex-grow**: Defines the ability of a flex item to grow if necessary.
```css
.item {
  flex-grow: 1;
}
```
2. **flex-shrink**: Defines the ability of a flex item to shrink if necessary.
```css
.item {
  flex-shrink: 1;
}
```
3. **flex-basis**: Defines the initial size of a flex item before any space distribution.
```css
.item {
  flex-basis: 100px;
}
```
4. **align-self**: Overrides the `align-items` property for individual flex items.
```css
.item {
  align-self: center;
}
```

By understanding and using Flexbox, you can create more flexible and responsive layouts for your web pages.
