# Project Guidelines for AI Agents

## 1. Overview
This repository contains a full-stack task management application built for internal operations.

## 2. Tech Stack & Tools
- **Frontend:** Next.js (App Router), TypeScript, Tailwind CSS
- **Backend/DB:** Node.js, Prisma ORM, PostgreSQL
- **Commands:**
  - Install: `npm install`
  - Run tests: `npm test`
  - Type check: `npm run typecheck`

## 3. Directory Structure
- `src/app/`: Next.js pages and API route handlers
- `src/components/`: Reusable UI elements
- `src/server/`: Prisma database clients and server actions

## 4. Core Constraints
- Never introduce a new external production dependency without explicit confirmation.
- Always write explicit TypeScript types (avoid using `any`).
- Always run `npm run typecheck` mentally or via terminal tools before declaring code changes complete.