# Internal CSS

## Learning Objectives

After completing this topic, you will be able to:

- Understand what Internal CSS is.
- Write CSS inside the `<style>` element.
- Apply styles to multiple HTML elements within a single webpage.
- Differentiate between Internal CSS and Inline CSS.
- Identify when Internal CSS should be used.
- Follow best practices while writing Internal CSS.

---

# Prerequisites

Before learning this topic, you should understand:

- HTML Basics
- CSS Introduction
- CSS Syntax
- Ways to Apply CSS
- Inline CSS

---

# Introduction

Internal CSS is one of the three methods used to apply CSS to an HTML document. Unlike Inline CSS, which applies styles to individual elements, Internal CSS allows multiple elements within the same webpage to share common styles.

The CSS rules are written inside the `<style>` element, which is placed within the `<head>` section of an HTML document.

Internal CSS is useful for single-page websites, prototypes, demonstrations, and webpages that do not require a separate stylesheet.

---

# Definition

Internal CSS is a method of applying CSS by writing style rules inside the `<style>` element of an HTML document.

The styles defined inside the `<style>` element apply only to the current webpage.

---

# Syntax

```html
<!DOCTYPE html>

<html>

<head>

    <style>

        selector {

            property: value;

        }

    </style>

</head>

<body>

</body>

</html>
```

---

# Syntax Breakdown

| Component | Description |
|-----------|-------------|
| `<style>` | HTML element used to define Internal CSS |
| `selector` | Selects the HTML element to style |
| `property` | Specifies what should be styled |
| `value` | Specifies how the property should appear |

---

# Basic Example

```html
<!DOCTYPE html>

<html>

<head>

    <style>

        h1{

            color: blue;

        }

    </style>

</head>

<body>

    <h1>Welcome to CSS</h1>

</body>

</html>
```

---

# How Internal CSS Works

1. The browser reads the HTML document.
2. It processes the `<style>` element inside the `<head>`.
3. CSS rules are stored.
4. Matching HTML elements are identified.
5. Styles are applied to all matching elements on that webpage.

---

# Characteristics

- CSS is written inside the `<style>` element.
- Styles apply only to the current HTML page.
- One CSS rule can style multiple elements.
- No external stylesheet is required.
- Easier to maintain than Inline CSS.

---

# Advantages

- Cleaner HTML compared to Inline CSS.
- Multiple elements can share the same styles.
- Easy to modify styles for a single webpage.
- No additional CSS file is required.
- Suitable for small projects and demonstrations.

---

# Disadvantages

- Styles cannot be reused across multiple webpages.
- HTML file size increases.
- Difficult to maintain for large websites.
- Not recommended for enterprise applications.

---

# When to Use Internal CSS

Internal CSS is suitable for:

- Single-page websites
- Demonstration programs
- Learning CSS
- Prototype applications
- Small web projects

---

# When to Avoid Internal CSS

Avoid Internal CSS when:

- Building multi-page websites
- Developing enterprise applications
- Creating reusable designs
- Working on large projects

In such cases, External CSS should be preferred.

---

# Internal CSS vs Inline CSS

| Feature | Inline CSS | Internal CSS |
|----------|------------|--------------|
| Location | Inside `style` attribute | Inside `<style>` element |
| Reusability | No | Within the same page |
| Maintainability | Poor | Better |
| Suitable for Multiple Elements | No | Yes |
| Suitable for Large Projects | No | No |

---

# Best Practices

- Place the `<style>` element inside the `<head>` section.
- Group related CSS rules together.
- Use meaningful selectors.
- Keep consistent indentation.
- Avoid duplicate CSS rules.
- Move reusable styles to an external stylesheet when the project grows.

---

# Common Beginner Mistakes

- Writing the `<style>` element inside the `<body>`.
- Mixing Inline CSS and Internal CSS unnecessarily.
- Writing duplicate CSS rules.
- Forgetting curly braces.
- Omitting semicolons between declarations.

---

# Interview Tips

Interviewers commonly ask:

- What is Internal CSS?
- Where is Internal CSS written?
- When should Internal CSS be used?
- What are the advantages of Internal CSS?
- What is the difference between Inline CSS and Internal CSS?

Support your answers with practical examples.

---

# Frequently Asked Interview Questions

## 1. What is Internal CSS?

Internal CSS is a method of applying CSS by writing style rules inside the `<style>` element within the `<head>` section of an HTML document.

---

## 2. Which HTML element is used for Internal CSS?

The `<style>` element.

---

## 3. Can Internal CSS style multiple elements?

Yes.

One CSS rule can style all matching elements within the current webpage.

---

## 4. Can Internal CSS be reused across multiple webpages?

No.

Its scope is limited to the HTML document in which it is written.

---

## 5. Is Internal CSS suitable for professional websites?

It can be used for small or single-page websites, but External CSS is preferred for professional and large-scale applications.

---

# Key Takeaways

- Internal CSS is written inside the `<style>` element.
- Styles apply only to the current webpage.
- It is more maintainable than Inline CSS.
- It is suitable for single-page applications.
- External CSS is preferred for large projects.

---

# Related Topics

Previous Topics

- Ways to Apply CSS
- Inline CSS

Next Topics

- External CSS
- CSS Comments

---

# Summary

Internal CSS provides a structured way to style multiple elements within a single HTML document by placing CSS rules inside the `<style>` element. It improves maintainability compared to Inline CSS and is well suited for small projects, demonstrations, and single-page applications. However, for reusable and scalable styling across multiple webpages, External CSS remains the recommended approach.
