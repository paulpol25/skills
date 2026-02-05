---
name: Agent Capabilities Reference
description: Master map of all agents, their skills, technologies, and assignment guidance.
---

# Agent Capabilities Reference

This is the canonical reference for all agents in the system. Use it when deciding which agent should own a task.

---

## Agent Manager

**Role:** Coordinates the team — decomposes requirements, delegates tasks, orchestrates workflows, and reviews output.

| Skill | Path | Description |
|-------|------|-------------|
| Delegating Tasks | `agent-manager/delegating-tasks/SKILL.md` | Decompose requirements and assign tasks to agents |
| Orchestrating Workflow | `agent-manager/orchestrating-workflow/SKILL.md` | Manage execution order, parallelism, and blocked tasks |
| Reviewing Agent Output | `agent-manager/reviewing-agent-output/SKILL.md` | Quality gates, acceptance criteria verification, integration checks |

**Key strengths:** Project decomposition, cross-agent coordination, dependency management, quality assurance.
**Technologies:** Markdown task tracking, workflow patterns, review checklists.

---

## Architect

**Role:** Designs system structure — data models, API contracts, component hierarchies, and technical decisions.

| Skill | Path | Description |
|-------|------|-------------|
| Designing Systems | `architect/designing-systems/SKILL.md` | High-level architecture and system design |
| Defining API Contracts | `architect/defining-api-contracts/SKILL.md` | REST/GraphQL endpoint specs, request/response shapes |
| Data Modeling | `architect/data-modeling/SKILL.md` | Entity relationships, schema design, normalization |

**Key strengths:** Big-picture thinking, cross-cutting technical decisions, establishing contracts that other agents build against.
**Technologies:** System diagrams, OpenAPI/Swagger, ERD notation, ADRs (Architecture Decision Records).
**Assign when:** Work requires defining structure before implementation begins, or a technical decision affects multiple agents.

---

## Frontend

**Role:** Builds user-facing interfaces — pages, components, state management, and client-side logic.

| Skill | Path | Description |
|-------|------|-------------|
| Building Components | `frontend/building-components/SKILL.md` | Create reusable UI components |
| Managing State | `frontend/managing-state/SKILL.md` | Client-side state, data fetching, caching |
| Implementing Pages | `frontend/implementing-pages/SKILL.md` | Full page composition, routing, layout |

**Key strengths:** Component architecture, responsive UI, client-side performance, accessibility.
**Technologies:** React, TypeScript, Next.js, Tailwind CSS, Zustand/Redux, React Query.
**Assign when:** Work involves anything the user sees or interacts with in the browser.

---

## Backend

**Role:** Implements server-side logic — API endpoints, business rules, middleware, and service integrations.

| Skill | Path | Description |
|-------|------|-------------|
| Building API Endpoints | `backend/building-api-endpoints/SKILL.md` | REST endpoint implementation with validation |
| Implementing Business Logic | `backend/implementing-business-logic/SKILL.md` | Domain rules, service layer, data transformations |
| Writing Middleware | `backend/writing-middleware/SKILL.md` | Request/response pipeline, logging, error handling |

**Key strengths:** API implementation, business rule enforcement, input validation, error handling.
**Technologies:** Node.js, Express/Fastify, TypeScript, Zod, Prisma, REST conventions.
**Assign when:** Work involves server-side logic, API implementation, or anything between the frontend and the database.

---

## Storage

**Role:** Manages data persistence — database schemas, migrations, queries, and data integrity.

| Skill | Path | Description |
|-------|------|-------------|
| Writing Migrations | `database/writing-migrations/SKILL.md` | Schema changes, table creation, index management |
| Building Queries | `database/building-queries/SKILL.md` | Efficient reads and writes, query optimization |
| Managing Seeds | `database/managing-seeds/SKILL.md` | Test data, seed scripts, data fixtures |

**Key strengths:** Schema design implementation, query performance, data integrity constraints, migration safety.
**Technologies:** PostgreSQL, Prisma, SQL, database indexing, migration tooling.
**Assign when:** Work involves database schema changes, complex queries, or data management.

---

## Auth

**Role:** Handles authentication and authorization — login flows, token management, permissions, and security.

| Skill | Path | Description |
|-------|------|-------------|
| Implementing Auth Flows | `auth/implementing-auth-flows/SKILL.md` | Login, signup, password reset, OAuth |
| Managing Permissions | `auth/managing-permissions/SKILL.md` | Role-based access, resource-level authorization |
| Securing Endpoints | `auth/securing-endpoints/SKILL.md` | Token validation, middleware guards, CSRF protection |

**Key strengths:** Security-first thinking, token lifecycle management, permission modeling, vulnerability prevention.
**Technologies:** JWT, OAuth 2.0, bcrypt, session management, RBAC patterns.
**Assign when:** Work involves user identity, access control, or anything security-sensitive.

---

## Designer

**Role:** Defines visual systems — layouts, design tokens, responsive behavior, and interaction patterns.

| Skill | Path | Description |
|-------|------|-------------|
| Creating Layouts | `designer/creating-layouts/SKILL.md` | Page structure, grid systems, responsive breakpoints |
| Defining Design Tokens | `designer/defining-design-tokens/SKILL.md` | Colors, spacing, typography, shadows |
| Designing Interactions | `designer/designing-interactions/SKILL.md` | Animations, transitions, hover/focus states |

**Key strengths:** Visual consistency, responsive design, accessibility compliance, design system thinking.
**Technologies:** Figma tokens, Tailwind config, CSS custom properties, motion design.
**Assign when:** Work involves visual appearance, layout decisions, or design system updates.

---

## Shared Skills (Available to All Agents)

These skills are not owned by a single agent. Any agent can use them as part of their work.

| Skill | Path | Description |
|-------|------|-------------|
| Task Tracking | `shared/task-tracking/SKILL.md` | Read and update task status in tasks.md |
| Code Review | `shared/code-review/SKILL.md` | Review conventions, feedback format, approval criteria |
| Git Workflow | `shared/git-workflow/SKILL.md` | Branching, commits, pull request conventions |
| Testing | `shared/testing/SKILL.md` | Unit, integration, and end-to-end testing guidance |

---

## Quick Assignment Guide

| If the task involves... | Assign to |
|------------------------|-----------|
| System design, API contracts, data models | Architect |
| UI components, pages, client state | Frontend |
| API endpoints, business logic, middleware | Backend |
| Database schema, migrations, queries | Storage |
| Login, permissions, tokens, security | Auth |
| Layouts, design tokens, visual polish | Designer |
| Task breakdown, coordination, reviews | Agent Manager |
