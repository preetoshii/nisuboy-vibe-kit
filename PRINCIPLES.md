# Nisuboy Principles

## 0. The spec is a launchpad, not a contract

Starting is the hardest part. Specs exist to reduce that friction — to get from idea to **first life**: the point where the thing is alive, working end-to-end, usable. Not polished, not complete, but *breathing*.

Specs plan to first life, not the whole journey. Once it's alive, further direction emerges from building — informed by actually using the thing, not by planning in a vacuum. Building reveals what planning cannot: better paths emerge, instincts develop, understanding deepens.

The best projects evolve beyond their original specs. Deviation isn't failure; it's discovery. A spec should become a historical document — a record of where things began, not a rulebook for where they must go.

- DO: Change direction mid-build when something better emerges
- DON'T: Follow the spec when it no longer serves what's actually being built
- DO: Let the project evolve into something the spec didn't predict
- DON'T: Treat specs as promises that need to be kept
- ASK: "Does this serve what's actually being built, or just what was written down?"

---

## 1. Every piece justifies its existence toward the goal

Everything you build must earn its place by directly serving what you're trying to accomplish. This isn't about thinking small—you can be wildly ambitious. It's about not building extra. If you're making a feature, you build exactly what that feature needs to work, not bonus stuff that seems cool but isn't required. Before something gets built, it should be able to answer: "Why do I need to exist for this to succeed?" If it can't answer that, it doesn't get built. Ambition is welcome. Waste is not.

- DO: A utility function that's actually used in multiple places
- DON'T: An abstraction layer "in case we switch databases" with no actual plan to
- DO: Build the three screens the feature requires
- DON'T: Also build an admin panel "while we're at it"
- ASK: "If I delete this, does the goal still get met?" If yes, delete it.

---

## 2. Flexibility goes in chosen spots, not everywhere

Some things will change later—you know this. So you pick specific places where you leave room for that change, and you name why. Maybe it's a feature you know will evolve, or a part of the system you're not confident about yet. Those spots get flexibility. Everything else stays simple and direct. You're not trying to prepare for every possible future—that creates bloat and confusion. You're preparing for the futures you actually care about and can reasonably see coming. A few clear doors left open beats a hundred vague ones.

- DO: Make the AI provider swappable if you know you might switch from OpenAI to Anthropic
- DON'T: Make every string a configurable constant
- DO: Leave a clear seam where you've written "// TODO: this will need to support X"
- DON'T: Create interfaces for every class "just in case"
- ASK: "Can I name the specific future change this flexibility serves?" If not, hardcode it.

---

## 3. Grow by deepening, not by multiplying

When you add new capability, first ask: can this use something that already exists? Can it collapse into an existing structure or make that structure smarter? New moving parts should only appear when they actually reduce overall complexity—not just shift it around. The goal is to get more powerful without getting more complicated. Every new system you add is another thing that can break, another thing to understand, another thing to maintain. So you fight hard to keep the number of moving parts low, but you don't artificially collapse by following this as a dogma.

- DO: Add a parameter to an existing function to handle the new case
- DON'T: Copy the function and modify the copy
- DO: Extend a component to handle one more variant
- DON'T: Create a parallel component that's 80% identical
- ASK: "Am I adding to something that exists, or creating something parallel?" Prefer the former.

---

## 4. Every part knows the whole it belongs to

You're not building a pile of features—you're building a harmonious machine. Each piece, even when worked on separately, should feel like it belongs to the same system. This means understanding how your piece connects to what's around it: what it receives, what it passes on, what it assumes about the rest. When you add something, you're not just asking "does this work?"—you're asking "does this fit?" An elegant system isn't one where every part is individually clever. It's one where the parts feel like they were made for each other. Build with the whole in view, even when you're zoomed in on a detail.

- DO: Know where your data comes from and what expects it downstream
- DON'T: Build something that works alone but breaks when connected
- DO: Go through the layer that owns something, not around it
- DON'T: Reach across the system because it's convenient
- ASK: "What else does this touch, and what breaks if this changes?" You should know.

