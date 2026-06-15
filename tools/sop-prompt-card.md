# Tool: SOP Prompt Card

> One prompt. Six rounds. Copy, paste, refine any framework.

---

## How to use

1. Copy the prompt below
2. Paste into any conversation with Claude, ChatGPT, or any capable AI
3. Replace `[NAME]` and `[2-3 SENTENCE DESCRIPTION]`
4. The AI will execute all six rounds sequentially

---

## The Prompt

```
I'm working on a concept/framework/system called [NAME]. Here's a brief description:

[2-3 SENTENCES]

I want you to run a structured adversarial refinement process. But first — ask questions.

ROUND 0 — EXHAUSTIVE CLARIFICATION (2 rounds minimum):
Before refining anything, ask me 4-5 questions about [NAME] to clarify what I actually need. Cover: form, audience, constraints, success criteria, relationship to existing work, evolution mechanism, boundaries. After I answer, ask 3-5 MORE questions — the non-obvious ones. Keep going until you have no more questions. Then say "Entering Round 1."

ROUND 1 — ONTOLOGICAL POSITIONING:
1. Define [NAME] in one sentence (max 30 words). Strip all adjectives.
2. Where does it sit in the knowledge landscape? Name one concept above (more abstract) and one below (more concrete).
3. What existing concept is closest to [NAME]? What's the key difference?
4. What does [NAME] say that no one has said before? Be honest — if the answer is "nothing new," say so.

ROUND 2 — PROPOSITION STRENGTH ANALYSIS:
1. Extract every proposition [NAME] makes. Rate each: STRONG / MODERATE / WEAK / UNDEFENDED.
2. Which propositions, if disproven, would collapse the entire framework?
3. For each WEAK or UNDEFENDED claim: recommend strengthening, narrowing, or flagging as speculative.

ROUND 3 — WEAK POINT ATTACK:
1. Role-play the most hostile, intelligent critic. Attack the weakest points from Round 2.
2. For each attack, rate: LETHALITY (HIGH/MEDIUM/LOW), DEFENSIBILITY (HIGH/MEDIUM/LOW), PATCHABILITY (HIGH/MEDIUM/LOW).
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

After all six rounds, summarize:
- What survives?
- What needs to change?
- Should [NAME] be published, revised, narrowed, or killed?
```

---

## Tips

- **Model**: Rounds 3-4 benefit from the most capable model available
- **Multi-model**: Run the same round with different models. Where they converge → high confidence.
- **Iterate**: You can loop back. If Round 5 reveals no user, go back to Round 1.
- **Save**: Keep each round's output. The trace of how your thinking evolved is itself valuable.

---

*This prompt card is part of AAA but is designed to be used independently.*
