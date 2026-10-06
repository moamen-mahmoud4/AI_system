# Authentication Design

## Unified Login
One login screen supports Manager and Teacher roles.

## Demo Accounts
Manager: manager@example.com / manager123

Teachers:
- john@example.com / teacher123
- ahmed@example.com / teacher123
- sara@example.com / teacher123

## Manager Pages
manager-dashboard.html, teachers.html, add-teacher.html, edit-teacher.html, delete-teacher.html

## Teacher Pages
teacher-home.html, generate-summary.html, upload-reference.html, previous-summaries.html, references.html

## Session
`currentUser` and `role` are stored in localStorage for this frontend demo. `requireRole()` blocks unauthorized roles and redirects to login. `logout()` clears the session.

> This is a frontend university demonstration, not production authentication. A real application must use secure backend authentication, hashed passwords, sessions/JWT, and server-side authorization.
