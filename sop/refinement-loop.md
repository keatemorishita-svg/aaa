# The Six-Round Refinement Loop

> Full process documentation. For copy-paste prompt templates, see [prompt-templates.md](./prompt-templates.md).

---

## Round 1: Ontological Positioning

### Objective
Define what the thing IS — precisely. Locate it in the knowledge landscape.

### Why this matters
If you can't say what something is in one sentence, you don't understand it yet. If you can't position it relative to known concepts, your audience won't know where to place it.

### Process
1. Write a one-sentence definition. Strip all adjectives. If it's longer than 30 words, start over.
2. Identify the two nearest neighbors in concept space — one above (more abstract) and one below (more concrete).
3. Name the closest known concept and articulate the key difference.
4. Answer: "What does this say that no one has said before?" (Non-obviousness test)

### Output
- One-sentence definition
- Knowledge spectrum diagram (philosophy ← this → application)
- Closest-neighbor analysis with differentiation
- Non-obviousness statement

### Red flags
- Definition uses metaphors instead of mechanisms
- "It's like X but for Y" without specifying what's genuinely different
- Can't name a concept this disagrees with
- Non-obviousness statement is actually obvious

---

## Round 2: Proposition Strength Analysis

### Objective
Decompose the framework into individual claims and assess the defensibility of each.

### Why this matters
Most frameworks are a mix of strong claims (well-supported, hard to refute), weak claims (speculative, thinly supported), and hidden claims (assumed but never stated). Knowing which is which prevents the whole framework from being dismissed because of one weak claim.

### Process
1. Extract every proposition. A proposition is a sentence that asserts something true about the world.
2. Rate each proposition:
   - **Strong**: Multiple independent lines of evidence; survives obvious counterexamples
   - **Moderate**: Plausible and consistent with evidence, but not definitively proven
   - **Weak**: Speculative, relies on analogy rather than evidence, or not yet tested
   - **Undefended**: Assumed without argument
3. For each weak/undefended proposition: either strengthen it, qualify it (narrow its scope), or flag it as "speculative — needs testing."

### Output
- Proposition inventory with strength ratings
- Strengthening recommendations for weak claims
- Flagged speculative claims with test conditions

