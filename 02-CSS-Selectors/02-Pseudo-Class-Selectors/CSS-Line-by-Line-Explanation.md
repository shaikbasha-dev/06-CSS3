# CSS Line-by-Line Explanation

This document explains every important selector, pseudo-class, property, and CSS rule used in the `style.css` file of the **Pseudo-Class Selectors** module.

---

# File Header

```css
/*
===============================================================================
File Name      : style.css
Topic          : Pseudo-Class Selectors
Repository     : 06-CSS3
===============================================================================
*/
```

## Explanation

This comment block contains metadata about the stylesheet.

It helps developers quickly identify:

- File name
- Topic
- Repository
- Purpose of the stylesheet

---

# Universal Selector

```css
* {

    margin: 0;

    padding: 0;

    box-sizing: border-box;

}
```

## Explanation

The Universal Selector (`*`) selects **every HTML element** on the webpage.

It is commonly used to reset the browser's default styling.

### margin: 0;

Removes the default outer spacing applied by browsers.

### padding: 0;

Removes the default inner spacing.

### box-sizing: border-box;

Includes padding and border inside the element's width and height.

This makes layouts easier to manage.

---

# Body Selector

```css
body {

    background-color: #f4f6f9;

    font-family: Arial, Helvetica, sans-serif;

    color: #333333;

    line-height: 1.8;

    padding: 30px;

}
```

## Explanation

The `body` selector styles the entire webpage.

### background-color

Applies a light gray background.

### font-family

Specifies the fonts used for all text.

If Arial is unavailable, Helvetica is used.

If Helvetica is unavailable, the browser uses any available sans-serif font.

### color

Sets the default text color.

### line-height

Adds vertical spacing between lines.

Improves readability.

### padding

Adds space between the browser edge and webpage content.

---

# Container Selector

```css
.container {

    max-width: 1200px;

    margin: auto;

    background-color: white;

    padding: 30px;

    border-radius: 10px;

    box-shadow: 0 5px 15px rgba(0,0,0,0.10);

}
```

## Explanation

The container groups all webpage content.

### max-width

Limits the maximum width.

### margin: auto

Centers the container horizontally.

### background-color

Creates a white content area.

### padding

Adds internal spacing.

### border-radius

Rounds the corners.

### box-shadow

Adds a soft shadow.

Creates depth.

---

# Heading Selectors

```css
h1 {

    color: #0d6efd;

    text-align: center;

    margin-bottom: 20px;

}
```

## Explanation

Styles the main heading.

### color

Changes the heading color.

### text-align

Centers the heading.

### margin-bottom

Adds space below the heading.

---

```css
h2 {

    color: #198754;

    margin-top: 35px;

    margin-bottom: 15px;

}
```

## Explanation

Styles section headings.

Creates consistent spacing.

---

# Paragraph Selector

```css
p {

    margin-bottom: 15px;

}
```

## Explanation

Adds spacing below every paragraph.

Improves readability.

---

# Section Selector

```css
section {

    margin-bottom: 30px;

}
```

## Explanation

Separates each example from the next.

---

# Horizontal Rule

```css
hr {

    margin: 35px 0;

}
```

## Explanation

Adds vertical spacing around horizontal lines.

---

# Navigation Links

```css
nav a {

    margin-right: 20px;

}
```

## Explanation

Selects only hyperlinks inside the `<nav>` element.

Adds spacing between navigation links.

---

# List Selectors

```css
ul,
ol {

    padding-left: 25px;

}
```

## Explanation

Adds indentation to ordered and unordered lists.

---

```css
li {

    margin-bottom: 10px;

}
```

## Explanation

Adds spacing between list items.

---

# Base Hyperlink Selector

```css
a {

    font-size: 18px;

    font-weight: bold;

    text-decoration: none;

    transition: all 0.3s ease;

}
```

## Explanation

The `a` selector applies styles to **every hyperlink**.

### font-size

Makes hyperlinks easier to read.

### font-weight

