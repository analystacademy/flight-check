# Flight Check

> A final-pass review for slide decks before they go in front of an audience. Free, open-source, works on every major AI.

Built by [Analyst Academy](https://analystacademy.com).

---

## Why this exists

In late 2025, Deloitte shipped a $290K report to the Australian government containing AI-fabricated court quotes and citations to academic papers that don't exist. A researcher caught all of it on first read. Deloitte refunded part of the fee.

If it happened to Deloitte, it'll happen to you. **Flight Check is the pass that catches it before the room does.**

## What it catches

→ **Fake sources** — AI-fabricated studies, invented court quotes, citations to papers that don't exist
→ **Bad math** — Incorrect arithmetic, percentages that don't add up, numbers that don't match the source
→ **Contradictions in logic** — Numbers on slide 4 that don't match slide 12, recommendations that contradict findings
→ **Inconsistent formatting** — `$4B` on one slide, `$4b` on the next; mismatched units; different decimal places
→ **Weak claims** — "Significant growth," "Strong performance," "The customer" — soft words where numbers or names should be
→ **AI writing** — "Leverage," "in today's fast-paced world," em-dashes everywhere — the patterns your audience spots before you do

The output is a structured report, organized by severity. Critical issues first, polish last. See [examples/sample-report.md](examples/sample-report.md) for what that looks like.

## Install

Flight Check is built on the [Agent Skills open standard](https://www.anthropic.com/engineering/equipping-agents-for-the-real-world-with-agent-skills), which means it runs natively on Claude and works as a paste-in prompt everywhere else.

### Claude.ai (paid plans)

1. Download [`flight-check.skill`](flight-check.skill) from this repo
2. Open Claude.ai → Settings → Capabilities → Skills
3. Upload the `.skill` file

### Claude Code

```bash
git clone https://github.com/YOUR-ORG/flight-check.git ~/.claude/skills/flight-check
```

Or for a single project:

```bash
git clone https://github.com/YOUR-ORG/flight-check.git .claude/skills/flight-check
```

### Claude API / Claude Platform on AWS / Microsoft Foundry

Upload via the Skills API and reference by `skill_id`. See the [Anthropic Skills documentation](https://platform.claude.com/docs/en/agents-and-tools/agent-skills/overview).

### ChatGPT

Open a new chat. Attach your deck (`.pptx` or `.pdf`). Paste the body of [`SKILL.md`](SKILL.md) (everything below the YAML frontmatter) as your first message, followed by: *"Run this checklist on the attached deck."*

For permanent use: create a Custom GPT, paste the body of `SKILL.md` into the GPT's instructions field, and upload the file as a knowledge document.

### Cursor

```bash
mkdir -p .cursor/rules
cp SKILL.md .cursor/rules/flight-check.mdc
```

### Gemini

Create a Gem, paste the body of `SKILL.md` into the custom instructions field.

### Anywhere else

The body of `SKILL.md` is plain Markdown. Paste it as a system prompt, custom instruction, or the first message of any AI conversation, then share your deck.

## How to use it

After installing, do one of these:

- **Drop your deck into Claude.ai** and ask "Run a Flight Check on this"
- **Paste slide text** and ask for a review
- **In Claude Code**, run `/flight-check` after sharing a deck file

The skill activates automatically when you share a deck and ask for a review. Output is the structured report with specific slide numbers and quoted text.

## What it won't do

- It won't redesign your slides
- It won't write new content for slides that need rebuilding
- It won't replace your own final read

Use it as a sweep *before* you do that final read, not instead of it.

## Repo structure

```
flight-check/
├── SKILL.md              # The skill itself
├── README.md             # This file
├── LICENSE               # MIT
├── flight-check.skill    # Packaged version for Claude.ai upload
└── examples/
    └── sample-report.md  # Example of what the skill produces
```

## License

MIT. Use it, fork it, adapt it, build a business on top of it. Attribution is appreciated but not required.

## Built by Analyst Academy

We teach analysts and consultants how to structure, design, and deliver decks that land in front of executive audiences. If Flight Check is useful to you, the courses go deeper:

- **[Presentation Storytelling](https://analystacademy.com)** — structure, story, and persuasion
- **[Data Visualization](https://analystacademy.com)** — charts that actually communicate
- **[Advanced PowerPoint](https://analystacademy.com)** — build faster, build cleaner

Find us at [analystacademy.com](https://analystacademy.com).

---

*If Flight Check catches something embarrassing in your deck, you saved yourself the Deloitte moment. That's the whole product.*
