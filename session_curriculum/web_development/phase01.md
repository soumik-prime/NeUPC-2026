# Phase 01 — Web Fundamentals & Frontend Foundation

**Netrokona University Programming Club (NeUPC) — Web Development Curriculum**
*(Schedule: 8 weeks, ~2–3 hours per session)*

---

## Purpose

This phase takes a complete beginner from *"I don't know how a website works"* to *"I can build an interactive frontend with HTML, CSS, and JavaScript — and I understand what the browser and the web are actually doing."*

This document is not just a syllabus. It is your **learning notebook**. Come back to any week after the session to revise, re-read the concept notes, and re-attempt the mini project if needed.



## Prerequisites

- Basic comfort using a computer (installing software, managing files/folders)
- No prior web development knowledge required
- Basic programming logic (variables, if/else, loops) is required

## Expected Duration

**8 weeks**, one NeUPC session per week (**~2–3 hours per session**), plus 1.5–3 hours of homework/mini-project time outside each session.

## Learning Outcomes

By the end of Phase 01, students will be able to:

- Explain what happens, step by step, when a user visits a website
- Write semantic, well-structured HTML documents
- Style pages using modern CSS, including Flexbox and Grid, and make them responsive
- Write fundamental JavaScript (variables, functions, arrays, objects, loops, conditionals)
- Use the DOM to make pages interactive and respond to user events
- Make basic HTTP requests using `fetch` and understand JSON
- Use Git and GitHub for version control and basic collaboration
- Use browser DevTools to inspect, debug, and understand a running page
- Build a complete, interactive, multi-feature frontend application without a framework

---

# How to Use This Notebook

Each week has the same structure:

1. **Learning Goals** — what you should be able to do afterward
2. **Concepts** — short, practical notes (this is your reference material)
3. **In-Session Practice** — what we do together during the session
4. **Mini Project** — required hands-on build for that week
5. **Homework** — follow-up work
6. **Quick Revision** — a fast checklist to refresh your memory later
7. **What Comes Next** — how this week connects to the next

Concepts you learn early will **come back later, deeper**. Don't worry about memorizing everything perfectly the first time — you will revisit it.

---

# Week 01 — What Is the Web? & HTML Basics

*(2.5–3 hours: this session covers both the "how the web works" orientation and your first real HTML.)*

## Learning Goals

By the end of this session, students should be able to:

- Explain the difference between the Internet and the Web
- Describe, in simple terms, what happens when you visit a website
- Explain the basic role of a browser, a client, and a server
- Understand elements, tags, attributes, and document structure
- Build a correctly structured HTML page using headings, paragraphs, links, and images

## Concepts

### What is the Internet?

**Simple Explanation**
The Internet is a giant network of computers connected together, all over the world, able to send data to each other.

**Why Does It Exist?**
Before it existed, computers could only share data if they were physically connected or data was carried on disks. The Internet lets any connected computer talk to any other one.

**Remember**
- The Internet is the network of connected computers.
- It's the "roads," not the "shops."

### What is the Web?

**Simple Explanation**
The Web (World Wide Web) is a system of pages/documents that live on the Internet and are linked together, viewable through a browser.

**Internet vs Web**

| Internet | Web |
|---|---|
| The network of connected computers | A system of linked pages that runs *on* the Internet |
| Existed first | Built on top of the Internet |
| Includes email, file transfer, the Web, etc. | Just one of the things that uses the Internet |

**Remember**
- The Internet is the network. The Web is one *service* that runs on it.

**Common Confusion**
- Beginners often think "Internet" and "Web" are the same word. They are related but not identical.

### Client, Server, and the Browser

**Simple Explanation**
A **client** is the program that *asks* for something (usually your browser). A **server** is a computer that *has* something and sends it back when asked. A **browser** is the program that requests pages, then reads and displays (renders) them.

**Remember**
- Client = asks. Server = answers. Browser = the client program you use.

*We will go much deeper into client/server architecture later — for now, this basic mental model is enough.*

### What happens when I visit a website? (beginner version)

```
You type a URL  →  Browser asks a server for the page
                →  Server sends back the page's files
                →  Browser reads the files and shows you the page
```

This is intentionally simplified. We will add DNS, HTTP, and more detail to this diagram in later weeks, once each new piece is useful.

### What is HTML?

**Simple Explanation**
HTML (HyperText Markup Language) is the language used to describe the *structure and content* of a webpage — headings, paragraphs, links, images, etc. It is not a programming language — it doesn't compute anything, it describes structure.

**Remember**
- Every webpage you've ever seen has HTML underneath it.