Displays hyperlinks in bold.

### text-decoration

Removes the default underline.

### transition

Creates smooth animation when hyperlink styles change.

---

# LVHA Rule

The hyperlink pseudo-classes should always be written in this order:

```css
a:link

a:visited

a:hover

a:active
```

This order is called the **LVHA Rule**.

It ensures browsers apply the correct styles.

---

# :link Pseudo-Class

```css
a:link {

    color: #0d6efd;

}
```

## Explanation

Selects hyperlinks that have **never been visited**.

The browser applies this style when the destination has not yet been opened.

---

# :visited Pseudo-Class

```css
a:visited {

    color: #6f42c1;

}
```

## Explanation

Selects hyperlinks that the user has already visited.

Modern browsers restrict which properties can be changed for privacy and security reasons.

---

# :hover Pseudo-Class

```css
a:hover {

    color: #dc3545;

    text-decoration: underline;

}
```

## Explanation

Selects hyperlinks while the mouse pointer is positioned over them.

### color

Changes the text color.

### text-decoration

Displays an underline during hovering.

This provides visual feedback to users.

---

# :active Pseudo-Class

```css
a:active {

    color: #198754;

}
```

## Explanation

Selects hyperlinks while the mouse button is pressed.

This state exists only briefly during the click operation.

---

# Preformatted Text

```css
pre {

    background-color: #eeeeee;

    padding: 20px;

    border-left: 5px solid #0d6efd;

    border-radius: 5px;

    overflow-x: auto;

}
```

## Explanation

Styles `<pre>` elements.

### background-color

Creates a highlighted code area.

### padding

Adds internal spacing.

### border-left

Displays a colored vertical line.

### border-radius

Rounds the corners.

### overflow-x

Allows horizontal scrolling if content is wider than the container.

---

# Footer Selector

```css
footer {

    margin-top: 40px;

    padding-top: 20px;

    border-top: 2px solid #dddddd;

    text-align: center;

}
```

## Explanation

Styles the footer.

Separates it visually from the rest of the page.

---

# Media Query

```css
@media (max-width:768px)
```

## Explanation

Applies responsive styles when the screen width is **768 pixels or less**.

This improves the appearance on tablets and mobile devices.

---

# Responsive Container

```css
.container {

    padding:20px;

}
```

## Explanation

Reduces the container padding on smaller screens.

---

# Responsive Headings

```css
h1 {

    font-size:30px;

}
```

## Explanation

Reduces the main heading size for mobile devices.

---

```css
h2 {

    font-size:24px;

}
```

## Explanation

Makes section headings fit smaller screens.

---

# Responsive Navigation

```css
nav a {

    display:block;

    margin-bottom:15px;

}
```

## Explanation

Displays navigation hyperlinks vertically instead of horizontally.

This improves readability on mobile devices.

---

# Responsive Hyperlinks

```css
a {

    font-size:17px;

}
```

## Explanation

Slightly reduces hyperlink size for smaller screens.

---

# Responsive Preformatted Text

```css
pre {

    font-size:15px;

}
```

## Explanation

Makes code blocks easier to fit on mobile displays.

---

# Complete Browser Workflow

When the webpage loads, the browser processes the stylesheet in the following order:

1. Reset browser default spacing.
2. Apply styles to the body.
3. Style the main container.
4. Style headings.
5. Style paragraphs and sections.
6. Style lists.
7. Apply default hyperlink styles.
8. Check the hyperlink state.
9. Apply one of the following pseudo-classes:
   - `:link`
   - `:visited`
   - `:hover`
   - `:active`
10. Apply responsive rules if the screen width is 768 pixels or smaller.

---

# Summary

The `style.css` file demonstrates how CSS Pseudo-Class Selectors create interactive hyperlinks. It combines general webpage styling with the four hyperlink pseudo-classes, follows the recommended **LVHA Rule**, and includes responsive design techniques. Together, these styles produce a clean, interactive, and beginner-friendly demonstration of state-based CSS styling.
