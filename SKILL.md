---
name: flight-check
description: Final-pass quality review for near-finished slide decks before they are sent or presented. Use when the user shares a PowerPoint, PDF, slide screenshots, or pasted slide text and asks for a review, final pass, sanity check, readiness check, polish check, source check, citation check, AI-tell check, or asks whether the deck is ready. Do not use for early-stage drafting, content generation, slide redesign, or building a deck from scratch.
---

# Flight Check — Pre-Flight Review for Decks

A final-pass review for slide decks before they go in front of a real audience. Built by Analyst Academy.

This is a *pre-flight* check, run after the deck is built and before it taxis to the runway. The job is to catch the things that quietly destroy credibility — AI-generated phrasing the audience will spot, unsourced numbers, weak headlines that don't carry the message, and the small mistakes that signal "draft." Clear it, or ground it.

It is not a drafting tool, not a redesign tool, and not a substitute for the pilot's own walkaround.

## When to run this

Run this skill when the user:

- Shares a `.pptx`, `.pdf`, or pasted slides and asks for a review
- Says things like "is this ready," "check this deck," "final pass," "anything I missed"
- Mentions AI-tells, sourcing, citations, polish, sanity check, or finalizing
- Asks whether their slides "sound like AI"

Don't run it when the user is still drafting (asking for new content, structure, or ideas). This checklist is for the *near-final* deck — for earlier stages, help them build first.

## Flight procedure

**Step 1. Identify what's in the cargo bay.** Before reviewing, note the input type. This determines what you can and can't check:

- **Full `.pptx`:** Slide text, layout, charts, footers, speaker notes (if accessible) — all checkable.
- **PDF export:** Visible slides only. Speaker notes, comments, and edit-layer artifacts will not be visible.
- **Screenshots or partial slides:** Only what is visually present. Full-deck consistency checks (cross-slide number reconciliation, structural arc) are limited.
- **Pasted slide text:** Wording, structure, action titles, specificity, source presence — yes. Visual polish, layout, chart honesty — no.

State the input type and limitations at the top of the report. Never claim a check passed if it wasn't actually performed.

**Step 2. Walk the full deck.** Don't sample. The whole point of a pre-flight check is catching the one slide that breaks the deck's credibility — the one with the fabricated stat, the topic-label headline, the leftover `[TBD]`.

**Step 3. Run all six diagnostic systems below.** Note specific findings as you go — quote exact text, name the exact slide number and title.

**Step 4. File the report** using the format at the bottom of this file. Lead with the most critical issues, not slide order. The pilot needs to know what could ground the flight, not what's on slide 1.

**Step 5. Resist the urge to be diplomatic.** A vague review ("consider strengthening some headlines") is useless. A pointed one ("Slide 7 title 'Market Overview' is a topic label, not a finding — what's the message?") is what makes this checklist worth running.

## Evidence standard

Every reported issue must be locatable. Each finding must include at least one of:

- Slide number (and title if available)
- Exact quoted text from the slide
- A precise visual reference ("the chart on slide 12," "the second bullet on slide 4")

If you can't point to where an issue is, don't include it in the report. Generic comments like "some titles feel weak" are not findings — they're impressions.

## The six diagnostic systems

### 1. The AI authorship check

The reader should not be able to tell whether a human or an AI wrote this deck. Audiences — especially executive ones — spot AI tells fast, and once they do, they discount everything that follows.

**The principle:** flag *patterns* of generic, inflated, or portable language. Do not flag individual words mechanically. "Leverage" appears in "leverage ratio" (legitimate). "Drive" appears in "drive revenue" (fine). The issue is when the language is repetitive, evidence-free, and could be lifted to any other deck unchanged.

**Patterns that signal AI authorship:**

*Language tells*
- Triplet adjectives: "comprehensive, robust, and scalable" / "innovative, agile, and customer-centric"
- Empty verbs *with no specific object*: "leverage capabilities," "unlock potential," "drive value," "optimize outcomes," "streamline operations"
- Stock openers: "In today's fast-paced world," "In an increasingly complex landscape," "It's worth noting that"
- Hedging without reason: "may potentially," "could possibly," "various," "numerous," "myriad"
- "Not just X — it's Y" or "It's not about X, it's about Y" framings, especially repeated
- Em-dashes used as connective tissue on every slide
- Sentences that sound formal but say nothing concrete: "We will deliver value through strategic alignment of capabilities"

*Structural tells*
- Every framework is exactly three steps, three pillars, three shifts
- Every breakdown is a 2x2 or four quadrants, even when the underlying logic isn't symmetric
- Bulleted lists where every bullet starts with the same verb form ("Identify... Analyze... Recommend...")
- Filler slides labeled "Overview," "Context," "Background" with no specific finding
- A conclusion slide that just restates the agenda

