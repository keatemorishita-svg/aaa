# Example: GitHub as a AAA Instance

GitHub is the closest existing implementation of AAA principles.

---

## Mapping GitHub to AAA

### Core Loop
```
Fork repo → Make changes → Open PR → Merge → Repeat
```

### Three Primitives
- **Access** — public repos are visible to everyone; anyone can create an account
- **Mutation** — anyone can fork and modify
- **Recursion** — PRs can be merged back; contribution guidelines can be updated

### Four Layers
- **Cognition** — Issues, Discussions, code search, Copilot
- **Protocol** — Git protocol, PR templates, CODEOWNERS, CI/CD rules
- **Execution** — Actions, deployments, package registry
- **Evolution** — Repository forks, branch experimentation, community governance

---

## What GitHub Gets Right

1. **Fork is zero-cost** — the barrier to divergence is near zero
2. **Merge is structured** — PR review process formalizes selection
3. **History is preserved** — every state is recoverable
4. **Identity is distributed** — no single owner controls the ecosystem

---

## What GitHub Gets Wrong (from AAA perspective)

1. **Centralized platform** — GitHub itself is a single point of control
2. **Ownership asymmetry** — the repo owner has disproportionate power
3. **Closed selection** — the owner decides what gets merged
4. **Platform lock-in** — Issues, Actions, Discussions are not portable

---

## The Lesson

GitHub proves that the Fork → Merge loop works at massive scale.

But it also proves that a platform is not the same as an evolution system — GitHub's own evolution is controlled by Microsoft, not by its users.

The next step beyond GitHub is a system where **the platform itself can be forked**.
