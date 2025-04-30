# Lesson 11: Building the Framework: HTML Basics

## Topics
- Document structure
- Main content tags (headings, paragraphs)
- Containers <div>
- Links <a>
- Images <img>

## Notes
HTML (HyperText Markup Language) is the standard language for creating web pages. It describes the structure of a web page and its content.

### Document Structure
An HTML document is structured with a series of nested elements. The basic structure includes:
```html
<!DOCTYPE html>
<html>
<head>
  <title>Page Title</title>
</head>
<body>
  <h1>This is a Heading</h1>
  <p>This is a paragraph.</p>
</body>
</html>
```

### Main Content Tags
1. **Headings**: Used to define headings in the document. There are six levels of headings, from `<h1>` to `<h6>`.
2. **Paragraphs**: Defined using the `<p>` tag. It is used to create paragraphs of text.

### Containers
The `<div>` tag is used as a container for other HTML elements. It is often used to group elements for styling purposes.

### Links
The `<a>` tag defines a hyperlink, which is used to link from one page to another. The `href` attribute specifies the URL of the page the link goes to.
```html
<a href="https://www.example.com">This is a link</a>
```

### Images
The `<img>` tag is used to embed images in an HTML page. The `src` attribute specifies the path to the image, and the `alt` attribute provides alternative text for the image.
```html
<img src="image.jpg" alt="Description of image">
```

By understanding these basic HTML elements, you can start building simple web pages and gradually add more complexity and interactivity.
