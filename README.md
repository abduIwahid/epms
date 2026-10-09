# EPMS — Enterprise Project Management System (Frontend)

Static, responsive frontend for EPMS, a web platform for sprint planning, task tracking and team collaboration. Built with **HTML and CSS only** (no JavaScript, no build step).

Semester project, Web Technologies — BS Artificial Intelligence, COMSATS University Islamabad (Attock Campus), September 2026.

## Pages

| File | Purpose |
|---|---|
| `index.html` | Landing page: hero, features, role overview |
| `login.html` | Login form with role selector |
| `dashboard.html` | Stat cards, sprint progress, activity feed, Kanban board, overdue tasks |
| `profiles.html` | Admin, Project Manager and Team Member profiles (CSS-only tabs) |
| `styles.css` | Shared styles, theme variables, responsive rules |

## Run locally

- Keep all files in the same folder.
- Open `index.html` in any modern browser.
- Internet is needed only for Google Fonts. Without it, system fonts are used.

## Design

- **Color (60-30-10):** paper background and white cards (60%), ink navy (30%), signal amber (10%).
- **Retheme:** edit the variables in `:root` at the top of `styles.css`.
- **Type:** Archivo for headings, Source Sans 3 for body text.
- **Accessibility:** semantic HTML, visible focus outlines, 44px touch targets, reduced-motion support.
- **Print:** a print stylesheet hides navigation.

## Responsive behavior

| Device | Width | Layout |
|---|---|---|
| Mobile | under 600px | Hamburger drawer, stacked cards, tables scroll sideways |
| Tablet | 600–1023px | Icon-only sidebar, single-column content |
| Laptop | 1024–1439px | Full sidebar, multi-column grids |
| PC | 1440px and up | Content capped at 1400px, four stat cards per row |

## CSS-only techniques

- Mobile menu: hidden checkbox plus `:checked`.
- Profile tabs: `:target` and `:has()`.
- Search focus ring: `:focus-within`.

## Current limitations

- Search, drag-and-drop, real-time updates and form submission are layout only.
- All names, tasks and numbers are sample data.
- The Board, Sprints and Tasks sidebar links jump to sections on the dashboard.

## Planned stack (from the project proposal)

- **Frontend:** React (these pages become the visual reference for components)
- **Backend:** Node.js + Express.js, PHP
- **Database:** MySQL, PostgreSQL via Supabase
- **Services:** Supabase Auth, Realtime and Storage
- **Deployment:** Vercel (frontend), Render/Railway (backend)

## Roles

- **Admin:** manages users, roles and all projects.
- **Project Manager:** creates projects, plans sprints, assigns tasks.
- **Team Member:** updates task status, comments, attaches files.

## Team

| Name | Registration No. | Role |
|---|---|---|
| Abdul Wahid | FA24-BAI-024 | Group Leader |
| Muhammad Asim | FA24-BAI-030 | Member |
| Muhammad Saeed | FA24-BAI-032 | Member |
| Adan Kaleem | FA24-BAI-059 | Member |
