# AI Lecture Generator — Frontend

A beginner-friendly frontend prototype based on the supplied Task 4 UI design for an AI system that helps teachers generate lecture summaries and presentations.

## Features
- Manager login and password recovery flow.
- Manager dashboard.
- Teacher management: search, add, edit and delete.
- Teacher home dashboard.
- Summary generation with reference, output format, length and quality characteristics.
- Reference upload with PDF/DOCX/PPTX validation.
- Previous summaries with search/open/delete.
- References with search/delete.
- Responsive desktop/tablet/mobile layout.
- Modern animations, cards, badges, modals and notifications.
- Dummy data stored in localStorage; no backend required.

## Run
1. Extract the ZIP.
2. Open `index.html` in a modern browser.
3. Manager demo login:
   - Email: `manager@example.com`
   - Password: `manager123`

## Project structure
- `index.html`: manager login.
- `pages/`: all application screens.
- `css/style.css`: global UI, dashboard, tables, forms, responsive styles and animations.
- `css/auth.css`: authentication screen styling.
- `js/main.js`: shared data, localStorage, sidebar and toast helpers.
- `js/auth.js`: login interaction.
- `assets/`: place images/icons here if needed.

## Main JavaScript functions
- `saveData()`: saves dummy data to localStorage.
- `showToast(message)`: displays a small success/info notification.
- `setupSidebar()`: controls the mobile sidebar.
- `logout()`: returns to manager login and clears the demo role.
- `renderTeachers(list)`: builds the teacher table.
- `searchTeachers()`: filters teachers using the search field.
- `openDelete(id)`: opens the teacher deletion confirmation modal.
- `confirmDelete()`: removes a teacher and refreshes the table.
- `renderSummaries(list)`: builds the previous summaries table.
- `renderReferences(list)`: builds the references table.

## Important note
This is a frontend-only academic prototype. Authentication, upload, summary generation and data changes are simulated in the browser. A production system should connect these interfaces to a secure backend/API and database.


## Authentication
Manager: manager@example.com / manager123
Teachers: john@example.com / teacher123, ahmed@example.com / teacher123, sara@example.com / teacher123

The unified login selects the account role. Manager-only and Teacher-only pages are protected by role checks. Logout clears the session.
