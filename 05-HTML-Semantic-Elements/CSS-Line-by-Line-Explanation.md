# CSS Line-by-Line Explanation

This document explains every CSS selector, every CSS property, and every logical section used in the `style.css` file.

The objective is to help beginners understand **what each CSS rule does, why it is used, and how it affects the appearance of the webpage.**

---

# File Header

```css
/*
===============================================================================
File Name      : style.css
Topic          : HTML Semantic Elements
Repository     : 06-CSS3
Description    : Stylesheet demonstrating HTML5 Semantic Elements.
===============================================================================
*/
```

## Explanation

The file header is a documentation comment.

It provides useful information for developers such as:

- File name
- Topic
- Repository
- Purpose of the stylesheet

This comment is ignored by browsers but improves code readability and maintainability.

---

# Global Reset

```css
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}
```

## Selector Explanation

```css
*
```

The asterisk (`*`) is called the **Universal Selector**.

It selects **every HTML element** on the webpage.

Examples include:

- `<body>`
- `<header>`
- `<nav>`
- `<section>`
- `<article>`
- `<table>`
- `<footer>`

---

## Property

```css
margin:0;
```

### Explanation

Removes the default outer spacing added by browsers.

Without this rule, browsers automatically place margins around many elements.

Using `margin:0` creates a consistent starting layout.

---

## Property

```css
padding:0;
```

### Explanation

Removes the default internal spacing added by browsers.

This allows developers to control spacing manually.

---

## Property

```css
box-sizing:border-box;
```

### Explanation

Changes how width and height are calculated.

Normally:

```
Total Width

Width
+ Padding
+ Border
```

With `border-box`:

```
Total Width

Width
(includes padding and border)
```

### Advantages

- Easier layout calculations
- Predictable element sizing
- Better responsive design

---

# Body Styling

```css
body{
    font-family:Arial, Helvetica, sans-serif;
    background-color:#f4f6f9;
    color:#333333;
    line-height:1.8;
}
```

## Selector Explanation

```css
body
```

Selects the webpage body.

Every visible element appears inside the `<body>` element.

The styles defined here become the default appearance for the webpage.

---

## Property

```css
font-family:Arial, Helvetica, sans-serif;
```

### Explanation

Defines the default font.

The browser checks fonts in this order:

1. Arial
2. Helvetica
3. Any available sans-serif font

This is called a **font fallback list**.

---

## Property

```css
background-color:#f4f6f9;
```

### Explanation

Sets a light gray background for the webpage.

A soft background color improves readability compared to pure white.

---

## Property

```css
color:#333333;
```

### Explanation

Sets the default text color.

Dark gray is easier on the eyes than pure black while still maintaining good contrast.

---

## Property

```css
line-height:1.8;
```

### Explanation

Controls the vertical spacing between lines of text.

A larger line height improves readability, especially for long paragraphs.

---

# Header Styling

```css
header{
    background-color:#0d6efd;
    color:#ffffff;
    text-align:center;
    padding:40px 20px;
}
```

## Selector Explanation

```css
header
```

Selects the HTML `<header>` element.

This styles the introductory section of the webpage.

---

## Property

```css
background-color:#0d6efd;
```

### Explanation

Applies a blue background to the header.

This visually separates the header from the rest of the webpage.

---

## Property

```css
color:#ffffff;
```

### Explanation

Changes the text color to white.

White text provides strong contrast against the blue background.

---

## Property

```css
text-align:center;
```

### Explanation

Horizontally centers all text inside the header.

---

## Property

```css
padding:40px 20px;
```

### Explanation

Adds internal spacing.

Breakdown:

```
40px → Top and Bottom

20px → Left and Right
```

Padding prevents the content from touching the edges of the header.

---

# Header Heading

```css
header h1{
    font-size:40px;
    margin-bottom:15px;
}
```

## Selector Explanation

This selector styles only the `<h1>` element inside the `<header>`.

It does not affect `<h1>` elements in other parts of the webpage.

---

## Property

```css
font-size:40px;
```

### Explanation

Increases the size of the main heading, making it the most prominent text on the page.

---

## Property

```css
margin-bottom:15px;
```

### Explanation

Adds space below the heading to separate it from the paragraph beneath it.

---

# Header Paragraph

```css
header p{
    font-size:18px;
    max-width:900px;
    margin:0 auto;
}
```

## Selector Explanation

