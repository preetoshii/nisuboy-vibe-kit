# Nisuboy Vibe Kit

**A shared prompt library for turning ideas into reality.**

This repo is our version of a Google Drive folder — a place to store reusable prompts and principles we copy-paste when starting new projects. The goal: reduce the friction between having an idea and actually building it.

We're not engineers. We're two brothers who vibe-code our way through projects with AI assistance. These prompts help us go from messy voice recordings to implementation-ready specs without losing the nuances of what we actually want.

---

## What's in here

### `PRINCIPLES.md`
Our base development principles. These get referenced in the prompts and adapted per-project to keep builds focused and intentional.

### `prompts/`
A 4-step prompt flow for turning rough ideas into clear specs:

| Prompt | Purpose |
|--------|---------|
| **PROMPT-1-VISION** | Paste a voice transcript → get a clean vision doc |
| **PROMPT-2-REVISION** | Add notes → refine the spec (repeat as needed) |
| **PROMPT-3-QA** | AI asks you implementation questions one by one |
| **PROMPT-4-FINAL-SPEC** | Compile everything into an implementation-ready spec |
| **PROMPT-5-PROJECT-SETUP** | Set up AGENTS.md and workspace before building |

---

## How we use it

1. Record ourselves talking through an idea (messy, redundant, stream-of-consciousness — that's fine)
2. Transcribe it
3. Copy-paste **PROMPT 1** into Cursor with the transcript
4. Iterate with **PROMPT 2** if needed
5. Run through **PROMPT 3** Q&A to nail down implementation details
6. Use **PROMPT 4** to generate the final spec
7. Use **PROMPT 5** to set up AGENTS.md and workspace files
8. Start building

---

## Why GitHub?

It's just a convenient place to store text files that we both can access and update. Nothing fancy.