### Elements, Tags, Attributes

```html
<a href="https://example.com">Visit Example</a>
```
`a` is the element, `href` is an attribute providing the link's destination.

**Remember**
- Most tags come in pairs: opening and closing (`<p>...</p>`). Some are self-closing, like `<img>` and `<br>`.
- Attributes go inside the opening tag only.

### Document Structure

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Page Title</title>
  </head>
  <body>
    <!-- visible content goes here -->
  </body>
</html>
```

**Remember**
- `<head>` = information *about* the page (not shown directly). `<body>` = everything the user actually sees.

### Text, Links, and Images

- **Headings:** `<h1>` (most important) through `<h6>` — use only one `<h1>` per page.
- **Paragraphs:** `<p>text</p>`
- **Links:** `<a href="url">link text</a>`
- **Images:** `<img src="path-or-url" alt="description">` — `alt` describes the image for accessibility and for when it fails to load.

**Remember**
- `alt` on images is not optional.
- Headings should follow a logical order (don't skip from `<h1>` to `<h4>`).

## In-Session Practice

- Open a browser, visit a few websites, and identify: what's a link, what's an image, what's text
- Briefly open DevTools (`F12` / right-click → Inspect) just to look — no need to understand it yet
- Set up a project folder in VS Code
- Build a document skeleton from memory, then add headings, paragraphs, a link, and an image

## Mini Project

### Goal
Build your first properly structured webpage: an "About Me" page.

### Requirements
- A single `index.html` file with the correct document skeleton (`doctype`, `html`, `head` with `title`, `body`)
- One `<h1>` with your name
- At least one `<h2>` subheading (e.g., "About Me", "My Interests")
- At least 2 paragraphs
- One image with proper `alt` text
- One link to something relevant (e.g., your GitHub, or the NeUPC page)

### Concepts Used
Browser/client/server basics, document structure, headings, paragraphs, links, images, attributes.

### Completion Criteria
Page opens correctly in a browser, structure is correct, all required elements are present.

### Optional Challenge
Add a second linked page (e.g., "Contact") and link between the two pages.

### Estimated Time
1.5–2 hours.

## Homework

Redraw the "What happens when I visit a website?" diagram from memory, and explore 2 real websites, identifying links/images/text in each.

## Quick Revision

- Internet = the network. Web = pages that run on it. Client asks, server answers.
- HTML describes structure/content, not appearance or behavior.
- Standard skeleton: `doctype → html → head (title) → body (content)`.

## What Comes Next?

Next session: more HTML — lists, tables, semantic structure, and forms — plus your first CSS, to make pages look good.

---

# Week 02 — HTML Basics II & CSS Basics I

*(2.5–3 hours)*

## Learning Goals

- Use lists and tables appropriately
- Understand semantic HTML and why it matters
- Build a basic form
- Explain why CSS exists and how it connects to HTML
- Use selectors, understand the cascade, and style colors/typography

## Concepts

### Lists

**Ordered list** (`<ol>`) — numbered, for sequences. **Unordered list** (`<ul>`) — bullets, for unordered groups. Both contain `<li>` items.

```html
<ul>
  <li>HTML</li>
  <li>CSS</li>
  <li>JavaScript</li>
</ul>
```

### Tables

Used for **tabular data only** — never for page layout.

```html
<table>
  <tr><th>Name</th><th>Role</th></tr>
  <tr><td>Soumik</td><td>Member</td></tr>
</table>
```

**Remember**
- `<th>` = header cell, `<td>` = data cell, `<tr>` = row.

### Semantic HTML

**Simple Explanation**
Semantic tags describe *meaning*, not just appearance: `<header>`, `<nav>`, `<main>`, `<article>`, `<section>`, `<footer>`, instead of generic `<div>` everywhere.

```html
<header>...</header>
<nav>...</nav>
<main><article>...</article></main>
<footer>...</footer>
```

**Remember**
- Semantic tags = same visual result as `<div>`, but with meaning attached. Use `<div>` only when no semantic tag fits.

### Basic Forms

```html
<form>
  <label for="name">Name:</label>
  <input type="text" id="name" name="name">
  <button type="submit">Submit</button>