This selector styles only paragraphs inside the `<header>` element.

---

## Property

```css
font-size:18px;
```

### Explanation

Makes the introductory paragraph larger than the default font size for improved readability.

---

## Property

```css
max-width:900px;
```

### Explanation

Limits the paragraph width.

Very long lines are difficult to read, so this property keeps the text at a comfortable reading width.

---

## Property

```css
margin:0 auto;
```

### Explanation

Centers the paragraph horizontally.

Breakdown:

- Top margin = 0
- Bottom margin = 0
- Left margin = auto
- Right margin = auto

The automatic left and right margins evenly distribute the remaining horizontal space, centering the element.

---

# Navigation Styling

```css
nav{
    background-color:#212529;
}
```

## Selector Explanation

```css
nav
```

This selector targets the HTML `<nav>` element.

The navigation section usually contains the major links of a webpage.

Examples include:

- Home
- About
- Services
- Contact
- Login

Applying styles directly to the semantic `<nav>` element makes the stylesheet easier to understand.

---

## Property

```css
background-color:#212529;
```

### Explanation

Sets a dark background color for the navigation bar.

A dark navigation bar creates visual separation between the header and the main content while improving link visibility.

---

# Navigation List

```css
nav ul{
    list-style:none;
    display:flex;
    justify-content:center;
    flex-wrap:wrap;
}
```

## Selector Explanation

This selector styles the unordered list (`<ul>`) inside the navigation.

The list stores all navigation links.

---

## Property

```css
list-style:none;
```

### Explanation

Removes the default bullet points from the unordered list.

Without this property, each navigation item would display a bullet.

---

## Property

```css
display:flex;
```

### Explanation

Converts the unordered list into a **Flexbox container**.

Each list item becomes a flex item, making alignment much easier than traditional CSS layouts.

---

## Property

```css
justify-content:center;
```

### Explanation

Centers all navigation items horizontally within the navigation bar.

This creates a balanced and professional appearance.

---

## Property

```css
flex-wrap:wrap;
```

### Explanation

Allows navigation items to move onto a new line when there is insufficient horizontal space.

This improves responsiveness on smaller screens.

---

# Navigation List Items

```css
nav ul li{
    margin:12px;
}
```

## Selector Explanation

Targets every list item inside the navigation menu.

Each `<li>` represents one navigation option.

---

## Property

```css
margin:12px;
```

### Explanation

Adds equal spacing around each navigation item.

This prevents links from appearing crowded together.

---

# Navigation Links

```css
nav ul li a{
    text-decoration:none;
    color:#ffffff;
    font-weight:bold;
    padding:10px 18px;
    transition:0.3s;
}
```

## Selector Explanation

Targets anchor (`<a>`) elements inside navigation list items.

These anchors create clickable navigation links.

---

## Property

```css
text-decoration:none;
```

### Explanation

Removes the default underline from hyperlinks.

This provides a cleaner navigation menu.

---

## Property

```css
color:#ffffff;
```

### Explanation

Changes the link text color to white.

White text provides excellent contrast against the dark navigation background.

---

## Property

```css
font-weight:bold;
```

### Explanation

Displays navigation text using a bold font weight.

Bold text helps important navigation links stand out.

---

## Property

```css
padding:10px 18px;
```

### Explanation

Adds internal spacing around each navigation link.

Breakdown:

- Top and Bottom = 10px
- Left and Right = 18px

Padding increases the clickable area, improving usability.

---

## Property

```css
transition:0.3s;
```

### Explanation

Creates a smooth animation whenever a property changes.

Instead of changing instantly, the browser gradually animates the effect over **0.3 seconds**.

---

# Navigation Hover Effect

```css
nav ul li a:hover{
    background-color:#0d6efd;
    border-radius:5px;
}
```

## Selector Explanation

The `:hover` pseudo-class applies styles when the user places the mouse pointer over a navigation link.

---

## Property

```css
background-color:#0d6efd;
```

### Explanation

Changes the background color while hovering.

This gives users visual feedback that the link is interactive.

---

## Property

```css
border-radius:5px;
```

### Explanation

Rounds the corners of the navigation link during the hover state.

Rounded corners create a softer, more modern appearance.

---

# Main Content Styling

```css
main{
    max-width:1200px;
    margin:30px auto;
    background-color:#ffffff;
    padding:40px;
    border-radius:10px;
    box-shadow:0 0 15px rgba(0,0,0,0.10);
}
```

