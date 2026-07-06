# Prompt Engineering Training — Course Design Guide

> **This is our master guide.** All content builds from this document.
> Tool-agnostic. Pure prompt engineering. Patterns drawn from the Prompt Pattern Library (75 patterns).

## At a glance

- **15 modules**, each ~1 hour, grouped into a front-of-course **Introduction** plus three levels (Beginner, Intermediate, Advanced).
- Every module has a **Core** (taught live, ~4 items) and an **Appendix** (reference only, not covered live).
- **12 modules taught live** (~12 hours total across levels; no one takes all three at once). **Module 15 is pure reference.**
- The **Introduction (Modules 1–2)** is a prerequisite everyone completes before Beginner.
- **Advanced is mostly read-only**, per decision.
- All 75 library patterns are placed in a Core or Appendix — nothing orphaned. Academic/niche reasoning methods are consolidated into read-only Module 15.

## Front matter (framing modeled on the sample TOC — intro only, no patterns borrowed)

**Course Intro Slide / Overview** — not a module. The opening frame: why this training exists, the three-level ladder, how to use the appendices, what you'll be able to do at the end.

---

## INTRODUCTION — Foundations
*Taught before any technique. No patterns yet — just the mental model.*

### Module 1 — What Prompt Engineering Is & How Models Read Prompts
**Purpose:** build the mental model before any technique.
**Core:** What prompt engineering is · How an LLM interprets a prompt (prediction, tokens, context window — kept high-level) · Why the same prompt varies · The "brilliant new hire with zero context" mindset.
**Appendix:** tokenization detail · sampling/temperature · context-window limits.

### Module 2 — The Anatomy of a Prompt
**Purpose:** name the parts every good prompt is built from.
**Core:** Prompt anatomy / components · Setup layer (role + task) · Material layer (context + input data) · Output-shaping layer (format, constraints, tone).
**Appendix:** Define success criteria first · Instruction hierarchy (must/should/avoid).

---

## LEVEL 1 — BEGINNER
*The patterns used in almost every prompt.*

### Module 3 — Writing Clear Instructions
**Purpose:** get the model to do exactly what you ask.
**Core:** Be clear and direct · Specificity · Instruction hierarchy (must/should/avoid) · Constraints as design tools.
**Appendix:** Define success criteria first · Positive instruction (say what to do).

### Module 4 — Structure & Formatting
**Purpose:** stop instructions and data from blurring together.
**Core:** Delimiters and tags · Separate data from instructions · Output tagging · Visual hierarchy / section markers.
**Appendix:** Multi-document tagging · Reusable prompt blocks.

### Module 5 — Roles, Personas & Audience
**Purpose:** set the model's voice, expertise, and perspective.
**Core:** Give the model a role · Persona / keep in character · Audience transformation · Tone calibration with anchors.
**Appendix:** Standing-instruction layers.

### Module 6 — Examples (In-Context Learning)
**Purpose:** teach by showing, not telling.
**Core:** Zero-shot vs. few-shot · Designing effective examples · Contrastive examples (good vs. bad) · Quantity, selection & ordering.
**Appendix:** — (fully covered live).

### Module 7 — Controlling the Output
**Purpose:** get output in the exact shape you need.
**Core:** Output contract · Template / fill-in-the-blank · Format specification (list, table, structured) · Format seeding (prefill).
**Appendix:** Structured outputs / JSON schema.

---

## LEVEL 2 — INTERMEDIATE
*Reasoning, grounding, reliability.*

### Module 8 — Grounding & Working with Sources
**Purpose:** keep answers tied to provided facts, not invention.
**Core:** Source-grounded answering · Quote-first grounding · Give-the-model-an-out · Facts vs. assumptions.
**Appendix:** Long-context placement · Map-reduce summarization.

### Module 9 — Reasoning & Chain-of-Thought
**Purpose:** make the model work through multi-step problems.
**Core:** Why reasoning aloud improves accuracy · Chain-of-thought · Zero-shot CoT ("think step by step") · Trade-offs and when to avoid (reasoning-model awareness).
**Appendix:** Structured thinking tags · Rephrase-and-respond.

### Module 10 — Decomposition & Multi-Step Tasks
**Purpose:** break a big task into reliable stages.
**Core:** Least-to-most decomposition · Extract → transform → produce · Plan-and-solve · Step-back prompting.
**Appendix:** Self-ask · Generated knowledge · Skeleton-of-thought.

### Module 11 — Verification, Consistency & Self-Correction
**Purpose:** get the model to check its own work and produce stable results.
**Core:** Self-refine / reflection · Chain-of-verification · Rubric-as-instruction · Confidence calibration.
**Appendix:** Best-of-N · Self-consistency · Increase output consistency · Edge-case / fallback.

---

## LEVEL 3 — ADVANCED
*Power users; mostly read-only.*

### Module 12 — Prompt Composition & Reuse *(taught)*
**Purpose:** build reusable, modular prompt systems.
**Core:** Reusable prompt blocks · Templates & variables · Standing / system instructions · Prompt chaining.
**Appendix:** Refactoring monolithic prompts into components.

### Module 13 — Meta-Prompting & Optimization *(taught)*
**Purpose:** use the model to create and improve prompts.
**Core:** Meta-prompting / APE · Prompt improvement & rewriting · Prompt debugging · Model-specific prompting.
**Appendix:** Automatic prompt generation.

### Module 14 — Reliability, Safety & Anti-Patterns *(taught)*
**Purpose:** harden prompts and recognize what breaks them.
**Core:** Reduce hallucinations · Spotlighting / datamarking untrusted input · Injection & jailbreak resistance · The six anti-patterns (wall of text, buried instruction, vague adjectives, mixed data/instructions, overloading, misleading examples).
**Appendix:** Prompt-leak prevention · ReAct · Tool-use prompting.

### Module 15 — Advanced Reasoning *(read-only reference — not taught live)*
**Purpose:** a reference tour of research-grade reasoning methods for the curious.
**Reference:** Tree-of-thoughts · Graph-of-thoughts · Self-discover · Program-aided (think in code) · Analogical prompting · Maieutic prompting · Directional stimulus · Emotion prompting.

---

## Build plan (agreed)

1. **Lock a module template** — build the repeatable "teach a pattern" slide skeleton once.
2. **Per-module slide skeleton:** Title + purpose → "Why this matters" (real scenario) → each core pattern (what it is → before/after example → when to use) → one hands-on exercise → appendix slides (marked "reference, not covered").
3. **Build order (sequential):** Intro/overview + Modules 1–2 (Foundations) → Module 3 (locks the pattern template) → Modules 4–7 (Beginner) → Modules 8–11 (Intermediate) → Modules 12–14 (Advanced taught) → Module 15 (read-only, last).
4. **Delivery:** one deck per level (Beginner / Intermediate / Advanced) plus the shared Intro — not one giant file. For SharePoint.
5. **Verify each level** before moving on — every library pattern covered, examples correct, nothing orphaned.

## Delivery model (agreed)

- Cohort-based workshops, spaced ~1–2 weeks apart between levels (apply skills before advancing).
- Live/virtual-live preferred over recorded — prompting is learned by doing.
- Pattern Pattern Library ships as the leave-behind reference alongside every course.
