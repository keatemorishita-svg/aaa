# COS-SOP

## How this was made

1. **Problem**: Chinese IIT calculation is complex — cumulative withholding, special deductions, year-end bonus optimization. Most people just trust their HR department.
2. **Design**: Pure client-side calculator. No server, no data collection. User owns their salary data.
3. **Optimization**: Compare separate vs. consolidated bonus taxation → recommend the cheaper method.

## Key Decisions

1. **Zero dependencies** — No React, no Vue, no npm. Pure HTML/CSS/JS. A tax calculator shouldn't have a supply chain.
2. **localStorage, not cloud** — Salary data stays on the user's machine. Privacy is the feature.
3. **Valid through 2026** — Explicitly dates the tax rules. Transparency about when the calculator needs updating.

## What you tried and abandoned

- Server-side calculation: unnecessary for the computation complexity; introduced privacy concerns
- Multi-country support: diluted focus; better as separate forks per tax jurisdiction
