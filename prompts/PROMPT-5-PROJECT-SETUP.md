# PROMPT 5: Project Setup

Before we start on the first implementation milestone, let's set up the project workspace for smooth AI-assisted development.

Using our final spec (particularly the Development Principles section), create the following files:

---

## 1. AGENTS.md (root directory)

This is the **single source of truth** for how AI agents should work on this project.

### Critical formatting guidance:

**Keep it concise — aim for under 150 lines total.** AI agents process this file on every interaction, so brevity matters for efficiency.

**EXCEPTION: Development Principles should be included IN FULL.** These are too important to summarize — the nuance and examples are what make them actionable. This is the one section where length is justified.

**Everything else: brief, actionable, no fluff.** Use bullet points. Use code blocks for commands. Cut anything that isn't directly useful.

### Required sections:

**Development Principles** (FULL — do not summarize)
- Include the complete development principles from the spec
- Keep the examples and the "DO/DON'T/ASK" format — these are what make them actionable
- Any project-specific additions or modifications

**Project Overview** (2-4 sentences max)
- What we're building
- Why it exists

**Tech Stack** (bullet list)
- Languages and frameworks
- Key dependencies
- One-line "why" for non-obvious choices

**Project Structure** (bullet list)
- Key directories and their purpose
- Only include what's helpful, not every folder

**Commands** (code blocks)
```bash
npm install     # install dependencies
npm run dev     # start dev server
npm run build   # production build
npm test        # run tests
```

**Code Conventions** (bullet list)
- Naming conventions
- File organization patterns
- Linting/formatting tools

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

**Single source of truth.** By putting everything in AGENTS.md and having .cursorrules and CLAUDE.md point to it, we:

- Avoid maintaining duplicate guidance across files
- Stay compatible with multiple AI tools (Cursor, Claude Code, and future tools)
- Keep everything in one place that's easy to update

---

Once these files are in place, we're ready to start building.
