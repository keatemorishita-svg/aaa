# COS-META

## Identity
- **Name**: ACA — Transcript Timestamp Cleaner
- **Author**: aaa-mvc
- **Version**: 1.0
- **Date**: 2026-06
- **Repo**: https://github.com/aaa-mvc/aca

## Architecture Mapping

- [ ] Cognition Layer
- [x] Protocol Layer — defines and enforces a cleaning protocol for transcription formats
- [x] Execution Layer — executes the cleaning on paste
- [ ] Evolution Layer

## Primitive Check

- **Access** — Makes transcript content accessible by removing timestamp noise
- **Mutation** — Regex patterns can be extended for new timestamp formats
- **Recursion** — The cleaning protocol can be improved as new formats emerge

## Dependencies
- **Requires**: Obsidian
- **Extends**: Obsidian plugin ecosystem
- **Conflicts**: None

## Fork Instructions
- **Best fork point**: Regex patterns (add new timestamp formats)
- **What to keep**: Three-pass engine architecture
- **What to change**: Supported formats, AI polish prompt
