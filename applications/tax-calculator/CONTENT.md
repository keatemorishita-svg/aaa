# Tax Calculator · 个人所得税计算器

> Chinese IIT calculator — monthly withholding + year-end bonus optimization. Zero dependencies.

**Repo**: [keatemorishita-svg/tax-calculator](https://github.com/keatemorishita-svg/tax-calculator)

---

## What it does

A Chinese Individual Income Tax (IIT) calculator. Simulates monthly payroll tax calculations and compares year-end bonus taxation methods (Separate vs. Consolidated) to recommend the lower-tax option. Based on China's 2019 tax reform, valid through 2026.

## Key features

- **12-month cumulative withholding projection** with social insurance and housing fund deductions
- **Year-end bonus optimization**: Compares two taxation methods, recommends cheaper
- **Configurable social insurance caps**: Adjustable by city (floor/ceiling)
- **8 special deductions**: Child education, continuing education, housing loan interest, housing rent, elderly care, infant care, major medical
- **localStorage persistence**: Auto-save salary data, settings, bonus history
- **Zero dependencies**: Pure HTML/CSS/JS, ES modules, no framework

## AAA Mapping

Tax Calculator is an **Execution Layer** application — it performs a specific computation (tax optimization) with transparent logic. It's the simplest and most practical AAA application: one job, done well.