**The replacement test.** Pick three content slides at random. If you swap the named company, industry, or topic for any other, does the slide still make sense? If yes, the slide is filler — real analytical content shouldn't be portable across contexts.

**False-positive guard.** A single instance of an em-dash or one use of "leverage" is not an AI tell. Flag the pattern, not the word. If a deck has one stock phrase across 30 slides, that's a polish issue; if it has them on every slide, that's an authorship issue.

### 2. The source check

Every quantitative claim, every external fact, every "research shows" needs a verifiable source. Missing or fabricated sources are how a deck loses a sophisticated room — and AI-assisted decks fabricate plausible-sounding citations constantly.

Run this check in three layers, and be explicit about which layer you actually completed.

**Layer 1 — Source presence.** Is there a source line for every external number, external claim, and quoted study? This is the floor. Missing citations get flagged regardless of anything else.

**Layer 2 — Source plausibility.** Does the citation *look* real? Specific report names from real organizations are higher confidence ("McKinsey Global Institute, *The State of Enterprise AI*, 2024"). Vague citations are lower ("McKinsey, 2024" or "industry research"). AI-fabricated sources often cite real organizations but invented report titles.

**Layer 3 — Source verification.** Does the cited source actually exist, and does the number match what the source says? This is the only layer where you can genuinely confirm a citation is real.

**Important:** Layer 3 requires the ability to search the web. If you have web search available, attempt to verify a sample of the most consequential citations (top-of-deck stats, market sizing figures, recommendation-supporting numbers). If web search is not available or fails, you cannot complete Layer 3 — say so plainly.

**Never claim a source was verified unless you actually verified it.** State which layer of the check you completed:

- "Source check completed at Layer 1 (presence only — verification not attempted)."
- "Source check completed at Layer 2 (presence + plausibility review; verification not possible without web access)."
- "Source check completed at Layer 3 (presence + plausibility + spot verification of [list of citations] via web search)."

**Common failure modes to flag specifically:**
- "Studies have shown..." without naming the study
- "Industry research suggests..." with no citation
- A number on a chart with no source line
- The same source cited for every claim (suggests one paper is being stretched)
- Sources that exist but appear unread — phrasing in the deck doesn't match the source's actual language
- Specific named reports from real organizations — these are the highest-risk for AI fabrication and the ones most worth verifying

### 3. The action title check

(Analyst Academy core principle.) On content slides, every title should state the message of the slide, not the topic. A reader who scans only the titles, in order, should get the full storyline.

For each *content* slide title, ask: **Could this be the title of a different slide with completely different content?**

If yes, the title is a topic label, not a finding. It needs a rewrite.

Examples:

- ❌ "Q3 Revenue Performance" → ✅ "Q3 revenue grew 12% — driven entirely by enterprise renewals"
- ❌ "Customer Segmentation" → ✅ "Three segments account for 80% of churn, and they share one trait"
- ❌ "Implementation Timeline" → ✅ "We can launch by Q2 if hiring closes in March"
- ❌ "Market Overview" → ✅ "The market is consolidating around two players; the third is the acquisition target"

**Apply this standard to content slides only.** These slides are exempt from action-title requirements:

- **Title slide** (deck cover) — typically just the deck name and date
- **Agenda / table of contents** — short labels are fine
- **Section dividers** — single-word or short-phrase dividers are appropriate
- **Appendix cover and appendix slides** — reference material, often labeled by topic
- **Q&A or "thank you" closers** — generic closing slides

These slides should still be purposeful and not filler, but they don't need full action titles. Flag a divider only if it's adding pages without function.

**The skim test.** Read only the content slide titles, in order. Do they form a coherent argument? If they don't tell the story on their own, the deck is built for a reader who'll read every word — and no executive does.

### 4. The specificity check

Vagueness is the analyst's tell that they didn't do the work. Every important claim should have a specific quantity, a specific named entity, or a specific mechanism.

Flag:

- **Adjectives where numbers belong:** "significant growth," "major reduction," "strong performance" — what percent? what dollar amount?
- **Pronouns or generic nouns where names belong:** "the customer," "a stakeholder," "the team" — which one? Named, if not confidential.
- **Outcomes without mechanisms:** "Costs will decrease" — through what action? "Engagement will improve" — by what change?
- **Suspiciously round numbers:** 50%, 80%, 2x — if it's a precise finding, why is it a round number? If it's an estimate, the slide should say so.
- **Time frames without anchors:** "in the near term," "going forward" — by when, specifically?

A useful test: mentally highlight every adjective in the deck. If most of them could be replaced by a number and the slide would be stronger, the analyst is hiding behind language.

