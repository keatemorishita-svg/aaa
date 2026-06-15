# Architecture — Constraint Layer (Immune System)

## Function: Preventing Self-Destruction

The Constraint Layer is what keeps an open system from being destroyed by its own openness.

Every system that evolves needs an immune system. Without one, the system cannot distinguish between:
- **Evolution** (divergence that strengthens the system)
- **Parasitism** (divergence that extracts value without contributing)
- **Capture** (divergence that seizes control of the system)
- **Destruction** (divergence that kills the system)

---

## Why AAA Needs This Layer

The original four-layer architecture (Cognition → Protocol → Execution → Evolution) describes how a system **grows**. It says nothing about how a system **defends**.

This is not an academic gap. Open systems face real threats:
- A bad actor forks AAA, changes the kernel to support authoritarianism, and out-markets the original
- A corporation adopts AAA's language to justify anti-competitive behavior as "natural Selection"
- A contributor uses the App Store to distribute content that violates the project's values
- The maintainer burns out and the project dies because there's no succession mechanism

Without a Constraint Layer, AAA's openness is also its vulnerability.

---

## Components

### 1. Identity Boundary

**What defines the system's "self"?**

Without an identity boundary, there is no way to say "this is AAA" vs "this is not AAA." Evolution without identity is dissolution.

AAA's identity boundary:
- **Invariants** (core/kernel.md): The Evolution Loop, Three Primitives, Self-Redefinition
- **Core Statement**: "一个文明首先是一套理论。但它不止于理论..."
- **Brand**: Logo concept, color system, typography

These don't prevent forks from diverging. They define what the original claims to be — so divergence is visible and intentional.

### 2. Selection Integrity

**How do we prevent Selection from being captured?**

Selection is the most easily captured stage of the Evolution Loop. If one actor controls what gets selected, the system evolves toward that actor's interests.

Selection integrity mechanisms:
- **Transparent criteria**: Merge standards are public and written (GOVERNANCE.md)
- **Forkable authority**: If the maintainer's Selection is corrupted, anyone can fork
- **Diverse selectors**: As the project grows, Selection should be distributed across multiple maintainers with different perspectives

### 3. Parasite Detection

**How do we distinguish beneficial divergence from parasitic capture?**

Not all forks are evolution. Some are extraction:
- Forking AAA, rebranding it, and selling it as proprietary consulting IP (legal under MIT, but parasitic)
- Using AAA's App Store to distribute content that harms the project's reputation
- Building a following within the AAA community, then using that following to pressure the maintainer into decisions that benefit the influencer

Detection mechanisms:
- **Transparency**: All contributions are public. Hidden capture is harder.
- **Community vigilance**: The community, not just the maintainer, watches for parasitic behavior
- **Cultural antibodies**: Norms that make parasitic behavior socially costly ("this fork contributes nothing back" is a legitimate criticism)

### 4. Succession

**What happens when the current maintainer disappears?**

Without succession, the system dies with its creator. The Constraint Layer must ensure continuity.

Succession mechanisms:
- **Documented merge criteria**: So merge decisions continue without the original maintainer
- **Named successors**: At least one person who has commit access and understands the vision
- **Fork as last resort**: If succession fails, the community can fork and continue — this is AAA's ultimate succession mechanism

### 5. Value Alignment

**How do we ensure the system evolves toward its stated values, not away from them?**

AAA's core value: systems should evolve without centralized control. A fork that creates a "AAA Certified Centralized Control Framework" is technically following the protocol but violating the value.

Value alignment mechanisms:
- **Not enforced through rules** — rules can be captured
- **Maintained through culture** — the community values openness, not just the protocols
- **Preserved through memory** — ANALYSIS.md, core questions, and case studies document WHY AAA values what it values

---

## Relationship to Other Layers

```
Cognition → understands threats
Protocol  → defines defense rules
Execution  → acts on threats
Evolution  → improves defenses over time
Constraint ← applies to ALL layers — every layer needs an immune function
```

The Constraint Layer is not a separate stack. It's a **cross-cutting concern** — every layer needs to consider how it defends itself, not just how it grows.

---

## Properties of a Healthy Constraint Layer

- **Present but not dominant** — enough defense to survive, not so much that it blocks evolution
- **Transparent** — defenses are visible and contestable, not secret
- **Evolvable** — the immune system itself can be improved
- **Proportional** — response matches threat level (a spam PR doesn't trigger the same response as a hostile fork)
- **Distributed** — defense is not concentrated in one person or mechanism

---

## Current State

AAA's Constraint Layer is **nascent**:
- Identity boundary exists (invariants, core statement)
- Selection integrity is partially addressed (BDFL + Forkable Authority)
- Parasite detection is implicit (no documented process)
- Succession is undefined (single maintainer, no named successor)
- Value alignment is cultural (not yet tested by external participation)

**This is AAA's most critical architectural gap.**
