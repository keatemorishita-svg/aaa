# Tool: COS File Generator

> One prompt. Three files. Submit any project to the AAA App Store.

---

## How to use

1. Copy the prompt below
2. Paste into any conversation with Claude or any capable AI
3. Replace `[PROJECT NAME]` and `[2-3 SENTENCES]`
4. The AI will generate your COS-META.md, COS-SOP.md, and COS-EVOLUTION.md

---

## The Prompt

```
I have a project and I want to submit it to the AAA App Store. Please help me generate three required files.

My project is called: [PROJECT NAME]
Here's what it does: [2-3 SENTENCES]

Please generate:

1. COS-META.md
- Identity: Name, Author, Version, Date
- Architecture mapping: Which AAA layer(s) does it work in? (Cognition / Protocol / Execution / Evolution)
- Primitive check: How does it serve Access, Mutation, and Recursion? One sentence each.
- Dependencies: What does it require? What does it extend? Any conflicts?
- Fork instructions: Best fork point? What to keep? What to change?

2. COS-SOP.md
- How was this project made? What was the method/process?
- What were the 3-5 key decisions and why?
- What was tried and abandoned? (Failures are valuable.)

3. COS-EVOLUTION.md
- Current maturity: Draft / Stable / Evolving / Legacy
- Known weaknesses (be honest — honesty is more valuable than perfection)
- Evolution invitation: Best contribution type? What needs improvement? What should NOT be changed?
- Fork policy: How fork-friendly? Merge preference?
- Succession: What happens if the creator disappears?

Make each file complete and ready to use. Follow the AAA App Store protocol format.
```

---

## After generating

1. Review the generated files — the AI is good but not perfect
2. Add your project's content (CONTENT.md)
3. Place all 4 files in `applications/<your-project-name>/`
4. Fork AAA, add your app to INDEX.md, open a PR

---

*This generator is part of AAA but is designed to be used independently.*
