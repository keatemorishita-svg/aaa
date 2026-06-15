# Prompt Templates — Copy, Paste, Refine

> Each template is designed to be copied directly into a conversation with an AI collaborator.
> Replace `[TOPIC]` with your concept/framework/system name.
> Replace `[DESCRIPTION]` with a brief (1–3 sentence) description of what you're working on.

---

## Round 0: Exhaustive Clarification (2 Rounds Minimum)

```
I'm considering working on [TOPIC]. Before we start any refinement, I want you to ask me the hard questions first.

ROUND 0.1 — Ask me 4-5 questions that will clarify what I actually need. Cover: form, audience, constraints, success criteria, relationship to existing work, evolution mechanism, boundaries.

ROUND 0.2 — After I answer, ask me 3-5 MORE questions. These should be the NON-obvious ones — the things I haven't thought about, the tensions I'm avoiding, the assumptions I'm making without knowing it.

Keep asking rounds of questions until you genuinely have no more questions. Then say "Entering Round 1" and begin the refinement process.

Do NOT start refining yet. Just ask questions.
```

---

## Round 1: Ontological Positioning

```
I'm working on a concept called [TOPIC]. Here's a brief description:

[DESCRIPTION]

Please perform an ontological positioning analysis:

1. **One-sentence definition**: Define what [TOPIC] is in one sentence. Strip all adjectives and metaphors. Maximum 30 words.

2. **Knowledge spectrum**: Where does [TOPIC] sit in the knowledge landscape? Identify one layer above (more abstract/philosophical) and one layer below (more concrete/applied).

3. **Closest known concept**: What existing concept is most similar to [TOPIC]? What is the key difference — the one thing [TOPIC] contributes that the existing concept doesn't?

4. **Non-obviousness test**: What does [TOPIC] say that no one has said before? If the answer is "nothing" or sounds obvious, say so honestly.

Be adversarial. If my concept is vague, say it's vague. If it's not new, say what it's duplicating.
```

---

## Round 2: Proposition Strength Analysis

```
Using the definition of [TOPIC] from Round 1, please perform a proposition strength analysis:

1. **Extract every proposition**. A proposition is a sentence that asserts something true about the world. Include implicit propositions — claims the framework depends on but doesn't state explicitly.

2. **Rate each proposition**:
   - STRONG: Multiple independent lines of evidence; survives obvious counterexamples
   - MODERATE: Plausible and consistent with evidence, but not definitively proven
   - WEAK: Speculative, relies on analogy, or not yet tested
   - UNDEFENDED: Assumed without argument

3. **For each WEAK or UNDEFENDED proposition**: recommend whether to strengthen (with what evidence), qualify (narrow the claim), or flag as speculative.

4. **Identify the load-bearing propositions** — which claims, if disproven, would cause the whole framework to collapse?

5. **Honesty check**: Are there any claims rated STRONG that, on reflection, should be downgraded?
```

---

## Round 3: Weak Point Targeted Attack

```
Now I want you to attack [TOPIC]. Be the most hostile, intelligent critic you can be.

Using the WEAK and UNDEFENDED propositions from Round 2:

1. **For each weak point**, construct the strongest possible attack. Don't pull punches. If an attack would kill the framework, say so.

2. **Rate each attack**:
   - LETHALITY: If this attack succeeds, does the framework collapse (HIGH), get significantly weakened (MEDIUM), or just get scratched (LOW)?
   - DEFENSIBILITY: Can the framework deflect this attack with existing evidence/logic (HIGH/MEDIUM/LOW)?
   - PATCHABILITY: If the attack succeeds, can the framework be modified to survive (HIGH/MEDIUM/LOW)?

3. **Prioritize**: LETHAL + LOW DEFENSIBILITY > LETHAL + HIGH DEFENSIBILITY > NON-LETHAL

4. **The kill shot**: If you had to kill [TOPIC] with one argument, what would it be? And is that argument actually correct?

5. **Honest assessment**: After this round, should [TOPIC] be published, revised, narrowed, or killed?
```

