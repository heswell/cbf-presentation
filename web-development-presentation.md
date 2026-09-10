---
marp: true
theme: default
paginate: true
---

# From Web Fundamentals to Modern UI Development

- How the browser turns code into interfaces
- From HTML, CSS and JavaScript to applications
- Tools, libraries, design systems and AI

---

# Session Roadmap

- Presentation: concepts and vocabulary
- Demos: seeing the concepts in practice
- Exercise: applying the concepts independently
- Goal: understand how the pieces fit together

---

# The Web Development Landscape

- The browser is the runtime environment
- Websites and applications are built from layers
- HTML: structure and meaning
- CSS: appearance and layout
- JavaScript: behaviour and interaction

---

# How a Browser Builds a Page

- Request and response
- HTML creates the document structure
- CSS is applied to the document
- JavaScript can inspect and change the page
- The browser renders the final result

---

# HTML: Structure and Meaning

- Elements describe the content
- Attributes provide additional information
- Semantic HTML improves accessibility and maintainability
- Common elements:
  - Headings
  - Paragraphs
  - Links
  - Images
  - Forms
  - Lists

---

# HTML: Building Good Foundations

- Use the right element for the right purpose
- Organise content hierarchically
- Associate labels with form controls
- Provide meaningful alternative text
- Prefer semantic elements over unnecessary `<div>` elements

---

# CSS: Describing Presentation

- Select elements to style
- Apply properties and values
- Understand the cascade
- Understand inheritance
- Use classes to create reusable styles
- Keep structure and presentation separate

---

# CSS Layout Fundamentals

- The box model
- `display`
- Flexbox
- CSS Grid
- Positioning
- Responsive layouts
- Designing for different screen sizes

---

# CSS: From Styling to Systems

- Repeated values become design tokens
- Shared patterns become reusable components
- Consistent spacing and typography improve usability
- Responsive and accessible behaviour should be intentional
- CSS can express both simple styles and complex layouts

---

# JavaScript in Modern Web Applications

- Connect user interactions to application behaviour
- Manage state and synchronise the interface
- Communicate with APIs and WebSocket services
- Respond to asynchronous events
- Update components efficiently
- Handle loading, error and disconnected states
- Keep application logic separate from presentation
- Use TypeScript and tooling to improve maintainability

---

# JavaScript in the Browser

- Selecting elements
- Listening for user events
- Updating content and styles
- Validating form input
- Managing application state
- Fetching and displaying data

---

# JavaScript and TypeScript

- JavaScript runs in the browser
- TypeScript adds static type checking
- Types document expected data
- Types help catch mistakes earlier
- TypeScript is compiled to JavaScript
- Both use the same underlying web platform

---

# From Pages to Applications

- A page primarily presents information
- An application manages interaction and state
- Applications often include:
  - Multiple views
  - Forms and validation
  - Remote data
  - User accounts
  - Complex workflows
- Complexity requires structure and conventions

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
  - Chat and collaboration tools
- Real-time interfaces must handle:
  - Connection loss
  - Reconnection
  - Out-of-order messages
  - High volumes of updates

---

# Libraries and Frameworks

- Libraries provide reusable functionality
- Frameworks provide stronger application structure
- Examples:
  - React
  - Vue
  - Angular
  - Svelte
- Learn the underlying web platform first
- Use abstractions when they solve a real problem

---

# Component Libraries

- Reusable UI building blocks
- Examples:
  - Buttons
  - Inputs
  - Dialogs
  - Tables
  - Navigation
- Components improve consistency
- APIs and states must be understood
- Components should remain accessible and adaptable

---

# Design Systems

- A shared language for design and development
- Design tokens:
  - Colour
  - Typography
  - Spacing
  - Borders
  - Elevation
- Component guidelines
- Accessibility expectations
- Design systems reduce duplication and inconsistency

---

# Design Tools and Sigma

- Design tools communicate ideas before implementation
- Inspect layouts, spacing, typography and colour
- Identify reusable components and states
- Compare design intent with browser behaviour
- Use Sigma as a bridge between design and implementation
- Ask questions when designs are ambiguous

---

# JavaScript Tooling

- Package managers: npm, pnpm or yarn
- Bundlers and development servers
- Linters and formatters
- Type checking
- Testing tools
- Version control with Git
- Tooling automates repetitive checks and tasks

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

---

# Putting the Pieces Together

- Design describes intent
- HTML provides structure
- CSS provides presentation
- JavaScript provides behaviour
- Components provide reuse
- Libraries provide abstractions
- Tooling supports quality and speed
- AI can support the developer throughout the process

---

# Common Beginner Mistakes

- Treating HTML as visual styling
- Using JavaScript for problems CSS already solves
- Ignoring accessibility
- Copying code without understanding it
- Adding libraries before understanding the problem
- Making components too large or too specific
- Not testing different screen sizes

---

# A Practical Development Workflow

- Understand the requirement
- Inspect the design
- Identify content and interactions
- Build semantic HTML
- Add layout and styling
- Add JavaScript behaviour
- Extract reusable components
- Test, review and refine

---

# What You Will See in the Demos

- Build a small interface from HTML and CSS
- Add interaction with JavaScript
- Introduce TypeScript or a component library
- Compare design and implementation
- Use browser developer tools
- Demonstrate AI-assisted development responsibly

---

# Exercise: Your First Implementation

- You will receive a design or interface brief
- Build a working implementation
- Use semantic HTML
- Apply responsive CSS
- Add the required interaction
- Submit your code and a short explanation
- Focus on clarity, correctness and accessibility

---

# Key Takeaways

- HTML, CSS and JavaScript remain the foundation
- Modern tools build on top of those fundamentals
- Components and design systems support consistency
- Tooling improves feedback and reliability
- AI is useful when guided and reviewed by a developer
- Good development starts with understanding the problem
