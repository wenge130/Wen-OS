---
name: audit
description: Weekly health check of the Wen OS system. Reviews context freshness, connection status, skill coverage, and launch sprint progress.
---

# Audit

Run this skill weekly to assess the health and completeness of your AIOS. It produces a score and a prioritized list of gaps to close.

## Workflow

### Step 1: Context Freshness
Check the last-modified dates of the following files:
- `context/about-me.md`
- `context/about-business.md`
- `context/priorities.md`

Flag any file not updated in the past 30 days. Ask Wen: "Is this still accurate?"

### Step 2: Connection Coverage
Review `connections.md`. For each row with `mechanism: not yet connected`, assess the impact:
- **High impact**: Google Workspace (email, calendar, files), Slack
- **Medium impact**: Shopify (Easein revenue), X, LinkedIn
- **Low impact**: YouTube

Report: "X of 7 domains connected. Highest-impact unconnected: [list]."

### Step 3: Skill Coverage
Review `.claude/skills/`. Check for gaps based on Wen's most common tasks:
- Content creation (Substack, LinkedIn, X, YouTube) → `manage-socials`
- Product launch tracking → `launch-product`
- Meeting processing → `process-voice-memo`
- Weekly health check → `audit` (this skill)

Flag any recurring task Wen mentions that doesn't have a corresponding skill.

### Step 4: Launch Sprint Health
Review `context/priorities.md` and the milestone checklists in `.claude/skills/launch-product/SKILL.md`. Report:
- How many milestones are complete for DMPtech.ai?
- How many milestones are complete for Easein?
- What is the biggest blocker for each?

### Step 5: Score & Report
Generate a brief report:
```
Wen OS Audit — [Date]
Context: [X/3 files fresh]
Connections: [X/7 connected]
Skills: [X skills active, Y gaps identified]
Launch Sprint: DMPtech [X%] | Easein [X%]
Top 3 actions: 
1. [Action]
2. [Action]
3. [Action]
```
