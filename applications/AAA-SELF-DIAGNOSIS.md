# Case Study: AAA Diagnoses Itself

> The first documented application of AAA's three-primitive diagnostic on a real system — AAA itself.
> 2026-06-15

---

## System Under Diagnosis

**AAA** — an open-source meta-system protocol project, 1 maintainer, 0 external contributors, ~40 markdown files.

---

## Three-Primitive Diagnostic

### ACCESS — Can new people and ideas enter?

**Score: 4/5**

Evidence:
- Public GitHub repo, MIT license
- README in plain language with bilingual core statement
- App Store protocol with clear contribution path (3 COS files → PR → Merge)
- SOP prompt templates are copyable without understanding the full framework

Gap:
- Framework assumes systems-thinking literacy
- Architecture documentation requires contextual knowledge the author has but hasn't fully externalized
- No onboarding guide for first-time visitors

### MUTATION — Can the system be changed by participants?

**Score: 5/5**

Evidence:
- Anyone can fork (MIT license)
- Anyone can PR
- CONTRIBUTING.md explicitly says "There is no wrong contribution"
- README-FOR-FORKERS.md explicitly encourages divergence
- SOP prompt templates are designed to be copied and modified

No significant gap. Mutation is AAA's strongest primitive.

### RECURSION — Can the rules for changing the system be changed?

**Score: 3/5**

Evidence:
- Governance model is declared (BDFL with Forkable Authority)
- Five maintainer oaths drafted (not yet formalized)
- Discussion mechanism exists (DISCUSSION.md)
- App Store protocol can be modified via PR

Gap:
- GOVERNANCE.md not yet written — governance is implicit, not explicit
- Single-owner GitHub repo means ultimate merge authority is centralized
- No defined process for challenging or replacing the maintainer
- Merge decisions are single-person, not protocol-driven

---

## Diagnosis

```
Access:   ████████░░ 4/5
Mutation: ██████████ 5/5
Recursion: ██████░░░░ 3/5

Pattern: Strong Access + Strong Mutation + Weaker Recursion
```

**Primary blockage**: RECURSION.

AAA is open and changeable but has not fully specified how changes are integrated or how the integration rules themselves can change. The system's evolution depends on a single maintainer's judgment. If the maintainer disappears, the merge path becomes unclear.

**Secondary risk**: Access (4/5) could degrade if documentation doesn't improve. New visitors who don't share the author's systems-thinking background may find the framework impenetrable.

---

## Prescription

1. **Write GOVERNANCE.md** — formalize the five maintainer oaths, define merge criteria, specify succession path
2. **Create onboarding guide** — a 5-minute path for first-time visitors: what to read first, what to skip, what to do
3. **Document merge criteria** — under what conditions is a PR merged? Make it explicit so merge decisions are predictable, not arbitrary

---

## What This Diagnosis Revealed

The diagnosis confirmed something the author already suspected (Recursion is the weakest primitive) but **added specificity**:

- Before diagnosis: "Governance needs work" (vague)
- After diagnosis: "Recursion is 3/5 because merge criteria are implicit and succession is undefined" (specific, actionable)

The diagnosis also revealed a non-obvious risk: **Access (4/5) could degrade** if the framework's complexity isn't addressed for non-expert visitors.

---

## Actions Taken

| Action | Status |
|---|---|
| GOVERNANCE.md written | ✅ This session |
| Onboarding guide | ⏳ Pending |
| Merge criteria documented | ✅ In GOVERNANCE.md |
| Selection primitives formalized | ✅ core/selection-primitives.md |
| Constraint layer added to architecture | ✅ architecture/constraint.md |

---

## Meta: Does this prove AAA has operational value?

**Partially.** This diagnosis was performed by the framework's co-creator (Claude) on the framework itself. It's a real diagnosis of a real system, but:

- It wasn't performed by an external user (solo user test not passed)
- The diagnosis confirmed known issues rather than revealing unknown ones
- The value was in **specificity** — turning vague intuitions into scored, actionable findings

**Next step**: An external user applying the same diagnostic to their own system, without the author present, and discovering something they didn't already know.
