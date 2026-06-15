# COS-SOP

## How this was made

1. **Problem**: Knowledge bases grow. What's in there? What's being neglected? What connections are invisible?
2. **Design**: Scanner that analyzes vault structure without requiring manual tagging or configuration.
3. **Output**: WeeklyManifesto — a reflective document, not a dashboard. Designed to be read, not monitored.

## Key Decisions

1. **Zero config** — The user doesn't set anything up. Ana works out of the box. This was the hardest design constraint.
2. **Weekly, not real-time** — Reflection needs distance. A real-time dashboard encourages monitoring; a weekly manifesto encourages thinking.
3. **Dormancy = 90 days** — Long enough to distinguish "abandoned" from "resting," short enough to catch neglect before it's permanent.

## What you tried and abandoned

- Real-time dashboard: encouraged passive monitoring, not active reflection
- Manual tagging requirement: defeated the purpose — users who tag everything don't need Ana
