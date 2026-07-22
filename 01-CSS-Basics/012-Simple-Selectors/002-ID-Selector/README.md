# ID Selector

## Learning Objectives

After completing this topic, you will be able to:

- Understand what an ID Selector is.
- Learn the syntax of an ID Selector.
- Apply styles to a specific HTML element using its unique ID.
- Understand when an ID Selector should be used.
- Differentiate between ID Selectors and other selector types.
- Follow best practices while using ID Selectors.

---

# Prerequisites

Before learning this topic, you should understand:

- HTML Basics
- CSS Introduction
- CSS Syntax
- CSS Selectors Overview
- Element Selector

---

# Introduction

The **ID Selector** is one of the most commonly used CSS selectors. It is used to style a **single, unique HTML element** by using the value of its `id` attribute.

Unlike the Element Selector, which styles every matching HTML element, the ID Selector targets only one specific element in an HTML document.

Every HTML document should contain **unique ID values**, meaning the same ID should not be assigned to multiple elements.

Because an ID uniquely identifies an element, it has a higher specificity than Element and Class Selectors.

---

# Definition

An **ID Selector** is a CSS selector that selects an HTML element based on the value of its `id` attribute.

The selector begins with the hash (`#`) symbol followed by the ID name.

---

# Syntax

## HTML

```html
<h1 id="title">Welcome to CSS</h1>
```

## CSS

```css
#title {

    color: blue;

}
```

---

# Syntax Breakdown

| Component | Description |
|-----------|-------------|
| `#` | Indicates an ID Selector |
| `title` | The unique ID value assigned to an HTML element |
| `{ }` | Contains CSS declarations |
| `property` | Specifies what should be styled |
| `value` | Specifies how the property should appear |

---

# How ID Selector Works

1. The browser reads the HTML document.
2. It loads the CSS stylesheet.
3. It finds the ID Selector.
4. It searches for the element having the specified ID.
5. The CSS properties are applied only to that element.

---

# Characteristics

- Uses the `id` attribute.
- Begins with the `#` symbol.
- Targets only one unique HTML element.
- Has higher specificity than Element and Class Selectors.
- Commonly used for unique webpage components.

---

# Advantages

- Targets a specific element.
- Higher specificity.
- Easy to identify important webpage sections.
- Ideal for unique page components.
- Frequently used for navigation and layout.

---

# Disadvantages

- Cannot be reused across multiple elements.
- Overusing IDs reduces CSS flexibility.
- Not suitable for reusable components.
- Duplicate IDs create invalid HTML.

---

# When to Use ID Selector

Use an ID Selector when:

- Styling a unique webpage element.
- Designing headers and footers.
- Styling navigation bars.
- Creating unique banners.
- Targeting a specific section of a webpage.

---

# When to Avoid ID Selector

Avoid using an ID Selector when:

- Multiple elements require identical styling.
- Creating reusable UI components.
- Building scalable CSS architectures.

In these situations, Class Selectors are a better choice.

---

# Real-World Examples

## Example 1

```css
#header {

    background-color: navy;

}
```

Styles only the webpage header.

---

## Example 2

```css
#footer {

    color: white;

}
```

Styles only the footer.

---

## Example 3

```css
#loginButton {

    background-color: green;

}
```

Styles only the login button.

---

## Example 4

```css
#banner {

    height: 300px;

}
```

Styles only the banner.

---

## Example 5

```css
#profileImage {

    border-radius: 50%;

}
```

Styles only the profile image.

---

# ID Selector vs Element Selector

| Feature | Element Selector | ID Selector |
|----------|------------------|-------------|
| Targets | All matching elements | One unique element |
| Syntax | `p` | `#idName` |
| Reusability | High | None |
| Specificity | Low | High |
| Usage | Common styling | Unique styling |

---

# Best Practices

- Keep every ID unique.
- Use meaningful ID names.
- Avoid spaces in ID names.
- Use camelCase or kebab-case consistently.
- Reserve IDs for unique elements.
- Use Classes for reusable styles.

---

# Common Beginner Mistakes

- Assigning the same ID to multiple elements.
- Forgetting to prefix the selector with `#`.
- Using IDs for reusable styling.
- Using meaningless ID names.
- Confusing IDs with Classes.

---

# Interview Tips

Interviewers commonly ask:

- What is an ID Selector?
- Why must IDs be unique?
- What symbol represents an ID Selector?
- Which has higher specificity: ID or Class?
- When should an ID Selector be used?

Support your answers with practical examples.

---

# Frequently Asked Interview Questions

## 1. What is an ID Selector?

An ID Selector selects an HTML element using the value of its `id` attribute.

---

## 2. Which symbol is used for an ID Selector?

The hash (`#`) symbol.

---

## 3. Can multiple elements have the same ID?

No.

Every ID value should be unique within an HTML document.

---

## 4. Does the ID Selector have higher specificity than the Class Selector?

Yes.

The ID Selector has higher specificity than the Class Selector.

---

## 5. When should an ID Selector be used?

It should be used when styling a unique HTML element.

---

# Key Takeaways

- Uses the `id` attribute.
- Begins with the `#` symbol.
- Targets one unique HTML element.
- Has higher specificity than Class and Element Selectors.
- Best suited for unique webpage components.

---

# Related Topics

Previous Topics

- CSS Selectors Overview
- Element Selector

Next Topics

- Class Selector
- Grouping Selector
- Universal Selector

---

# Summary

The ID Selector is used to style a single, unique HTML element by selecting its `id` attribute. It provides greater specificity than Element and Class Selectors, making it suitable for unique webpage components such as headers, navigation bars, banners, and footers. Since every ID must be unique within an HTML document, developers should use ID Selectors carefully and reserve them for elements that require unique styling.
