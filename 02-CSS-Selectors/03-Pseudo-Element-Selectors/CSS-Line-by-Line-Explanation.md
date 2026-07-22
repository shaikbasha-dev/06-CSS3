# CSS Line-by-Line Explanation

## Introduction

This document explains every important CSS selector, pseudo-element, and property used in the `style.css` file for the **Pseudo-Element Selectors** module.

The stylesheet is responsible for transforming the basic HTML structure into a visually attractive, readable, and responsive webpage while demonstrating the practical use of CSS Pseudo-Elements.

---

# File Header

```css
/*
===============================================================================
File Name      : style.css
Topic          : CSS Pseudo-Element Selectors
Repository     : 06-CSS3
===============================================================================
*/
```

## Explanation

The header comment provides basic information about the stylesheet.

It helps developers quickly identify:

- File name
- Topic
- Repository
- Purpose of the stylesheet

---

# Universal Selector

```css
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}
```

## Selector Explanation

The Universal Selector (`*`) selects every HTML element on the webpage.

It is commonly used to create a consistent starting point for styling.

---

## Property Explanation

### `margin: 0;`

Removes the default outer spacing added by browsers.

---

### `padding: 0;`

Removes the default inner spacing.

---

### `box-sizing: border-box;`

Includes padding and borders inside the element's total width and height.

This makes layouts easier to manage.

---

# Body Selector

```css
body{
    font-family:Arial, Helvetica, sans-serif;
    background-color:#f4f6f9;
    color:#333333;
    padding:30px;
    line-height:1.8;
}
```

## Selector Explanation

The `body` selector styles the entire webpage.

All visible elements inherit many of these styles.

---

## Property Explanation

### `font-family`

Specifies the default font for the webpage.

---

### `background-color`

Sets the page background color.

---

### `color`

Defines the default text color.

---

### `padding`

Creates space between the browser edges and webpage content.

---

### `line-height`

Controls the spacing between lines of text.

A larger value improves readability.

---

# Container Selector

```css
.container{
    max-width:1100px;
    margin:auto;
    background-color:#ffffff;
    padding:40px;
    border-radius:10px;
    box-shadow:0px 0px 15px rgba(0,0,0,0.10);
}
```

## Selector Explanation

The `.container` class creates the main content area.

It keeps the webpage centered and organized.

---

## Property Explanation

### `max-width`

Limits the maximum width of the content.

---

### `margin:auto`

Centers the container horizontally.

---

### `background-color`

Applies a white background.

---

### `padding`

Creates internal spacing.

---

### `border-radius`

Rounds the container corners.

---

### `box-shadow`

Adds a subtle shadow around the container.

---

# Main Heading Selector

```css
h1{
    text-align:center;
    color:#0d6efd;
    margin-bottom:20px;
    font-size:38px;
}
```

## Selector Explanation

Styles the main page heading.

---

## Property Explanation

### `text-align`

Centers the heading.

---

### `color`

Changes the heading color.

---

### `margin-bottom`

Creates space below the heading.

---

### `font-size`

Increases the heading size.

---

# Section Heading Selector

```css
h2{
    color:#198754;
    margin-top:30px;
    margin-bottom:15px;
    border-left:6px solid #198754;
    padding-left:12px;
}
```

## Selector Explanation

Styles every level-two heading.

---

## Property Explanation

### `color`

Changes the heading color.

---

### `margin-top`

Creates space above the heading.

---

### `margin-bottom`

Creates space below the heading.

---

### `border-left`

Displays a decorative vertical border.

---

### `padding-left`

Creates spacing between the border and the heading text.

---

# Paragraph Selector

```css
p{
    margin-bottom:18px;
    text-align:justify;
}
```

## Selector Explanation

Styles every paragraph.

---

## Property Explanation

### `margin-bottom`

Separates paragraphs.

---

### `text-align`

Aligns text evenly on both sides.

---

# Introduction Selector

```css
.introduction{
    font-size:18px;
    font-style:italic;
    color:#555555;
}
```

## Selector Explanation

Styles the introduction paragraph.

---

## Property Explanation

### `font-size`

Makes the text slightly larger.

---

### `font-style`

Displays italic text.

---

### `color`

Changes the text color.

---

# Horizontal Rule Selector

```css
hr{
    margin:35px 0;
    border:none;
    border-top:2px solid #dddddd;
}
```

## Selector Explanation

Styles every horizontal separator.

---

## Property Explanation

### `margin`

