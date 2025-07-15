# spec.md

## Project Title: **DevBoard** — Scalable Team Collaboration App

## Overview

**DevBoard** is a full-stack project and task management platform, optimized for modern dev teams. It supports real-time collaboration, secure authentication, third-party integrations, and a refined UI using ShadCN and TailwindCSS. Built to demonstrate ownership, system design, and clean, scalable code practices.

## Tech Stack

| Layer         | Technology                                                                 |
|---------------|------------------------------------------------------------------------------|
| Frontend      | Next.js (App Router) + React + TypeScript                                   |
| UI Components | **ShadCN/UI**, TailwindCSS, Lucide Icons                                     |
| State Mgmt    | Zustand + React Query (TanStack Query)                                       |
| Forms         | React Hook Form + Zod (validation schema)                                   |
| Backend       | Node.js + Express (REST API)                                                |
| ORM           | Prisma (with PostgreSQL)                                                    |
| Auth          | **Auth.js** (v5+) with Google/GitHub OAuth + Credentials                    |
| Realtime      | Socket.IO                                                                   |
| Deployment    | Vercel (Frontend), Railway or Fly.io (API/DB), Docker (optional)            |
| CI/CD         | GitHub Actions (Test, Lint, Build, Deploy)                                  |
| Testing       | Vitest, Playwright (E2E), Supertest (API)                                   |
| Extras        | Slack Webhooks, Notion API, Framer Motion, Dnd-kit                          |

## Key Features

- **Modern Authentication**
  - Auth.js (v5+) with Google, GitHub, and email/password
  - JWT-based session handling with Prisma Adapter

- **Kanban Task Boards**
  - Drag & drop tasks across columns (using dnd-kit)
  - Real-time sync via WebSockets
  - Task priorities, labels, and assignees

- **Project & Team Management**
  - Invite teammates via email
  - Role-based access control (Admin/Member)
  - Activity feed, project audit trail

- **Integrated Chat (optional)**
  - Socket.IO-based live chat for each project
  - Markdown + emoji support

- **Dashboard & Insights**
  - Project summary metrics
  - Task velocity, active users, and team activity charts

- **Third-Party Integrations**
  - Sync with Notion DB
  - Send Slack alerts when tasks update

## Architecture

- **Frontend (Next.js App Router)**
  - ShadCN UI components for clean design
  - Modular routes and layouts
  - Server Actions for form submissions
  - Suspense-based data fetching with React Query
  - Zustand for local/global UI state

- **Backend (Express + PostgreSQL)**
  - RESTful API: `/api/v1/*`
  - Prisma schema with relational models (User, Project, Task, Comment)
  - Zod validation middleware
  - Auth.js integration with Prisma adapter and JWT strategy

- **Realtime**
  - Socket.IO event system for:
    - Task updates
    - Live chat
    - Board syncing

- **Database (PostgreSQL)**
  - Hosted via Railway or Supabase
  - Daily backups
  - Prisma migrations & seed data

## DevOps

- **CI/CD**: GitHub Actions (test, lint, deploy on push to `main`)
- **Linting/Formatting**: ESLint + Prettier
- **Docker**: Container for backend in production
- **Monitoring**: Vercel analytics + Railway logs

## Testing Strategy

| Layer         | Tool              | Coverage                            |
|---------------|-------------------|-------------------------------------|
| Unit Tests     | Vitest             | Utils, hooks, logic                 |
| API Tests      | Supertest          | Endpoints, auth flow                |
| E2E Tests      | Playwright         | User interactions, flows            |
| CI Enforcement | GitHub Actions     | Run on PRs                          |

## Timeline

| Phase              | Duration      | Status     |
|--------------------|---------------|------------|
| UI/UX Planning     | Week 1        | ✅ Done     |
| Frontend Setup     | Week 2–3      | ✅ Done     |
| Backend/API        | Week 3–4      | ✅ Done     |
| Realtime & Auth    | Week 5–6      | ✅ Done     |
| Testing & CI/CD    | Week 6–7      | ✅ Done     |
| Final Deployment   | Week 8        | ✅ Done     |

## Live Demo & Code

- **Live Site**: [https://devboard.app](https://devboard.app)
- **Frontend Repo**: [github.com/yourname/devboard-frontend](https://github.com/yourname/devboard-frontend)
- **Backend Repo**: [github.com/yourname/devboard-api](https://github.com/yourname/devboard-api)

## Goals & Outcomes

- Prove full ownership of a real-world, production-grade full-stack project
- Showcase ShadCN + modern frontend with scalable backend practices
- Highlight expertise in team workflows, DevOps, testing, and deployments
- Demonstrate usage of trending tools (Auth.js, Prisma, Zustand, TanStack, etc.)

