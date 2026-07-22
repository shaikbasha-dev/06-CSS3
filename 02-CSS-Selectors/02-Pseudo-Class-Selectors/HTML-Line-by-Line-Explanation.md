# HTML Line-by-Line Explanation

This document explains every important line and section of the `index.html` file used in the **Pseudo-Class Selectors** module.

---

# File Header

```html
<!--
File Name      : index.html
Topic          : Pseudo-Class Selectors
Repository     : 06-CSS3
Description    : Demonstrates the complete hyperlink lifecycle.
-->
```

### Explanation

This comment block provides metadata about the file.

It helps developers identify:

- File name
- Topic
- Repository
- Purpose of the file

---

# Document Type

```html
<!DOCTYPE html>
```

### Explanation

Declares the document as an **HTML5** document.

Without this declaration, browsers may enter **Quirks Mode**, causing inconsistent rendering.

---

# Root Element

```html
<html lang="en">
```

### Explanation

Represents the root element of the webpage.

The `lang="en"` attribute informs browsers and screen readers that the page content is written in English.

---

# Head Section

```html
<head>
```

### Explanation

Contains metadata that is not displayed directly on the webpage.

It provides information required by browsers and search engines.

---

# Character Encoding

```html
<meta charset="UTF-8">
```

### Explanation

Specifies UTF-8 character encoding.

This allows the webpage to correctly display:

- English
- Mathematical symbols
- Currency symbols
- Unicode characters

---

# Viewport

```html
<meta name="viewport"
      content="width=device-width, initial-scale=1.0">
```

### Explanation

Makes the webpage responsive.

It tells mobile browsers to use the device width and display the page at normal zoom.

---

# Title

```html
<title>Pseudo-Class Selectors</title>
```

### Explanation

Displays the title in:

- Browser tab
- Bookmarks
- Search results

---

# External CSS

```html
<link rel="stylesheet" href="style.css">
```

### Explanation

Connects the HTML document with the external stylesheet.

All visual styling is controlled from `style.css`.

---

# Body

```html
<body>
```

### Explanation

Contains everything visible on the webpage.

---

# Main Container

```html
<div class="container">
```

### Explanation

Acts as the primary wrapper.

It groups all webpage content together so CSS can control:

- Width
- Alignment
- Padding
- Background
- Shadow

---

# Main Heading

```html
<h1>CSS Pseudo-Class Selectors</h1>
```

### Explanation

Displays the main title of the webpage.

Only one `<h1>` should normally appear on a page.

---

# Introduction Paragraph

```html
<p>...</p>
```

### Explanation

Introduces the topic.

It explains that the page demonstrates:

- `:link`
- `:visited`
- `:hover`
- `:active`

---

# Horizontal Rule

```html
<hr>
```

### Explanation

Creates a horizontal divider between sections.

It improves readability.

---

# Section Element

```html
<section>
```

### Explanation

Represents a logical section of related content.

Each demonstration example is enclosed inside its own section.

---

# Example Headings

```html
<h2>Example 1</h2>
```

### Explanation

Introduces each practical demonstration.

Each example focuses on a different real-world use case.

---

# Hyperlink

```html
<a href="https://www.example.com">
```

### Explanation

Creates a hyperlink.

This is the most important element in this project because the pseudo-class selectors operate on hyperlinks.

---

# href Attribute

```html
href="https://www.example.com"
```

### Explanation

Specifies the destination URL.

When clicked, the browser navigates to this location.

---

# target Attribute

```html
target="_blank"
```

### Explanation

Opens the destination webpage in a new browser tab.

---

# Navigation Element

```html
<nav>
```

### Explanation

Represents website navigation.

It groups multiple navigation hyperlinks together.

---

# Unordered List

```html
<ul>
```

### Explanation

Creates a bulleted list.

Used for documentation links and best practices.

---

# List Item

```html
<li>
```

### Explanation

Represents one item inside the unordered list.

---

# Ordered List

```html
<ol>
```

### Explanation

Creates a numbered list.

Used to explain the hyperlink lifecycle in sequence.

---

# Preformatted Text

```html
<pre>
```

### Explanation

Displays text exactly as written.

Preserves:

- Spaces
- Line breaks
- Indentation

Used here to present the **LVHA Rule** clearly.

---

# Strong Element

```html
<strong>
```

### Explanation

Marks important text.

Browsers typically display it in bold.

Screen readers also treat it as emphasized content.

---

# Footer

```html
<footer>
```

### Explanation

Represents the footer section of the webpage.

Used to conclude the demonstration.

---

# Closing Elements

```html
</div>

</body>

</html>
```

### Explanation

These closing tags complete the HTML document.

- `</div>` closes the main container.
- `</body>` ends the visible webpage.
- `</html>` ends the HTML document.

---

# Overall Working

The HTML document performs the following sequence:

1. Creates the webpage structure.
2. Loads the external stylesheet.
3. Displays several hyperlinks.
4. Allows users to interact with those hyperlinks.
5. The browser changes the hyperlink state.
6. CSS automatically applies the corresponding pseudo-class.
7. The user observes different visual styles for each hyperlink state.

---

# Summary

The `index.html` file provides the complete structure required to demonstrate CSS Pseudo-Class Selectors. It contains multiple real-world hyperlink examples, organized using semantic HTML5 elements, allowing learners to observe how browsers apply `:link`, `:visited`, `:hover`, and `:active` states during user interaction.