## Selector Explanation

Targets the HTML `<main>` element.

This element contains the primary content of the webpage.

---

## Property

```css
max-width:1200px;
```

### Explanation

Limits the maximum width of the content.

Large screens would otherwise create lines of text that are difficult to read.

---

## Property

```css
margin:30px auto;
```

### Explanation

Centers the `<main>` element horizontally.

Breakdown:

- Top and Bottom Margin = 30px
- Left Margin = auto
- Right Margin = auto

The automatic margins center the content area.

---

## Property

```css
background-color:#ffffff;
```

### Explanation

Applies a white background to the content area.

This contrasts with the light gray page background and highlights the main content.

---

## Property

```css
padding:40px;
```

### Explanation

Adds internal spacing so that the content does not touch the edges of the container.

---

## Property

```css
border-radius:10px;
```

### Explanation

Rounds the corners of the main content container.

Rounded corners create a modern, visually appealing design.

---

## Property

```css
box-shadow:0 0 15px rgba(0,0,0,0.10);
```

### Explanation

Applies a soft shadow around the main container.

This creates depth and makes the content appear elevated from the background.

---

# Section Styling

```css
section{
    margin-bottom:40px;
}
```

## Selector Explanation

Targets every semantic `<section>` element.

Each section represents a major content area of the webpage.

---

## Property

```css
margin-bottom:40px;
```

### Explanation

Creates spacing below each section.

This visually separates sections and improves readability.

---

# Section Heading Styling

```css
section h2{
    color:#198754;
    border-left:6px solid #198754;
    padding-left:12px;
    margin-bottom:20px;
}
```

## Selector Explanation

Targets only `<h2>` headings that appear inside a `<section>`.

---

## Property

```css
color:#198754;
```

### Explanation

Changes the heading text color to green, helping section titles stand out.

---

## Property

```css
border-left:6px solid #198754;
```

### Explanation

Creates a decorative green vertical border on the left side of each heading.

This improves visual emphasis.

---

## Property

```css
padding-left:12px;
```

### Explanation

Adds spacing between the decorative border and the heading text.

---

## Property

```css
margin-bottom:20px;
```

### Explanation

Creates space below the heading before the following content begins.

---

# Article Styling

```css
article{
    background-color:#f8f9fa;
    border-left:5px solid #0d6efd;
    padding:20px;
    margin-bottom:20px;
    border-radius:6px;
}
```

## Selector Explanation

The `article` selector targets every HTML `<article>` element.

An article represents independent, self-contained content such as:

- Blog posts
- Tutorials
- News articles
- Product reviews
- Documentation

Applying consistent styling helps visually separate each article from surrounding content.

---

## Property

```css
background-color:#f8f9fa;
```

### Explanation

Applies a light gray background color to each article.

This improves readability and distinguishes article content from the page background.

---

## Property

```css
border-left:5px solid #0d6efd;
```

### Explanation

Adds a blue vertical border to the left side of every article.

This decorative border highlights the beginning of each article and improves visual organization.

---

## Property

```css
padding:20px;
```

### Explanation

Creates internal spacing between the article content and its border.

Adequate padding prevents text from touching the edges of the container.

---

## Property

```css
margin-bottom:20px;
```

### Explanation

Adds space below each article, preventing adjacent articles from appearing crowded.

---

## Property

```css
border-radius:6px;
```

### Explanation

Rounds the corners of each article container.

Rounded corners contribute to a modern and visually appealing design.

---

# Horizontal Rule Styling

```css
hr{
    border:none;
    border-top:2px solid #dddddd;
    margin:35px 0;
}
```

## Selector Explanation

The `hr` selector styles every horizontal rule (`<hr>`) element.

Horizontal rules create visual separation between major sections of the webpage.

---

## Property

```css
border:none;
```

### Explanation

Removes the browser's default horizontal rule styling.

---

## Property

```css
border-top:2px solid #dddddd;
```

### Explanation

Creates a custom horizontal line using the top border.

This provides a cleaner and more consistent appearance.

---

## Property

```css
margin:35px 0;
```

### Explanation

Adds vertical spacing above and below the horizontal rule.

Breakdown:

- Top and Bottom = 35px
- Left and Right = 0

This spacing clearly separates major content sections.

---

# Paragraph Styling

```css
p{
    margin-bottom:15px;
    text-align:justify;
}
```

## Selector Explanation