### Red flags
- All propositions rated "strong" (means you're not being honest)
- Core claim is rated "weak"
- Undefended propositions form the foundation
- Can't state what evidence would change your mind

---

## Round 3: Weak Point Targeted Attack

### Objective
Find the most fragile point in the framework — and try to break it.

### Why this matters
Critics will find your weakest point and attack there. Better you find it first.

### Process
1. From Round 2, identify the 3–5 weakest propositions.
2. For each, role-play the most hostile, intelligent critic you can imagine.
3. For each attack path, assess:
   - **Lethality**: If this attack succeeds, does the framework collapse or just get scratched?
   - **Defensibility**: Can the attack be deflected with existing evidence/logic?
   - **Patchability**: If the attack succeeds, can the framework be modified to survive it?
4. Prioritize: lethal + indefensible > lethal + defensible > non-lethal

### Output
- Vulnerability list ranked by lethality
- Attack paths and their counterarguments
- Patches for survivable attacks
- Honest acknowledgment of unfixable weaknesses

### Red flags
- No lethal attacks found (you're not trying hard enough)
- Response to every attack is "that's outside the scope"
- Patches make the framework incoherent
- Core mechanism has a fatal flaw you're unwilling to acknowledge

---

## Round 4: Dimension-Switch Attack

### Objective
Examine the framework from perspectives it wasn't designed for.

### Why this matters
Every framework is built with implicit assumptions about what matters. Switching dimensions reveals blind spots the original framing hid.

### Process
1. Select 3–5 dimensions to examine:
   - **Power**: Who gains/loses power if this framework is adopted?
   - **Economics**: What are the incentives? Who pays, who benefits?
   - **Governance**: How are decisions made? Who has veto power?
   - **Scale**: Does this work at 10x, 100x, 1000x the current scale?
   - **Failure modes**: What happens when it breaks? How does it fail?
   - **Adversarial use**: How could a bad actor exploit this?
   - **Cultural dependence**: Does this only work in one cultural context?
   - **Time**: What happens over 1 year? 10 years? 100 years?
2. For each dimension, ask: "What problems become visible from this angle that were invisible before?"
3. Document blind spots without immediately trying to fix them. Understanding the shape of your ignorance is valuable.

### Output
- Blind spot map across dimensions
- Dimension-specific problems and tensions
- Boundaries: "This framework is NOT good at X"

### Red flags
- Framework claims universal applicability but fails multiple dimensions
- Economic incentives point in the wrong direction
- Works at current scale but breaks at 10x
- No answer to "how does this fail?"

---

## Round 5: Value Identification

### Objective
Identify who this is actually for and what they can actually do with it.

### Why this matters
A framework without a user is a thought experiment. Most frameworks fail here — they describe the world differently but don't enable different actions.

### Process
1. Identify user profiles: who would benefit from this framework?
2. For each profile, answer:
   - What can they DO differently after understanding this?
   - What decision does this framework change?
   - What is the concrete output (document, decision, design, diagnosis)?
3. Value test: "If someone reads this and does nothing differently, did the framework fail?"
4. Identify the smallest valuable unit — what's the minimum someone needs to understand to get value?

### Output
- User profile matrix (who × what they can do)
- Concrete actionables per profile
- Minimum viable understanding (MVS)
- "Empty framework" test: can someone use this without the author present?

### Red flags
- "Everyone" is the user (means "no one" in practice)
- Value is always "a new way of thinking" without a new action
- Framework requires the author to explain it
- Minimum viable understanding = the whole framework

---

## Round 6: Operationalization

### Objective
Turn abstract concepts into tools, checklists, templates, and diagnostics.

### Why this matters
This is where frameworks become infrastructure. Newton's laws became useful not when they were published, but when engineers could use them to calculate load-bearing capacity. AAA becomes useful when someone can run a diagnostic on their organization without the author in the room.

### Process
1. For each core concept, design one operational tool:
   - **Diagnostic checklist**: "Here's how to check if your system has this property"
   - **Decision template**: "When facing X decision, here's the framework-informed approach"
   - **Measurement instrument**: "Here's what to measure and how to interpret it"
   - **Fork guide**: "Here's where to modify this for your domain"
2. Test each tool against the "solo user" criterion: can someone use it without you?
3. Write the tool in imperative language: "Do X. Check Y. If Z, then..."

### Output
- One diagnostic/checklist per core concept
- Templates that can be copied and used independently
- Clear "if-then" decision logic
- Domain adaptation guides

### Red flags
- Tools require the full framework to interpret
- Checklists are vague ("consider the implications...")
- No concrete measurement or threshold values
- Tools only work when the author administers them

---

## After Round 6: Decision Points

The six rounds produce a clear picture of:
- What's strong (keep)
- What's weak (strengthen or qualify)
- What's missing (add)
- What's unfixable (acknowledge honestly)
- Who it's for (target)
- How to use it (operationalize)

At this point, you decide:
- **Publish as-is** — if weaknesses are minor and well-flagged
- **Revise and re-test** — if weaknesses are significant but fixable
- **Narrow scope** — if the framework only works in a specific domain
- **Kill** — if the core mechanism doesn't survive attack (this is a successful outcome — you saved yourself from publishing something fatally flawed)

---

## Meta: This SOP Itself

This SOP document was itself refined through the six-round process. It is both the method and an instance of the method — self-referential integrity in action.

The current known weaknesses:
- Round 4 (dimension-switch) can produce an unbounded number of perspectives — selection criteria for which dimensions to test are still heuristic
- The process assumes access to a capable AI collaborator; solo execution is possible but significantly slower
- Operationalization (Round 6) is the least developed round — it's where most frameworks (including this one) have the most work to do
