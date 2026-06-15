# COS-SOP

## How this was made

1. **Friction identified**: Pasting transcripts from YouTube/Feishu into Obsidian required manual timestamp removal — every time.
2. **Pattern cataloging**: Collected 8 distinct timestamp formats across 3 platforms.
3. **Regex engineering**: Three-pass design — line-start removal (fastest), global sweep (catches mid-paragraph timestamps), whitespace normalization (clean output).
4. **Optional AI layer**: Added DeepSeek/OpenAI polish for users who want fluent prose, not just clean text.

## Key Decisions

1. **Three passes, not one** — A single regex pass catches 90% of timestamps. Three passes catches 99%+ and handles edge cases (mid-paragraph timestamps, Chinese formats).
2. **Paste hook, not manual command** — The plugin works on paste because that's when the problem occurs. A manual clean-up command would add friction.
3. **AI polish as opt-in** — Not everyone wants AI-rewritten transcripts. Keep the core function deterministic.

## What you tried and abandoned

- Single-pass regex: missed mid-paragraph timestamps and Chinese variants
- Full-text AI cleaning only: too slow, too expensive, too unpredictable for the core use case
