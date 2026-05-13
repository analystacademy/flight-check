# Flight Check

> A final-pass review for slide decks before they go in front of an audience. Free, open-source, works on every major AI.

Built by [Analyst Academy](https://analystacademy.com).

---

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
git clone https://github.com/analystacademy/flight-check.git ~/.claude/skills/flight-check
```

Or for a single project:

```bash
git clone https://github.com/analystacademy/flight-check.git .claude/skills/flight-check
```

### Claude API / Claude Platform on AWS / Microsoft Foundry

Upload via the Skills API and reference by `skill_id`. See the [Anthropic Skills documentation](https://platform.claude.com/docs/en/agents-and-tools/agent-skills/overview).

### ChatGPT

Flight Check is not a native ChatGPT Skill yet, but it works well as a reusable prompt or Custom GPT instruction.

#### One-time use

1. Open a new ChatGPT conversation
2. Attach your deck as a `.pptx` or `.pdf`
3. Paste the body of [`SKILL.md`](SKILL.md), excluding the YAML frontmatter
4. Add:  
   > Run a Flight Check on the attached deck.

For best results, use a model that can read uploaded files and inspect slide content.

#### Permanent use with a Custom GPT

1. Create a new Custom GPT
2. Paste the body of [`SKILL.md`](SKILL.md), excluding the YAML frontmatter, into the GPT’s Instructions field
3. Optionally upload `SKILL.md` as a reference file
4. Start a new conversation with that GPT, attach a deck, and ask:  
   > Run a Flight Check on this deck.

Important: put the Flight Check instructions in the GPT’s main Instructions field, not only in a knowledge file. Knowledge files are useful for reference, but the checklist works best when the review behavior is part of the GPT’s core instructions.

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
