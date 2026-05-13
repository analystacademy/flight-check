---
name: flight-check
description: Final-pass review for slide decks before they go in front of an audience. Use this skill whenever a user shares a presentation, PowerPoint, or PDF of slides and asks for a review, a check, a final pass, or wants to know if the deck is ready to send or present. Also trigger on mentions of AI-tells, missing sources, citation checks, weak headlines, action titles, polish, sanity check, or finalizing a deck. Use this skill even when the user doesn't explicitly say "review" — if they share a near-finished deck without another clear task, run the checklist.
---

# Flight Check — Post-Flight Review for Decks

A final-pass review for slide decks before they go in front of a real audience. Built by Analyst Academy.

This is a *post-flight* check, run after the deck is built and before it's finalized. The job is to catch the things that quietly destroy credibility: AI-generated phrasing that the audience will spot, unsourced numbers, weak headlines that don't carry the message, and the small mistakes that signal "draft." It is not a drafting tool, not a redesign tool, and not a substitute for the analyst's own read.

## When to run this

Run this skill when the user:

- Shares a `.pptx`, `.pdf`, or pasted slides and asks for a review
- Says things like "is this ready," "check this deck," "final pass," "anything I missed"
- Mentions AI-tells, sourcing, citations, polish, sanity check, or finalizing
- Asks whether their slides "sound like AI"

Don't run it when the user is still drafting (asking for new content, structure, or ideas). This checklist is for the *near-final* deck — for earlier stages, help them build first.

## How to run the review

1. **Get the deck.** Ask the user to share the file (`.pptx`, `.pdf`, or pasted slide text). If they only have screenshots or a single slide, work with what they give you, but note that visual issues and consistency checks need the full deck.

2. **Read every slide.** Don't sample. The whole point of a final pass is catching the one slide that breaks the deck's credibility — the one with the fabricated stat, the one with the topic-label headline, the one with the leftover `[TBD]`.

3. **Run all six checks below, slide by slide.** Note specific findings as you go — quote the exact text, name the exact slide number.

4. **Produce the report** using the format at the bottom of this file. Lead with the most critical issues, not with slide order. The user needs to know what could break the presentation, not what's on slide 1.

5. **Resist the urge to be diplomatic.** A vague review ("consider strengthening some headlines") is useless. A pointed one ("Slide 7 title 'Market Overview' is a topic label, not a finding — what's the message?") is what makes this checklist worth running.

## The six checks

### 1. The AI authorship check

The reader should not be able to tell whether a human or an AI wrote this deck. Audiences — especially executive ones — spot AI tells fast, and once they do, they discount everything that follows.

Flag any of these patterns:

**Language tells**
- Triplet adjectives: "comprehensive, robust, and scalable" / "innovative, agile, and customer-centric"
- Empty verbs without specific objects: "leverage," "unlock," "drive," "optimize," "streamline," "enhance"
- Stock openers: "In today's fast-paced world," "In an increasingly complex landscape," "It's worth noting that"
- Hedging without reason: "may potentially," "could possibly," "various," "numerous," "myriad"
- "Not just X — it's Y" or "It's not about X, it's about Y" framings, especially repeated
- Em-dashes used as connective tissue on every slide
- Sentences that sound formal but say nothing concrete: "We will deliver value through strategic alignment of capabilities"
- Overuse of "navigate," "journey," "ecosystem," "landscape," "paradigm," "delve"

**Structural tells**
- Every content slide has exactly three bullets
- Every framework is a 2x2 or four quadrants, even when the underlying logic isn't symmetric
- Bulleted lists where every bullet starts with the same verb form ("Identify... Analyze... Recommend...")
- Slide titles that are noun phrases describing the topic, not the message ("Market Dynamics," "Operational Considerations," "Strategic Implications")
- Filler slides labeled "Overview," "Context," "Background" with no specific finding
- A conclusion slide that just restates the agenda

