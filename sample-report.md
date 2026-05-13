# Sample Flight Check Report

This is what Flight Check produces when run on a slide deck. Paste [`SKILL.md`](https://github.com/analystacademy/flight-check/blob/main/SKILL.md) into your AI tool of choice (Claude, ChatGPT, Gemini, Cursor), share a `.pptx` or `.pdf`, and ask for a flight check — you'll get something like the report below.

**About the deck:** Lumen Workflow's $12M Series A pitch — a fictional AI-native workflow automation startup at $4.8M ARR with 142 customers. 50 slides. The deck was built specifically to demonstrate Flight Check; every flagged issue is something the skill surfaced in a single pass.

---

## Flight Check: Lumen Workflow Series A Deck

**Cargo manifest:** Full `.pptx` (50 slides, including speaker notes)
**Source check altitude:** Layer 2 — presence + plausibility review completed; Layer 3 (web verification) attempted on six headline market stats, three returned no matching source.
**Limitations:** None — full deck inspectable, speaker notes available, web search active during review.

### Readiness verdict

**GROUNDED — CRITICAL FIXES REQUIRED**

Five critical issues will materially damage the deck's credibility in front of a Series A audience. Three of them (slides 25, 26, 31) are credibility-killers any investor will catch in the first 30 seconds. Two more (slides 7–11, 33) involve unsourced or unverifiable claims that diligence will challenge directly. Do not send before these are resolved.

### Grounded — critical issues (must fix before takeoff)

- **Slide 25 (Traction) — "18% NRR" is almost certainly a typo for "118%."** Slides 34, 41, and 45 all state NRR is 118%. As shown, "18% NRR" would mean customers are shrinking 82% YoY — the description right under it ("expansion offsets churn 5x over") cannot be true at 18%. Any investor will catch this in the first 30 seconds.

- **Slide 25 — "$4M ARR" headline contradicts "$4.8M ARR" everywhere else** (exec summary slide 3, milestones slide 41). The caption directly below the $4M circle says "Annualized recurring revenue at Oct 2025" — i.e., the same number that's $4.8M on slide 41. Either round consistently or use the exact figure; don't do both on the same deck.

- **Slide 25 — "142 Customer" is mislabeled.** Should be "142 Customers" (plural), and the caption "Customers added Q3 2025; 88% from inbound demand or word of mouth" reads as if 142 were added in Q3, contradicting the 142-total in the exec summary. Rewrite the caption to make clear 142 is the cumulative total.

- **Slide 31 (Unit econ) — "xxx" placeholder still on the slide, plus all five headline stats are shifted one column to the left.** The description for "Magic #" says sales efficiency is 1.4, but the headline reads "xxx." Worse, the other four headlines (4.2x / 41% / 19% / 73%) don't match the labels they sit above — 4.2x belongs to LTV/CAC, not Lead; 41% belongs to Lead, not Trial; and so on down the row. Every headline number needs to move one position right, and "xxx" needs to become "1.4."

- **Slide 26 (Pelican case study) — customer name spelled two ways.** "VP Ops, Pelica" in M. Chen's title, "Pelican is a 600-person fintech…" in the body. Same slide. Pick one (presumably "Pelican") and fix the title.

- **Slides 7, 8, 9, 11, 15 — every external market and pain-point stat is unsourced.** Specifically: "$48B TAM," "23% CAGR through 2030," "$9.2B SAM," "$640M SOM," "$1.2M waste per year," "23 hours per week maintaining automations," "62% break weekly," "six weeks of senior engineer time per quarter." Layer 3 web verification attempted on the four TAM/SAM/SOM figures — could not locate primary sources for any of them. AI-assisted decks fabricate plausible-sounding stats constantly; treat every one of these as suspect until you can produce the primary source. Add footnote citations ("Source: [Org], [Year]") under each figure.

- **Internal contradiction in the cost-of-inaction stats.** Slide 7 says "23 hours per week" (≈58% of a 40-hr week). Slide 8 says "23% ops time on upkeep" — different number, but the visual makes them look like the same finding. Slide 8 also says "six weeks of senior engineer time per quarter" (≈46% of senior eng capacity). The three figures cannot all be true of the same population. Reconcile them — or pick the one that's actually sourced and drop the others.

### Pre-flight warnings (fix if time allows)

- **Slide 15 (By numbers) — every dollar figure wraps mid-number** because the text boxes are too narrow: "$48B" renders as "$48 / B," "$9.2B" as "$9. / 2B," "$640M" as "$64 / 0M." The middle one looks like "$9 dot 2B." Widen the circles or shrink the font; the headline numbers must read as single tokens.

- **MoM growth claim is mathematically inconsistent with the milestones.** Exec summary says "growing 18% MoM." But slide 41 says you crossed $1M ARR in Sept 2024 and hit $4.8M in Oct 2025 — that's 4.8× over 13 months, or ~12.7% average MoM. If 18% is a recent inflection, say so explicitly ("18% MoM for the last six months"). Otherwise the number won't survive due-diligence math.

- **Slide 33 sales funnel math doesn't ground.** 3.2k MQLs/quarter × 23% × 31% = ~228 wins per quarter, or ~900 customers per year. But the deck says total customers = 142. The funnel either describes a future state, a single channel, or fabricated rates — say which.

- **Slide 28 revenue streams sum to 99%.** Platform 76% + Add-ons 11% + Services 12% = 99%. Usage has no percentage. If Usage really is 1%, the description "scales with customer success" oversells it; if it's higher, the other percentages are off.

- **Slide 37 (Compare) — Lumen wins every row.** Agent-native, auto-recovery, audit trail: Lumen "Yes / Native / Replay" while Zapier, Workato, n8n all score worse on all three. Sophisticated audiences distrust matrices where the seller wins everything. Add at least one row where a competitor is at par or ahead, or pick categories where the result is more nuanced.

- **Slide 40 (Leadership) — half the names are first-name-only or single-letter last names.** "Alex P," "Tara," "Omar," "Eva," "Sam B," "Pat L" sit next to full names like "Sara Liu" and "Dan Kim." For a Series A, every leader needs a full name plus a one-line credential. Also: 11 senior leaders at $4.8M ARR is top-heavy and will draw questions — be ready to defend or consolidate.

- **Slide 49 (5-year vision) — "Dominate the $9B SAM by 2028 with 1,000+ customers" alongside "$100M ARR by end of 2028."** $100M of $9B is ~1.1% share. That's a strong outcome, but it's not dominance. The language overreaches against the math on the same slide.

- **Topic-label titles throughout content slides.** Most slide titles state the topic rather than the message: "The Problem" (s6), "The Cost of Doing Nothing" (s8), "The Market" (s10), "Position" (s14), "By numbers" (s15), "How it works" (s16), "Compare" (s37), "Differentiation" (s38), "Unit econ" (s31). Title slides, dividers, and the appendix cover are correctly labeled and exempt from this check. For content slides, run the skim test — read titles 1–50 in order. They tell you the agenda, not the argument. Each one needs a rewrite to a finding (e.g., s8 → "Mid-market firms waste $1.2M/yr on automation upkeep [Source]"; s37 → "Lumen is the only platform that's agent-native and replay-auditable").

- **AI authorship pattern — repetitive triplet structures.** Every framework in the deck is exactly three steps: Connect/Decide/Execute (s16), Describe/Deploy/Monitor (s20), Adaptive/Audited/Governed (s18), Land/Expand/Defend (s34), Direct/Channel/PLG (s35), Top/SQO/Won (s33), plus the three "pillars," "shifts," and "pillars of the deck." Em-dashes appear on roughly half the content slides as connective tissue. Individual em-dashes are fine; this volume of them combined with the rigid triplet pattern is what makes audiences ask "did an AI write this?" Break the rhythm: use a 2-step framework, a 4-step framework, anything that isn't another triplet.

- **Slide 18 — "Three pillars of the deck"** should be "of the platform" or "of the product." Pillars are of the thing being sold, not of the slide deck.

- **Slide 13 — segment labels truncated/typo'd:** "SaaS/Fintec" and "E-comm/Retl." Fix to full words.

- **Slide 35 — column header "Direct / Channel"** sits above rows labeled "Direct / Partner / PLG." The header categories don't match the row categories; PLG isn't a channel partnership. Re-label.

### Cabin checks (catch on the final walkthrough)

- **Slide 1 — "Lumen - Business Plan Deck."** It's a Series A pitch; "business plan deck" is the wrong genre label. Either "Series A" alone or "Lumen — Series A Pitch."

- **Slides 46 and 48 — both titled "Roadmap."** Distinguish them (e.g., s46 = "Operating Roadmap (12 months)" and s48 = "Milestones to Series B").

- **Slide 24 chart label "MAU & Cust"** — abbreviated, and MAU is an odd metric for B2B SaaS at this stage (you typically track logos, seats, or workspace activity). Spell it out and pick the right denominator.

- **Slides 23, 24, 29, 43, 44 — chart titles are topic labels** ("Quarterly revenue," "Customer growth," "Revenue mix," "3-year projection," "Cost & margin"). Headlines on data slides should be the finding ("ARR has compounded 4.8× in 13 months"), not the topic.

- **Slide 44 — visible "Category A" / "Category B" labels** on the margin chart axis. Those are PowerPoint default chart placeholders that didn't get replaced.

- **Slide 45 — "NRR has stayed above 110% for the last six quarters."** Platform went GA in Mar 2024 (slide 41), so six quarters back from Q3 2025 lands at Q2 2024 — one quarter after GA. NRR measured one quarter after launch is mathematically possible but commercially thin. Be ready to defend the lookback window.

- **Slide 21 — "Numbers reflect the median of 142 paying customers measured across Q3 2025."** Tighten — clarify whether the 73% / 94% / 4.2× are measured on all 142 customers or a subset, and over what tenure.

- **Deck date is Nov 2025.** If you're presenting now, refresh the date; if you're presenting against historical numbers, make that explicit.

### What's working

- **Slide 26 (Pelican case study) — concrete, specific outcomes.** "Two engineers redeployed within the first quarter," "books closed two days faster," "tier-1 resolution from 18 hours to under 4." This is the specificity level the rest of the deck needs.
- **Slide 47 (Use of funds) — the math holds and the asks are specific.** 55% / 30% / 15% × $12M is correct, 14 AEs and 6 SEs is concrete, 30-month runway reconciles with the exec summary.
- **Slide 30 pricing — three named tiers at $1,200 / $4,800 / $14,400/month with ARPU growth $19K → $34K** is the kind of internal data you can defend in diligence.
- **One positioning line lands:** "iPaaS gives you the wires; we give you the brain that decides what to do with them" (s14). That sentence should probably appear on the executive summary slide.

### Suggested next step

Fix slide 25 (18% → 118%, $4M → $4.8M, Customer → Customers), slide 26 (Pelica → Pelican), and slide 31 (shift headline stats one column right, replace "xxx" with "1.4") before doing anything else. Those four edits remove the credibility-killers any investor will catch in the first pass. Then go hunt down primary sources for every market and pain-point stat on slides 7, 8, 9, 11, and 15 — the unsourced numbers are the deeper risk, and Layer 3 verification couldn't locate three of the six headline figures.

---

*Generated by [Flight Check](https://github.com/analystacademy/flight-check). For more examples or to learn how to run this on your own decks, see the [README](https://github.com/analystacademy/flight-check/blob/main/README.md).*
