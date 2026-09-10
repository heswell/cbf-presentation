---
marp: true
theme: default
paginate: true
---

# Session Roadmap

- Presentation: concepts and vocabulary
- Demos: seeing the concepts in practice
- Exercise: applying the concepts independently

---

# From Web Fundamentals to Modern Application Development

- How the browser turns code into interfaces
- From HTML, CSS and JavaScript to assembled applications
- Pre-existing components, data sources and glue code

---

# Key Building Blocks

- React: the application UI framework
- Salt: the design system, including themes and components (https://www.saltdesignsystem.com/salt/index)
- Vuu: reusable components and functionality for data-driven applications (https://github.com/finos/vuu)
- We will describe each building block in more detail later

---

# The Web Development Landscape

- The browser is the runtime environment
- Applications are assembled from layers and reusable parts
- HTML: structure and meaning
- CSS: appearance and layout
- JavaScript: behaviour and interaction
- Component libraries provide much of the UI
- The Salt design system provides shared design guidance and themes

# HTML: Structure and Meaning

- Elements describe the content
- Attributes provide additional information
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
- TypeScript is a development time extension to JavaScript that is stripped away before the JavaScript is deployed
- Types document expected data
- Types eliminate a certain category of bugs
- Types help navigate a large codebase and show the impact of changes
- Types can be used by tools to help automate refactoring

---

# Libraries, Component Libraries and Frameworks

- Libraries provide reusable functionality that application code can call
- Component libraries provide pre-built UI building blocks
- Frameworks provide conventions and structure for organising applications
- `@salt-ds` is a component library (so are Material UI and shadcn/ui)
- `@vuu-ui` includes framework and component library packages
- D3.js and Moment.js are examples of libraries
- React is a library that encroaches in places into framework territory
- Next.js is a framework
- Internal libraries provide domain-specific functionality

---

# Web Development Tooling

- Package managers: npm, pnpm or yarn
- Bundlers and development servers
- Linters and formatters
- Type checking
- Testing tools
- Version control with Git
- Tooling automates repetitive checks and tasks

---

# Building Web Applications

- Use a foundational library - React is the most popular
- Combine and configure existing and custom components with layout to construct 'pages' or 'views'
- Bind components to application behaviour and data
- Manage state and synchronise the interface
- Communicate with APIs and WebSocket services
- Respond to asynchronous events
- Handle loading, error and disconnected states
- Keep application logic separate from presentation

---

# Features of Modern Web Applications

- An application presents information and manages interaction
- Applications often include:
  - Multiple views
  - Forms and validation
  - Remote data, possibly real-time
  - User accounts with varied permissioning
  - Persisting user settings across sessions
  - Complex workflows

---

# Real-Time Web Applications

- Some applications must update without a page refresh
- A WebSocket creates a persistent connection between:
  - The server
  - The browser client
- The server can push events to the browser immediately
- The browser listens for messages and updates the interface
- Common examples:
  - Trading screens
  - Live prices and market data
  - Order status updates

# Design Systems

- Salt is a complete design system, not just a component library
- A shared language for design and development
- The Salt theme is a collection of CSS custom variables
- Shared design tokens:
  - Colour
  - Typography
  - Spacing
  - Borders
  - Elevation
- Component guidelines
- Accessibility expectations
- Design systems reduce duplication and inconsistency

---

# Accessibility

- We aspire to support WCAG 2.1
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
- Use Figma as a bridge between design and implementation
- Ask questions when designs are ambiguous

---

# AI-Assisted Development

- Useful for explanation, exploration and boilerplate
- Can help:
  - Explain unfamiliar code
  - Suggest alternatives
  - Generate tests
  - Find likely bugs
  - Translate design intent into code
- Always review, test and understand generated code
- Do not outsource responsibility for correctness or security
