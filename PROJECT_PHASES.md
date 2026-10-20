# Project Phases — Anu Daily Planner

## Project status

**Current stage:** Planning and product definition  
**Implementation status:** Not started  
**Initial design direction:** Selectable Pink and Blue themes

This roadmap keeps the work small, sequential, and based on the intended user's feedback. A phase is not complete just because its issue exists; close a phase only after its exit criteria are met.

## Phase tracker

| Phase | Focus | Status | GitHub Issue |
|---|---|---|---|
| 01 | Requirements & Product Definition | Not started | [#1](https://github.com/BoyidapuMaheshBabu/anu-daily-planner/issues/1) |
| 02 | UI/UX Design & Pink/Blue Theme System | Not started | [#2](https://github.com/BoyidapuMaheshBabu/anu-daily-planner/issues/2) |
| 03 | Technical Architecture & Data Model | Not started | [#3](https://github.com/BoyidapuMaheshBabu/anu-daily-planner/issues/3) |
| 04 | Core Task Management | Not started | [#4](https://github.com/BoyidapuMaheshBabu/anu-daily-planner/issues/4) |
| 05 | Alarms, Scheduled Reminders & Recurring Schedules | Not started | [#5](https://github.com/BoyidapuMaheshBabu/anu-daily-planner/issues/5) |
| 06 | Personalization & Experience Polish | Not started | [#6](https://github.com/BoyidapuMaheshBabu/anu-daily-planner/issues/6) |
| 07 | Testing & Reliability | Not started | [#7](https://github.com/BoyidapuMaheshBabu/anu-daily-planner/issues/7) |
| 08 | Real-User Review & Refinement | Not started | [#8](https://github.com/BoyidapuMaheshBabu/anu-daily-planner/issues/8) |
| 09 | Release, Documentation & Maintenance | Not started | [#9](https://github.com/BoyidapuMaheshBabu/anu-daily-planner/issues/9) |

## Phase goals

### Phase 01 — Requirements & Product Definition
Clarify the user's day-to-day problem and turn it into user stories and acceptance criteria. Explicitly distinguish a task reminder from an alarm clock: agree what the alarm should do when it rings, whether it repeats on selected days, and which Stop/Snooze controls are expected. Confirm whether Pink should be the initial default and that Blue should be available as an alternate theme. Agree on the MVP and record privacy expectations.

### Phase 02 — UI/UX Design & Pink/Blue Theme System
Define the main screen flows, including task lists, task editing, alarm creation/editing, active alarm states, reminder controls, and theme selection. Build a consistent theme system based on centralized color tokens.

**Pink theme (initial default):**
- **Blush:** `#FFF0F6`
- **Soft pink:** `#F4B6D2`
- **Rose accent:** `#D94D8A`

**Blue theme (alternative):**
- **Ice blue:** `#F2F7FF`
- **Soft blue:** `#B8D8FF`
- **Azure accent:** `#3978D4`

Use gradients selectively and keep task and alarm controls readable. Design a theme selector, selected-state feedback, and a consistent application of colors across screens. Check contrast and accessibility. Validate the design with the intended user before treating it as final.

### Phase 03 — Technical Architecture & Data Model
Choose the platform and stack, define task, alarm, and recurrence data, and decide on storage. Determine how the selected theme preference will be saved locally and restored on app launch. Research and document the platform's scheduling APIs, exact-alarm or notification permissions where applicable, reboot/rescheduling behavior, and battery/background constraints. Avoid accounts, cloud sync, or a backend unless requirements justify them.

### Phase 04 — Core Task Management
Implement the agreed task lifecycle: create, view, edit, delete, schedule where needed, and mark tasks complete. Persist task state and validate user input. Keep task lifecycle behavior separate from alarm lifecycle behavior where needed.

### Phase 05 — Alarms, Scheduled Reminders & Recurring Schedules
Implement and verify the agreed alarm-clock workflow separately from task reminders. Scope to confirm in Phase 01 includes:
- Creating, editing, enabling/disabling, and deleting an alarm.
- Choosing an alarm time and repeat days if required.
- Defining ring, Stop, and Snooze behavior and any sound/vibration settings included in the MVP.
- Scheduling task reminders and recurring tasks separately from alarms.
- Handling permission denial, cancellation/rescheduling, app restart, and device reboot according to platform capabilities.
- Checking for duplicate alerts and missed schedules.

Test on the real target device. Do not assume precise delivery or full alarm-clock behavior without testing the chosen platform and its constraints.

### Phase 06 — Personalization & Experience Polish
Apply the Pink and Blue themes consistently and let the user switch themes in the app's settings. Persist her choice locally so it remains selected after the app is reopened. Add only the personalization that helps the intended user. Keep the common task and alarm actions quick, clear, and accessible.

### Phase 07 — Testing & Reliability
Exercise task flows, alarm creation and ringing behavior, Stop/Snooze actions, recurrence edge cases, permissions, app restart/device reboot behavior, persistence, and duplicate-alert risks. Verify the theme selector and that both themes apply consistently to all relevant screens, including after an app restart. Track defects in GitHub Issues and link fixes to commits.

### Phase 08 — Real-User Review & Refinement
Let the intended user try a test build, gather feedback with permission, prioritize improvements, and retest affected workflows. Ask specifically whether alarm behavior and both theme choices fit her expectations. Keep private conversations and unnecessary personal details out of public artifacts.

### Phase 09 — Release, Documentation & Maintenance
Verify a release candidate, document setup and permissions, list tested and untested behavior, record known limitations, and create a versioned release only when a usable build is ready.

## Working rules

- Keep the MVP small; move nonessential ideas to a later phase.
- Do not mark planned features as implemented until they are built and tested.
- Use GitHub Issues to track decisions, bugs, and follow-up work.
- Prefer evidence: tests, screenshots, commits, and release notes over unsupported claims.
- Protect the intended user's privacy in the repository and in public demonstrations.
