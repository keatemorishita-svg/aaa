# ATA — Atlas Time Archive

> Save your workspace. Restore it. Like a time capsule for your desktop.

**Repo**: [keatemorishita-svg/ata](https://github.com/keatemorishita-svg/ata)

---

## What it does

ATA is a Windows desktop session recovery tool. It captures all open windows, folder locations, and monitor positions into a JSON snapshot before shutdown. On next boot, it restores those applications and positions to recreate the prior session.

## Key features

- **One-click save/restore**: Snapshots → JSON → restore on reboot
- **AI Insight Engine**: Three tiers — instant (at save), daily (on first restore), weekly (work pattern reports)
- **ANA Bridge**: Syncs with Obsidian daily notes
- **Automation**: Auto-start on boot, scheduled saves
- **Rollback & Logging**: Snapshot history with diff comparison
- **Explorer Adapter**: Restores File Explorer state

## AAA Mapping

ATA is an **Execution Layer** application — it captures and restores system state. The AI Insight Engine adds a Cognition Layer dimension (understanding work patterns from session data).
