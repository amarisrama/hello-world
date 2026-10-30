---
name: code-review
description: Pre-PR code review protocol. Use when the user asks to review changes, audit a branch, or check code quality before merging.
---

# Code Review Instructions

When this skill is triggered, execute the following workflow step-by-step:

## Step 1: Diff and Scope Analysis
- Inspect all modified files in the current workspace or branch diff.
- Verify whether any changes violate the rules specified in `AGENTS.md` (such as unauthorized package installs or missing TypeScript types).

## Step 2: Evaluation Matrix
Check the code against these three risk criteria:
1. **Security & Data Safety:** Look for exposed credentials, unescaped SQL queries, or missing input validation.
2. **Error Handling:** Ensure asynchronous operations contain proper `try/catch` wrappers.
3. **Performance:** Flag any nested loops or expensive rendering logic.

## Step 3: Structured Reporting
Format your feedback clearly using these priority tags:
- 🔴 **[Blocking]**: Critical bugs or security vulnerabilities that must be fixed immediately.
- 🟡 **[Important]**: Missing error boundaries or code style violations.
- 🟢 **[Nit]**: Minor naming improvements or optional cleanups.