# Anu — Daily Planner, Reminders & Alarm

A personalized daily-planning app concept designed to help its intended user organize everyday tasks, remember scheduled activities, set alarms for important times, and choose a visual theme that suits her preferences.

> **Project status:** Planning and product definition. Implementation has not started.

## 🎯 Problem

People sometimes forget activities they intended to complete at a particular time. Anu aims to make everyday planning easier through task management, useful reminders, recurring schedules, a dedicated alarm-clock feature, and a personalized interface.

## ✨ Planned MVP

The scope will be confirmed during requirements gathering. Current planned capabilities include:

- **Task management** — Create, edit, and delete tasks.
- **Scheduled task reminders** — Receive a reminder about a task at its scheduled date and time.
- **Alarm clock** — Set an alarm for an important time, with clear Stop and Snooze controls as agreed in the requirements.
- **Recurring schedules** — Repeat tasks and alarms on selected days as agreed in the requirements.
- **Task completion** — Mark activities complete and distinguish completed from pending tasks.
- **Theme selection** — Switch between Pink and Blue visual themes, with the selected preference remembered locally.
- **Reminder and alarm controls** — Manage schedules and preferences, subject to the chosen platform's permissions and behavior.

**An alarm is not the same as a task reminder.** A task reminder is associated with an activity; an alarm is intended to alert the user at a chosen time, even when they are not actively using the app. The exact audible behavior, repeat options, snooze, stop controls, and platform constraints must be specified and tested before release.

These are planned features, not claims about an implemented build.

## 🎨 Initial Theme System

The app is planned to include two selectable themes. **Pink is the initial default; Blue is an alternative.** The user should be able to switch themes in settings, and the chosen theme should remain selected after the app is reopened.

### Pink theme

| Token | Hex | Intended use |
|---|---|---|
| Blush | `#FFF0F6` | Main background and soft surfaces |
| Soft pink | `#F4B6D2` | Gradient transitions and decorative details |
| Rose accent | `#D94D8A` | Primary actions and selected states |

### Blue theme

| Token | Hex | Intended use |
|---|---|---|
| Ice blue | `#F2F7FF` | Main background and soft surfaces |
| Soft blue | `#B8D8FF` | Gradient transitions and decorative details |
| Azure accent | `#3978D4` | Primary actions and selected states |

The theme system should use shared components and centrally defined color tokens rather than duplicate screen implementations. Contrast, readable task surfaces, accessible controls, and a calm notification experience take priority over decoration. Colors will be checked during UI implementation.

## 🗺️ Development Roadmap

See **[PROJECT_PHASES.md](./PROJECT_PHASES.md)** for the nine-phase plan and links to the GitHub Issues used to track each phase.

1. Requirements & Product Definition
2. UI/UX Design & Pink/Blue Theme System
3. Technical Architecture & Data Model
4. Core Task Management
5. Alarms, Scheduled Reminders & Recurring Schedules
6. Personalization & Experience Polish
7. Testing & Reliability
8. Real-User Review & Refinement
9. Release, Documentation & Maintenance

## 🛠️ Technology Stack

The target platform and technology stack have not been finalized. They will be chosen after requirements are clarified, with particular attention to alarm and notification behavior, appropriate data storage, maintainability, theme preference persistence, and the intended user's device.

## 🧪 Engineering Approach

- Validate requirements with the intended user.
- Keep scope small and prioritize the essential workflow.
- Track decisions and bugs in GitHub Issues.
- Test task reminders and alarm behavior on a real device, including relevant app/device lifecycle scenarios.
- Verify both themes, theme switching, and saved theme preference.
- Document verified features, test results, and known limitations honestly.

## 🔒 Privacy

The repository is public. Do not publish private conversations, personal schedules, or other identifying details about the intended user without explicit permission. Use anonymized examples in public documentation and screenshots.

## 📌 Current Status

This repository currently documents the plan and design direction. No app implementation, theme switching, release, alarm delivery, or reminder behavior is being claimed yet.