Creates vertical spacing.

---

### `border`

Removes the default border.

---

### `border-top`

Creates a custom horizontal line.

---

# Table Selector

```css
table{
    width:100%;
    border-collapse:collapse;
    margin-top:20px;
}
```

## Selector Explanation

Styles the comparison table.

---

## Property Explanation

### `width`

Makes the table occupy the available width.

---

### `border-collapse`

Merges adjacent cell borders into a single border.

---

### `margin-top`

Creates spacing above the table.

---

# Table Cell Selector

```css
th,
td{
    border:1px solid #cccccc;
    padding:12px;
    text-align:left;
}
```

## Selector Explanation

Styles both table headers and table data cells.

---

## Property Explanation

### `border`

Creates visible cell borders.

---

### `padding`

Adds spacing inside cells.

---

### `text-align`

Aligns text to the left.

---

# Table Header Selector

```css
th{
    background-color:#0d6efd;
    color:white;
}
```

## Selector Explanation

Styles only table header cells.

---

## Property Explanation

### `background-color`

Applies a blue background.

---

### `color`

Changes the text to white.

---

# ::first-line Selector

```css
.first-line-demo::first-line
```

## Selector Explanation

Selects only the first rendered line of the paragraph.

The browser automatically determines which text belongs to the first line based on the available width.

---

## Property Explanation

### `color`

Changes the first line color.

---

### `font-weight`

Makes the first line bold.

---

### `text-transform`

Converts the first line to uppercase.

---

### `letter-spacing`

Increases spacing between letters.

---

# ::first-letter Selector

```css
.first-letter-demo::first-letter
```

## Selector Explanation

Selects only the first letter of the paragraph.

This effect is commonly used in newspapers and magazines.

---

## Property Explanation

### `font-size`

Enlarges the first letter.

---

### `font-weight`

Makes the letter bold.

---

### `color`

Changes the first letter color.

---

### `margin-right`

Creates space after the letter.

---

### `float`

Allows surrounding text to wrap around the enlarged letter.

---

### `line-height`

Adjusts the height of the enlarged character.

---

# ::before Selector

```css
.before-demo li::before
```

## Selector Explanation

Creates virtual content before every list item.

The generated content does not exist in the HTML document.

---

## Property Explanation

### `content`

Generates a check mark before every list item.

---

### `color`

Changes the check mark color.

---

### `font-weight`

Makes the generated content bold.

---

### `margin-right`

Creates spacing between the generated content and the list text.

---

# ::after Selector

```css
.after-demo::after
```

## Selector Explanation

Creates virtual content after the paragraph.

The browser generates this content during rendering.

---

## Property Explanation

### `content`

Creates additional text after the paragraph.

---

### `color`

Changes the generated text color.

---

### `font-weight`

Makes the generated text bold.

---

### `margin-left`

Creates spacing before the generated content.

---

# Ordered List Selector

```css
ol
```

## Explanation

Styles numbered lists used in the browser workflow section.

---

# Unordered List Selector

```css
ul
```

## Explanation

Styles bullet lists used throughout the webpage.

---

# Footer Selector

```css
footer
```

## Explanation

Styles the webpage footer.

It separates the footer from the remaining content and centers its text.

---

# Media Query

```css
@media (max-width:768px)
```

## Explanation

Creates responsive styles for smaller screens.

The browser applies these styles only when the screen width is **768 pixels or less**.

This ensures the webpage remains readable on tablets and mobile devices.

---

# Browser Rendering Workflow

```text
Load HTML
      │
      ▼
Load CSS
      │
      ▼
Match Selectors
      │
      ▼
Identify Pseudo-Elements
      │
      ▼
Generate Virtual Content
      │
      ▼
Apply Styles
      │
      ▼
Render Final Webpage
```

---

# Key Takeaways

- CSS controls the appearance of the HTML document.
- Pseudo-Elements style specific parts of an element.
- `::before` and `::after` generate virtual content.
- `::first-line` and `::first-letter` style existing text.
- Responsive CSS ensures the webpage works on multiple devices.
- Proper commenting improves readability and maintainability.

---

# Summary

The `style.css` file provides all visual styling for the Pseudo-Element Selectors module. It defines the overall layout, typography, tables, lists, and responsive behavior while demonstrating the four primary pseudo-elements: `::first-line`, `::first-letter`, `::before`, and `::after`. Together with the HTML structure, these styles create a clean, professional, and educational example suitable for learning, revision, and interview preparation.
