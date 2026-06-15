# SOP — 6-Round Adversarial Refinement

> Stress-test any conceptual framework before you publish it.
> Copy the prompt. Paste into Claude. Run 6 rounds. Your framework survives or it dies. Either way, you win.

---

## Quick Start (30 seconds)

```
COPY THIS ENTIRE PROMPT INTO A CONVERSATION WITH CLAUDE OR ANY CAPABLE AI:

---

I'm working on a concept/framework/system called [NAME]. Here's a brief description:

[2-3 SENTENCES]

I want you to run a structured adversarial refinement process. But first — ask questions.

ROUND 0 — EXHAUSTIVE CLARIFICATION (2 rounds minimum):
Before refining anything, ask me 4-5 questions about [NAME] to clarify what I actually need. Cover: form, audience, constraints, success criteria, relationship to existing work, evolution mechanism, boundaries. After I answer, ask 3-5 MORE questions — the non-obvious ones. Keep going until you have no more questions. Then say "Entering Round 1."

ROUND 1 — ONTOLOGICAL POSITIONING:
1. Define [NAME] in one sentence (max 30 words). Strip all adjectives.
2. Where does it sit in the knowledge landscape? Name one concept above and one below.
3. What existing concept is closest to [NAME]? What's the key difference?
4. What does [NAME] say that no one has said before? Be honest.

ROUND 2 — PROPOSITION STRENGTH ANALYSIS:
1. Extract every proposition [NAME] makes. Rate each: STRONG / MODERATE / WEAK / UNDEFENDED.
2. Which propositions, if disproven, would collapse the entire framework?
3. For each WEAK or UNDEFENDED claim: recommend strengthening, narrowing, or flagging as speculative.

ROUND 3 — WEAK POINT ATTACK:
1. Role-play the most hostile, intelligent critic. Attack the weakest points from Round 2.
2. For each attack, rate: LETHALITY / DEFENSIBILITY / PATCHABILITY (HIGH/MEDIUM/LOW).
3. What's the kill shot — the one argument that could end [NAME]?

ROUND 4 — DIMENSION-SWITCH ATTACK:
Examine [NAME] from these perspectives:
- Power: Who gains/loses power?
- Economics: What are the incentives?
- Governance: How are decisions made?
- Scale: What breaks at 10x? 100x?
- Failure Modes: How does it fail?
- Adversarial Use: How could a bad actor exploit it?
- Cultural Dependence: Does it only work in one cultural context?
- Time: What happens in 1, 5, 10, 50 years?

ROUND 5 — VALUE IDENTIFICATION:
1. Who is [NAME] actually for? Be specific (not "everyone").
2. For each user: what can they DO differently after understanding [NAME]?
3. What's the minimum viable understanding — the smallest subset that still provides value?
4. Can someone use [NAME] without the author present?

ROUND 6 — OPERATIONALIZATION:
Take the strongest concepts from [NAME] and turn each into a tool someone can use without you:
- A diagnostic checklist
- A decision template
- A measurement instrument
- A fork guide (where to modify this for different domains)

After all rounds, summarize:
- What survives?
- What needs to change?
- Should [NAME] be published, revised, narrowed, or killed?
```

---

## What you get

After running all 7 rounds (Round 0 + 6 rounds):

- A **defense map** — you know exactly where your framework is weak
- A **user manual** — you know exactly who it's for and what they should do
- A **fork guide** — others know where to modify and where to preserve
- A **method trace** — anyone can see how you arrived at your conclusions
- A **kill/no-kill decision** — publish, revise, narrow, or kill

---

## Example: AAA's own SOP output

This is what AAA itself produced when run through the same SOP:

| Round | Finding |
|---|---|
| 0 | 5 questions clarified form, audience, brand, experience, evolution |
| 1 | AAA = minimal generative grammar for open systems |
| 2 | 19 propositions: 3 strong, 5 weak, 3 hidden claims |
| 3 | Kill shot: "So What?" — no documented case study |
| 4 | 8 dimension blind spots; missing immune system is critical |
| 5 | 4 user profiles; SOP + 3-primitive diagnostic most valuable |
| 6 | 4 standalone tools; 14 applications onboarded |

→ [Full SOP output](https://github.com/aaa-mvc/aaa/tree/main/sop)

---

## Tips

- **Model choice**: Rounds 3-4 benefit from the most capable model. Rounds 0-2 work with any capable model.
- **Multi-model**: Run the same round with different models. Convergence = high confidence. Divergence = genuinely hard question.
- **Iterate**: You can loop back. Round 5 reveals no user → back to Round 1.
- **Save everything**: The trace of your thinking is itself valuable — it's your method trace for future contributors.
- **Killing is winning**: If Round 3 finds a fatal flaw, killing the framework saved you from public embarrassment. That's success.

---

## Relationship to AAA

This SOP is built with the [AAA](https://github.com/aaa-mvc/aaa) refinement methodology. It is both part of the AAA ecosystem and a fully independent tool — you do not need to understand AAA to use it.

AAA is a Minimum Viable Civilization. This SOP is one of its working applications.

---

*Copy. Paste. Refine. Fork.*
