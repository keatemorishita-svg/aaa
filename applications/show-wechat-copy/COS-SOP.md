# COS-SOP

## How this was made

1. **Problem**: WeChat Moments posts feel performative. Most people either overthink or underthink their posts.
2. **Design**: Multi-axis customization — not just "what tone" but "who are you being, in what context, for what purpose, at what rhythm?"
3. **Constraint**: Single-file deployment, zero build step, privacy-respecting.

## Key Decisions

1. **4 axes, not 1** — Tone alone is insufficient. Persona + scenario + purpose + rhythm captures the full expression space.
2. **Dual AI backend** — Lock-in to one provider is fragility. DeepSeek for cost, OpenAI for quality.
3. **Vanilla stack** — Python server + HTML frontend. No framework overhead for a single-purpose tool.

## What you tried and abandoned

- Single-axis (tone only): Outputs felt generic — missing context, purpose, and persona
- Mobile app: maintenance overhead not justified for a tool this focused
