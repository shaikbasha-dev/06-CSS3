# Class Selector

## Learning Objectives

After completing this topic, you will be able to:

- Understand what a Class Selector is.
- Learn the syntax of a Class Selector.
- Apply the same CSS styles to multiple HTML elements.
- Understand when to use a Class Selector.
- Differentiate between Class Selectors and ID Selectors.
- Follow best practices for writing reusable CSS.

---

# Prerequisites

Before learning this topic, you should understand:

- HTML Basics
- CSS Introduction
- CSS Syntax
- CSS Selectors Overview
- Element Selector
- ID Selector

---

# Introduction

The **Class Selector** is one of the most powerful and frequently used CSS selectors. It is used to apply the same styles to **multiple HTML elements** by using the value of their `class` attribute.

Unlike the ID Selector, which targets only one unique element, the Class Selector allows developers to reuse the same styling across many elements, making CSS cleaner, more organized, and easier to maintain.

Class Selectors are widely used in professional web development because they promote reusable and scalable styling.

---

# Definition

A **Class Selector** is a CSS selector that selects one or more HTML elements based on the value of their `class` attribute.

The selector begins with a period (`.`) followed by the class name.

---

# Syntax

## HTML

```html
<p class="highlight">Learning CSS</p>

<h2 class="highlight">Class Selector Example</h2>
```

## CSS

```css
.highlight {

    color: blue;

    font-weight: bold;

}
```

---

# Syntax Breakdown

| Component | Description |
|-----------|-------------|
| `.` | Indicates a Class Selector |
| `highlight` | Name of the CSS class |
| `{ }` | Contains CSS declarations |
| `property` | Specifies what should be styled |
| `value` | Specifies how the property should appear |

---

# How Class Selector Works

1. The browser reads the HTML document.
2. It loads the CSS stylesheet.
3. It finds the Class Selector.
4. It searches for all elements having the specified class.
5. The CSS properties are applied to every matching element.

---

# Characteristics

- Uses the `class` attribute.
- Begins with the `.` symbol.
- Can target multiple HTML elements.
- Reusable throughout the webpage.
- Lower specificity than an ID Selector.
- One element can have multiple classes.

---

# Advantages

- Promotes code reusability.
- Reduces duplicate CSS.
- Easy to maintain.
- Suitable for large websites.
- Helps create consistent user interfaces.
- Supports multiple classes on a single element.

---

# Disadvantages

- Lower specificity than ID Selectors.
- Poor naming conventions can reduce readability.
- Excessive classes can make HTML difficult to manage.

---

# When to Use Class Selector

Use a Class Selector when:

- Multiple elements require the same style.
- Creating reusable UI components.
- Styling buttons.
- Designing cards.
- Creating alerts.
- Building responsive layouts.

---

# When to Avoid Class Selector

Avoid using a Class Selector when:

- Styling a unique element that appears only once.
- The element requires unique identification.

In these situations, an ID Selector is more appropriate.

---

# Real-World Examples

## Example 1

```css
.button {

    background-color: green;

}
```

Styles all buttons having the `button` class.

---

## Example 2

```css
.card {

    border-radius: 8px;

}
```

Styles every card component.

---

## Example 3

```css
.highlight {

    background-color: yellow;

}
```

Highlights important content.

---

## Example 4

```css
.warning {

    color: red;

}
```

Displays warning messages.

---

## Example 5

```css
.center {

    text-align: center;

}
```

Centers multiple HTML elements.

---

# Class Selector vs ID Selector

| Feature | Class Selector | ID Selector |
|----------|---------------|-------------|
| Syntax | `.className` | `#idName` |
| Targets | Multiple elements | One unique element |
| Reusable | Yes | No |
| Specificity | Medium | High |
| HTML Attribute | `class` | `id` |

---

# Best Practices

- Use meaningful class names.
- Follow consistent naming conventions.
- Keep class names reusable.
- Avoid unnecessary class duplication.
- Use kebab-case or camelCase consistently.
- Keep class names simple and descriptive.

---

# Common Beginner Mistakes

- Confusing Class Selectors with ID Selectors.
- Forgetting to use the `.` symbol.
- Using meaningless class names.
- Creating too many unnecessary classes.
- Using IDs where reusable classes are more appropriate.

---

# Interview Tips

Interviewers frequently ask:

- What is a Class Selector?
- Which symbol represents a Class Selector?
- Can multiple elements have the same class?
- Can one element have multiple classes?
- What is the difference between Class and ID Selectors?

Provide practical examples while answering.

---

# Frequently Asked Interview Questions

## 1. What is a Class Selector?

A Class Selector selects one or more HTML elements using the value of their `class` attribute.

---

## 2. Which symbol represents a Class Selector?

The period (`.`) symbol.

---

## 3. Can multiple elements have the same class?

Yes.

A Class Selector is specifically designed for reusable styling across multiple elements.

---

## 4. Can one HTML element have multiple classes?

Yes.

An element can contain multiple class names separated by spaces.

Example:

```html
<button class="button primary rounded">
    Save
</button>
```

---

## 5. Which has higher specificity?

The ID Selector has higher specificity than the Class Selector.

---

# Key Takeaways

- Uses the `class` attribute.
- Begins with the `.` symbol.
- Styles multiple HTML elements.
- Promotes reusable CSS.
- One element can have multiple classes.
- Ideal for scalable web development.

---

# Related Topics

Previous Topics

- CSS Selectors Overview
- Element Selector
- ID Selector

Next Topics

- Grouping Selector
- Universal Selector

---

# Summary

The **Class Selector** is one of the most important CSS selectors because it enables developers to apply consistent styles to multiple HTML elements using the `class` attribute. Since Class Selectors are reusable, they improve maintainability, reduce duplicate CSS code, and help build scalable web applications. They are preferred whenever multiple elements share the same appearance, while unique elements should generally use ID Selectors.
