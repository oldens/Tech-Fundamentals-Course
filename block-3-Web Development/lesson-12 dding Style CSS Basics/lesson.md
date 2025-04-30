# Lesson 12: Adding Style: CSS Basics

## Topics
- Connecting CSS
- Selectors (classes, ID, tags)
- Basic properties (color, font, background, size)

## Notes
CSS (Cascading Style Sheets) is a stylesheet language used to describe the presentation of a document written in HTML. It allows you to control the layout, colors, fonts, and other visual aspects of a web page.

### Connecting CSS
There are three ways to add CSS to an HTML document:
1. **Inline CSS**: Using the `style` attribute within HTML elements.
```html
<p style="color: red;">This is a red paragraph.</p>
```
2. **Internal CSS**: Using the `<style>` tag within the `<head>` section of the HTML document.
```html
<head>
  <style>
    p {
      color: blue;
    }
  </style>
</head>
```
3. **External CSS**: Linking to an external CSS file using the `<link>` tag within the `<head>` section.
```html
<head>
  <link rel="stylesheet" href="styles.css">
</head>
```

### Selectors
Selectors are used to target HTML elements and apply styles to them. Common selectors include:
1. **Class Selector**: Targets elements with a specific class attribute. Classes are defined with a period (`.`) followed by the class name.
```css
.my-class {
  color: green;
}
```
2. **ID Selector**: Targets a single element with a specific ID attribute. IDs are defined with a hash (`#`) followed by the ID name.
```css
#my-id {
  font-size: 20px;
}
```
3. **Tag Selector**: Targets all elements of a specific type.
```css
p {
  margin: 10px;
}
```

### Basic Properties
CSS properties define the styles applied to elements. Some common properties include:
1. **Color**: Sets the text color.
```css
p {
  color: red;
}
```
2. **Font**: Sets the font family, size, and style.
```css
p {
  font-family: Arial, sans-serif;
  font-size: 16px;
  font-style: italic;
}
```
3. **Background**: Sets the background color or image.
```css
body {
  background-color: lightgray;
}
```
4. **Size**: Sets the width and height of elements.
```css
div {
  width: 100px;
  height: 50px;
}
```

By understanding these basic CSS concepts, you can start adding styles to your web pages and create visually appealing designs.