Targets every paragraph (`<p>`) element in the document.

---

## Property

```css
margin-bottom:15px;
```

### Explanation

Creates space below each paragraph.

Proper spacing improves readability and prevents paragraphs from appearing too close together.

---

## Property

```css
text-align:justify;
```

### Explanation

Aligns text evenly along both the left and right margins.

Justified text creates a neat, document-like appearance.

---

# List Styling

```css
ul,
ol{
    margin-left:30px;
    margin-bottom:20px;
}

li{
    margin-bottom:10px;
}
```

## Selector Explanation

- `ul` targets unordered lists.
- `ol` targets ordered lists.
- `li` targets individual list items.

---

## Property

```css
margin-left:30px;
```

### Explanation

Creates indentation for lists.

Indented lists improve readability and clearly distinguish list content from surrounding text.

---

## Property

```css
margin-bottom:20px;
```

### Explanation

Adds spacing below each list.

---

## Property

```css
margin-bottom:10px;
```

### Explanation

Creates spacing between individual list items, making lists easier to read.

---

# Table Styling

```css
table{
    width:100%;
    border-collapse:collapse;
    margin-bottom:30px;
}
```

## Selector Explanation

Targets every HTML table.

Tables are used to display structured information in rows and columns.

---

## Property

```css
width:100%;
```

### Explanation

Expands the table to occupy the full width of its parent container.

---

## Property

```css
border-collapse:collapse;
```

### Explanation

Combines adjacent table borders into a single border.

This creates a cleaner table appearance.

---

## Property

```css
margin-bottom:30px;
```

### Explanation

Adds spacing below the table before the next section begins.

---

# Preformatted Text Styling

```css
pre{
    background-color:#212529;
    color:#ffffff;
    padding:20px;
    border-radius:6px;
    overflow-x:auto;
}
```

## Selector Explanation

Targets the `<pre>` element used to display preformatted text.

Examples include:

- Source code
- Directory structures
- ASCII diagrams
- Command-line output

---

## Property Explanation

- `background-color` creates a dark background for improved code readability.
- `color` changes the text color to white for high contrast.
- `padding` adds internal spacing around the content.
- `border-radius` rounds the corners of the container.
- `overflow-x:auto` enables horizontal scrolling if the content exceeds the available width.

---

# Footer Styling

```css
footer{
    background-color:#212529;
    color:#ffffff;
    text-align:center;
    padding:30px;
    border-radius:8px;
}
```

## Selector Explanation

Targets the HTML `<footer>` element.

The footer contains concluding information about the webpage.

---

## Property Explanation

- `background-color` applies a dark background.
- `color` changes text to white.
- `text-align:center` centers the footer content.
- `padding` creates internal spacing.
- `border-radius` rounds the corners for a polished appearance.

---

# Anchor Styling

```css
a{
    color:inherit;
}

a:hover{
    text-decoration:underline;
}
```

## Selector Explanation

The `a` selector styles all hyperlinks.

The `a:hover` selector applies styles when the user moves the mouse pointer over a link.

---

## Property Explanation

- `color:inherit` makes links use the text color of their parent element.
- `text-decoration:underline` displays an underline during the hover state, providing clear visual feedback.

---

# Utility Classes

```css
.text-center{
    text-align:center;
}

.font-bold{
    font-weight:bold;
}

.mt-20{
    margin-top:20px;
}
```

## Explanation

Utility classes are reusable CSS classes that perform a single styling task.

Benefits include:

- Reducing repeated CSS code.
- Improving maintainability.
- Making styles easier to reuse across multiple HTML elements.

---

# Responsive Media Query

```css
@media screen and (max-width:768px){
    ...
}
```

## Explanation

A media query applies CSS rules only when specific conditions are met.

In this example, the styles inside the media query are applied when the screen width is **768 pixels or less**.

This improves the webpage layout on:

- Tablets
- Mobile phones
- Smaller screens

Responsive design ensures that webpages remain readable and usable across different devices.

---

# Summary

The `style.css` file demonstrates how CSS enhances the appearance of an HTML5 semantic webpage.

It includes:

- Global reset
- Typography styling
- Header and navigation styling
- Main content layout
- Section and article styling
- Lists and tables
- Preformatted text
- Footer design
- Utility classes
- Responsive design using media queries

Understanding these CSS selectors and properties enables developers to create webpages that are visually appealing, maintainable, responsive, and accessible.
