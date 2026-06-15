# COS-SOP

## How this was made

1. **Threat modeling**: Identified the attack surface of AI Agent Skills — code injection, prompt injection, mixed attacks.
2. **Taxonomy design**: Mapped to MalSkillBench three-dimensional attack space (15 malicious behavior categories).
3. **Dual-engine design**: Rule engine for speed (deterministic, sub-second), semantic engine for depth (LLM-powered intent analysis).
4. **Benchmarking**: Tested on 7,891 skills to calibrate detection accuracy.

## Key Decisions

1. **Dual engines, not one** — Pure regex is fast but misses semantic attacks. Pure LLM is deep but slow and expensive. Dual-engine gives both.
2. **Exit-code integration** — Designed for CI/CD from day one. Security that requires manual execution doesn't get used.
3. **YAML rules, not hardcoded** — The threat landscape evolves. Rules must evolve with it.

## What you tried and abandoned

- Pure LLM scanning: too slow for CI/CD, too expensive for daily use
- Signature-based only: missed novel attacks that didn't match known patterns
