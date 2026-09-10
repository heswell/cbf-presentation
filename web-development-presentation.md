---
marp: true
theme: default
paginate: true
size: 16:9
style: |
  @import url('https://fonts.googleapis.com/css2?family=DM+Mono:wght@400;500&family=Manrope:wght@400;500;600;700;800&display=swap');

  :root {
    --ink: #11243d;
    --muted: #53708f;
    --canvas: #f4f8fc;
    --surface: #ffffff;
    --blue: #0b65d8;
    --aqua: #17bebb;
    --orange: #ff9f1c;
  }

  section {
    background:
      radial-gradient(circle at 92% 10%, rgba(23, 190, 187, .16), transparent 23%),
      linear-gradient(135deg, #f7fbff 0%, var(--canvas) 100%);
    color: var(--ink);
    font-family: 'Manrope', sans-serif;
    font-size: 25px;
    font-weight: 500;
    letter-spacing: -.02em;
    line-height: 1.35;
    padding: 62px 78px;
  }

  h1 {
    color: var(--ink);
    font-size: 52px;
    font-weight: 800;
    letter-spacing: -.05em;
    line-height: 1.08;
    margin: 0 0 30px;
    max-width: 1100px;
  }

  h2 {
    color: var(--blue);
    font-size: 17px;
    font-weight: 800;
    letter-spacing: .13em;
    margin: 0 0 18px;
    text-transform: uppercase;
  }

  ul { margin: 18px 0 0; }
  li { margin: 10px 0; }
  li::marker { color: var(--aqua); }
  ul ul { font-size: .8em; margin: 4px 0; }
  strong { color: var(--blue); }
  em { color: var(--muted); }
  code {
    background: #e3efff;
    border-radius: 5px;
    color: #0752ad;
    font-family: 'DM Mono', monospace;
    font-size: .8em;
    padding: .12em .32em;
  }
  a { color: var(--blue); }
  footer {
    color: var(--muted);
    font-size: 13px;
  }
  section::after {
    color: var(--blue);
    font-size: 14px;
    font-weight: 800;
  }
  section.lead {
    background:
      radial-gradient(circle at 85% 20%, rgba(23, 190, 187, .45), transparent 25%),
      linear-gradient(135deg, #0d2543 0%, #123c6a 100%);
    color: #eaf5ff;
  }
  section.lead h1 { color: #fff; font-size: 66px; max-width: 900px; }
  section.lead h2 { color: #61e4db; }
  section.lead strong { color: #61e4db; }
  section.lead footer, section.lead::after { color: #a9cae8; }
  section.section-break {
    background: linear-gradient(135deg, #0b65d8 0%, #10488e 100%);
    color: #fff;
  }
  section.section-break h1 { color: #fff; font-size: 64px; }
  section.section-break h2 { color: #84f3e9; }
  section.section-break::after { color: #bcdcff; }
  .two-columns {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 58px;
  }
  .two-columns ul { margin-top: 0; }
  section.vuu-server {
    background:
      radial-gradient(circle at 86% 24%, rgba(199, 203, 222, .28), transparent 24%),
      linear-gradient(135deg, #2a015f 0%, #6d18bd 100%);
    color: #f5f6f7;
  }
  section.vuu-server h1 { color: #fff; }
  section.vuu-server strong { color: #c7cbde; }
  section.vuu-server small {
    color: #fff;
    font-weight: 700;
    text-decoration: underline;
    text-underline-offset: 3px;
  }
  section.vuu-server::after { color: #c7cbde; }
  section.vuu-server li::marker { color: #c7cbde; }
---

<!-- _class: lead -->
<!-- _paginate: false -->

## A practical introduction

# From Web Fundamentals to Modern Application Development

**HTML, CSS and JavaScript** remain the foundation. Today, we use them to assemble rich applications from design systems, reusable components and data-driven services.

<br>

*Concepts, vocabulary and the building blocks behind our applications*

---

## Today

# Session Roadmap

1. **Foundation** &mdash; the browser, HTML, CSS and JavaScript
2. **Building blocks** &mdash; libraries, design systems and tooling
3. **Application development** &mdash; components, data and real-time behaviour

---

# Key Building Blocks

- **React** &mdash; the application UI library
- **Salt** &mdash; the design system, including themes and components<br><small>https://www.saltdesignsystem.com/salt/index</small>
- **Vuu** &mdash; reusable components and functionality for data-driven applications<br><small>https://github.com/finos/vuu</small>
- **Vuu Server** &mdash; streaming real-time data

*We will return to each of these in more detail.*

---

<!-- _class: section-break -->

## Part 1

# The foundations

How the browser platform, HTML, CSS and JavaScript work together.

---

# The Web Development Landscape

- The **browser** is the runtime environment
- Applications are assembled from layers and reusable parts
- **HTML** provides structure and meaning
- **CSS** provides appearance and layout
- **JavaScript** provides behaviour and interaction
- Component libraries provide much of the UI
- The **Salt design system** provides shared design guidance and themes

---

# HTML: Structure and Meaning

- Elements describe content; attributes provide additional information
- Semantic HTML improves accessibility and maintainability
- Define the page structure and layout
- Use semantic elements where application code needs them
- Associate labels with form controls
- Preserve accessibility when composing components

---

# CSS: Describing Presentation with a Design System

- Component libraries provide most of the detailed styling
- Define layout, spacing and application-specific composition
- Keep structure and presentation separate
- Consistent spacing and typography improve usability
- Shared patterns become reusable components
- Salt theme variables provide shared design tokens
- Responsive and accessible behaviour should be intentional
- CSS custom properties connect the theme to component styling

---

# JavaScript and TypeScript

- JavaScript runs in the browser
- TypeScript adds static type checking
- TypeScript is a development-time extension to JavaScript that is stripped away before JavaScript is deployed
- Types document expected data
- Types eliminate a certain category of bugs
- Types help navigate a large codebase and show the impact of changes
- Types can be used by tools to help automate refactoring

---

<!-- _class: section-break -->

## Part 2

# Reuse at scale

Libraries, component libraries, frameworks and the tooling that connects them.

---

# Libraries, Component Libraries and Frameworks

<div class="two-columns">

<div>

- **Libraries** provide reusable functionality that application code can call
- **Component libraries** provide pre-built UI building blocks
- **Frameworks** provide conventions and structure for organising applications
- Internal libraries provide domain-specific functionality

</div>

<div>

- `@salt-ds` is a component library
- `@vuu-ui` includes framework and component library packages
- D3.js and Moment.js are examples of libraries
- React is a library that encroaches in places into framework territory
- Next.js is a framework

</div>

</div>

---

<!-- _class: vuu-server -->

# The Vuu Server

- **Open-source Vuu project**<br><small>https://vuu.finos.org/desktop/</small>
- Streaming real-time data provider for web front ends
- A “backend for frontend”

---

# Web Development Tooling

| Tooling category | Why it matters |
| --- | --- |
| Package managers | npm, pnpm or yarn manage dependencies |
| Bundlers and dev servers | Build and run applications locally |
| Linters and formatters | Keep code consistent |
| Type checking and tests | Find problems before release |
| Git | Track, review and share changes |

> Tooling automates repetitive checks and tasks so developers can focus on the application.

---

<!-- _class: section-break -->

## Part 3

# Building applications

Composing UI, connecting data, and delivering useful browser-based experiences.

---

# Building Web Applications

- Use a foundational library &mdash; **React is the most popular**
- Combine and configure existing and custom components with layout to construct “pages” or “views”
- Bind components to application behaviour and data
- Manage state and synchronise the interface
- Communicate with APIs and WebSocket services
- Respond to asynchronous events
- Handle loading, error and disconnected states
- Keep application logic separate from presentation

---

# Features of Modern Web Applications

An application presents information **and** manages interaction.

Applications often include:

- Multiple views
- Forms and validation
- Remote data, possibly real-time
- User accounts with varied permissioning
- Persisting user settings across sessions
- Complex workflows

---

# Real-Time Web Applications

- Some applications must update without a page refresh
- A **WebSocket** creates a persistent connection between the server and browser client
- The server can push events to the browser immediately
- The browser listens for messages and updates the interface

**Common examples**

- Trading screens
- Live prices and market data
- Order status updates

---

# Design Systems

- **Salt is a complete design system**, not just a component library
- It provides a shared language for design and development
- The Salt theme is a collection of CSS custom variables
- Shared design tokens include:
  - Colour, typography and spacing
  - Borders and elevation
- Component guidelines and accessibility expectations reduce duplication and inconsistency

---

# Accessibility

## Our aspiration: support WCAG 2.1

- Use semantic HTML and accessible names
- Ensure keyboard access and visible focus states
- Provide sufficient colour contrast
- Support clear structure, labelling and error feedback
- Prefer accessible components and preserve their intended behaviour
- Test critical workflows with automated and manual checks

---

# Design Tools and Figma

- Design tools communicate ideas before implementation
- Inspect layouts, spacing, typography and colour
- Identify reusable components and states
- Compare design intent with browser behaviour
- Use **Figma** as a bridge between design and implementation
- Ask questions when designs are ambiguous

---

# AI-Assisted Development

AI is useful for **explanation, exploration and boilerplate**.

- Explain unfamiliar code
- Suggest alternatives
- Generate tests
- Find likely bugs
- Translate design intent into code

> Always review, test and understand generated code. Do not outsource responsibility for correctness or security.
