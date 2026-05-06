# Wen OS

A personal AI Operating System for **Wen Ge** — Chief AI & Product Officer at [DMPtech.ai](https://dmptech.ai) and Co-founder & CEO of [Easein](https://easein-6053.myshopify.com).

Personalized for Wen's specific context, businesses, and workflows.

---

## What is this?

Wen OS is a structured folder that acts as persistent memory and a command center for your AI assistant (Claude Code or any AI coding tool). Every session, the AI reads this folder to understand who you are, what you're building, and how you work — so you never have to re-explain yourself.

---

## Getting Started

1. **Clone or download** this folder into your project directory.
2. **Copy `.env.example` to `.env`** and fill in your API keys (never commit `.env`).
3. **Open in Claude Code** (or your preferred AI coding tool) and run `/audit` to see your current system health.
4. **Update `context/` files** whenever your priorities or business context changes.

---

## Folder Structure

```
Wen-OS/
├── CLAUDE.md                   # The AI's core instructions — read first, every session
├── connections.md              # Registry of every tool/system the AI can reach
├── .env.example                # Template for API keys (copy to .env, never commit)
├── .gitignore                  # Keeps secrets and noise out of version control
│
├── context/
│   ├── about-me.md             # Who Wen is, background, pain points
│   ├── about-business.md       # DMPtech.ai & Easein business context
│   └── priorities.md           # Current 90-day launch priorities
│
├── references/
│   └── voice.md                # Writing style samples and register guide
│
├── .claude/
│   └── skills/
│       ├── audit/              # Weekly system health check
│       ├── launch-product/     # 90-day launch sprint tracker
│       ├── manage-socials/     # Substack, LinkedIn, X, YouTube SOP
│       └── process-voice-memo/ # iPhone Voice Memo → structured notes
│
├── decisions/
│   └── log.md                  # Append-only record of decisions
│
└── archives/                   # Old docs. Don't delete. Move here.
```

---

## Skills

| Skill | Command | What it does |
|---|---|---|
| Audit | `/audit` | Weekly health check — context freshness, connections, launch progress |
| Launch Product | `/launch-product` | Tracks 90-day launch milestones for DMPtech.ai and Easein |
| Manage Socials | `/manage-socials` | Drafts and cross-pollinates content for Substack, LinkedIn, X, YouTube |
| Process Voice Memo | `/process-voice-memo` | Converts iPhone Voice Memos into structured meeting notes |

---

## Connections

See `connections.md` for the full registry. Priority connections to wire up:
1. **Google Workspace** — email, calendar, Drive (MCP or API)
2. **Slack** — team communication
3. **Shopify** — Easein revenue and orders

---

## Growing the System

When you find yourself doing the same task 3+ times, build a new skill:
1. Create a new folder under `.claude/skills/{skill-name}/`
2. Add a `SKILL.md` file with a frontmatter block and a step-by-step workflow
3. Run `/audit` to confirm the skill is registered

---
