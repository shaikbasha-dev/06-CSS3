# Element Selector

## Learning Objectives

After completing this topic, you will be able to:

- Understand what an Element Selector is.
- Learn the syntax of an Element Selector.
- Apply styles to HTML elements using their tag names.
- Understand when an Element Selector should be used.
- Differentiate Element Selectors from other selector types.
- Follow best practices while using Element Selectors.

---

# Prerequisites

Before learning this topic, you should understand:

- HTML Basics
- CSS Introduction
- CSS Syntax
- CSS Selectors Overview

---

# Introduction

The **Element Selector** is the simplest and most commonly used CSS selector. It selects HTML elements based on their tag names.

Whenever an Element Selector is used, the browser applies the specified CSS properties to **every matching HTML element** on the webpage.

For example, if the selector is `p`, every `<p>` element in the document will receive the specified styles.

Element Selectors are ideal for applying common styles to all instances of a particular HTML element.

---

# Definition

An **Element Selector** is a CSS selector that selects HTML elements using their tag names.

It applies the specified styles to every matching element in the document.

---

# Syntax

```css
element-name {

    property: value;

}
```

---

# Syntax Breakdown

| Component | Description |
|-----------|-------------|
| `element-name` | The HTML tag name to be selected |
| `{ }` | Contains CSS declarations |
| `property` | Specifies what should be styled |
| `value` | Specifies how the property should appear |

---

# Basic Example

## HTML

```html
<h1>Welcome to CSS</h1>

<p>This is the first paragraph.</p>

<p>This is the second paragraph.</p>
```

## CSS

```css
p {

    color: blue;

}
```

### Output

Both paragraph elements become blue because the selector targets every `<p>` element.

---

# How Element Selector Works

1. The browser reads the HTML document.
2. It loads the CSS stylesheet.
3. It finds the Element Selector.
4. It searches for all HTML elements having the specified tag name.
5. The CSS declarations are applied to every matching element.

---

# Characteristics

- Uses HTML tag names.
- Selects all matching elements.
- Easy to understand.
- Very beginner friendly.
- Frequently used in CSS.

---

# Advantages

- Simple syntax.
- Easy to learn.
- Styles multiple elements simultaneously.
- Reduces duplicate CSS code.
- Useful for applying global element styles.

---

# Disadvantages

- Cannot target individual elements.
- Affects every matching element.
- Less flexible than Class and ID Selectors.
- Not suitable for selective styling.

---

# When to Use Element Selector

Use an Element Selector when:

- Every element of the same type should have identical styling.
- Applying default styles.
- Styling headings.
- Styling paragraphs.
- Styling tables.
- Styling lists.

---

# When to Avoid Element Selector

Avoid using an Element Selector when:

- Only one element needs styling.
- Different elements require different appearances.
- Reusable component styling is needed.

In these situations, use Class or ID Selectors.

---

# Real-World Examples

### Example 1

```css
h1 {

    color: navy;

}
```

Styles every `<h1>` element.

---

### Example 2

```css
p {

    font-size: 18px;

}
```

Styles every paragraph.

---

### Example 3

```css
table {

    border-collapse: collapse;

}
```

Styles every table.

---

### Example 4

```css
img {

    width: 200px;

}
```

Styles every image.

---

### Example 5

```css
button {

    background-color: green;

}
```

Styles every button.

---

# Best Practices

- Use Element Selectors for common styles.
- Combine with Class Selectors when necessary.
- Avoid excessive Element Selector usage in large projects.
- Keep selectors simple and readable.
- Maintain consistent formatting.

---

# Common Beginner Mistakes

- Expecting only one element to be styled.
- Confusing Element Selectors with Class Selectors.
- Confusing Element Selectors with ID Selectors.
- Applying too many styles globally.
- Ignoring selector specificity.

---

# Interview Tips

Interviewers commonly ask:

- What is an Element Selector?
- How does an Element Selector work?
- Can it style multiple elements?
- When should Element Selectors be used?
- What are its limitations?

Support your answers with practical examples.

---

# Frequently Asked Interview Questions

## 1. What is an Element Selector?

An Element Selector selects HTML elements using their tag names.

---

## 2. Can an Element Selector select multiple elements?

Yes.

It styles every HTML element having the specified tag name.

---

## 3. Is an Element Selector reusable?

Yes.

Every matching HTML element automatically receives the specified styles.

---

## 4. Does an Element Selector have high specificity?

No.

It has lower specificity than Class and ID Selectors.

---

## 5. When should an Element Selector be used?

It should be used when all elements of the same type require identical styling.

---

# Key Takeaways

- Uses HTML tag names.
- Styles all matching elements.
- Simple and beginner friendly.
- Commonly used for default styling.
- Lower specificity than Class and ID Selectors.

---

# Related Topics

Previous Topics

- CSS Selectors Overview

Next Topics

- ID Selector
- Class Selector
- Grouping Selector
- Universal Selector

---

# Summary

The Element Selector is the simplest CSS selector and forms the foundation of CSS styling. By selecting HTML elements through their tag names, it allows developers to apply consistent styles across all matching elements with minimal code. Although it is ideal for global styling and beginner-friendly projects, more specific selectors such as Class and ID Selectors should be used when individual or reusable styling is required.
