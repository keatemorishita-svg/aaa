# COS-META

## Identity
- **Name**: Tax Calculator · 个人所得税计算器
- **Author**: keatemorishita-svg
- **Version**: 1.0
- **Date**: 2026-06
- **Repo**: https://github.com/keatemorishita-svg/tax-calculator

## Architecture Mapping

- [ ] Cognition Layer
- [x] Protocol Layer — Implements Chinese tax law as executable protocol
- [x] Execution Layer — Performs tax computation and optimization
- [ ] Evolution Layer

## Primitive Check

- **Access** — Makes tax calculation transparent and accessible without an accountant
- **Mutation** — Tax parameters (rates, caps, deductions) can be updated as laws change
- **Recursion** — Tax law changes → calculator updates → users get correct results

## Dependencies
- **Requires**: Local HTTP server (ES module CORS)
- **Extends**: AAA Execution Layer — pure utility
- **Conflicts**: None

## Fork Instructions
- **Best fork point**: Tax parameters (adapt to other countries' tax systems)
- **What to keep**: Optimization logic (compare methods, recommend cheaper)
- **What to change**: Tax brackets, deduction types, social insurance rules
