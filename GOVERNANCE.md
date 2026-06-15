# AAA — Governance

> "No permanent center. Centers exist locally and decay."

---

## Governance Model: BDFL with Forkable Authority

AAA uses a **Benevolent Dictator For Life (BDFL) with Forkable Authority** model.

**What this means**:
- The maintainer has final merge authority on the main repository
- Any participant who disagrees with the maintainer's decisions can fork the project
- The fork is not a threat — it is the system's primary governance escape valve

**Why this model**:
- AAA is currently a single-maintainer project. Full distributed governance would be performative — pretending to have a community that doesn't exist yet.
- BDFL is honest about where power currently resides.
- Forkable Authority ensures that the BDFL's power is never permanent or absolute — it lasts only as long as the community chooses not to fork.

---

## Maintainer's Oath

The maintainer commits to:

### 1. Temporary Trust
> I hold merge authority as a temporary trust, not as a permanent right. My authority exists because the community has not yet chosen to fork. The moment a fork becomes more useful than this repository, my authority ends.

### 2. Public Decisions
> I will explain every merge rejection publicly. If I cannot articulate why a contribution was rejected, the rejection was illegitimate.

### 3. Rules Apply to Me
> I am subject to the same contribution standards as every participant. I will not merge my own PRs without review when review is available.

### 4. Active Succession
> I will actively prepare at least one other person to replace me. If I disappear for 90 days without notice, the project's continuity should not depend on my return.

### 5. Celebrate Better Forks
> If a fork of AAA becomes more useful, more adopted, and more alive than this repository, I will publicly acknowledge it. The system working as designed is not my failure.

---

## Merge Criteria

A PR is merged when:

1. **Protocol compliance**: For App Store submissions, COS-META.md and COS-SOP.md are complete
2. **Non-duplication**: The contribution is not an exact duplicate of existing content (similar is fine; identical is not)
3. **License compatibility**: The contribution is compatible with MIT license
4. **No active harm**: The contribution does not contain malware, harassment, or illegal content

A PR is NOT rejected because:
- The maintainer disagrees with its content
- It challenges AAA's core concepts
- It is "not good enough" by subjective quality standards
- It comes from an unknown contributor

**Content quality is determined by usage, not by the maintainer.**

---

## What Happens During Disagreement

### Level 1: Discussion
Disagreements are discussed publicly in GitHub Discussions or the PR thread.

### Level 2: Maintainer Decision
If discussion doesn't resolve the disagreement, the maintainer makes a decision and explains it publicly.

### Level 3: Fork
If the maintainer's decision is unacceptable to a significant portion of the community, anyone can fork. The fork is the ultimate check on maintainer authority.

### Level 4: Community Migration
If the fork gains more usage, contributors, and vitality than the original, the community has effectively chosen new governance. This is not a crisis — it is the system working as designed.

---

## Succession Plan

### Current State
- **Maintainer**: keatemorishita-svg
- **Named successor**: None (project is pre-community)
- **Succession trigger**: Maintainer absence > 90 days without notice

### When a community forms
1. At least one other person gains commit access
2. That person is publicly named as successor
3. Merge decisions require at least one other reviewer when available

### If succession fails
The community forks. The fork becomes the de facto continuation. AAA's ultimate succession mechanism is the fork.

---

## Changing Governance

This GOVERNANCE.md can be changed through the same PR process as any other file. The maintainer's oath applies to governance changes: they must be explained publicly, and they must not eliminate the fork escape valve.

**The one unchangeable rule**: The right to fork cannot be removed. If a governance change eliminates the community's ability to fork and continue independently, that change is illegitimate regardless of how many approvals it receives.

---

## Current Limitations (Honest Acknowledgment)

1. **Single point of failure**: The maintainer is the only person with commit access. This will be addressed when a community forms.
2. **Untested**: These governance mechanisms have not been tested by real disagreement. They are design, not precedent.
3. **Platform dependence**: GitHub's terms of service and availability affect AAA's governance. A future migration to decentralized infrastructure would strengthen AAA's alignment with its own principles.

---

*This governance document is version 1.0. It will evolve as AAA evolves.*
