# PROMPT 5: Project Setup

Before we start on the first implementation milestone, let's set up the project workspace for smooth AI-assisted development.

Using our final spec (particularly the Development Principles section), create the following files:

## 1. AGENTS.md

This is the single source of truth for how AI agents should work on this project. It should include:

- The development principles we established for this project (from the spec)
- Any project-specific guidance, conventions, or constraints worth knowing
- Key context an AI would need to make good decisions

Keep it focused and useful — not a wall of text, but enough that an AI dropping into this project understands how to operate.

## 2. .cursorrules

This file should simply point to AGENTS.md:

```
Read AGENTS.md for all project guidelines and principles.
```

## 3. CLAUDE.md

Same as above — point to AGENTS.md:

```
Read AGENTS.md for all project guidelines and principles.
```

---

The goal is one source of truth (AGENTS.md) that both Cursor and Claude Code respect, so we're not maintaining duplicate guidance across files.

Once these are in place, we're ready to start building.

