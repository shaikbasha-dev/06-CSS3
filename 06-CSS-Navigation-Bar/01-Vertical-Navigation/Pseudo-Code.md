# Pseudo Code

This document explains the logical workflow behind creating and displaying a **Vertical Navigation Bar**. Unlike HTML and CSS syntax, pseudo code focuses on the sequence of steps required to build and render the navigation menu.

---

# Objective

Create a professional Vertical Navigation Bar that:

- Displays navigation links vertically.
- Provides easy navigation between webpages.
- Highlights the active page.
- Responds to user interactions.
- Maintains accessibility and readability.

---

# High-Level Algorithm

```
Start

↓

Create HTML Document

↓

Create Navigation Container

↓

Create Navigation List

↓

Add Navigation Items

↓

Create Hyperlinks

↓

Link External CSS

↓

Apply Navigation Styles

↓

Display Vertical Navigation Bar

↓

Wait for User Interaction

↓

Highlight Hovered Link

↓

Highlight Active Link

↓

End
```

---

# Detailed Algorithm

```
Step 1

Start the HTML document.

↓

Step 2

Create the <head> section.

↓

Step 3

Add metadata.

↓

Step 4

Link the external CSS file.

↓

Step 5

Create the <body> section.

↓

Step 6

Create the <nav> element.

↓

Step 7

Create an unordered list (<ul>).

↓

Step 8

Create multiple list items (<li>).

↓

Step 9

Insert hyperlinks (<a>) inside each list item.

↓

Step 10

Assign the active class to the current page.

↓

Step 11

Load the CSS stylesheet.

↓

Step 12

Remove default list bullets.

↓

Step 13

Set the navigation width.

↓

Step 14

Apply background colors.

↓

Step 15

Style hyperlinks.

↓

Step 16

Add spacing using padding.

↓

Step 17

Apply hover effects.

↓

Step 18

Highlight the active navigation item.

↓

Step 19

Display the completed Vertical Navigation Bar.

↓

Stop
```

---

# HTML Workflow

```
Start

↓

Create HTML Document

↓

Create <head>

↓

Add Metadata

↓

Link style.css

↓

Create <body>

↓

Create <nav>

↓

Create <ul>

↓

Create <li>

↓

Create <a>

↓

Repeat for Remaining Navigation Links

↓

Complete HTML Structure

↓

End
```

---

# CSS Workflow

```
Start

↓

Load style.css

↓

Reset Default Browser Styles

↓

Style Body

↓

Style Navigation Container

↓

Remove List Bullets

↓

Style Navigation Items

↓

Style Navigation Links

↓

Apply Hover Effect

↓

Apply Active Link Style

↓

Apply Keyboard Focus Style

↓

Render Styled Navigation

↓

End
```

---

# Browser Rendering Workflow

```
User Opens Webpage

↓

Browser Reads HTML

↓

Browser Builds DOM Tree

↓

Browser Loads CSS File

↓

Browser Parses CSS Rules

↓

Browser Matches CSS Selectors

↓

Browser Builds Render Tree

↓

Browser Calculates Layout

↓

Browser Paints Navigation Bar

↓

Navigation Menu Appears on Screen
```

---

# User Interaction Workflow

```
User Opens Webpage

↓

Navigation Menu is Displayed

↓

User Moves Mouse

↓

Hover Effect Applied

↓

User Clicks Navigation Link

↓

Requested Page Opens

↓

Active Navigation Item Updates

↓

User Continues Navigation
```

---

# Real-World Example

Consider a **Student Management System**.

The left sidebar contains the following navigation menu:

```
Dashboard

Students

Faculty

Courses

Library

Attendance

Reports

Settings

Logout
```

Workflow:

```
Student Logs In

↓

Dashboard Opens

↓

Dashboard Menu Item is Active

↓

Student Clicks "Courses"

↓

Courses Page Opens

↓

Courses Menu Item Becomes Active

↓

Student Clicks "Reports"

↓

Reports Page Opens

↓

Reports Menu Item Becomes Active
```

This workflow helps users always understand their current location within the application.

---

# Execution Flow

```
Start

↓

Load HTML

↓

Load CSS

↓

Create Navigation Structure

↓

Style Navigation Components

↓

Display Vertical Navigation Bar

↓

Wait for User Interaction

↓

Apply Hover Effects

↓

Highlight Active Link

↓

Navigate to Requested Page

↓

Repeat Until User Leaves Website

↓

End
```

---

# Summary

A Vertical Navigation Bar combines semantic HTML and CSS to create an organized and user-friendly navigation system.

The HTML document defines the navigation structure, while CSS controls the visual appearance, layout, colors, spacing, and interactive behavior.

When the webpage loads, the browser builds the HTML structure, applies CSS rules, renders the styled navigation bar, and continuously responds to user interactions such as hovering over links or selecting different pages.

Understanding this workflow helps developers build accessible, maintainable, responsive, and professional navigation menus for modern web applications.
