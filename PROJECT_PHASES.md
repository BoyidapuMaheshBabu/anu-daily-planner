# Project Phases — Anu Daily Planner

## Project status

**Current stage:** Planning and product definition  
**Implementation status:** Not started  
**Initial visual direction:** Blush, soft pink, and rose accent

This roadmap keeps the work small, sequential, and based on the intended user's feedback. A phase is not complete just because its issue exists; close a phase only after its exit criteria are met.

## Phase tracker

| Phase | Focus | Status | GitHub Issue |
|---|---|---|---|
| 01 | Requirements & Product Definition | Not started | [#1](https://github.com/BoyidapuMaheshBabu/anu-daily-planner/issues/1) |
| 02 | UI/UX Design & Pink Theme | Not started | [#2](https://github.com/BoyidapuMaheshBabu/anu-daily-planner/issues/2) |
| 03 | Technical Architecture & Data Model | Not started | [#3](https://github.com/BoyidapuMaheshBabu/anu-daily-planner/issues/3) |
| 04 | Core Task Management | Not started | [#4](https://github.com/BoyidapuMaheshBabu/anu-daily-planner/issues/4) |
| 05 | Scheduled Reminders & Recurring Tasks | Not started | [#5](https://github.com/BoyidapuMaheshBabu/anu-daily-planner/issues/5) |
| 06 | Personalization & Experience Polish | Not started | [#6](https://github.com/BoyidapuMaheshBabu/anu-daily-planner/issues/6) |
| 07 | Testing & Reliability | Not started | [#7](https://github.com/BoyidapuMaheshBabu/anu-daily-planner/issues/7) |
| 08 | Real-User Review & Refinement | Not started | [#8](https://github.com/BoyidapuMaheshBabu/anu-daily-planner/issues/8) |
| 09 | Release, Documentation & Maintenance | Not started | [#9](https://github.com/BoyidapuMaheshBabu/anu-daily-planner/issues/9) |

## Phase goals

### Phase 01 — Requirements & Product Definition
Clarify the user's day-to-day problem, turn it into user stories and acceptance criteria, agree on the MVP, and record privacy expectations.

### Phase 02 — UI/UX Design & Pink Theme
Define the main screen flows and establish the visual system. The chosen initial palette is:
- **Blush:** `#FFF0F6`
- **Soft pink:** `#F4B6D2`
- **Rose accent:** `#D94D8A`

Use pink gradients selectively, keep task surfaces readable, and check contrast and accessibility. Validate the design with the intended user before treating it as final.

### Phase 03 — Technical Architecture & Data Model
Choose the platform and stack, define task and recurrence data, decide on storage, and document notification/permission trade-offs. Avoid accounts, cloud sync, or a backend unless requirements justify them.

### Phase 04 — Core Task Management
Implement the agreed task lifecycle: create, view, edit, delete, schedule where needed, and mark tasks complete. Persist task state and validate user input.

### Phase 05 — Scheduled Reminders & Recurring Tasks
Implement and verify one-time notifications, agreed recurrence patterns, reminder cancellation/rescheduling, and snooze or missed-reminder behavior. Test on the real target device; do not assume exact delivery behavior without testing platform constraints.

### Phase 06 — Personalization & Experience Polish
Apply the theme consistently and add only the personalization that helps the intended user. Keep the common actions quick, clear, and accessible.

### Phase 07 — Testing & Reliability
Exercise core flows, recurrence edge cases, permissions, app restart/device reboot behavior, persistence, and duplicate-notification risks. Track defects in GitHub Issues and link fixes to commits.

### Phase 08 — Real-User Review & Refinement
Let the intended user try a test build, gather feedback with permission, prioritize improvements, and retest affected workflows. Keep private conversations and unnecessary personal details out of public artifacts.

### Phase 09 — Release, Documentation & Maintenance
Verify a release candidate, document setup and permissions, list tested and untested behavior, record known limitations, and create a versioned release only when a usable build is ready.

## Working rules

- Keep the MVP small; move nonessential ideas to a later phase.
- Do not mark planned features as implemented until they are built and tested.
- Use GitHub Issues to track decisions, bugs, and follow-up work.
- Prefer evidence: tests, screenshots, commits, and release notes over unsupported claims.
- Protect the intended user's privacy in the repository and in public demonstrations.
