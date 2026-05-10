# LazyTasks — QA / SDET Showcase

This repository documents my **Quality Assurance** and **SDET** work on **[LazyTasks](https://lazytasks.com)**, a WordPress project management plugin by **LazyCoders LLC**.

> The plugin source code is private. This repo is a public summary of the QA scope, the testing approach I follow, and the tools I use day-to-day.

---

## About LazyTasks

LazyTasks is a full-featured project management plugin for WordPress. It ships a web dashboard plus a companion mobile app, and supports a wide feature set:

- **Multiple views** — List, Board (Kanban), Gantt Chart, Calendar
- **Add-ons** — Whiteboard, Time Tracker, Performance Scorer
- **Imports** — Trello, Todoist
- **Workspaces & Projects** with tiered delete model
- **Roles & Permissions** — fine-grained, 45+ permissions across UI scopes
- **Portal customization** — branding, headers, navigation modes
- **Integrations** — SMTP, Google OAuth, V3 REST API
- **Mobile app** — iOS & Android, V3 API parity
- **i18n** — multi-language support (incl. Bangla translation)

---

## My Role

**QA / SDET** — responsible for verifying releases across web and mobile, building automated test coverage, and reporting issues with clear reproduction steps.

### What I cover
- **Web** — WordPress plugin UI, V3 API, role/permission matrix, multi-view consistency
- **Mobile** — iOS & Android app flows (auth, tasks, comments, profile, notifications)
- **Cross-cutting** — regression, smoke, exploratory, and release sign-off testing

---

## Testing Toolkit

| Area | Tools |
|------|-------|
| Web automation | Selenium WebDriver, Java, JUnit |
| Mobile automation | Appium (iOS & Android) |
| API testing | Postman |
| Bug tracking | GitHub Issues, internal trackers |
| Test management | Manual test plans, regression checklists |
| Build / IDE | IntelliJ IDEA, Gradle |
| Version control | Git, GitHub |

---

## Sample Areas Tested in v1.5.0

A snapshot of feature areas signed off in the latest release:

- Time Tracker add-on — start/stop timer, header stopwatch, time logs, reports
- Performance Scorer — scoring rules, dashboard, KPI charts
- Trello & Todoist import wizards
- Permission system — 75 → 45 consolidation, parent-child constraints, 4-level cross-scope chains
- Gantt Chart — drag & resize, Day/Week/Month views
- Calendar — drag & resize, drop, RTE create-drawer
- Global search across all views
- V3 API end-to-end coverage
- Mobile app V3 API migration with full permission parity

---

## Selected Bugs Caught & Verified

- Critical PHP 7.4 compatibility regression
- Security fix on `toggle_super_admin`
- Task privacy API security gap
- 403 errors across V3 routes for non-admin users
- Superadmin bypass in 4 frontend locations
- Project member removal not unassigning tasks
- Unarchived tasks disappearing from list view
- Status picker wiping status on change

---

## Contact

**Nusrat Rita** — QA / SDET @ LazyCoders LLC
- Email: nmkhan@lazycoders.co
- GitHub: [@nusratrita](https://github.com/nusratrita)

---

*LazyTasks is a product of LazyCoders LLC. This repository is a personal portfolio summary and contains no proprietary source code.*