**The replacement test.** Pick three slides at random. If you swap the named company, industry, or topic for any other, does the slide still make sense? If yes, the slide is filler. Real analytical content shouldn't be portable across contexts.

### 2. The source check

Every quantitative claim, every external fact, every "research shows" needs a verifiable source. Missing sources aren't just sloppy — they're how a deck loses a sophisticated room.

For each slide, ask:

- **Is every number sourced?** A footnote with "Source: [Org], [Year]" or equivalent. "Internal analysis" is acceptable for proprietary work, but only if the analyst can defend the methodology if challenged.
- **Are the sources real?** This is the big one with AI-assisted decks. If a citation references a specific report or study, treat it as suspect until verified. AI fabricates plausible-sounding sources constantly — "McKinsey Global Institute, 2023" is a real organization, but the specific report named may not exist. When you spot a specific citation in the deck, flag it for the user to verify directly.
- **Are the sources current?** A 2019 industry stat in a 2026 deck is a flag. If the data is older, the slide should acknowledge why (most recent available, intentional comparison, etc.).
- **Are the sources strong?** A vendor whitepaper, a blog post, and a peer-reviewed study don't carry equal weight. Match source quality to the strength of the claim.
- **Does the cited number actually match what the source says?** When numbers travel through secondary citations they often drift. If the deck says "30% of CFOs," verify the source says exactly that — not "roughly a third," not "many CFOs."

**Common failure modes to flag specifically:**
- "Studies have shown..." without naming the study
- "Industry research suggests..." with no citation
- A number on a chart with no source line
- The same source cited for every claim (suggests one paper is being stretched to support points it doesn't actually make)
- Sources that exist but appear unread — phrasing in the deck doesn't match the source's actual language

### 3. The action title check

(Analyst Academy core principle.) Every slide title should state the message of the slide, not the topic. A reader who scans only the titles, in order, should get the full storyline.

For each slide title, ask: **Could this be the title of a different slide with completely different content?**

If yes, the title is a topic label, not a finding. It needs a rewrite.

Examples:

- ❌ "Q3 Revenue Performance" → ✅ "Q3 revenue grew 12% — driven entirely by enterprise renewals"
- ❌ "Customer Segmentation" → ✅ "Three segments account for 80% of churn, and they share one trait"
- ❌ "Implementation Timeline" → ✅ "We can launch by Q2 if hiring closes in March"
- ❌ "Market Overview" → ✅ "The market is consolidating around two players; the third is the acquisition target"

**The skim test.** Read only the titles, in order. Do they form a coherent argument? If they don't tell the story on their own, the deck is built for a reader who'll read every word — and no executive does.

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

## Output format

Produce the review report in this structure:

```
## Flight Check: [Deck name or topic]

### Critical issues (fix before sending)
- Slide [N]: [specific issue with exact quote from the deck]
- ...

### High-priority issues (fix if time allows)
- Slide [N]: [specific issue]
- ...

### Polish issues (catch on a final read)
- Slide [N]: [specific issue]
- ...

### What's working
[Two to four specific things the deck does well. Not flattery — this tells the user which patterns to keep.]

### Suggested next step
[One sentence: what to fix first.]
```

Order by criticality, not by slide number. The user needs to know what could break the presentation before they know what's on slide 1.

When quoting from the deck, use the exact text. When naming a slide, use both the number and the title so the user can find it instantly.

## What this skill won't do

- It won't redesign slides. Visual redesign is a separate task; flag visual issues but don't try to fix them in-line.
- It won't write new content. If a slide is fundamentally broken, say so and tell the user what the slide needs to do — but don't draft a replacement unless they ask.
- It won't replace the analyst's own read. AI can miss context that depends on knowing the audience, the prior conversation, or the firm's house style. Always tell the user to do a final read themselves.

---

Built by Analyst Academy. Free to use, share, and adapt. analystacademy.com
