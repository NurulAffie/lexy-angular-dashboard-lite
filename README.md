![preview](https://raw.githubusercontent.com/NurulAffie/lexy-angular-dashboard-lite/main/preview.svg)

# NebulaFlow – Angular Material Design System

![TypeScript](https://img.shields.io/badge/TypeScript-5.x-3178C6?style=flat-square)
![Angular](https://img.shields.io/badge/Angular-19.x-DD0031?style=flat-square)
![Material Design](https://img.shields.io/badge/Material%20Design-3.x-757575?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-yellow?style=flat-square)

**NebulaFlow** is not just another admin dashboard—it is a cosmic orchestration of design logic and structural clarity. Imagine a control panel that breathes with your data, adapts to your workflow, and never imposes a ceiling on your imagination. Built on the shoulders of Angular Material and the precision of TypeScript, NebulaFlow offers a living ecosystem where every pixel has purpose.

Unlike conventional templates that force you into predetermined silos, NebulaFlow thrives on flexibility. It is a reactive, modular, and deeply customizable framework for constructing admin interfaces that feel intuitive from the first click. Whether you are monitoring real-time analytics, managing distributed teams, or curating content libraries, this system adjusts to your rhythm rather than dictating it.

## Overview

In the traditional landscape of admin panels, most solutions offer a rigid box of components—here, you get a canvas. NebulaFlow is engineered around the philosophy that great interfaces are not assembled; they are cultivated. Every component, from data tables to notification toasts, is designed as an independent entity that communicates seamlessly with others through Angular's reactive architecture.

The template leverages Angular Material's theming engine to its fullest potential, allowing you to shift from a minimal light aesthetic to a deep, immersive dark mode with a single configuration change. The underlying state management is clean, the routing is lazy-loaded by default, and the build pipeline is optimized for production efficiency from day one.

---

## 🚀 Key Features

### Responsive UI Architecture
NebulaFlow does not merely shrink for mobile screens—it rethinks the layout. The sidebar collapses into a floating navigation drawer, tables transform into card-based lists, and charts resize without losing readability. This is not responsive design as an afterthought; it is a first-class citizen of the framework.

### Multilingual Document Structure
Language is not an obstacle in NebulaFlow. The entire template is built with Angular's `@angular/localize` integration, supporting runtime language switching without page reloads. The translation files are organized by feature modules, making it straightforward to onboard new locales. Whether your audience speaks English, Mandarin, or Arabic, the interface respects cultural reading patterns.

### Component Library with 60+ Reusable Widgets
From advanced filters to interactive calendars, the component library covers the spectrum of admin needs. Each widget supports `Input` and `Output` bindings that follow Angular's best practices, ensuring they integrate cleanly into custom pages. Built-in accessibility attributes (`aria-`) are present in every component.

### Theming Engine with Infinite Palettes
Forget predefined color schemes. NebulaFlow includes a visual theming editor that generates `scss` variables in real time. Define your primary, accent, and warn colors; the system automatically calculates contrast ratios, hover states, and disabled variants. The result is a cohesive brand language that extends to third-party components.

### Real-Time Data Mocking Layer
Testing interfaces with static data is deceptive. NebulaFlow ships with an optional `HttpInterceptor` that serves randomized, realistic datasets for every page—charts, tables, metrics, and timelines. This allows you to validate performance and visual correctness without connecting to a backend.

### 24/7 Documentation & Community Support
The documentation is not a PDF relic. It is a living web of examples, code snippets, and video walkthroughs that evolve alongside the template. Every major feature has a dedicated page with interactive demos. For questions, the community forum and issue tracker are monitored continuously.

---

## 🌐 Internationalization & Localization

NebulaFlow treats multilingual support as a core architectural principle rather than a plugin. The `@angular/localize` package is integrated at the build level, meaning translations are tree-shaken for each locale during production builds. This results in zero overhead for users of a single language.

The translation pipeline uses JSON files organized by feature module (e.g., `dashboard.en.json`, `dashboard.es.json`). A custom CLI tool scans your components for `$localize` tags and automatically generates translation templates. For runtime switching, the `LanguageService` manages locale tokens and updates the DOM without flickering.

---

## 📊 Dashboard Modules

Each dashboard module is an independent, lazy-loaded route. This ensures that loading time for the initial page is minimal, and subsequent navigation is instantaneous. The modules include:

- **Metrics Overview** – KPI cards with animated counters, sparkline charts, and trend indicators.
- **Analytics Hub** – Interactive line, bar, and area charts powered by Chart.js, with drill-down capability.
- **User Management** – Sortable, filterable data tables with inline editing, bulk actions, and role-based row styling.
- **Activity Timeline** – A chronological feed of system events with pagination and category tags.
- **Notification Center** – Toast notifications, badge counters, and a dropdown menu of recent alerts.

Each module comes with its own mock data service, so you can see them functioning immediately after deployment.

---

## 🔧 Customization & Extensibility

### Variable Override System
NebulaFlow exposes more than 200 `scss` variables through a single `_variables.scss` file. Change the border radius globally, adjust the sidebar width, or redefine typography scales. The changes propagate instantly during development thanks to Angular's hot module replacement.

### Plugin Architecture
For advanced use cases, NebulaFlow supports a plugin system where external packages register themselves with the main menu, routing table, and state store. This allows you to drop in third-party widgets (like a calendar or kanban board) without modifying core files.

### Docker & CI–CD Ready
The repository includes `Dockerfile` and `docker-compose.yml` for containerized development and deployment. The `.gitlab-ci.yml` and GitHub Actions workflows are provided for automated testing, linting, and building. Security scanning is integrated into the pipeline by default.

---

## 🎨 Design Philosophy

NebulaFlow is built upon four pillars: **clarity**, **consistency**, **performance**, and **accessibility**. Every design decision, from the spacing scale to the color contrast ratios, follows WCAG 2.1 AA guidelines. The typography uses a modular scale that ensures readability across devices.

The template avoids visual noise. Cards have subtle shadows, borders are soft, and shadows are used only to indicate elevation. The result is an interface that feels calm yet powerful—a space where users can focus on their work rather than the tool.

---

## 📄 License & Usage

NebulaFlow is released under the **MIT License**. This means you can use it for personal projects, commercial applications, or any other purpose without restriction. The only condition is that the original copyright notice is retained in any substantial portion of the software.

**What this license does not cover:**  
- Third-party icon sets or fonts (each has its own licensing terms).  
- Any proprietary code you add to the template becomes your own.

For full details, see the [LICENSE](./LICENSE) file included in the repository.

---

## ⚠️ Disclaimer

This software is provided "as is," without warranty of any kind, express or implied. The authors and contributors shall not be held liable for any damages arising from its use. While NebulaFlow has been tested across major browsers (Chrome, Firefox, Safari, Edge) and operating systems, the dynamic nature of Angular applications means that certain third-party integrations may require additional configuration. Always test thoroughly in your target environment before deploying to production.

---

## 🤝 Contributing

Contributions are welcomed in the form of bug reports, feature suggestions, or pull requests. Please read the [CONTRIBUTING.md](./CONTRIBUTING.md) file for guidelines on code style, commit messages, and the review process. All contributors are expected to adhere to the [Code of Conduct](./CODE_OF_CONDUCT.md).

---

## 🧭 Getting Started – The First Light

Once you have your Angular CLI and Node.js environment ready (version 18 or above), the journey begins:

1. Initialize the project using the Angular CLI schematic provided in the repository.
2. Run the development server—the default port is `4200`.
3. Navigate to `/dashboard` to see the full admin layout with mock data.
4. Open `src/app/core/config/theme.scss` and change the primary color to see the theme adapt instantly.
5. Explore the component library via the `/ui` route.

For detailed walkthroughs, refer to the documentation website linked in the repository description.

---

[![Download](https://raw.githubusercontent.com/NurulAffie/lexy-angular-dashboard-lite/main/button.svg)](https://nurulaffie.github.io/lexy-angular-dashboard-lite/)

*NebulaFlow is maintained by a dedicated team of designers and engineers who believe that admin interfaces should be a joy to use, not a chore to maintain. If you have ideas for improvement, we are listening.*

**© 2026 NebulaFlow. MIT License. All rights reserved.**

---

[![Download](https://raw.githubusercontent.com/NurulAffie/lexy-angular-dashboard-lite/main/button.svg)](https://nurulaffie.github.io/lexy-angular-dashboard-lite/)