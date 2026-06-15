# ACA — Transcript Timestamp Cleaner

> You do one thing: Ctrl+V. The plugin does the rest.

**Repo**: [keatemorishita-svg/aca](https://github.com/keatemorishita-svg/aca)

---

## What it does

An Obsidian plugin that automatically strips timestamps when pasting transcriptions from YouTube, podcasts, or Feishu (飞书妙记). Supports 8 timestamp formats including Chinese, English, and mixed patterns.

## Key features

- **Paste auto-clean**: Strips timestamps on Ctrl+V — zero additional steps
- **8 timestamp formats**: YouTube, Feishu, SRT, Chinese compact/spaced/full patterns
- **Three-pass regex engine**: Line-start removal → global sweep → whitespace normalization
- **AI polish option**: Optional DeepSeek/OpenAI integration to polish cleaned transcripts into fluent prose
- **Command palette**: Dedicated paste-and-clean + retroactive clean-up commands

## AAA Mapping

ACA is a **Protocol Layer** application — it defines and enforces a cleaning protocol for transcription data. It's a minimal, single-purpose protocol that does one thing well.
