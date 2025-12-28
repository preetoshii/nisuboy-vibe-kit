# PROMPT 4: Launchpad Spec

Now take the resolved Q&A and integrate it into our existing vision spec to produce the **Launchpad Spec**.

The Launchpad Spec plans to **first life** — the point where the thing is alive, working end-to-end, tangible, usable. Not polished, not complete, but *breathing*. We're not planning the whole journey here. Once it's alive, further direction emerges from actually building and using it.

Don't fundamentally restructure what we already have unless we really need to — build on top of it. Add new sections where needed, adjust content as needed, deepen existing sections with technical detail where relevant, and weave in the decisions we made.

**Ideas for sections or information to include:**
- Tech stack and key dependencies (only as deep as needed for first life)
- System architecture / how components relate (for the foundation)
- Data flow / how data moves through the system (for core functionality)
- Interfaces / APIs (if relevant to first life)
- Launchpad Milestones (see note below)
- Anything else necessary to reach first life — without over-specifying to the point where it discourages intelligent judgment on implementation.

**Regarding Launchpad Milestones:**

The goal is **first life** — the point where the core idea works end-to-end and you can actually use the thing. Not an arbitrary number of milestones, but however many it takes to reach that point.

Outcome-oriented milestones, humanly worded — not "build the database layer" but "Characters can speak to each other" or "We can preview a scene in the browser."

Each milestone should be a vertical slice — a small but complete, testable thing. We want to grow a cupcake into a cake, not build incomplete layers of a grand cake we can't taste until the end.

**Don't plan beyond first life.** Once it's alive, you'll know things you can't know now. Further direction emerges from building, not from this spec.

**Regarding the right level of detail on technical details** (whether tech stack, data flow, etc):

There's a spectrum:
1. **Too vague:** "Make it work well" — no real guidance
2. **Directional:** "Use a web framework. Consider FFmpeg for video composition." — points a direction but not good enough
3. **Clearly and Strategically Guided:** "We'll use FFmpeg for composition and Web Audio API for acoustics, as the system needs instant preview and video export." — clear decisions, explains the why
4. **Over-specified:** "Create /src/components/VideoPlayer/index.tsx with a useVideoPlayer hook that returns..." — prescribes implementation details

**The sweet spot is level 3.** Make real decisions, name specific technologies, explain the reasoning — but don't prescribe folder structures, file names, or actual code. Leave room for intelligent judgment during execution instead of trying to pre-code everything.

Don't fill in details we didn't discuss — if we didn't decide it, don't invent it. The developer or AI agent is better positioned to navigate those choices in context.

---

**At the end of the spec, include a brief note** reminding future readers (human or AI) that this is a Launchpad Spec — it plans to first life, not the whole journey. Once the thing is alive, further direction emerges from building. The spec will become a historical document, and that's exactly what it should be.

