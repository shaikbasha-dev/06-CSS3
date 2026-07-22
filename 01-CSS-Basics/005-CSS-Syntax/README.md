# CSS Syntax

## Learning Objectives

After completing this topic, you will be able to:

- Understand the syntax of CSS.
- Identify the different parts of a CSS rule.
- Write valid CSS rules using proper syntax.
- Apply CSS properties and values correctly.
- Follow standard CSS coding conventions.
- Avoid common syntax errors.

---

# Prerequisites

Before learning this topic, you should understand:

- HTML Basics
- CSS Introduction
- Why CSS is Used
- History of CSS
- Advantages of CSS

---

# Introduction

Every programming or styling language follows a specific syntax. CSS also has a well-defined syntax that determines how style rules are written and interpreted by web browsers.

Understanding CSS syntax is one of the most important fundamentals because every CSS rule, whether simple or complex, follows the same structure.

Without proper syntax, browsers cannot correctly apply styles to HTML elements.

---

# Definition

CSS Syntax is the standard structure used to write CSS rules that define how HTML elements should be displayed.

A CSS rule consists of a selector and a declaration block.

---

# Why CSS Syntax is Important

Proper CSS syntax helps developers:

- Write valid CSS code.
- Improve code readability.
- Reduce syntax errors.
- Make styles easier to maintain.
- Improve collaboration among developers.
- Ensure browser compatibility.

---

# Basic CSS Syntax

```css
selector {

    property: value;

}
```

---

# Syntax Components

A CSS rule consists of the following parts:

## 1. Selector

The selector identifies the HTML element that should receive the style.

Example:

```css
h1
```

Here,

`h1` is the selector.

---

## 2. Declaration Block

The declaration block contains one or more CSS declarations.

It is enclosed inside curly braces.

Example:

```css
{

}
```

---

## 3. Property

A property specifies which style should be changed.

Examples:

```css
color
font-size
background-color
margin
padding
```

---

## 4. Value

A value specifies how the property should be applied.

Examples:

```css
red
blue
20px
center
bold
```

---

## Complete Example

```css
h1 {

    color: blue;

    font-size: 40px;

}
```

Explanation:

- Selector → h1
- Property → color
- Value → blue
- Property → font-size
- Value → 40px

---

# General Syntax Formula

```text
Selector
{
    Property : Value;
}
```

---

# Syntax Rules

Follow these rules while writing CSS:

- Every declaration must end with a semicolon.
- Properties and values are separated using a colon.
- Declarations must be enclosed inside curly braces.
- Property names are case-insensitive, but lowercase is recommended.
- Property values must be valid.
- Write one declaration per line for better readability.

---

# Multiple Declarations

```css
p {

    color: black;

    font-size: 18px;

    text-align: justify;

}
```

---

# Incorrect Syntax

```css
h1

color blue

font-size 40px
```

Problems:

- Missing braces.
- Missing colon.
- Missing semicolon.

---

# Correct Syntax

```css
h1 {

    color: blue;

    font-size: 40px;

}
```

---

# Real-World Example

```css
button {

    background-color: royalblue;

    color: white;

    padding: 12px;

    border-radius: 6px;

}
```

This rule styles every button on a webpage.

---

# Best Practices

- Use proper indentation.
- Write one declaration per line.
- Use meaningful selectors.
- Keep property names lowercase.
- Group related properties together.
- Maintain consistent formatting throughout the project.

---

# Common Beginner Mistakes

- Forgetting semicolons.
- Missing curly braces.
- Misspelling property names.
- Using invalid values.
- Writing properties outside the declaration block.
- Forgetting the colon between property and value.

---

# Interview Tips

Interviewers commonly ask:

- What is CSS syntax?
- What are the components of a CSS rule?
- What is a selector?
- What is a declaration block?
- What happens if a semicolon is omitted?

Practice writing CSS rules instead of only memorizing definitions.

---

# Frequently Asked Interview Questions

## 1. What is CSS syntax?

CSS syntax is the standard structure used to write CSS rules.

---

## 2. What are the main parts of CSS syntax?

- Selector
- Declaration Block
- Property
- Value

---

## 3. Why is a semicolon used?

A semicolon separates one declaration from another.

---

## 4. Can a declaration block contain multiple properties?

Yes.

A declaration block can contain any number of valid CSS declarations.

---

## 5. Why are curly braces used?

Curly braces define the beginning and end of a declaration block.

---

# Key Takeaways

- Every CSS rule follows the same syntax.
- A selector identifies the HTML element.
- Properties define what should change.
- Values specify how the change should occur.
- Correct syntax is essential for writing valid CSS.

---

# Related Topics

Previous Topics

- CSS Introduction
- Why CSS
- History of CSS
- Advantages of CSS

Next Topic

- Ways to Apply CSS

---

# Summary

CSS syntax provides the foundation for writing every stylesheet. By understanding selectors, declaration blocks, properties, and values, developers can create clean, maintainable, and standards-compliant CSS. Mastering CSS syntax is the first step toward building responsive, professional, and visually appealing web applications.
