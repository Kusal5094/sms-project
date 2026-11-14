# School Management System (SMS)

A web-based school management system that replaces paper-based teacher absence handling, substitutions, timetables and notices with one platform.

**Live demo:** https://sms-project-lac.vercel.app

## Problem

Interviews with a vice principal and teachers at a local school showed that:

- Substitute teachers are arranged on paper every morning.
- Notices are passed around on WhatsApp groups and often get missed.
- Timetable clashes are hard to spot by hand.
- There is no record of school equipment.

SMS is built around these problems.

## Features

| Module | What it does |
|---|---|
| Authentication | Separate admin and teacher logins, password reset, pre-approved teacher registration |
| Academics | Teacher and class management, timetable builder, double-booking guard, Excel bulk import |
| Absence and Substitution | Full-day or period-wise absence reporting, admin approval, automatic cover, swap requests, cut-off rules |
| Communication | Targeted announcements with read receipts, in-app notifications, real-time staff chat (Hive) |
| Resources | Equipment inventory with check-out and return, low-stock alerts, school calendar with public and Poya holidays |
| Security | Row Level Security for every role, database constraints and triggers, audit logs |
| PWA | Installable on phones with offline support |

## User roles

Admin, Vice Principal, Sectional Head and Teacher. Each role has its own dashboard and can only read and change the data it is meant to.

## Tech stack

- Frontend: Next.js, TypeScript
- Backend: Supabase (PostgreSQL, Auth, Realtime)
- Hosting: Vercel
- Other: Serwist (PWA), SWR (caching), xlsx (Excel import), GitHub Actions (keep-alive workflow)

## Project phases

| Month (2026) | Phase | Main focus |
|---|---|---|
| January | Phase 1: Initiation | Team formation, problem study, proposal |
| February | Phase 2: Analysis and Design | SRS, tech stack, ERD, wireframes |
| March | Phase 3: Foundation | Project setup, authentication, roles, design system |
| April | Phase 4: Academics Module | Classes, teachers, timetable builder, Excel import |
| May | Phase 5: Absence and Substitution | Absence reporting, auto cover, swaps |
| June | Phase 6: Communication | Announcements, notifications, Hive staff chat |
| July | Phase 7: Resources and Refactor | Inventory, school calendar, PWA, UI clean-up |
| August | Phase 8: Security and Testing | RLS rewrite, DB safeguards, user testing |
| September | Phase 9: Deployment and Closure | Vercel deployment, documentation, final demo |

## Branches

`main` holds stable, reviewed code. Each module has its own branch for ongoing work.

| Branch | Module |
|---|---|
| main | Stable code |
| feature/academics | Teachers, classes, timetable builder, Excel import |
| feature/substitution | Absence reporting, auto cover, swaps |
| feature/communication | Announcements, notifications, Hive chat |
| feature/resources | Inventory, school calendar, PWA |
| feature/security-testing | RLS policies, database safeguards, testing |

Changes reach `main` only through a pull request reviewed by the repository owner. See CONTRIBUTING.md.

## Getting started

Requirements: Node.js 18 or later, a Supabase project, Git.

    git clone https://github.com/Kusal5094/sms-project.git
    cd sms-project
    npm install
    cp .env.example .env.local

Add your Supabase URL and keys to `.env.local`, then run:

    npm run dev

Open http://localhost:3000.

## Documentation

- [Database overview](docs/DATABASE_OVERVIEW.md)
- [Deployment guide](docs/DEPLOYMENT.md)
- [Project plan](docs/PLAN.md)
- [Refactoring progress](docs/PROGRESS.md)

## Team

| Name | Role / branch |
|---|---|
| Kusal | Repository owner, main review, feature/security-testing |
| NAME 1 | feature/academics |
| NAME 2 | feature/substitution |
| NAME 3 | feature/communication |
| NAME 4 | feature/resources |

Mentor: MENTOR NAME
