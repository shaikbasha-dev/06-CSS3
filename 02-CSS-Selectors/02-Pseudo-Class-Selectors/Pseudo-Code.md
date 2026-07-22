# Pseudo Code

## Objective

This document explains the logical workflow of the **Pseudo-Class Selectors** demonstration. Unlike source code, pseudocode focuses on the sequence of operations performed by the browser and the interactions between the user, HTML, and CSS.

---

# Introduction

Pseudo-Class Selectors allow CSS to apply different styles based on the current state of an HTML element.

In this module, a hyperlink changes its appearance depending on how the user interacts with it.

The browser automatically detects the current state and applies the corresponding pseudo-class.

The four hyperlink states demonstrated are:

- `:link`
- `:visited`
- `:hover`
- `:active`

---

# High-Level Algorithm

```text
START

Load HTML document

↓

Load external CSS stylesheet

↓

Display webpage

↓

Display hyperlinks

↓

Wait for user interaction

↓

Determine the current hyperlink state

↓

Apply matching pseudo-class

↓

Update hyperlink appearance

↓

Continue listening for user interaction

↓

END
```

---

# Detailed Pseudocode

```text
START

Load the HTML document.

Load the external CSS file.

Display all webpage content.

Display every hyperlink.

FOR each hyperlink

    Check whether the hyperlink has been visited.

    IF the hyperlink has NOT been visited THEN

        Apply :link style.

    ELSE

        Apply :visited style.

    END IF

END FOR

Wait for mouse movement.

IF the mouse pointer moves over a hyperlink THEN

    Apply :hover style.

END IF

Wait for mouse click.

IF the mouse button is pressed on a hyperlink THEN

    Apply :active style.

END IF

IF the browser opens the destination webpage THEN

    Save the webpage in browser history.

END IF

WHEN the webpage is opened again

    Apply :visited style.

STOP
```

---

# Browser Processing Flow

```text
HTML Document
      │
      ▼
Load CSS File
      │
      ▼
Create Webpage
      │
      ▼
Display Hyperlinks
      │
      ▼
Browser Checks Link State
      │
      ├──────────────► Never Visited
      │                     │
      │                     ▼
      │                 Apply :link
      │
      └──────────────► Already Visited
                            │
                            ▼
                      Apply :visited
```

---

# User Interaction Flow

```text
User Sees Hyperlink
        │
        ▼
Mouse Pointer Moves
        │
        ▼
Apply :hover
        │
        ▼
Mouse Button Pressed
        │
        ▼
Apply :active
        │
        ▼
Browser Opens Destination
        │
        ▼
Save Browsing History
        │
        ▼
Next Visit
        │
        ▼
Apply :visited
```

---

# Hyperlink Lifecycle

```text
Page Loads
      │
      ▼
Hyperlink Created
      │
      ▼
Is Link Already Visited?
      │
 ┌────┴────┐
 │         │
 ▼         ▼
No        Yes
 │         │
 ▼         ▼
:link   :visited
 │
 ▼
Mouse Over?
 │
 ▼
:hover
 │
 ▼
Mouse Click?
 │
 ▼
:active
 │
 ▼
Open Destination
 │
 ▼
Save History
 │
 ▼
:visited
```

---

# LVHA Rule Workflow

The browser expects hyperlink pseudo-classes in the following order.

```text
L
│
▼
:link

↓

V

↓

:visited

↓

H

↓

:hover

↓

A

↓

:active
```

This order prevents one pseudo-class from overriding another unexpectedly.

---

# HTML Workflow

```text
Create HTML Document

↓

Create Head Section

↓

Load External CSS

↓

Create Body

↓

Create Main Container

↓

Create Headings

↓

Create Paragraphs

↓

Create Hyperlinks

↓

Create Lists

↓

Create Footer

↓

Display Webpage
```

---

# CSS Workflow

```text
Load Stylesheet

↓

Reset Browser Default Styles

↓

Style Body

↓

Style Container

↓

Style Headings

↓

Style Paragraphs

↓

Style Lists

↓

Style Hyperlinks

↓

Check Hyperlink State

↓

Apply

:link

OR

:visited

OR

:hover

OR

:active

↓

Render Updated Styles
```

---

# Browser Decision Process

```text
FOR every hyperlink

    Is hyperlink visited?

        YES

            Apply :visited

        NO

            Apply :link

    Is mouse over hyperlink?

        YES

            Apply :hover

    Is mouse button pressed?

        YES

            Apply :active

END FOR
```

---

# Complete Execution Flow

```text
START

↓

Read HTML

↓

Read CSS

↓

Create DOM

↓

Display Webpage

↓

Display Hyperlinks

↓

Check Link History

↓

Apply :link OR :visited

↓

User Moves Mouse

↓

Apply :hover

↓

User Clicks Hyperlink

↓

Apply :active

↓

Navigate to Destination

↓

Store Link History

↓

Future Visits

↓

Apply :visited

↓

END
```

---

# Real-World Example

Consider a student opening an online learning portal.

```text
Student Opens Website

↓

Course Link Appears

↓

Browser Applies :link

↓

Student Moves Mouse

↓

Browser Applies :hover

↓

Student Clicks

↓

Browser Applies :active

↓

Course Opens

↓

Browser Saves History

↓

Student Returns Tomorrow

↓

Browser Applies :visited
```

This demonstrates how a single hyperlink transitions through different states during normal user interaction.

---

# Key Takeaways

- HTML creates the webpage structure.
- CSS controls the appearance.
- Pseudo-Class Selectors respond to element states.
- Browsers automatically determine which pseudo-class to apply.
- The four hyperlink states work together as part of a continuous lifecycle.
- Following the LVHA rule ensures predictable and consistent styling behavior.

---

# Summary

The Pseudo-Class Selectors module demonstrates how browsers dynamically style hyperlinks based on user interaction. By combining HTML structure with CSS pseudo-classes, webpages can provide clear visual feedback without JavaScript. Understanding the sequence of `:link`, `:visited`, `:hover`, and `:active` states helps developers create intuitive, accessible, and interactive user interfaces.
