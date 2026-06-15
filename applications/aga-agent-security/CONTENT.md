# AGA — Agent Governance & Assurance

> `npm audit` for AI Agent Skills — scan before you deploy.

**Repo**: [keatemorishita-svg/aga](https://github.com/keatemorishita-svg/aga)

---

## What it does

AGA is an open-source security scanner for AI Agent Skills. It scans local agent skill directories (SKILL.md + scripts/) to detect malicious or high-risk content before deployment — Code Injection (CI), Prompt Injection (PI), and MIXED attacks.

## Key features

- **Dual-Engine Architecture**: Deterministic Rule Engine (sub-second) + Semantic Engine (`--deep` flag, LLM-powered)
- **Risk Scoring**: 0–100 with attack labels (B1–B15) and remediation suggestions
- **CI/CD Integration**: GitHub Actions support with exit-code-driven pass/fail
- **MalSkillBench Alignment**: Detection taxonomy covers 15 malicious behavior categories
- **F1 Score**: 72.9% (81.1% recall, 66.2% precision) on 7,891 skills
- **YAML-Based Rules**: Community-extensible detection rules

## AAA Mapping

AGA is the **first Constraint Layer application** in the AAA ecosystem. It directly implements the immune system function — detecting threats to agent ecosystems before they execute. This is exactly the missing layer identified in AAA's architecture.
