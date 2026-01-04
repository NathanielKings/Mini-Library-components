Mini Component Library

A lightweight pure CSS component library showcasing reusable UI patterns. Built to practice consistent design systems, CSS variables, and predictable, reusable styles.

Table of Contents

Features

Getting Started

Components

Buttons

Inputs

Cards

Badges

Alerts

Navbar

Modal

Customization

Deployment

Features

Fully HTML + CSS only.

Reusable components with consistent naming.

CSS variables for colors, spacing, and fonts.

Predictable hover, focus, and error states.

Easy to extend with new components.

Getting Started

Clone the repository:

git clone https://github.com/yourusername/mini-component-library.git

Open index.html in your browser.

Link components via CSS in your own project or use as a reference.

Components
Buttons
Class Description
.button Base button style
.button-primary Primary action button (blue)
.button-secondary Secondary action button (orange)
.button-disabled Disabled button (grey)

Example:

<button class="button button-primary">Primary</button>
<button class="button button-secondary">Secondary</button>
<button class="button button-disabled">Disabled</button>

Inputs
Class Description
.input Base input field
.input-error Input field with error state
.error-text Text describing the error

Example:

<input type="text" class="input" placeholder="Normal input">
<input type="text" class="input input-error" placeholder="Error input">
<div class="error-text">This field is required</div>

Cards
Class Description
.card Basic card container with padding and shadow

Example:

<div class="card">
  This is a simple card.
</div>

Badges
Class Description
.badge Base badge
.badge-primary Primary badge (blue)
.badge-success Success badge (green)
.badge-error Error badge (red)
.badge-warning Warning badge (yellow)
.badge-info Info badge (light blue)

Example:

<span class="badge badge-primary">Primary</span>
<span class="badge badge-success">Success</span>

Alerts
Class Description
.alert Base alert
.alert-success Success alert
.alert-error Error alert
.alert-warning Warning alert
.alert-info Info alert

Example:

<div class="alert alert-success">Success alert</div>
<div class="alert alert-error">Error alert</div>

Navbar
Class Description
.navbar Top navigation bar
.navbar a Navbar links

Example:

<nav class="navbar">
  <div>Logo</div>
  <div>
    <a href="#">Home</a>
    <a href="#">Components</a>
  </div>
</nav>

Modal
Class Description
.modal Overlay container (hidden by default)
.modal.show Displays modal
.modal-content Modal content box

Example:

<button class="button button-primary" onclick="document.querySelector('.modal').classList.add('show')">Open Modal</button>

<div class="modal" onclick="this.classList.remove('show')">
  <div class="modal-content" onclick="event.stopPropagation()">
    <h3>Modal Title</h3>
    <p>This is a modal.</p>
    <button class="button button-secondary" onclick="document.querySelector('.modal').classList.remove('show')">Close</button>
  </div>
</div>

Customization

You can easily customize colors, spacing, fonts, and border-radius using CSS variables in variables.css:

:root {
--primary-color: #4f46e5;
--secondary-color: #f97316;
--spacing-md: 16px;
--border-radius: 8px;
--font-family: 'Segoe UI', sans-serif;
}

Deployment

Use GitHub Pages or Netlify to deploy the showcase.

Simply push your code and enable static site hosting.
