# COS-SOP

## How this was made

1. **Problem**: Meaningful connection in comment sections is hard. Most comments are noise.
2. **Design**: 3 intents × 6 styles × 4 tones = a matrix of comment generation possibilities.
3. **Privacy constraint**: API key stays local. Content goes directly to DeepSeek. No intermediary.
4. **Simplicity**: Flask backend + vanilla frontend. Zero build step. Clone and run.

## Key Decisions

1. **3 intents, not more** — Networking, self-warming, and alt-account cover the core social goals. More would be noise.
2. **Privacy as feature** — In a world of data-collecting social tools, "your key stays local" is a differentiator.
3. **Vanilla frontend** — No React, no build step. The tool is simple enough that a framework would be overhead.

## What you tried and abandoned

- More intents (7+): users couldn't distinguish between them; 3 is the right granularity
- SaaS model: privacy requirement made local-first the only viable architecture
