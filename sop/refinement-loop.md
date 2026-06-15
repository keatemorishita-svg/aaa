# The Six-Round Refinement Loop

> Full process documentation. For copy-paste prompt templates, see [prompt-templates.md](./prompt-templates.md).

---

## Round 0: Exhaustive Clarification (2 Rounds Minimum)

**Before you start the six rounds, you must ask questions. Not answer them — ASK them.**

### The Principle

The single most common failure mode of any refinement process is **answering the wrong question beautifully.** You invest six rounds in polishing a framework, only to discover at the end that you've been refining something the user didn't actually need.

Round 0 prevents this. The rule: **before entering Round 1, the AI must ask at least 2 rounds of exhaustive questions.** Each round asks N questions (typically 3-5) about the user's intent, context, constraints, and expectations. The user answers. The AI asks again. Only when no new questions emerge does the process move to Round 1.

### Why 2 rounds minimum

- **Round 0.1**: Surface-level clarification. The AI asks the obvious questions. The user answers. These answers reveal the shape of what's actually needed.
- **Round 0.2**: Depth-level clarification. The AI asks the NON-obvious questions — the ones that only emerge after hearing the first round of answers. This is where the real requirements surface.

One round of questioning is politeness. Two rounds is rigor. Three or more is permissible if the domain is complex or the user's intent is still evolving. But never fewer than two.

### The pattern

```
AI: I have N questions about [TOPIC]. Here they are:
     Q1: ...
     Q2: ...
     Q3: ...
     Q4: ...
     Q5: ...

User: [Answers]

AI: Based on your answers, I have N more questions:
     Q1: ...
     Q2: ...
     Q3: ...

User: [Answers]

AI: No further questions. Entering Round 1.

OR

AI: I still have questions. Round 3 of clarification:
     ...
```

### The AI-First Pattern: Answer, Don't Just Ask

**The Rule**: In Round 0, the AI does not just throw questions at the user and wait. For every question asked, the AI also provides its own best answer — with reasoning. The user's job is not to answer from scratch. It is to confirm or correct.

**Why**: Asking questions without answering them is intellectual laziness disguised as Socratic method. It shifts all cognitive load to the user while the AI performs the cheap role of interrogator. The AI must earn the right to ask a question by demonstrating it has already thought about the answer.

**The pattern**:

```
AI: Q1 — [Question]
    My assessment: [Answer based on available context]
    Reasoning: [Why I think this]
    → Confirm or correct?

User: Correct. / Change X to Y. / I actually think Z.

AI: Q2 — [Question, now informed by the user's correction to Q1]
    ...
```

**This is not the AI "answering its own questions."** It is the AI doing the cognitive work first, presenting a draft answer, and letting the user edit. Editing is always faster than creating from scratch. The user's role shifts from author to editor — a strictly lower cognitive burden.

### What to ask about

| Category | Example Questions |
|---|---|
| **Form** | Is this a document, a tool, a framework, a skill, or something else? |
| **Audience** | Who will use this? What's their first contact point? |
| **Constraints** | What are the hard constraints? (platform, format, time, brand) |
| **Success** | What does "done" look like? How will you know this worked? |
| **Relationship** | How does this relate to existing work/projects/brands? |
| **Evolution** | How should this evolve over time? Who decides? |
| **Boundaries** | What is this NOT? What's explicitly out of scope? |

### Red flags

- Zero questions asked → immediately suspect. You're refining blind.
- AI asks but doesn't answer → cognitive burden shifted entirely to user. Lazy.
- AI's answers are vague ("it depends") → AI hasn't done its homework.
- All user responses are "correct" → either the AI is too agreeable or the user isn't being challenged. AI should flag: "I notice you've confirmed all my answers. Am I being too safe with my assessments?"
- User says "just start, I'll tell you what's wrong" → valid, but AI should flag: "Without Round 0, we may waste rounds refining the wrong thing. Your call."

### This mechanism in action — two examples

**Example 1: SOP Skill itself.** Before building the SOP Skill, the AI asked 5 questions — AND answered each with its own assessment. The user confirmed most, corrected one (name stays SOP, not ASA). Three rounds of 15 questions total. The answers shaped everything. Without Round 0, SOP would have been a documentation page, not a "say five words" trigger command.

