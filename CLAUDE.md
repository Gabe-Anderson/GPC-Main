# CLAUDE.md — Graph Paper Capital (GPC-Main)

This file provides context and guidance for AI assistants (Claude and others) working in this repository.

---

## Repository Overview

**GPC-Main** is the main monorepo for Graph Paper Capital builds. It is in early-stage development; as of the initial commit, only a README exists. This document will grow alongside the project.

- **Organization**: Graph Paper Capital
- **Remote**: Proxied git server (local proxy at `127.0.0.1:44623`)
- **Primary author**: Gabe Anderson (`gkandersoninc@gmail.com`)

---

## Current Repository State

```
GPC-Main/
├── CLAUDE.md       ← this file
└── README.md       ← one-line project description
```

No source code, packages, or infrastructure files exist yet. The tech stack and architecture are to be determined as the project evolves.

---

## Git Workflow

### Branch Naming

- Feature branches: `feature/<short-description>`
- Bug fixes: `fix/<short-description>`
- Claude-driven branches: `claude/<task-description>-<session-id>`
- Never commit directly to `main` or `master`

### Commit Convention

Use short, imperative commit messages:

```
Add user authentication module
Fix null pointer in payment flow
Update CLAUDE.md with API conventions
```

- One concern per commit — keep commits small and focused
- Prepend with a scope if useful: `docs:`, `feat:`, `fix:`, `chore:`, `refactor:`

### Push Workflow

Always push with upstream tracking:

```bash
git push -u origin <branch-name>
```

For Claude-driven branches, the branch name must start with `claude/` and end with the matching session ID.

---

## Development Principles

These conventions should be applied consistently once code is written:

### General

- Prefer clarity over cleverness — code is read more than written
- Keep functions small and single-purpose
- Avoid premature abstractions — three similar lines of code is better than a poorly timed helper
- Do not add error handling for scenarios that cannot happen; only validate at system boundaries (user input, external APIs)
- Do not add docstrings, comments, or type annotations to code that wasn't changed

### Security

- Never commit secrets, tokens, or credentials — use environment variables
- Validate all user-supplied input at boundaries
- Avoid shell injection, SQL injection, XSS, and other OWASP Top 10 vulnerabilities

### File Hygiene

- Do not create files unless they are strictly necessary
- Prefer editing existing files over creating new ones
- Remove dead code rather than commenting it out

---

## For AI Assistants

### What to do

- Read files before editing them — never modify code you haven't seen
- Understand the existing pattern before introducing a new one
- Keep changes minimal and scoped to what was requested
- Commit and push only to the designated branch (see task instructions for branch name)
- Ask before taking irreversible actions (deleting files, force pushing, dropping data)

### What not to do

- Do not refactor, rename, or "clean up" code beyond what was requested
- Do not add features, abstractions, or extra configurability unless explicitly asked
- Do not push to `main` or `master` without explicit permission
- Do not guess at URLs — only use URLs provided by the user or confirmed in source files
- Do not use `--no-verify` to bypass git hooks

### Searching the codebase

- Use `Glob` to find files by name/pattern
- Use `Grep` to search file contents
- Use `Read` to inspect individual files
- Reserve `Bash` for shell operations that have no dedicated tool equivalent

---

## Adding to This File

As the project grows, keep CLAUDE.md up to date with:

- New top-level directories and their purposes
- Tech stack decisions (language, framework, database, etc.)
- Environment variable requirements
- Build, test, and lint commands
- API conventions (REST vs GraphQL, auth method, versioning)
- Deployment pipeline and environments
- Any project-specific gotchas or constraints
