# COS-SOP

## How this was made

1. **Problem**: AI news is overwhelming — quantity over structure. Reading doesn't equal understanding.
2. **Insight**: Different AI leaders would interpret the same news differently. Simulating their perspectives reveals structure.
3. **Design**: 6 personas × daily news feed × consensus detection = structured knowledge network
4. **Implementation**: Obsidian plugin + LLM API + 9 prompt files as core pipeline

## Key Decisions

1. **6 personas, not 3 or 10** — 3 loses diversity; 10 creates noise. 6 hits the sweet spot of meaningful divergence without overwhelming the user.
2. **Consensus as signal** — When 3+ independent simulated perspectives converge, that's worth paying attention to. This is distributed Selection.
3. **Obsidian-native** — Output is a vault, not a dashboard. Knowledge lives where the user already works.

## What you tried and abandoned

- Auto-posting to social media — added noise without adding understanding
- Real-time feed — too noisy; daily batch is the right cadence for reflection