</form>
```

**Remember**
- `<label>` should always connect to its input via `for`/`id`.
- Common input types: `text`, `email`, `password`, `checkbox`, `radio`.
- At this stage, submitting a form doesn't send data anywhere real yet — we'll revisit forms with JavaScript soon, and with real APIs in Phase 02.

### Why does CSS exist?

**Simple Explanation**
HTML describes structure/content. CSS (Cascading Style Sheets) describes *appearance* — colors, fonts, spacing, layout.

```html
<link rel="stylesheet" href="style.css">
```
placed inside `<head>`, connects an external CSS file to your HTML page.

**Remember**
- HTML = what it *is*. CSS = how it *looks*. Keep CSS in a separate file.

### Selectors

```css
p { color: navy; }
.highlight { background: yellow; }
#main-title { font-size: 2rem; }
```

| Selector | Targets |
|---|---|
| `p` | all `<p>` elements |
| `.classname` | elements with `class="classname"` |
| `#idname` | the single element with `id="idname"` |

**Remember**
- Class = reusable, can appear on many elements. ID = unique, once per page.

### The Cascade (beginner level)

**Simplified priority (low → high):** `element selector < class selector < id selector < inline style`

**Remember**
- More specific selectors win. If specificity ties, the rule written *later* wins.

### Colors and Typography

```css
h1 {
  color: #1e293b;
  font-family: "Segoe UI", sans-serif;
  font-size: 2rem;
  font-weight: 600;
}
```

**Remember**
- Always give `font-family` a fallback (e.g., `sans-serif`).

## In-Session Practice

- Convert a paragraph of "steps" into an ordered list; build a small table
- Rebuild a page section using semantic tags instead of `<div>`
- Build a simple form (no functionality yet)
- Link an external CSS file and style a heading with element, class, and ID selectors — observe which wins

## Mini Project

### Goal
Build and style a "NeUPC Session Schedule" page.

### Requirements
- Semantic structure: `<header>`, `<main>`, `<footer>` at minimum
- A table listing at least 4 upcoming session topics and dates
- An unordered list of "What to bring" or "Prerequisites"
- A basic feedback form (name, email, message, submit button) with properly linked labels
- An external `style.css` file with: custom colors, a custom font stack, at least one class-based style, and at least one ID-based style

### Concepts Used
Lists, tables, semantic HTML, forms, CSS linking, selectors, colors, typography, cascade.

### Completion Criteria
Page uses semantic tags correctly, table displays cleanly, form inputs are properly labeled, and CSS styles apply without unintended conflicts.

### Optional Challenge
Deliberately create a specificity conflict (style the same element with both a class and an ID differently) and add a comment explaining which one won and why.

### Estimated Time
2–2.5 hours.

## Homework

Find one real website and use DevTools to check whether it uses semantic tags or mostly `<div>`s.

## Quick Revision

- `<ul>`/`<ol>` + `<li>` for lists; tables for tabular data only.
- Semantic tags add meaning: `header`, `nav`, `main`, `article`, `section`, `footer`.
- CSS selectors: element `<` class `<` id `<` inline, in specificity.

## What Comes Next?

Next session: the **box model** and **Flexbox** — the foundation for real layout and spacing.

---

# Week 03 — CSS Box Model & Flexbox

*(2.5–3 hours)*

## Learning Goals

- Explain the CSS box model
- Control spacing using margin, padding, and borders
- Use `display` to control basic layout behavior
- Explain the problem Flexbox solves and use it to build row/column layouts

## Concepts

### The Box Model

**Simple Explanation**
Every HTML element is a rectangular box made of four layers, from inside out: **content → padding → border → margin**.

```
┌───────────────margin───────────────┐
│  ┌─────────────border─────────────┐ │
│  │  ┌───────padding─────────┐    │ │
│  │  │      content           │    │ │
│  │  └────────────────────────┘    │ │
│  └─────────────────────────────────┘ │
└───────────────────────────────────────┘
```

**Remember**
- **Padding** = space *inside* the border, around the content. **Margin** = space *outside* the border, between elements.

**Common Mistakes**
- Confusing margin and padding — padding pushes content inward; margin pushes other elements away.

### box-sizing

```css
* { box-sizing: border-box; }
```

**Remember**
- By default, `width` doesn't include padding/border, causing sizing bugs. `border-box` makes `width` include them — most real projects set this globally.

### display

| Value | Behavior |
|---|---|
| `block` | Full width, starts on a new line (`<div>`, `<p>`) |
| `inline` | Only as wide as content, stays in line (`<span>`, `<a>`) |
| `inline-block` | Inline positioning but respects width/height |
| `none` | Removes the element from the page entirely |

### Why Flexbox?

**Simple Explanation**
Before Flexbox, arranging boxes side by side, evenly spaced, or centered required awkward tricks. Flexbox is a layout system purpose-built for arranging items in a row or column.

**Remember**
- Flexbox is **one-dimensional**: it arranges items along a single row or column.

### The Flex Container and Flex Items

