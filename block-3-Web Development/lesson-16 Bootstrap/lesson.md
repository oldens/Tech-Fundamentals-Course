# Lesson 16: Accelerating Development: Bootstrap

## Topics
- Connecting
- Grid system
- Main components
- Utility classes

## Notes
Bootstrap is a popular front-end framework that helps in building responsive and mobile-first websites quickly and easily. It provides a collection of CSS and JavaScript components that can be used to create modern and visually appealing web pages.

### Connecting Bootstrap
To use Bootstrap in your project, you need to include the Bootstrap CSS and JavaScript files. You can either download them or use a CDN (Content Delivery Network).

#### Using CDN
Add the following lines to the `<head>` section of your HTML document to include Bootstrap CSS:
```html
<link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
```
Add the following lines before the closing `</body>` tag to include Bootstrap JavaScript and its dependencies:
```html
<script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.5.4/dist/umd/popper.min.js"></script>
<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>
```

### Grid System
Bootstrap's grid system is a flexible and responsive layout system that allows you to create complex layouts with ease. It is based on a 12-column layout, and you can use classes to define the number of columns an element should span.

#### Example
```html
<div class="container">
  <div class="row">
    <div class="col-md-4">Column 1</div>
    <div class="col-md-4">Column 2</div>
    <div class="col-md-4">Column 3</div>
  </div>
</div>
```

### Main Components
Bootstrap provides a wide range of pre-designed components that you can use to build your web pages. Some of the most commonly used components include:

1. **Navbar**: A responsive navigation bar.
```html
<nav class="navbar navbar-expand-lg navbar-light bg-light">
  <a class="navbar-brand" href="#">Navbar</a>
  <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
    <span class="navbar-toggler-icon"></span>
  </button>
  <div class="collapse navbar-collapse" id="navbarNav">
    <ul class="navbar-nav">
      <li class="nav-item active">
        <a class="nav-link" href="#">Home <span class="sr-only">(current)</span></a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="#">Features</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="#">Pricing</a>
      </li>
    </ul>
  </div>
</nav>
```

2. **Buttons**: Pre-styled buttons with various styles and sizes.
```html
<button type="button" class="btn btn-primary">Primary</button>
<button type="button" class="btn btn-secondary">Secondary</button>
<button type="button" class="btn btn-success">Success</button>
```

3. **Cards**: Flexible content containers with various options for headers, footers, and content.
```html
<div class="card" style="width: 18rem;">
  <img src="..." class="card-img-top" alt="...">
  <div class="card-body">
    <h5 class="card-title">Card title</h5>
    <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
    <a href="#" class="btn btn-primary">Go somewhere</a>
  </div>
</div>
```

### Utility Classes
Bootstrap includes a variety of utility classes that can be used to quickly style elements without writing custom CSS. These classes cover a wide range of properties, such as spacing, typography, colors, and more.

#### Example
```html
<div class="text-center p-3 mb-2 bg-primary text-white">Centered text with padding and background color</div>
```

By using Bootstrap, you can significantly speed up the development process and create responsive, modern, and visually appealing web pages with minimal effort.
