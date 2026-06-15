# COS-META

## Identity
- **Name**: AGA — Agent Governance & Assurance
- **Author**: keatemorishita-svg
- **Version**: 1.0
- **Date**: 2026-06
- **Repo**: https://github.com/keatemorishita-svg/aga

## Architecture Mapping

- [ ] Cognition Layer
- [x] Protocol Layer — Defines detection rules as YAML protocol
- [ ] Execution Layer
- [x] **Constraint Layer** — This is the first AAA Constraint Layer application. It provides the immune system for agent ecosystems.

## Primitive Check

- **Access** — Makes agent skill security transparent and scannable
- **Mutation** — YAML rules are community-extensible; anyone can contribute detection patterns
- **Recursion** — Detection rules improve as new attack patterns are discovered and integrated

## Dependencies
- **Requires**: Python 3.x, optional LLM API for deep scan
- **Extends**: AAA Constraint Layer — proves the layer is not just theoretical
- **Conflicts**: None

## Fork Instructions
- **Best fork point**: Detection rules (YAML)
- **What to keep**: Dual-engine architecture, MalSkillBench alignment
- **What to change**: Add detection rules for your specific agent framework
