# The Three Primitives

## Access, Mutation, Recursion

These three conditions are necessary for open evolution. They are not sufficient — Selection determines whether evolution produces fitness or failure. But without all three, evolution cannot begin.

---

## Access

> The system must be enterable.

Access means a new participant can observe, interact with, or join the system.

### Forms of Access

- **Transparent Access** — the system is visible (open source code, public science)
- **Participatory Access** — the system can be joined (contribution guidelines, APIs)
- **Structural Access** — the system can be understood (documentation, models, theory)

### Without Access

The system is a **black box**. It may evolve internally, but no external variation can enter. Evolution is limited to internal mutation only.

---

## Mutation

> The system must be modifiable.

Mutation means a participant can change some part of the system.

### Forms of Mutation

- **Replicative Mutation** — copy and modify (fork, clone, branch)
- **In-situ Mutation** — modify in place (edit, patch, update)
- **Compositional Mutation** — recombine existing parts (remix, compose, assemble)

### Without Mutation

The system is **frozen**. It may be accessed and understood, but it cannot change. No evolution is possible.

---

## Recursion

> The system must accept its own changes.

Recursion means modifications can be reintegrated into the system, and the system's rules for accepting change can themselves be changed.

### Two Levels of Recursion

1. **First-order recursion** — the system accepts modifications (merge)
2. **Second-order recursion** — the system can modify its own rules for accepting modifications (meta-evolution)

### Without Recursion

Change is **destructive**. Every modification creates a permanent fork that can never return. The system fragments but does not evolve.

---

## Relationship to the Evolution Loop

| Primitive | Loop Stage |
|-----------|-----------|
| Access | Enables Fork |
| Mutation | Enables Experiment |
| Recursion | Enables Merge |

Selection is the **environmental filter** — it is not a primitive of the system itself, but of the context in which the system operates.

---

## Why three?

One primitive → insufficient.
Two primitives → incomplete.
Three primitives → minimal and complete.

- Access + Mutation without Recursion → fragmentation
- Access + Recursion without Mutation → stagnation
- Mutation + Recursion without Access → elitism
- All three → open evolution
