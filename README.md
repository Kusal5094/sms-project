# School Management System (SMS)

A web system for school timetables, teacher absences, substitutions, announcements, staff chat, inventory and a school calendar.

**Tech stack:** Next.js, TypeScript, Supabase (PostgreSQL, Auth, Realtime), Vercel, PWA

## Branches
| Branch | Module |
|---|---|
| main | Stable code |
| feature/academics | Teachers, classes, timetable |
| feature/substitution | Absences, cover, swaps |
| feature/communication | Announcements, notifications, chat |
| feature/resources | Inventory, calendar, PWA |
| feature/security-testing | RLS, constraints, testing |

Changes reach `main` only through a pull request reviewed by the repository owner.

## Monthly progress
Notes for each month of the project are in `docs/progress/`.

## Setup
    npm install
    cp .env.example .env.local   # then add your Supabase keys
    npm run dev
