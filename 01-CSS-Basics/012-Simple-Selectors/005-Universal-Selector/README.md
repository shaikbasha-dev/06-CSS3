# Universal Selector

## Learning Objectives

After completing this topic, you will be able to:

- Understand what the Universal Selector is.
- Learn the syntax of the Universal Selector.
- Apply styles to every HTML element on a webpage.
- Understand common use cases of the Universal Selector.
- Follow best practices while using the Universal Selector.

---

# Prerequisites

Before learning this topic, you should understand:

- HTML Basics
- CSS Introduction
- CSS Syntax
- CSS Selectors Overview
- Element Selector
- ID Selector
- Class Selector
- Grouping Selector

---

# Introduction

The **Universal Selector** is a CSS selector that targets **every HTML element** on a webpage.

Instead of selecting specific elements, classes, or IDs, the Universal Selector applies the specified CSS rules to all elements within the selected scope.

The Universal Selector is commonly used to reset default browser styles, ensuring a consistent appearance across different browsers before applying custom styling.

---

# Definition

A **Universal Selector** is a CSS selector that selects every HTML element.

It is represented by the asterisk (`*`) symbol.

---

# Syntax

```css
* {

    margin: 0;

    padding: 0;

}
```

---

# Syntax Breakdown

| Component | Description |
|-----------|-------------|
| `*` | Universal Selector |
| `{ }` | Contains CSS declarations |
| `property` | CSS property to apply |
| `value` | Value assigned to the property |

---

# How Universal Selector Works

1. The browser reads the HTML document.
2. The CSS stylesheet is loaded.
3. The Universal Selector matches every HTML element.
4. The specified CSS properties are applied to all matched elements.
5. More specific selectors can override the Universal Selector.

---

# Characteristics

- Uses the `*` symbol.
- Selects every HTML element.
- Has very low specificity.
- Often used at the beginning of a stylesheet.
- Commonly used for CSS resets.
- Can be overridden by more specific selectors.

---

# Advantages

- Removes default browser spacing.
- Creates consistent layouts.
- Reduces repetitive reset code.
- Simplifies global styling.
- Useful for professional CSS development.

---

# Disadvantages

- Affects every HTML element.
- Overuse may reduce performance on very large pages.
- Can unintentionally style elements that should remain unchanged.
- Requires more specific selectors to override styles.

---

# When to Use Universal Selector

Use the Universal Selector when:

- Resetting browser default styles.
- Applying `box-sizing` globally.
- Removing default margins and padding.
- Creating consistent layouts.
- Building reusable CSS templates.

---

# When to Avoid Universal Selector

Avoid using the Universal Selector when:

- Only specific elements need styling.
- Large-scale styling should be limited to selected elements.
- Fine-grained control is required.

---

# Real-World Examples

## Example 1

```css
* {

    margin: 0;

    padding: 0;

}
```

Removes the default spacing from all HTML elements.

---

## Example 2

```css
* {

    box-sizing: border-box;

}
```

Ensures padding and borders are included within an element's total width and height.

---

## Example 3

```css
* {

    font-family: Arial, sans-serif;

}
```

Applies the same font to every HTML element.

---

## Example 4

```css
* {

    color: #333333;

}
```

Sets a default text color for all elements.

---

## Example 5

```css
* {

    transition: all 0.3s ease;

}
```

Adds a default transition effect to all elements.

---

# Universal Selector vs Element Selector

| Feature | Universal Selector | Element Selector |
|----------|--------------------|------------------|
| Syntax | `*` | `p`, `h1`, `div` |
| Targets | Every HTML element | Specific HTML elements |
| Scope | Entire webpage | Selected elements only |
| Common Use | CSS Reset | Normal styling |
| Specificity | Very Low | Low |

---

# Best Practices

- Use it mainly for CSS resets.
- Keep the Universal Selector near the top of the stylesheet.
- Avoid unnecessary styling through the Universal Selector.
- Override global styles using more specific selectors.
- Combine it with `box-sizing: border-box` whenever appropriate.

---

# Common Beginner Mistakes

- Styling every element unnecessarily.
- Assuming the Universal Selector has high specificity.
- Forgetting that more specific selectors override it.
- Using it where an Element or Class Selector would be more appropriate.
- Applying excessive global styles.

---

# Interview Tips

Interviewers commonly ask:

- What is the Universal Selector?
- Which symbol represents the Universal Selector?
- Why is it commonly used in CSS resets?
- Does the Universal Selector have high specificity?
- Why is `box-sizing: border-box` often used with it?

Support your answers with practical examples.

---

# Frequently Asked Interview Questions

## 1. What is the Universal Selector?

The Universal Selector selects every HTML element on a webpage.

---

## 2. Which symbol represents the Universal Selector?

The asterisk (`*`) symbol.

---

## 3. Why is the Universal Selector commonly used?

It is commonly used to reset browser default styles and create consistent layouts.

---

## 4. Does the Universal Selector have high specificity?

No.

It has very low specificity and can easily be overridden by more specific selectors.

---

## 5. What is the most common use of the Universal Selector?

Applying CSS reset rules such as:

```css
* {

    margin: 0;

    padding: 0;

    box-sizing: border-box;

}
```

---

# Key Takeaways

- Uses the `*` symbol.
- Targets every HTML element.
- Commonly used for CSS resets.
- Has very low specificity.
- Creates consistent layouts.
- Frequently appears at the beginning of CSS stylesheets.

---

# Related Topics

Previous Topics

- Element Selector
- ID Selector
- Class Selector
- Grouping Selector

Next Topics

- Link Pseudo-Class Selector
- Visited Pseudo-Class Selector

---

# Summary

The **Universal Selector** is represented by the `*` symbol and selects every HTML element on a webpage. It is primarily used for resetting browser default styles, applying global settings such as `box-sizing: border-box`, and creating consistent layouts across different browsers. Since it affects all elements, it should be used carefully and combined with more specific selectors whenever detailed styling is required.
