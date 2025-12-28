# PROMPT 5: Project Setup

Before we start on the first implementation milestone, let's set up the project workspace for smooth AI-assisted development.

Using our final spec (particularly the Development Principles section), create the following files:

---

## 1. AGENTS.md (root directory)

This is the **single source of truth** for how AI agents should work on this project. Following best practices from the emerging AGENTS.md standard (see github.com/openai/agents.md), it should include:

### Required sections:

**Development Principles**
- The development principles we established for this project (from the spec)
- Any project-specific values or orientations worth emphasizing

**Project Overview**
- Brief description of what we're building and why
- Key features or goals

**Tech Stack**
- Languages, frameworks, and key dependencies
- Why these choices were made (brief context)

**Project Structure**
- High-level overview of how the codebase is organized
- Purpose of key directories

**Development Commands**
- How to install dependencies
- How to run the dev server
- How to build for production
- How to run tests

**Code Style & Conventions**
- Naming conventions
- File organization patterns
- Any linters/formatters in use

**Testing Guidelines**
- Testing framework
- How to run tests
- What should be tested

### Best practices to follow:

- **Be specific**: Use exact commands, not vague descriptions
- **Use code blocks**: Wrap all commands in backticks
- **Explain the why**: Brief context helps agents make better decisions
- **Keep it focused**: This isn't a novel — include what's useful, skip what's not

---

## 2. .cursorrules (root directory)

Keep this minimal — just point to AGENTS.md:

```
Read AGENTS.md for all project guidelines, principles, and conventions.
```

---

## 3. CLAUDE.md (root directory)

Same approach — point to AGENTS.md:

```
Read AGENTS.md for all project guidelines, principles, and conventions.
```

---

## Why this structure?

**Single source of truth.** AGENTS.md is becoming the standard file that AI coding tools look for. By putting everything there and having .cursorrules and CLAUDE.md point to it, we:

- Avoid maintaining duplicate guidance across files
- Stay compatible with multiple AI tools (Cursor, Claude Code, and future tools)
- Keep everything in one place that's easy to update

---

## Note on monorepos

If the project grows into a monorepo with multiple packages/apps, you can add additional AGENTS.md files in subdirectories with context specific to that part of the codebase. AI agents will use the closest AGENTS.md to the code they're working on.

---

Once these files are in place, we're ready to start building.
