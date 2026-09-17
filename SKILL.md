---
name: grill-prd
description: >
  Interview the user relentlessly about a product idea, memo, or PRD until reaching
  shared understanding, resolving each branch of the product decision tree before
  writing anything. Use when the user wants to write a PRD, one-pager, launch memo,
  strategy doc, or wants to avoid vague AI-generated product writing.
  Keywords: grill, PRD, spec, one-pager, product decision, trade-offs, launch memo.
---

# Grill PRD

Interview me relentlessly about every aspect of this product until we reach a shared
understanding across all the areas below. Walk down each branch of the product
decision tree, resolving dependencies one-by-one.

## Rules

- Ask multiple related questions per round (3–5 at a time), grouped by the themes
  below, so I can answer them all in a single reply. Do NOT ask one question at a
  time — batch them by theme.
- For each question, provide your recommended answer. I will agree, refine, or skip.
- If I reply "skip" or "not sure" to a question, mark it as an open question and
  move on. Do not re-ask it.
- If existing docs, briefs, experiment results, or context in this conversation can
  answer a question, use that — don't ask me again.
- Challenge fuzzy language immediately:
  - "users" → which users? what segment?
  - "feature" → what outcome does it enable?
  - "improve" → improve what metric, by how much?
  - "soon" → what's the actual target date?
- After all themes are covered (or skipped), output a structured summary of
  resolved decisions and a clearly labeled list of open questions.
- Only draft the PRD, memo, or document after I explicitly say I'm ready.

## Grilling Themes (cover in this order)

### 1. Problem & Context
- What is the user pain or business problem being solved?
- Why is this worth solving now — what changed?
- Who specifically has this problem (user segment, role, company size)?
- What evidence exists that this is real (research, data, support volume)?

### 2. Goal & Success
- What is the desired outcome for the user?
- What is the desired outcome for the business?
- How will success be measured (primary metric, guardrail metrics)?
- What does "good enough" look like at launch vs. long-term?

### 3. Scope & Non-Goals
- What is explicitly in scope for V1?
- What is explicitly out of scope or deferred?
- What are the non-goals (things we will not try to do with this)?
- Are there adjacent problems we are intentionally ignoring?

### 4. Users & Edge Cases
- Who is the primary user? Who is excluded?
- What does the happy path look like end to end?
- What are the key edge cases or failure modes?
- Are there accessibility, localization, or compliance constraints?

### 5. Alternatives & Trade-offs
- What alternative solutions were considered?
- Why were they rejected?
- What key trade-offs did we make in choosing this approach?
- Is there a simpler version that solves 80% of the problem?

### 6. Dependencies & Constraints
- What teams, systems, or APIs does this depend on?
- Are there technical constraints (platform, performance, data)?
- Are there legal, privacy, or policy constraints?
- What is the realistic timeline and what drives it?

### 7. Risks & Open Questions
- What assumptions are we making that could be wrong?
- What could cause this to fail?
- What do we need to learn before or during development?
- What would trigger us to stop or pivot?

### 8. Rollout & Measurement
- How will this ship (flag, phased rollout, full launch)?
- How will it be announced or communicated?
- How will we know if it is working post-launch?
- What is the rollback plan if something goes wrong?

## Output Format

When I say I'm ready, produce TWO documents — always both, always in this order:

### Document 1: The TL;DR (required, always first)

A single page. No headers beyond the title. No bullet forests. No "this document describes."
Written in plain English, like a sharp memo from a PM who thought hard and reached conviction.

Structure (prose paragraphs, not bullets):
- The problem — one paragraph on what's broken and why it matters now
- What we're building — one paragraph on the solution and the core bet we're making
- The key decisions — the 3–5 hardest calls we made and why (trade-offs explicit, not implied)
- What success looks like — the number(s) we're betting on, and the guardrail we won't cross
- What could go wrong — the one or two things that could kill this, honestly stated

No filler. No passive voice. No "we will look to explore." If something is uncertain, say it is uncertain. If a trade-off was painful, say it was painful. A reader should finish this in under 3 minutes and know exactly what was decided and why.

### Document 2: The Full PRD

Standard structured spec covering all resolved themes. Open questions clearly marked.
This is the detailed reference — the TL;DR above is what people will actually read.
