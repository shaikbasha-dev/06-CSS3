# Pseudo-Class Selectors

## Learning Objectives

After completing this section, you will be able to:

- Understand what Pseudo-Class Selectors are.
- Learn why Pseudo-Class Selectors are used.
- Understand how browsers apply different states to HTML elements.
- Learn the four hyperlink pseudo-classes.
- Apply multiple pseudo-classes to the same hyperlink.
- Understand the correct order of pseudo-classes (LVHA Rule).
- Build interactive webpages using CSS Pseudo-Class Selectors.

---

# Prerequisites

Before learning Pseudo-Class Selectors, you should understand:

- HTML Basics
- CSS Syntax
- CSS Selectors
- Simple Selectors
- Hyperlinks (`<a>` tag)

---

# Introduction

CSS allows developers to style HTML elements based on different conditions.

Sometimes an element changes its appearance because of user interaction.

For example:

- A hyperlink before visiting
- A hyperlink after visiting
- A hyperlink when the mouse pointer is placed over it
- A hyperlink while it is being clicked

These temporary conditions are called **Pseudo Classes**.

Instead of adding JavaScript, CSS can automatically detect these states and apply different styles.

This makes webpages interactive while keeping the code simple and efficient.

---

# Definition

A **Pseudo-Class Selector** selects an HTML element based on its current state rather than its position or attributes.

A pseudo-class begins with a single colon (`:`).

Example:

```css
a:hover {

    color: red;

}
```

---

# Why Pseudo-Class Selectors?

Pseudo-Class Selectors help developers:

- Create interactive webpages.
- Improve user experience.
- Provide visual feedback.
- Highlight clickable elements.
- Make navigation easier.
- Improve accessibility.
- Reduce JavaScript for simple interactions.

---

# Syntax

```css
selector:pseudo-class {

    property: value;

}
```

Example

```css
a:hover {

    color: red;

}
```

---

# Syntax Breakdown

| Component | Description |
|-----------|-------------|
| `selector` | HTML element to target |
| `:` | Indicates a pseudo-class |
| `pseudo-class` | Current state of the element |
| `{ }` | Contains CSS declarations |
| `property` | CSS property |
| `value` | Assigned value |

---

# Pseudo-Class Selectors Covered

This section demonstrates the complete lifecycle of a hyperlink using the following four pseudo-classes.

| No. | Pseudo-Class | Purpose |
|----:|--------------|---------|
| 1 | `:link` | Styles hyperlinks that have not yet been visited. |
| 2 | `:visited` | Styles hyperlinks that have already been visited. |
| 3 | `:hover` | Styles hyperlinks when the mouse pointer is placed over them. |
| 4 | `:active` | Styles hyperlinks while they are being clicked. |

---

# Browser Working Process

Whenever a webpage loads, the browser checks the current state of every hyperlink.

Depending on that state, the browser automatically applies the appropriate pseudo-class.

Example:

- Never opened
  - `:link`

↓

- Mouse pointer enters

  - `:hover`

↓

- Mouse button pressed

  - `:active`

↓

- Page opens

↓

- Browser saves browsing history

↓

- Next time

  - `:visited`

---

# Hyperlink Lifecycle

```text
Create Link
      │
      ▼
Page Loads
      │
      ▼
a:link
      │
      ▼
Mouse Moves Over Link
      │
      ▼
a:hover
      │
      ▼
Mouse Button Pressed
      │
      ▼
a:active
      │
      ▼
Navigation Completed
      │
      ▼
a:visited
```

---

# The LVHA Rule

When writing hyperlink pseudo-classes, always use the following order:

```css
a:link

a:visited

a:hover

a:active
```

This is called the **LVHA Rule**.

Meaning:

- L → Link
- V → Visited
- H → Hover
- A → Active

Following this order prevents unexpected styling behavior.

---

# Explanation of Each Pseudo-Class

## 1. :link

Targets hyperlinks that have never been visited.

Example

```css
a:link {

    color: blue;

}
```

---

## 2. :visited

Targets hyperlinks that were previously visited.

Example

```css
a:visited {

    color: purple;

}
```

---

## 3. :hover

Targets hyperlinks while the mouse pointer is over them.

Example

```css
a:hover {

    color: red;

}
```

---

## 4. :active

Targets hyperlinks while the mouse button is being pressed.

Example

```css
a:active {

    color: green;

}
```

---

# Complete Example

```css
a:link {

    color: blue;

}

a:visited {

    color: purple;

}

a:hover {

    color: red;

}

a:active {

    color: green;

}
```

---

# Real-World Applications

Pseudo-Class Selectors are commonly used for:

- Website navigation menus
- Buttons
- Sidebar links
- Footer links
- Documentation websites
- E-commerce websites
- Government portals
- Educational platforms
- Portfolio websites

---

# Advantages

- Improves user interaction.
- Makes webpages dynamic.
- Provides visual feedback.
- Requires no JavaScript.
- Easy to implement.
- Improves usability.
- Widely supported by browsers.

---

# Limitations

- Depends on browser state.
- Some browser security restrictions apply to `:visited`.
- Limited compared to JavaScript interactions.

---

# Best Practices

- Always follow the LVHA Rule.
- Keep colors consistent.
- Ensure sufficient contrast.
- Do not rely only on color to indicate state.
- Test hyperlinks after styling.
- Keep hover effects smooth and meaningful.

---

# Common Beginner Mistakes

- Writing pseudo-classes in the wrong order.
- Forgetting the colon (`:`).
- Styling only `:hover`.
- Ignoring `:visited`.
- Using identical styles for every state.

---

# Interview Tips

Interviewers commonly ask:

- What is a Pseudo-Class Selector?
- What is the difference between a pseudo-class and a pseudo-element?
- What is the LVHA Rule?
- Why is `:visited` restricted?
- Which pseudo-class is applied while clicking?

Support your answers with practical examples.

---

# Frequently Asked Interview Questions

## 1. What is a Pseudo-Class Selector?

A Pseudo-Class Selector styles an element based on its current state.

---

## 2. Which symbol represents a pseudo-class?

A single colon (`:`).

---

## 3. What does `:hover` do?

It styles an element while the mouse pointer is placed over it.

---

## 4. What does `:visited` do?

It styles hyperlinks that have already been visited.

---

## 5. What is the correct order of hyperlink pseudo-classes?

Link → Visited → Hover → Active

(LVHA Rule)

---

# Key Takeaways

- Pseudo-Class Selectors style elements based on state.
- Hyperlinks have four common states.
- Follow the LVHA Rule.
- Improve user interaction without JavaScript.
- Used extensively in modern websites.

---

# Folder Structure

```text
013-Pseudo-Class-Selectors/
│
├── README.md
├── index.html
├── style.css
├── HTML-Line-by-Line-Explanation.md
├── CSS-Line-by-Line-Explanation.md
└── Pseudo-Code.md
```

---

# Related Topics

Previous Topics

- CSS Selectors
- Simple Selectors

Next Topics

- Pseudo-Element Selectors
- Combinator Selectors
- Attribute Selectors

---

# Summary

Pseudo-Class Selectors enable CSS to style HTML elements according to their current state, creating interactive and user-friendly webpages without requiring JavaScript. This module demonstrates the complete lifecycle of a hyperlink using `:link`, `:visited`, `:hover`, and `:active`, explains the LVHA Rule, and provides the foundation for understanding state-based styling in modern web development.
