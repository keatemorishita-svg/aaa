# 🧬 AAA Refinement SOP

> The methodology that built AAA — now available as a standalone tool.

---

## What this is

A six-round adversarial refinement process for stress-testing any conceptual framework before you publish it.

This is the same methodology used to build AAA itself. It is the first application running on the AAA kernel.

---

## Who this is for

- **Framework builders** — before you publish, run your framework through all six rounds
- **Researchers** — replace (or supplement) peer review with structured AI adversarial testing
- **Teams designing architecture/governance** — use the rounds as a design review checklist
- **AI-native workers** — a demonstration of how to collaborate with AI on complex conceptual work

---

## What you need

- A concept, framework, or system design (anything from a one-pager to a book)
- An AI collaborator (Claude, ChatGPT, etc.)
- 1–3 hours per round (rounds can be split across sessions)

---

## The Six Rounds

| Round | Name | Core Question | Output |
|---|---|---|---|
| 1 | Ontological Positioning | What is this, and where does it sit in the knowledge landscape? | One-sentence definition + knowledge map |
| 2 | Proposition Strength Analysis | Which claims are strong (defensible) and which are weak? | Claim inventory with strength ratings |
| 3 | Weak Point Attack | What's the most fragile part — and how would you kill it? | Vulnerability list + lethality scores |
| 4 | Dimension-Switch Attack | What new problems appear when you change perspective? | Blind spot map across dimensions |
| 5 | Value Identification | Who is this for, and what can they actually do with it? | User profiles + actionable tools |
| 6 | Operationalization | How do abstract concepts become checklists, templates, tools? | Diagnostic instruments + templates |

---

## Why six rounds?

One round → you find the obvious problems.
Two rounds → you find the less obvious ones.
Three rounds → you start questioning your assumptions.
Four rounds → you see what you're blind to.
Five rounds → you realize it has no user.
Six rounds → it becomes a tool, not just a theory.

Most frameworks stop after round 0 (publish raw intuition). The difference between a good idea and a resilient system is roughly four rounds of adversarial refinement.

---

## How to use

### Quick mode (one session)
Copy the prompt templates. Feed them to your AI collaborator in sequence. Expect 2–3 hours.

### Deep mode (multi-session)
One round per session. Let the findings from each round settle before starting the next. Expect 1–2 weeks.

### Team mode
Each team member runs rounds independently. Compare findings. Where they converge → probably right. Where they diverge → investigate.

---

## What this SOP produces

Not just a better framework. It produces:
- A **defense map** — you know exactly where your framework is weak
- A **user manual** — you know exactly who it's for and what they should do with it
- A **fork guide** — others know exactly where to modify and where to preserve
- A **method trace** — anyone can see how you arrived at your conclusions

---

## Relationship to AAA

This SOP is an instance of the AAA Evolution Loop applied to conceptual work:

```
Fork (diverge from existing ideas)
  → Experiment (run a round of adversarial testing)
    → Selection (keep what survives attack)
      → Merge (integrate survivors into the framework)
        → Repeat (next round)
```

It is also the reason AAA is not empty — every concept in this repository has passed through multiple rounds of this process before being committed.

---

## Get started

→ [Refinement Loop (full process)](./refinement-loop.md)
→ [Prompt Templates (copy-paste ready)](./prompt-templates.md)
