# Bootstrap 5 Migration & UI Modernization: Coding Club Website

## 📖 Project Overview

This repository documents the evolution of a web ecosystem I originally engineered using **Bootstrap 4.5.2**, and subsequently refactored to meet modern **Bootstrap 5.3.8** standards.

The goal of this project is to demonstrate full lifecycle development: from the initial architecture of a responsive layout to the complex task of auditing and migrating a legacy codebase. It highlights the ability to manage technical debt, remove heavy dependencies (jQuery), and implement modern CSS logical properties within a production-ready environment.

## ⚙️ Technical Highlights (The "Under the Hood" Features)

This project displays technical growth and maintenance skills across two distinct phases of development:

### Phase 1: Original Architecture (Bootstrap 4)
* **Responsive Layouts:** Designed a custom grid system to handle complex content structures, including the 3-column "Gallery" view that stacks vertically on mobile devices.
* **Constraint Validation:** Implemented HTML5 regex patterns in the initial build to enforce data integrity for user emails and phone numbers (`123-456-7890`).

### Phase 2: The Migration (Refactoring to Bootstrap 5)
* **Dependency Decoupling:** Successfully decoupled the project from **jQuery**, rewriting dynamic behaviors (modals, dropdowns, togglers) to use Bootstrap 5's native vanilla JavaScript bundle.
* **Syntax Modernization:** Audited the codebase to transition from the deprecated `data-*` syntax to the new namespaced `data-bs-*` standard, ensuring zero console errors in the updated environment.
* **Logical Spacing:** Updated layout utilities to support internationalization standards (RTL support) by replacing directional margins (e.g., `ml-auto`) with logical margins (e.g., `me-auto`).

### 🔍 Refactoring Examples (Key Differences)
The table below illustrates the types of syntax and architectural updates I implemented during the migration:

| Feature | Original Approach (Bootstrap 4) | Updated Approach (Bootstrap 5) |
| :--- | :--- | :--- |
| **JS Triggers** | `data-toggle="collapse"` | `data-bs-toggle="collapse"` |
| **Targeting** | `data-target="#navbar"` | `data-bs-target="#navbar"` |
| **Spacing (RTL)** | `class="ml-auto"` (Left) | `class="me-auto"` (End) |
| **Close Buttons** | `class="close"` | `class="btn-close"` |

## ✨ Functional Features

### 1. User Interface & Layout
* **Responsive Navigation:** A fully responsive navbar that collapses on mobile devices, originally built with jQuery dependency and refactored to vanilla JS attributes.
* **Grid Systems:** Utilization of the grid system to manage content density across devices, ensuring readability on both mobile and desktop views.

### 2. Educational & Media Components
* **Code Presentation:** The "Tips & Tricks" section renders raw code snippets using preformatted text blocks (`<pre><code>`) to demonstrate syntax highlighting for educational purposes.
* **Media Gallery:** A grid-based media gallery featuring hover-state interactivity and optimized image rendering.
* **Member Spotlights:** A dedicated layout for displaying user profiles using circular avatars and bio text.

## 🛠️ Technology Stack

* **Framework:** Bootstrap 5.3.8 (Migrated from 4.5.2)
* **Scripting:** Vanilla JavaScript (Refactored from jQuery)
* **Markup:** HTML5 (Semantic Structure)
* **Styling:** CSS3 (Custom animations & overrides)

## 🗄️ File Structure

The repository is organized to facilitate a review of the modernization process:

* **`/v1-bootstrap-4`**: Contains the original source code.
* **`/v2-bootstrap-5`**: Contains the modernized, production-ready code.

## 🚀 Installation & Usage

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/AshleyKlibowitz/coding-club-ui-architecture.git](https://github.com/AshleyKlibowitz/coding-club-ui-architecture.git)
    ```
2.  **Navigate to the version:**
    Go to the `/v2-bootstrap-5` directory to see the modernized site.
3.  **Launch:**
    Open `final.html` in any modern web browser. No server setup is required as the project utilizes CDN links for all dependencies.