```css
.container {
  display: flex;
  flex-direction: row;     /* or column */
  justify-content: center;  /* main-axis alignment */
  align-items: center;      /* cross-axis alignment */
  gap: 1rem;
}
```

**Remember**
- `display: flex` on the parent turns direct children into flex items.
- `justify-content` aligns along the main axis; `align-items` aligns along the cross axis.
- `gap` adds spacing between items without margin tricks.

### Common Flexbox Patterns

| Goal | CSS |
|---|---|
| Center everything | `justify-content: center; align-items: center;` |
| Space items evenly | `justify-content: space-between;` |
| Items in a column | `flex-direction: column;` |
| Item grows to fill space | `flex: 1;` on that item |

**Common Mistakes**
- Forgetting `display: flex` on the *parent*.
- Applying `justify-content`/`align-items` to the item instead of the container.

## In-Session Practice

- Inspect box model values live in DevTools' "Computed" panel
- Practice margin vs padding, and `block`/`inline`/`inline-block`
- Build a navbar with a logo on one side and links on the other using `justify-content: space-between`
- Center a box perfectly using Flexbox

## Mini Project

### Goal
Build a styled profile card row with a navbar, using the box model and Flexbox.

### Requirements
- A navbar using Flexbox: title/logo on one side, 3+ nav links on the other
- A row of at least 3 profile/info cards, laid out with Flexbox, evenly spaced with `gap`
- Each card styled with border, padding, and rounded corners (correct box model usage)
- `box-sizing: border-box` applied globally

### Concepts Used
Box model, margin/padding/border, box-sizing, display, Flexbox container/items, alignment.

### Completion Criteria
Navbar and card row align cleanly with no manual margin hacks or unexpected overflow.

### Optional Challenge
Make the navbar switch to `flex-direction: column` at narrow widths (a quick preview of responsive design — covered fully next week).

### Estimated Time
2–2.5 hours.

## Homework

Take a previous project page and fix its spacing using proper margin/padding instead of guessing; convert any `inline-block` layouts to Flexbox.

## Quick Revision

- Box model, inside out: content → padding → border → margin. `box-sizing: border-box` makes sizing predictable.
- `display: block/inline/inline-block/none` control layout flow.
- Flexbox: `display: flex` on parent; `justify-content` = main axis, `align-items` = cross axis; one-dimensional.

## What Comes Next?

Next session: **CSS Grid** for two-dimensional layouts, plus making pages properly **responsive**.

---

# Week 04 — CSS Grid & Responsive Design