**Example 2: ASA Retrospective.** The user said "执行SOP" on an ASA review document. The AI asked 5 questions and answered each: Q1 (audience: internal + future self), Q2 (completeness: missing an architectural lesson), Q3 (direction: v1.0 endpoint, observe don't build), Q4 (unease: "on-demand = existence depends on invocation frequency"), Q5 (output: honesty checklist + public article + honesty verification). Every answer came with reasoning. The user only needs to say "correct" or "change X."

The meta-principle: **the questions you ask before you build determine what you build. But the answers you propose before the user responds determine whether you're a partner or a questionnaire.**

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

## Round 7: Publication & Distribution — The Five Deliverables

**After the framework survives, you ship it. Round 7 is the shipping checklist.**

This is not an optional step. A framework that survives six rounds of attack but has no distribution strategy is like a weapon that was forged but never sharpened. Round 7 turns the refined framework into a publicly discoverable, instantly usable, virally spreadable product.

### The Five Deliverables

#### 1. GitHub Repo Description (330 bytes, bilingual)

A single description that fits within GitHub's 330-byte limit. Must contain: what it is, how to trigger it, and the win condition. In both English and Chinese.

**Why 330 bytes**: This is the first and sometimes only text people see in search results. Every character must earn its place.

**Template**:
```
[What it is] + [Trigger command] + [Win condition] + [Evolves]  [中文版：是什么 + 怎么触发 + 赢家逻辑 + 进化]
```

**Example (SOP)**:
```
A recursive skill that stress-tests any conceptual framework through 6 rounds of adversarial refinement. Say "Execute SOP" — your framework faces 7 rounds of attack. Survive or die, you win either way. It evolves every time you use it.  执行SOP——六轮攻击，七轮精炼。零安装。零配置。活下来或被杀死，你都是赢家。每用一次，进化一次。
```

#### 2. Twenty Search Keywords

Twenty keywords across four tiers, optimized for GitHub discoverability.

| Tier | Count | Purpose | Example |
|---|---|---|---|
| Tier 1 | 5 | High intent — they're looking for exactly this | `framework stress test`, `adversarial refinement` |
| Tier 2 | 5 | Specific use case — they have a problem | `ai peer review`, `find flaws in my theory` |
| Tier 3 | 5 | Method & approach — they want a way of working | `red team your ideas`, `steel man argument prompt` |
| Tier 4 | 5 | Ecosystem discovery — cross-linking | `recursive self improvement tool`, `ai native methodology` |

**Where they go**: Tier 1 → GitHub Topics. Tier 2-3 → README headers and body. Tier 4 → cross-links with ecosystem projects.

#### 3. Distribution Article (WeChat / Blog)

A narrative article telling the complete story: origin, birth, development, operation, solidification. Not a technical document — a story that makes people want to use the thing.

**Required structure**:
- Chapter 1: Origin — the pain that caused this to exist
- Chapter 2: Birth — how it was built (including how it was used on itself)
- Chapter 3: Development — what broke and how it was fixed
- Chapter 4: Operation — the trigger command, the experience
- Chapter 5: Solidification — how it evolves itself
- Chapter 6: Honesty — its known failure modes (admitted publicly)
- Chapter 7: Relationship — how it connects to the larger ecosystem (if any)
- Call to action: the trigger command

#### 4. Trigger Command

A single, memorable command that activates the entire framework. Five words or fewer in the target language.

**Why a trigger command**: Copying prompts is friction. Saying five words is not. The trigger command is the user interface. The prompt is the implementation detail.

**Rules**:
- Five words or fewer in the target language
- Works across all platforms (Claude Code, Claude.ai, ChatGPT, any AI tool)
- Preloaded once; triggered forever after
- Bilingual if the project is bilingual

**Example (SOP)**: `执行SOP` / `Execute SOP`

#### 5. GitHub Repo Name (pre-reserved)

The repository name must be reserved before publication. It must be: unique, memorable, pronounceable, and consistent with the project's naming system (if any).

**Checklist**:
- [ ] Repo name matches org/ecosystem naming convention
- [ ] Name is not already taken by a competing project
- [ ] Name is pronounceable in the project's primary language
- [ ] Name can be trademarked if the project grows to that scale
- [ ] Both `github.com/org-name/repo` and `github.com/org-name` are resolved (org name is repo name if flagship)

### Why Round 7 Exists

The most common failure mode after Round 6 is this: a beautifully refined framework that nobody finds, nobody uses, and nobody forks. Round 7 prevents that.

The five deliverables are not marketing. They are the final layer of the framework's design — the interface between the framework and the world.

A framework that cannot be discovered, triggered, and spread is not a framework. It's a private thought.

---

## Meta: This SOP Itself

This SOP document was itself refined through the six-round process. It is both the method and an instance of the method — self-referential integrity in action.

The current known weaknesses:
- Round 4 (dimension-switch) can produce an unbounded number of perspectives — selection criteria for which dimensions to test are still heuristic
- The process assumes access to a capable AI collaborator; solo execution is possible but significantly slower
- Operationalization (Round 6) is the least developed round — it's where most frameworks (including this one) have the most work to do
