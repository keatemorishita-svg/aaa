# COS-SOP

## How this was made

1. **Friction identified**: Shutting down means losing context. Reopening everything manually is wasted time.
2. **State capture design**: JSON snapshot of window positions, folder locations, monitor layout.
3. **AI layer**: DeepSeek/OpenAI analysis of work patterns — what do your sessions reveal about how you work?
4. **Integration**: Bridge with Ana for Obsidian daily note syncing.

## Key Decisions

1. **JSON, not binary** — Snapshots are human-readable and diffable. Transparency > efficiency.
2. **Three-tier AI insight** — Instant/daily/weekly. Different questions at different timescales.
3. **PowerShell native** — No dependencies beyond what Windows already has.

## What you tried and abandoned

- Binary snapshot format: faster but opaque — couldn't inspect or diff
- Real-time continuous capture: too much data, too little signal