*(2–2.5 hours — this session is naturally lighter, giving room to finish Phase 01's CSS work solidly.)*

## Learning Goals

- Explain when to use Grid vs Flexbox
- Build a basic two-dimensional grid layout
- Use media queries to make a page responsive

## Concepts

### Why Grid?

**Simple Explanation**
Grid arranges items in **rows and columns at the same time** — a true two-dimensional layout system, unlike Flexbox's single direction.

```css
.gallery {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 1rem;
}
```
This creates 3 equal-width columns, with items automatically flowing into rows.

**Remember**
- Flexbox: one-dimensional (a row, or a column). Grid: two-dimensional (rows *and* columns together).
- `fr` unit = "a fraction of the available space."

**Common Confusion**
- Rule of thumb: arranging things in one direction → Flexbox; true grid layout → Grid. It's common to use both on the same page.

### Responsive Design & Media Queries

**Simple Explanation**
Responsive design means a page adapts to different screen sizes. Media queries let CSS apply different rules based on screen width.

```css
.gallery { grid-template-columns: repeat(3, 1fr); }

@media (max-width: 600px) {
  .gallery { grid-template-columns: 1fr; }
}
```

**Remember**
- Common breakpoints: ~600px (mobile), ~900px (tablet), ~1200px (desktop) — guidelines, not strict rules.

**Common Mistakes**
- Forgetting the viewport meta tag, which breaks mobile responsiveness:
```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

## In-Session Practice

- Build a 3-column photo/feature gallery with CSS Grid
- Add a media query that collapses the gallery to 1 column on small screens
- Test responsiveness using DevTools' device toolbar

## Mini Project

### Goal
Transform your accumulated pages (About Me, schedule, cards/navbar) into one cohesive, fully responsive personal/landing page.

### Requirements
- Use Grid for at least one section (e.g., a gallery or feature grid)
- Use Flexbox for at least one section (e.g., the navbar, from last week)
- At least 2 media query breakpoints
- Correct viewport meta tag
- Page must look reasonable on both a phone-sized and desktop-sized viewport

### Concepts Used
Grid, Flexbox, media queries, responsive design, box model.

### Completion Criteria
Layout does not visually break at any width between ~320px and ~1440px.

### Optional Challenge
Make font sizes scale using `rem` units with a mobile-adjusted base size.

### Estimated Time
2–3 hours. *(This mini project doubles as strong practice for your Phase 01 Project later.)*

## Homework

Pick 2 real websites, resize your browser window slowly, and note exactly where their layout changes (their breakpoints).

## Quick Revision

- Grid = two-dimensional; Flexbox = one-dimensional. Use both together as needed.
- Media queries apply CSS conditionally based on screen width.
- Always include the viewport meta tag for responsive pages.

## What Comes Next?

Your pages look great but are still completely static. Next session: **JavaScript** — making pages actually *do* things.

---

# Week 05 — JavaScript Fundamentals

*(2.5–3 hours: variables through functions, loops, arrays, and objects in one sitting — this is a dense session, so pace it deliberately with breaks.)*

## Learning Goals

- Explain what JavaScript does that HTML/CSS cannot
- Use variables, data types, and operators
- Write conditional logic
- Use loops to repeat actions
- Write and call functions
- Use arrays and objects to organize data

## Concepts

### Why JavaScript?

**Simple Explanation**
HTML = structure. CSS = appearance. JavaScript = **behavior** — logic, interactivity, calculations, responding to user actions.

```html
<script src="script.js"></script>
```
placed at the end of `<body>` (so the page loads before the script runs).

### Variables and Data Types

```javascript
let age = 20;              // number
let name = "Soumik";       // string
let isMember = true;       // boolean
let nothing = null;        // intentionally empty
let notSet;                // undefined
```

**Remember**
- Use `let` for values that may change, `const` for values that shouldn't be reassigned. Avoid `var`.

### Operators

```javascript
5 + 3     // 8   addition
"a" + "b" // "ab"  string concatenation
5 === 5   // true   strict equality (checks type too)
5 !== 3   // true
```

**Remember**
- Always prefer `===` and `!==` over `==`/`!=` to avoid type-conversion bugs.

### Conditionals

```javascript
if (age >= 18) {
  console.log("Adult");
} else if (age >= 13) {
  console.log("Teen");
} else {
  console.log("Child");
}
```

**Remember**
- Conditions run top to bottom; the first true condition's block executes, the rest are skipped.

### Loops

```javascript
for (let i = 0; i < 5; i++) {
  console.log(i);
}

let count = 0;
while (count < 3) {
  console.log(count);
  count++;
}
```

**Remember**
- `for` loops: best when you know how many times to repeat. `while` loops: best when repetition depends on a changing condition.

**Common Mistakes**
- Forgetting to update the loop variable, causing an infinite loop.

### Functions

```javascript
function greet(name) {
  return `Hello, ${name}!`;
}

const add = (a, b) => a + b; // arrow function shorthand
```

**Remember**
- Functions let you reuse logic instead of repeating code. `return` sends a value back out; without it, the function returns `undefined`.

### Arrays

```javascript
let fruits = ["apple", "banana", "mango"];
fruits[0];            // "apple"
fruits.push("kiwi");
fruits.length;         // 4

for (let fruit of fruits) {
  console.log(fruit);
}
```

**Remember**
- Arrays are ordered lists, indexed from `0`. `for...of` is a clean way to loop over values.

### Objects

```javascript
let student = { name: "Soumik", id: "202204023", isMember: true };
student.name;      // "Soumik"
student["id"];      // "202204023"
```

**Remember**
- Objects store data as `key: value` pairs — use them to represent "a thing with properties."

## In-Session Practice

- Experiment with variables and operators live in the console
- Write conditional snippets (e.g., "even or odd," "pass or fail")
- Write a loop that sums numbers 1 to 100
- Write a function that checks if a number is prime
- Build an array of NeUPC members (objects with `name`/`role`) and loop through it, printing each

## Mini Project

### Goal
Build a **Student Score Analyzer** (console-based).

### Requirements
- An array of at least 6 student objects: `{ name, score }`
- A function `getGrade(score)` that returns a letter grade using conditionals
- A loop that prints each student's name and grade to the console
- A running total/average calculated using a loop or accumulator variable
- Basic validation: if a score is above 100 or below 0, print an error message instead of a grade

### Concepts Used
Variables, data types, operators, conditionals, loops, functions, arrays, objects.

### Completion Criteria
Console correctly prints each student's grade, handles invalid scores gracefully, and prints the class average.

### Optional Challenge
Add a function `getTopStudent(students)` that returns the student with the highest score.

### Estimated Time
2–2.5 hours.

## Homework

Extend the Student Score Analyzer with 3 more students and manually trace through the code on paper to predict the output before running it — then verify.

## Quick Revision

- JS = behavior/logic. `let`/`const` over `var`. Always use `===`/`!==`.
- `if/else if/else` for branching; `for`/`while` for repetition.
- Functions reuse logic; arrays = ordered lists; objects = key-value data.

## What Comes Next?

Your JavaScript works, but only in the console. Next session: the **DOM** — connecting JavaScript to the actual page, plus building interactive, persistent UI.

---

# Week 06 — The DOM: Selecting, Events, Forms & Storage

*(2.5–3 hours: from your first DOM selection to a fully working, persistent To-Do app.)*

## Learning Goals

- Explain what the DOM is and why JavaScript needs it
- Select and modify elements from a page
- Handle user events
- Read values from form inputs
- Create and remove elements dynamically
- Use `localStorage` to persist data between visits

## Concepts

### What is the DOM?

**Simple Explanation**
The DOM (Document Object Model) is the browser's live, in-memory representation of your HTML page — structured as a tree of objects that JavaScript can read and change.

**Remember**
- HTML file = the *blueprint*. DOM = the *live building* the browser constructs from it, in memory, while the page runs.
- Changing the DOM with JavaScript changes what's on screen immediately — without reloading the page.

### Selecting and Modifying Elements

```javascript
const title = document.querySelector("h1");
document.querySelectorAll("li");             // all matches
document.getElementById("main-title");

title.textContent = "New Title";
title.style.color = "blue";
title.classList.add("highlight");
```

**Remember**
- `querySelector`/`querySelectorAll` accept CSS-style selectors — the same ones you already know from CSS.
- `textContent` changes text; `classList` adds/removes CSS classes (usually preferred over inline `style`).

### Events

```javascript
const button = document.querySelector("button");
button.addEventListener("click", function () {
  alert("Button clicked!");
});
```

**Remember**
- `addEventListener(eventType, handlerFunction)` is the standard way to respond to user actions: `"click"`, `"input"`, `"submit"`, etc.

**Common Mistakes**
- Selecting an element *before* it exists in the HTML — this is why `<script>` goes at the end of `<body>`.

### Reading Form Input

```html
<input type="text" id="guess">
<button id="submit-btn">Guess</button>
```
```javascript
const input = document.querySelector("#guess");
input.value; // reads current content
```

**Remember**
- Prevent a form's default page-reload behavior with `event.preventDefault()` inside a `"submit"` handler.

### Creating and Removing Elements Dynamically

```javascript
const list = document.querySelector("#todo-list");
const item = document.createElement("li");
item.textContent = "Buy groceries";
list.appendChild(item);

item.remove();
```

**Remember**
- `createElement` + `appendChild` = adding new content dynamically. `.remove()` deletes an element from the page.

### localStorage

```javascript
localStorage.setItem("username", "Soumik");
localStorage.getItem("username");
localStorage.removeItem("username");
```

**Simple Explanation**
`localStorage` lets a webpage save small amounts of data **in the browser**, persisting even after the page is closed and reopened.

**Remember**
- `localStorage` only stores strings — use `JSON.stringify()`/`JSON.parse()` for arrays/objects.
- This is *not* a real database — it's local to one browser on one device. (We'll build real persistent storage with a database in Phase 02.)

## In-Session Practice

- Select and modify several elements from an existing page in the console
- Add a click event that toggles visibility and cycles background color
- Build a form that reads a name and greets the user dynamically
- Save and load a value using `localStorage`

## Mini Project

### Goal
Build a working **To-Do List app**.

### Requirements
- An input field and "Add" button
- Clicking "Add" creates a new list item with the typed text
- Each item has a "Delete" button that removes it
- The list persists using `localStorage` (reload the page — items should still be there)
- At least one button elsewhere on the page that toggles a UI element's visibility or style using `classList` (reinforcing basic event handling)

### Concepts Used
DOM selection, event handling, dynamic element creation/removal, form input reading, `localStorage`, JSON, arrays/objects (from Week 05).

### Completion Criteria
Items can be added, removed, and survive a page reload.

### Optional Challenge
Add a "mark as complete" feature (strikethrough styling via `classList.toggle`).

### Estimated Time
2.5–3 hours.

## Homework

Rebuild the Week 05 "Student Score Analyzer" as a real interactive page: an input for a student name/score, an "Add Student" button, and a dynamically updated list + running average shown on the page instead of just the console.

## Quick Revision

- DOM = the browser's live, in-memory tree built from your HTML.
- `querySelector`/`querySelectorAll` to select; `textContent`/`classList` to modify; `addEventListener` to respond to events.
- `.value` reads form input; `createElement`/`appendChild`/`remove()` for dynamic UI; `localStorage` persists data in-browser only.

## What Comes Next?

So far, all your "data" lives only in your own browser. Next session: **Browser/Web APIs and Fetch** — getting data *from the internet*, plus Git/GitHub and your developer workflow.

---

# Week 07 — Browser APIs, Fetch, and Developer Workflow

*(2–2.5 hours)*

## Learning Goals

- Revisit and deepen the client/server/HTTP model from Week 01
- Understand what an API is and use `fetch` to get real data
- Use Git and GitHub for basic version control
- Use browser DevTools confidently for debugging

## Concepts

### Revisiting the Request/Response Model

Back in Week 01, we had this simplified picture:

```
You type a URL  →  Browser asks a server for the page
                →  Server sends back the page's files
                →  Browser reads the files and shows you the page
```

Now that you understand JavaScript and the DOM, let's go one level deeper.

**HTTP (HyperText Transfer Protocol)** is the *language* browsers and servers use to talk to each other. A **request** asks for something; a **response** sends something back — including a **status code** (e.g., `200` = OK, `404` = Not Found), which we'll use more in Phase 02.

### What is an API?

**Simple Explanation**
An API (Application Programming Interface) is a way for one program to ask another program for data or functionality — often over HTTP, returning data instead of a full webpage.

**Remember**
- An API request is still an HTTP request — it just usually returns structured data (often JSON), not a whole HTML page.

### JSON

```json
{ "name": "Soumik", "skills": ["HTML", "CSS", "JavaScript"] }
```

**Remember**
- JSON is the most common format APIs use to send data.
- `JSON.parse()` turns JSON text into a real object; `JSON.stringify()` does the reverse.

### Using fetch

```javascript
fetch("https://api.example.com/data")
  .then(response => response.json())
  .then(data => console.log(data))
  .catch(error => console.error("Something went wrong:", error));
```

**Remember**
- `fetch()` sends an HTTP request and returns a **Promise** (covered fully in Phase 02 — for now, just recognize this pattern).
- `.then()` runs once the response arrives; `.json()` converts the response body into usable data.

**Common Mistakes**
- Forgetting that `fetch` doesn't return data directly — it returns a Promise that resolves later.

### Developer Workflow — DevTools

| Tab | Use |
|---|---|
| Elements | Inspect/edit the live DOM and CSS |
| Console | Run JS, view logs/errors |
| Network | See every request the page makes, including `fetch` calls |
| Sources | Set breakpoints, step through JS |

### Developer Workflow — Git & GitHub

```bash
git init
git add .
git commit -m "Initial commit"
git remote add origin <your-repo-url>
git push -u origin main
```

**Remember**
- `git add` stages changes, `git commit` saves a snapshot with a message, `git push` uploads it to GitHub. Commit often, with clear messages.

## In-Session Practice

- Fetch data from a free public API (e.g., a joke or quote API) and display it on the page
- Watch the request happen live in the Network tab
- Initialize Git in an existing project folder, commit, and push to GitHub

## Mini Project

### Goal
Build a small **"Random Fact/Quote Fetcher"** page, and get all your Phase 01 work under version control.

### Requirements
- A button that fetches a new fact/quote/joke from a public API using `fetch`
- Fetched data displayed dynamically on the page (not the console)
- Basic error handling (e.g., a message shown if the fetch fails)
- Every project folder from Weeks 01–07 initialized with Git and pushed to a GitHub repository, with at least 3 separate, clearly-labeled commits (not one giant commit)

### Concepts Used
`fetch`, `.then()`/JSON, DOM updates, Git/GitHub basics.

### Completion Criteria
Fetch button reliably displays new data on each click; GitHub repository is public (or shared with the instructor) and shows real commit history.

### Optional Challenge
Add a loading indicator that shows while the fetch is in progress.

### Estimated Time
1.5–2 hours.

## Homework

Review your Week 06 To-Do app and add one `fetch`-based feature to it (e.g., fetching a "task of the day" suggestion from a public API when the page loads).

## Quick Revision

- HTTP = the request/response conversation between client and server. APIs return structured data (usually JSON).
- `fetch()` → Promise → `.then(response => response.json())` → `.then(data => ...)`.
- Git: `add` → `commit` → `push`. DevTools Network tab shows real requests.

## What Comes Next?

You now know enough to build a complete, interactive frontend application. Next session is fully dedicated to building your **Phase 01 Project**.

---

# Week 08 — Phase 01 Project Build Session

*(2.5–3 hours, dedicated project time — this session has no new concepts; it's for building, debugging, and polishing.)*

## Learning Goals

- Combine everything from Weeks 01–07 into one complete, working application
- Practice debugging your own code independently, using DevTools
- Finish with a deployed-to-GitHub, portfolio-ready project

## In-Session Practice

- Plan your Quiz Application's structure before writing code (questions data, HTML skeleton, CSS layout, JS logic)
- Build incrementally: static structure first, then styling, then interactivity, then the API call, then persistence
- Pair up with another NeUPC member partway through the session for a quick code review / fresh-eyes bug check
- Commit to Git at each meaningful milestone, not just once at the end

## Phase 01 Project — Quiz Application

### Goal

Build a complete, interactive **Quiz Application** using only HTML, CSS, and JavaScript (no frameworks, no backend yet).

### Requirements

- Semantic, well-structured HTML
- Responsive layout using Flexbox and/or Grid, tested on mobile and desktop widths
- At least 5 quiz questions with multiple-choice answers, stored as an array of objects in JavaScript
- Dynamic rendering: questions and options are generated with JavaScript/DOM, not hardcoded one-by-one in HTML
- Score tracking as the user answers
- A results screen at the end showing the final score
- At least one `fetch` call to a public API somewhere in the app (e.g., fetching quiz questions from a trivia API, or fetching a fun fact to display on the results screen)
- Data (e.g., high score) persisted with `localStorage`
- Project pushed to GitHub with a clear commit history and a short `README.md` explaining the app

### Concepts Used

Everything from Phase 01: HTML structure, CSS layout/responsiveness, JavaScript fundamentals, DOM manipulation, events, `fetch`/JSON, Git/GitHub.

### Completion Criteria

- App runs correctly from start (question 1) to finish (results screen) without errors
- Score calculation is accurate
- Layout doesn't break on mobile-sized screens
- Code is organized into separate `index.html`, `style.css`, and `script.js` files

### Optional Challenge

Add a timer per question, or a "restart quiz" button that resets all state cleanly.

### Estimated Time

If not finished by the end of the session, budget an additional 3–5 hours outside it to complete and polish.

## Quick Revision

This week is a synthesis of the entire phase — if you get stuck, the concept is almost certainly covered in an earlier week's notes. Check there first before asking for help.

## What Comes Next?

Phase 02 introduces modern JavaScript, React, and your first real backend and database — the next step from "I can build a frontend" to "I can build a full application."

---

# Phase 01 Completion

## What You Should Be Able to Do

- Build a multi-page, semantic HTML site from scratch
- Style and lay out a page responsively using Flexbox and Grid
- Write JavaScript to manipulate the DOM, handle events, and manage application state
- Fetch real data from a public API and display it dynamically
- Use `localStorage` for simple client-side persistence
- Use Git/GitHub to track and back up your projects
- Explain, at a solid beginner-to-intermediate level, what happens between typing a URL and seeing a rendered, interactive page

## Phase Checklist

- [ ] I can explain the difference between the Internet and the Web
- [ ] I can build a correctly structured HTML document from memory
- [ ] I understand and can use CSS selectors, the box model, and the cascade
- [ ] I can build responsive layouts using Flexbox and Grid
- [ ] I can write JavaScript variables, conditionals, loops, functions, arrays, and objects
- [ ] I can select and modify DOM elements and handle events
- [ ] I can read form input and build dynamic, interactive UI
- [ ] I understand what an API is and can use `fetch` to retrieve data
- [ ] I can use Git and GitHub for basic version control
- [ ] I completed the Phase 01 Project (Quiz Application)

## Recommended Resources

| Topic | Primary | Optional |
|---|---|---|
| HTML | [MDN: HTML Basics](https://developer.mozilla.org/en-US/docs/Learn/HTML) | web.dev HTML |
| CSS | [MDN: CSS Basics](https://developer.mozilla.org/en-US/docs/Learn/CSS) | [web.dev CSS](https://web.dev/learn/css) |
| Flexbox/Grid | [CSS-Tricks: A Complete Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) | [MDN Grid](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_grid_layout) |
| JavaScript | [JavaScript.info](https://javascript.info/) | MDN JavaScript Guide |
| DOM | [MDN: Introduction to the DOM](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Introduction) | — |
| Git/GitHub | [GitHub Docs: Git Handbook](https://docs.github.com/en/get-started/using-git) | — |

---

*End of Phase 01. Continue to `phase-02-modern-frontend-backend.md`.*