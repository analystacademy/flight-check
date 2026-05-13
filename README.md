# Flight Check

> A final-pass review for slide decks before they go in front of an audience. Free, open-source, runs natively on Claude — and pastes into any other AI.

Built by [Analyst Academy](https://analystacademy.com).

---

## Why this exists

AI is in everyone's workflow now. So are the problems AI introduces: fabricated citations, numbers that don't match across slides, headlines that describe the topic instead of stating the message, and phrasing that telegraphs "ChatGPT wrote this." Most of those mistakes survive a casual proofread.

Flight Check is the pass that catches them.

## What it catches

Flight Check runs six checks across your deck:

**1. AI writing tells.** Phrases like "leverage," "in today's fast-paced world," triplet adjectives, em-dashes used as connective tissue, every slide having exactly three bullets — the patterns audiences spot before you do.

**2. Sources that don't hold up.** Fabricated studies, citations to papers that don't exist, "research shows" without a named source, numbers on charts with no citation line, and sources that don't actually say what the slide claims.

**3. Topic-label headlines.** Slide titles like "Market Overview" or "Q3 Performance" that describe what's on the slide instead of stating its message. A reader scanning only titles should get the full story.

**4. Vague claims.** "Significant growth," "strong performance," "the customer" — soft words where numbers, names, or specific mechanisms belong.

**5. Arguments that don't hold together.** Numbers on slide 4 that don't match slide 12, recommendations that don't trace back to findings, breakdowns that overlap or leave gaps.

**6. Polish problems.** Mixed currency formats (`$4B` vs `$4b`), misspelled names, leftover `[TBD]` tags, 3D charts, truncated axes, mismatched fonts — the small things that mark a deck as draft.

The output is a structured report, organized by severity: critical issues first, polish last. See [examples/sample-report.md](examples/sample-report.md) for what that looks like.

## Two ways to run it

Flight Check is built on the [Agent Skills open standard](https://www.anthropic.com/engineering/equipping-agents-for-the-real-world-with-agent-skills). That gives you two ways to use it:

**1. Native skill (Claude only).** On Claude.ai, Claude Code, the Claude API, and Claude on AWS Bedrock or Microsoft Foundry, Flight Check installs as a proper skill. It activates automatically when you share a deck and ask for a review.

**2. Paste-in prompt (everywhere else).** ChatGPT, Gemini, Microsoft Copilot, Perplexity, Cursor — and basically any other chatbot — can run Flight Check too. You paste the instructions in as a custom instruction or first message. The checklist is the same; you trigger it manually instead of automatically.

The instructions live in [`SKILL.md`](SKILL.md). Everything below the YAML block at the very top is the part you paste into non-Claude tools. The packaged `flight-check.skill` file is for Claude.ai uploads specifically — other platforms can't read it.

---

## Install

### Claude.ai (paid plans)

1. Download [`flight-check.skill`](flight-check.skill) from this repo.
2. In Claude.ai, open **Settings → Capabilities → Skills**.
3. Click **Upload skill** and pick the file.

Then drop a deck into a chat and ask for a Flight Check.

### Claude Code

In your terminal, install for all projects:

```
git clone https://github.com/analystacademy/flight-check.git ~/.claude/skills/flight-check
```

Or just one project:

```
git clone https://github.com/analystacademy/flight-check.git .claude/skills/flight-check
```

### Claude API / Claude on AWS Bedrock / Claude on Microsoft Foundry

Upload via the Skills API and reference by `skill_id`. See the [Anthropic Skills documentation](https://platform.claude.com/docs/en/agents-and-tools/agent-skills/overview).

### ChatGPT — one-off use

1. Open [`SKILL.md`](SKILL.md) and copy everything *below* the YAML block at the top.
2. Start a new ChatGPT chat and attach your deck (`.pptx` or `.pdf`).
3. Paste the SKILL.md body as your first message, then add: *"Run this checklist on the attached deck."*

### ChatGPT — permanent setup (Custom GPT)

1. Go to **Create a GPT** in ChatGPT.
2. In the **Instructions** field, paste the body of `SKILL.md`.
3. Under **Knowledge**, upload `SKILL.md` as a file.
4. Save. From then on, attach a deck to that GPT and say "Run Flight Check."

### Gemini

1. Open **Gems** in Gemini.
2. Create a new Gem and paste the body of `SKILL.md` into the custom instructions field.
3. Save. Attach a deck and ask for a Flight Check.

### Microsoft Copilot

1. In Copilot, create a new **Agent** (or open the agent builder).
2. Paste the body of `SKILL.md` into the instructions field.
3. Save and use it the same way — attach a deck and run the check.

### Perplexity

1. Create a new **Space**.
2. Paste the body of `SKILL.md` into the Space's **AI Instructions**.
3. Drop your deck into a thread inside that Space and ask for a Flight Check.

### Cursor (and other coding AIs)

Save the body of `SKILL.md` as a rules file in your project:

```
mkdir -p .cursor/rules
cp SKILL.md .cursor/rules/flight-check.mdc
```

Windsurf and similar tools have their own rules folders — same idea, different path.

### Any other AI

The body of `SKILL.md` is plain Markdown and model-agnostic. Open any chatbot, paste the body in as your first message or system prompt, then share your deck.

---

## How to use it

After installing, do one of these:

- **In Claude.ai**, drop your deck in and ask "Run a Flight Check on this."
- **In Claude Code**, share a deck file and run `/flight-check`.
- **In any other AI**, paste the SKILL.md body, attach your deck, and say "Run this checklist on the attached deck."

Output is a structured report with specific slide numbers and quoted text.

## What it won't do

- It won't redesign your slides.
- It won't write new content for slides that need rebuilding.
- It won't replace your own final read.

Use it as a sweep *before* you do that final read, not instead of it.

## Repo structure

```
flight-check/
├── SKILL.md              # The instructions
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