### 5. The structure check

The deck should hold up as an argument, not just a sequence of slides.

- **Top-down logic.** The first slide (or executive summary slide) states the answer. Every subsequent slide is in service of that answer or its supporting points. Slides that don't ladder up either need a new home or need cutting.
- **No internal contradictions.** Numbers on slide 4 match numbers on slide 12. The framing on slide 2 isn't undermined by data on slide 8.
- **MECE where it matters.** When the deck presents a breakdown (segments, drivers, options, regions), the categories should be Mutually Exclusive and Collectively Exhaustive. Overlapping or incomplete breakdowns signal sloppy thinking and invite the audience to attack the structure instead of engaging the content.
- **Recommendations trace to findings.** Every recommendation in the summary or appendix should trace back to a specific earlier finding. Recommendations that appear from nowhere are a flag.

### 6. The polish pass

The small things that mark a deck as "draft" even when the content is strong.

- **Typography:** One heading font, one body font. Same size for the same level of hierarchy. No mixed weights without intent.
- **Alignment:** Elements snap to a grid. Text boxes aren't one pixel off. Charts use consistent axis treatments, consistent bar widths, consistent color logic.
- **Names spelled correctly.** Search every person, company, and product name. Verify spelling. This is the single most common embarrassment in finalized decks — and it's the easiest to fix.
- **Numbers formatted consistently.** Same decimal places, same units, same currency formatting. "$1.2M" and "$1,200,000" should not both appear. "$4B" and "$4b" should not both appear.
- **Charts honest.** Y-axis starts at zero unless there's a specific reason to truncate (call it out if so). No 3D charts. No pie charts where a bar chart would be clearer. No chart junk.
- **Page numbers, footers, version date present and correct.**
- **No tracked changes, comment bubbles, `[TBD]`, `[insert source]`, or lorem ipsum.** Check the speaker notes too — that's where these hide.

## How to decide what's critical

Treat an issue as **grounded** if it could:

- Make the audience doubt the deck's credibility (fabricated stat, broken citation, internal contradiction)
- Materially change the recommendation if corrected
- Expose an unsupported or possibly fabricated claim
- Create confusion about the main message
- Embarrass the presenter in front of the audience (misspelled exec name, leftover `[TBD]`, wrong client name)

Treat as **pre-flight warning** if it weakens the argument or polish but won't break the presentation: topic-label titles on content slides, weak specificity, unsourced soft claims, inconsistent formatting at the section level.

Treat as **cabin check** if a careful reader would notice but the audience likely won't: minor typography, single instances of soft language, alignment issues, formatting inconsistencies at the word level.

## Output format

Produce the review report in this structure:

```
## Flight Check: [Deck name or topic]

**Cargo manifest:** [Full .pptx / PDF / screenshots / pasted text]
**Source check altitude:** [Layer 1 / Layer 2 / Layer 3 — see source check section]
**Limitations:** [Any checks that were not fully possible, and why]

### Readiness verdict
**[GROUNDED — critical fixes required / HOLDING — fixes needed before clearance / CLEARED WITH NOTES — minor polish / CLEARED FOR DEPARTURE — ready to send]**

### Grounded — critical issues (must fix before takeoff)
- Slide [N] — "[exact title]": [specific issue with exact quoted text]
- ...

### Pre-flight warnings (fix if time allows)
- Slide [N] — "[exact title]": [specific issue]
- ...

### Cabin checks (catch on the final walkthrough)
- Slide [N] — "[exact title]": [specific issue]
- ...

### What's working
[Two to four specific things the deck does well. Not flattery — this tells the pilot which patterns to keep.]

### Suggested next step
[One sentence: what to fix first.]
```

Order by criticality, not by slide number. The pilot needs to know what could ground the flight before they know what's on slide 1.

When quoting from the deck, use the exact text. When naming a slide, use both the number and the title so the user can find it instantly.

## What this skill won't do

- **It won't redesign slides.** Visual redesign is a separate task; flag visual issues but don't try to fix them in-line.
- **It won't write new content wholesale.** If a slide is fundamentally broken, say so and tell the user what the slide needs to do. For weak titles or vague claims, you *may* provide a single example rewrite when it clarifies the issue — but keep the focus on diagnosis. Don't draft replacements unless the user asks.
- **It won't replace the pilot's own walkaround.** AI can miss context that depends on knowing the audience, the prior conversation, or the firm's house style. Always tell the user to do a final read themselves.
- **It won't claim checks it didn't perform.** If source verification wasn't possible, say so. If the input was screenshots only, don't claim to have checked the full-deck arc.

---

Built by Analyst Academy. Free to use, share, and adapt. analystacademy.com