---

## Round 4: Dimension-Switch Attack

```
Examine [TOPIC] from perspectives it wasn't designed for. For each dimension below, ask: "What problems become visible from this angle that were invisible before?"

Dimensions to examine:

1. **POWER**: Who gains power if this framework is adopted? Who loses it? What power dynamics does it assume or ignore?

2. **ECONOMICS**: What are the incentives? Who pays, who benefits? What happens when money is involved?

3. **GOVERNANCE**: How are decisions made? Who has veto power? What happens during a dispute?

4. **SCALE**: Does this work at 10x the current scale? 100x? 1000x? What breaks first?

5. **FAILURE MODES**: How does this fail? What does "broken" look like? How would you know it's not working?

6. **ADVERSARIAL USE**: How could a bad actor exploit this framework? What's the worst thing someone could justify using it?

7. **CULTURAL DEPENDENCE**: Does this only work in one cultural context? What assumptions about people/society does it embed?

8. **TIME**: What happens after 1 year? 10 years? 100 years? Does the framework become more or less useful over time?

For each dimension, document the blind spot without immediately trying to fix it. Understanding what you don't see is valuable.
```

---

## Round 5: Value Identification

```
Now identify who [TOPIC] is actually for and what they can actually do with it.

1. **User profiles**: List the specific types of people who would benefit from [TOPIC]. Not "everyone" or "organizations" — be specific. "A CTO of a 50–200 person company who feels their engineering culture is stagnating" is a profile. "Leaders" is not.

2. **For each profile**, answer:
   - What can they DO differently after understanding [TOPIC]?
   - What decision does [TOPIC] change?
   - What is the concrete output (a document? a decision? a design? a diagnosis?)?

3. **Value test**: "If someone reads the full framework and does nothing differently, did it fail?" If yes — what's the minimum someone needs to understand to get value?

4. **Minimum viable understanding**: What's the smallest subset of [TOPIC] that still provides value? Can someone get value from 20% of it?

5. **Empty framework test**: Can someone use [TOPIC] without the author present? If the author disappeared tomorrow, would the framework still be usable?

6. **Killer question**: Is [TOPIC] actually more useful than the nearest alternative? If someone is already using [CLOSEST ALTERNATIVE], why should they switch?
```

---

## Round 6: Operationalization

```
Turn the abstract concepts of [TOPIC] into tools that someone can use without you in the room.

1. **Diagnostic checklist**: For each core concept in [TOPIC], design a checklist that lets someone assess whether their system/thinking has that property. Use imperative language: "Check if X. If Y, then Z."

2. **Decision template**: Design a template for the most common decision [TOPIC] is supposed to inform. What questions should someone ask? What factors should they weigh?

3. **Measurement instrument**: What should someone measure to know if [TOPIC] is working? Define at least one metric with thresholds: "If X > Y, the system has property Z."

4. **Fork guide**: Write a guide for someone who wants to adapt [TOPIC] to their domain. What should they keep? What should they change? Where are the natural fork points?

5. **Solo user test**: For each tool above — can someone use it without you explaining it? If not, what additional context does the tool need?

6. **Self-test**: Apply each tool to [TOPIC] itself. Does it pass its own diagnostics?
```

---

## Usage notes

### Model selection
- Rounds 1–2: Any capable model works
- Rounds 3–4: Benefit from the most capable model available (these require creative adversarial thinking)
- Rounds 5–6: Benefit from models with strong practical/product thinking

### Multi-model strategy
Run the same round with different models. Where they converge → high confidence. Where they diverge → the question is genuinely hard.

### Iteration
You can loop back. If Round 5 reveals you have no user, go back to Round 1 and redefine. If Round 3 finds a fatal flaw Round 6 can't operationalize away, kill the framework and start over. Killing a bad framework early is a success.

### Record keeping
Save each round's output. The trace of how your thinking evolved is itself valuable — it's your COS-SOP.md for future contributors.
